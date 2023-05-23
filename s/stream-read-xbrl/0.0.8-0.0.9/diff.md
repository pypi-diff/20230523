# Comparing `tmp/stream_read_xbrl-0.0.8.tar.gz` & `tmp/stream_read_xbrl-0.0.9.tar.gz`

## Comparing `stream_read_xbrl-0.0.8.tar` & `stream_read_xbrl-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    15511 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/stream_read_xbrl.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/LICENSE
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/README.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    19955 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/stream_read_xbrl.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/README.md
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 stream_read_xbrl-0.0.9/PKG-INFO
```

### Comparing `stream_read_xbrl-0.0.8/stream_read_xbrl.py` & `stream_read_xbrl-0.0.9/stream_read_xbrl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import datetime
 import os
 import re
 import urllib.parse
-from collections import OrderedDict
+from dataclasses import dataclass
+from collections import defaultdict
 from contextlib import contextmanager
 from decimal import Decimal
 from itertools import chain
 from io import BytesIO
+from typing import Optional, Callable
 
 import dateutil
 import dateutil.parser
 from bs4 import BeautifulSoup
 import httpx
 from lxml import etree
 from lxml.etree import XMLSyntaxError
@@ -44,309 +46,296 @@
 
     def _parse_bool(element, text):
         return False if text == 'false' else True if text == 'true' else None
 
     def _parse_reversed_bool(element, text):
         return False if text == 'true' else True if text == 'false' else None
 
-    # XPATH helpers
-    # XML element syntax: <ns:name attribute='value'>content</ns:name>
-    def _element_has_tag_name(name):
-        return f"//*[local-name()='{name}']"
-
-    def _element_has_name_attr_value(attr_value):
-        return (
-            f"//*[contains(@name, ':{attr_value}') "
-            f"and substring-after(@name, ':{attr_value}') = '']"
-        )
-
-    def _element_has_tag_name_or_name_attr_value(value):
-        return (
-            f"//*[local-name()='{value}' or (contains(@name, ':{value}') "
-            f"and substring-after(@name, ':{value}') = '')]"
-        )
+    # Parsing strategy
+    #
+    # The XBRL format is a "tagging" format that can tag elements in any order with machine readable metadata.
+    # While flexible, this means that it's difficult to efficiently convert to a dataframe.
+    #
+    # The simplest way to do this would XPath repeatedly to find extract the data for each columnn. This was
+    # done in previous versions, but took about 3 times as long as the current solution. The current solution
+    # leverages the fact that dictionary lookups are fast, and so constructs dictionaries that can be looked up
+    # while iterating through all the elements in the document.
+
+    # Although in some cases a dictionary lookup doesn't seem possible, and so a custom matcher can be defined
+
+    @dataclass
+    class _test():
+        name: Optional[str]
+        search: Callable = lambda element, local_name, attribute_name, context_ref: (element,)
+
+    @dataclass
+    class _tn(_test):
+        # (Local) Tag name, i.e. withoout namespace
+        pass
+
+    @dataclass
+    class _av(_test):
+        # Attribute value. Matches on the "name" attribute, but stripping off the namespace prefix
+        pass
+
+    @dataclass
+    class _custom(_test):
+        # Custom test when matching on tag name or name attribute isn't enought
+        pass
 
-    # aliases
-    _tn = _element_has_tag_name
-    _av = _element_has_name_attr_value
-    _tn_av = _element_has_tag_name_or_name_attr_value
-
-    # {attribute: ([xpath_expressions], attribute_type)}
-    #   attribute: identifier for financial attribute
-    #   xpath_expressions: xpaths that will be tried to locate
-    #   financial attribute in XBRL tree (until a value is found)
-    #   attribute_type: type used to parse the attribute value
     GENERAL_XPATH_MAPPINGS = {
         'balance_sheet_date': (
             [
-                _av('BalanceSheetDate'),
-                _tn('BalanceSheetDate'),
-            ],
-            _parse_date,
+                (_av('BalanceSheetDate'), _parse_date),
+                (_tn('BalanceSheetDate'), _parse_date),
+            ]
         ),
         'companies_house_registered_number': (
             [
-                _av('UKCompaniesHouseRegisteredNumber'),
-                _tn('CompaniesHouseRegisteredNumber'),
-            ],
-            _parse_str,
+                (_av('UKCompaniesHouseRegisteredNumber'), _parse_str),
+                (_tn('CompaniesHouseRegisteredNumber'), _parse_str),
+            ]
         ),
         'entity_current_legal_name': (
             [
-                _av('EntityCurrentLegalOrRegisteredName'),
-                _tn('EntityCurrentLegalName'),
-                (
-                    "(//*[contains(@name, ':EntityCurrentLegalOrRegisteredName') "
-                    "and substring-after(@name, ':EntityCurrentLegalOrRegisteredName') = '']"
-                    "//*[local-name()='span'])[1]"
-                ),
-            ],
-            _parse_str,
+                (_av('EntityCurrentLegalOrRegisteredName'), _parse_str),
+                (_tn('EntityCurrentLegalName'), _parse_str),
+                (_custom(None, lambda element, local_name, attribute_name, context_ref: element.xpath("./*[local-name()='span'][1]")), _parse_str),
+            ]
         ),
         'company_dormant': (
             [
-                _av('EntityDormantTruefalse'),
-                _av('EntityDormant'),
-                _tn('CompanyDormant'),
-                _tn('CompanyNotDormant'),
-            ],
-            [_parse_bool, _parse_bool, _parse_bool, _parse_reversed_bool],
+                (_av('EntityDormantTruefalse'), _parse_bool),
+                (_av('EntityDormant'), _parse_bool),
+                (_tn('CompanyDormant'), _parse_bool),
+                (_tn('CompanyNotDormant'), _parse_reversed_bool),
+            ]
         ),
         'average_number_employees_during_period': (
             [
-                _av('AverageNumberEmployeesDuringPeriod'),
-                _av('EmployeesTotal'),
-                _tn('AverageNumberEmployeesDuringPeriod'),
-                _tn('EmployeesTotal'),
-            ],
-            _parse_decimal_with_colon,
+                (_av('AverageNumberEmployeesDuringPeriod'), _parse_decimal_with_colon),
+                (_av('EmployeesTotal'), _parse_decimal_with_colon),
+                (_tn('AverageNumberEmployeesDuringPeriod'), _parse_decimal_with_colon),
+                (_tn('EmployeesTotal'), _parse_decimal_with_colon),
+            ]
         ),
     }
 
     PERIODICAL_XPATH_MAPPINGS = {
         # balance sheet
         'tangible_fixed_assets': (
             [
-                _tn_av('FixedAssets'),
-                _tn_av('TangibleFixedAssets'),
-                _av('PropertyPlantEquipment'),
-            ],
-            _parse_decimal,
+                (_tn('FixedAssets'), _parse_decimal),
+                (_av('FixedAssets'), _parse_decimal),
+                (_tn('TangibleFixedAssets'), _parse_decimal),
+                (_av('TangibleFixedAssets'), _parse_decimal),
+                (_av('PropertyPlantEquipment'), _parse_decimal),
+            ]
         ),
         'debtors': (
             [
-                _tn_av('Debtors'),
-            ],
-            _parse_decimal,
+                (_tn('Debtors'), _parse_decimal),
+                (_av('Debtors'), _parse_decimal),
+            ]
         ),
         'cash_bank_in_hand': (
             [
-                _tn_av('CashBankInHand'),
-                _av('CashBankOnHand'),
-            ],
-            _parse_decimal,
+                (_tn('CashBankInHand'), _parse_decimal),
+                (_av('CashBankInHand'), _parse_decimal),
+                (_av('CashBankOnHand'), _parse_decimal),
+            ]
         ),
         'current_assets': (
             [
-                _tn_av('CurrentAssets'),
-            ],
-            _parse_decimal,
+                (_tn('CurrentAssets'), _parse_decimal),
+                (_av('CurrentAssets'), _parse_decimal),
+            ]
         ),
         'creditors_due_within_one_year': (
             [
-                _av('CreditorsDueWithinOneYear'),
-                (
-                    "//*[contains(@name, ':Creditors') and substring-after(@name, ':Creditors')"
-                    " = '' and contains(@contextRef, 'WithinOneYear')]"
-                ),
-            ],
-            _parse_decimal,
+                (_av('CreditorsDueWithinOneYear'), _parse_decimal),
+                (_av('Creditors', lambda element, local_name, attribute_name, context_ref: (element,) if 'WithinOneYear' in element.get('contextRef') else ()), _parse_decimal),
+            ]
         ),
         'creditors_due_after_one_year': (
             [
-                _av('CreditorsDueAfterOneYear'),
-                (
-                    "//*[contains(@name, ':Creditors') and substring-after(@name, ':Creditors')"
-                    " = '' and contains(@contextRef, 'AfterOneYear')]"
-                ),
-            ],
-            _parse_decimal,
+                (_av('CreditorsDueAfterOneYear'), _parse_decimal),
+                (_custom(None, lambda element, local_name, attribute_name, context_ref: (element,) if 'Creditors' == local_name and 'AfterOneYear' in context_ref else ()), _parse_decimal)
+            ]
         ),
         'net_current_assets_liabilities': (
             [
-                _tn_av('NetCurrentAssetsLiabilities'),
-            ],
-            _parse_decimal,
+                (_tn('NetCurrentAssetsLiabilities'), _parse_decimal),
+                (_av('NetCurrentAssetsLiabilities'), _parse_decimal),
+            ]
         ),
         'total_assets_less_current_liabilities': (
             [
-                _tn_av('TotalAssetsLessCurrentLiabilities'),
-            ],
-            _parse_decimal,
+                (_tn('TotalAssetsLessCurrentLiabilities'), _parse_decimal),
+                (_av('TotalAssetsLessCurrentLiabilities'), _parse_decimal),
+            ]
         ),
         'net_assets_liabilities_including_pension_asset_liability': (
             [
-                _tn_av('NetAssetsLiabilitiesIncludingPensionAssetLiability'),
-                _tn_av('NetAssetsLiabilities'),
-            ],
-            _parse_decimal,
+                (_tn('NetAssetsLiabilitiesIncludingPensionAssetLiability'), _parse_decimal),
+                (_av('NetAssetsLiabilitiesIncludingPensionAssetLiability'), _parse_decimal),
+                (_tn('NetAssetsLiabilities'), _parse_decimal),
+                (_av('NetAssetsLiabilities'), _parse_decimal),
+            ]
         ),
         'called_up_share_capital': (
             [
-                _tn_av('CalledUpShareCapital'),
-                (
-                    "//*[contains(@name, ':Equity') and substring-after(@name, ':Equity') = '' "
-                    "and contains(@contextRef, 'ShareCapital')]"
-                ),
-            ],
-            _parse_decimal,
+                (_tn('CalledUpShareCapital'), _parse_decimal),
+                (_av('CalledUpShareCapital'), _parse_decimal),
+                (_custom(None, lambda element, local_name, attribute_name, context_ref: (element,) if 'Equity' == attribute_name and 'ShareCapital' in element.get('contextRef', '') else ()), _parse_decimal),
+            ]
         ),
         'profit_loss_account_reserve': (
             [
-                _tn_av('ProfitLossAccountReserve'),
-                (
-                    "//*[contains(@name, ':Equity') and substring-after(@name, ':Equity') = '' "
-                    "and contains(@contextRef, 'RetainedEarningsAccumulatedLosses')]"
-                ),
-            ],
-            _parse_decimal,
+                (_tn('ProfitLossAccountReserve'), _parse_decimal),
+                (_av('ProfitLossAccountReserve'), _parse_decimal),
+                (_custom(None, lambda element, local_name, attribute_name, context_ref: (element,) if 'Equity' == attribute_name and 'RetainedEarningsAccumulatedLosses' in element.get('contextRef', '') else ()), _parse_decimal),
+            ]
         ),
         'shareholder_funds': (
             [
-                _tn_av('ShareholderFunds'),
-                (
-                    "//*[contains(@name, ':Equity') and substring-after(@name, ':Equity') = '' "
-                    "and not(contains(@contextRef, 'segment'))]"
-                ),
-            ],
-            _parse_decimal,
+                (_tn('ShareholderFunds'), _parse_decimal),
+                (_av('ShareholderFunds'), _parse_decimal),
+                (_custom(None,  lambda element, local_name, attribute_name, context_ref: (element,) if 'Equity' == attribute_name and 'segment' not in context_ref else ()), _parse_decimal),
+            ]
         ),
         # income statement
         'turnover_gross_operating_revenue': (
             [
-                _tn_av('TurnoverGrossOperatingRevenue'),
-                _tn_av('TurnoverRevenue'),
-            ],
-            _parse_decimal,
+                (_tn('TurnoverGrossOperatingRevenue'), _parse_decimal),
+                (_av('TurnoverGrossOperatingRevenue'), _parse_decimal),
+                (_tn('TurnoverRevenue'), _parse_decimal),
+                (_av('TurnoverRevenue'), _parse_decimal),
+            ]
         ),
         'other_operating_income': (
             [
-                _tn_av('OtherOperatingIncome'),
-                _tn_av('OtherOperatingIncomeFormat2'),
-            ],
-            _parse_decimal,
+                (_tn('OtherOperatingIncome'), _parse_decimal),
+                (_av('OtherOperatingIncome'), _parse_decimal),
+                (_tn('OtherOperatingIncomeFormat2'), _parse_decimal),
+                (_av('OtherOperatingIncomeFormat2'), _parse_decimal),
+            ]
         ),
         'cost_sales': (
             [
-                _tn_av('CostSales'),
-            ],
-            _parse_decimal,
+                (_tn('CostSales'), _parse_decimal),
+                (_av('CostSales'), _parse_decimal),
+            ]
         ),
         'gross_profit_loss': (
             [
-                _tn_av('GrossProfitLoss'),
-            ],
-            _parse_decimal,
+                (_tn('GrossProfitLoss'), _parse_decimal),
+                (_av('GrossProfitLoss'), _parse_decimal),
+            ]
         ),
         'administrative_expenses': (
             [
-                _tn_av('AdministrativeExpenses'),
-            ],
-            _parse_decimal,
+                (_tn('AdministrativeExpenses'), _parse_decimal),
+                (_av('AdministrativeExpenses'), _parse_decimal),
+            ]
         ),
         'raw_materials_consumables': (
             [
-                _tn_av('RawMaterialsConsumables'),
-                _tn_av('RawMaterialsConsumablesUsed'),
-            ],
-            _parse_decimal,
+                (_tn('RawMaterialsConsumables'), _parse_decimal),
+                (_av('RawMaterialsConsumables'), _parse_decimal),
+                (_tn('RawMaterialsConsumablesUsed'), _parse_decimal),
+                (_av('RawMaterialsConsumablesUsed'), _parse_decimal),
+            ]
         ),
         'staff_costs': (
             [
-                _tn_av('StaffCosts'),
-                _tn_av('StaffCostsEmployeeBenefitsExpense'),
-            ],
-            _parse_decimal,
+                (_tn('StaffCosts'), _parse_decimal),
+                (_av('StaffCosts'), _parse_decimal),
+                (_tn('StaffCostsEmployeeBenefitsExpense'), _parse_decimal),
+                (_av('StaffCostsEmployeeBenefitsExpense'), _parse_decimal),
+            ]
         ),
         'depreciation_other_amounts_written_off_tangible_intangible_fixed_assets': (
             [
-                _tn_av('DepreciationOtherAmountsWrittenOffTangibleIntangibleFixedAssets'),
-                _tn_av('DepreciationAmortisationImpairmentExpense'),
-            ],
-            _parse_decimal,
+                (_tn('DepreciationOtherAmountsWrittenOffTangibleIntangibleFixedAssets'), _parse_decimal),
+                (_av('DepreciationOtherAmountsWrittenOffTangibleIntangibleFixedAssets'), _parse_decimal),
+                (_tn('DepreciationAmortisationImpairmentExpense'), _parse_decimal),
+                (_av('DepreciationAmortisationImpairmentExpense'), _parse_decimal),
+            ]
         ),
         'other_operating_charges_format2': (
             [
-                _tn_av('OtherOperatingChargesFormat2'),
-                _tn_av('OtherOperatingExpensesFormat2'),
-            ],
-            _parse_decimal,
+                (_tn('OtherOperatingChargesFormat2'), _parse_decimal),
+                (_av('OtherOperatingChargesFormat2'), _parse_decimal),
+                (_tn('OtherOperatingExpensesFormat2'), _parse_decimal),
+                (_av('OtherOperatingExpensesFormat2'), _parse_decimal),
+            ]
         ),
         'operating_profit_loss': (
             [
-                _tn_av('OperatingProfitLoss'),
-            ],
-            _parse_decimal,
+                (_tn('OperatingProfitLoss'), _parse_decimal),
+                (_av('OperatingProfitLoss'), _parse_decimal),
+            ]
         ),
         'profit_loss_on_ordinary_activities_before_tax': (
             [
-                _tn_av('ProfitLossOnOrdinaryActivitiesBeforeTax'),
-            ],
-            _parse_decimal,
+                (_tn('ProfitLossOnOrdinaryActivitiesBeforeTax'), _parse_decimal),
+                (_av('ProfitLossOnOrdinaryActivitiesBeforeTax'), _parse_decimal),
+            ]
         ),
         'tax_on_profit_or_loss_on_ordinary_activities': (
             [
-                _tn_av('TaxOnProfitOrLossOnOrdinaryActivities'),
-                _tn_av('TaxTaxCreditOnProfitOrLossOnOrdinaryActivities'),
-            ],
-            _parse_decimal,
+                (_tn('TaxOnProfitOrLossOnOrdinaryActivities'), _parse_decimal),
+                (_av('TaxOnProfitOrLossOnOrdinaryActivities'), _parse_decimal),
+                (_tn('TaxTaxCreditOnProfitOrLossOnOrdinaryActivities'), _parse_decimal),
+                (_av('TaxTaxCreditOnProfitOrLossOnOrdinaryActivities'), _parse_decimal),
+            ]
         ),
         'profit_loss_for_period': (
             [
-                _tn_av('ProfitLoss'),
-                _tn_av('ProfitLossForPeriod'),
-            ],
-            _parse_decimal,
+                (_tn('ProfitLoss'), _parse_decimal),
+                (_av('ProfitLoss'), _parse_decimal),
+                (_tn('ProfitLossForPeriod'), _parse_decimal),
+                (_av('ProfitLossForPeriod'), _parse_decimal),
+            ]
         ),
     }
 
+    ALL_MAPPINGS = dict(**GENERAL_XPATH_MAPPINGS, **PERIODICAL_XPATH_MAPPINGS)
+
+    TAG_NAME_TESTS = {
+        test.name: (name, priority, test, parser)
+        for (name, tests) in ALL_MAPPINGS.items()
+        for (priority, (test, parser)) in enumerate(tests)
+        if isinstance(test, _tn)
+    }
+
+    ATTRIBUTE_VALUE_TESTS = {
+        test.name: (name, priority, test, parser)
+        for (name, tests) in ALL_MAPPINGS.items()
+        for (priority, (test, parser)) in enumerate(tests)
+        if isinstance(test, _av)
+    }
+
+    CUSTOM_TESTS = tuple(
+        (name, priority, test, parser)
+        for (name, tests) in ALL_MAPPINGS.items()
+        for (priority, (test, parser)) in enumerate(tests)
+        if isinstance(test, _custom)
+    )
+
     # columns names used to store the companies financial attributes
     columns = (
         ['run_code', 'company_id', 'date', 'file_type', 'taxonomy']
         + [key for key in GENERAL_XPATH_MAPPINGS.keys()]
         + ['period_start', 'period_end'] + [key for key in PERIODICAL_XPATH_MAPPINGS.keys()]
     )
 
     def xbrl_to_rows(name, xbrl_xml_str):
 
-        def _general_attributes(xpath_expressions, attr_type_maybe_list):
-            for i, xpath in enumerate(xpath_expressions):
-                attr_type = \
-                    attr_type_maybe_list[i] if isinstance(attr_type_maybe_list, list) else \
-                    attr_type_maybe_list
-                # Reversed so we choose the last non None in the document, which stands the best
-                # chance of being for the most recent period, so the current state of the company
-                for e in reversed(document.xpath(xpath)):
-                    yield _parse(e, e.text, attr_type)
-
-        def _periodical_attributes(xpath_expressions, attr_type_maybe_list):
-            for i, xpath in reversed(list(enumerate(xpath_expressions))):
-                attr_type = \
-                    attr_type_maybe_list[i] if isinstance(attr_type_maybe_list, list) else \
-                    attr_type_maybe_list
-                for e in reversed(document.xpath(xpath)):
-                    context_ref_attr = e.xpath('@contextRef')
-                    if not context_ref_attr:
-                        continue
-                    dates = context_dates[context_ref_attr[0]]
-                    if not dates:
-                        continue
-                    value = _parse(e, e.text, attr_type)
-                    yield (dates, value)
-
         def _get_dates(context):
             instant_elements = context.xpath("./*[local-name()='instant']")
             start_date_text_nodes = context.xpath("./*[local-name()='startDate']/text()")
             end_date_text_nodes = context.xpath("./*[local-name()='endDate']/text()")
             return \
                 (None, None) if context is None else \
                 (instant_elements[0].text.strip(), instant_elements[0].text.strip()) if instant_elements else \
@@ -371,62 +360,133 @@
         core_attributes = (
             run_code,
             company_id,
             _date(date),
             filetype,
             ';'.join(set(allowed_taxonomies) & set(document.getroot().nsmap.values())),
         )
+
+        # Mutable dictionaries to store the "priority" (lower is better) of a found value
+        general_attributes_with_priorities = {
+            name: (10, None)
+            for name in GENERAL_XPATH_MAPPINGS.keys()
+        }
+        periodic_attributes_with_priorities = defaultdict(lambda: {
+            name: (10, None)
+            for name in PERIODICAL_XPATH_MAPPINGS.keys()
+        })
+
+        def tag_name_tests(local_name):
+            try:
+                yield from (TAG_NAME_TESTS[local_name],)
+            except KeyError:
+                pass
+
+        def attribute_value_tests(attribute_value):
+            try:
+                yield from (ATTRIBUTE_VALUE_TESTS[attribute_value],)
+            except KeyError:
+                pass
+
+        def handle_general(element, local_name, attribute_value, context_ref, name, priority, test, parse):
+            best_priority, best_value = general_attributes_with_priorities[name]
+
+            if priority > best_priority:
+                return
+
+            for element in test.search(element, local_name, attribute_value, context_ref):
+                value = _parse(element, element.text, parse)
+                if value is not None:
+                    general_attributes_with_priorities[name] = (priority, value)
+                    break
+
+        def handle_periodic(element, local_name, attribute_value, context_ref, name, priority, test, parse):
+            if not context_ref:
+                return
+            dates = context_dates[context_ref]
+            if not dates:
+                return
+
+            for element in test.search(element, local_name, attribute_value, context_ref):
+                best_priority, best_value = periodic_attributes_with_priorities[dates][name]
+
+                if priority >= best_priority:
+                    return
+
+                value = _parse(element, element.text, parse)
+                if value is not None:
+                    periodic_attributes_with_priorities[dates][name] = (priority, value)
+                    break
+
+        for element in document.xpath('//*'):
+            _, _, local_name = element.tag.rpartition('}')
+            _, _, attribute_value = element.get('name', '').rpartition(':')
+            context_ref = element.get('contextRef', '')
+
+            for name, priority, test, parse in chain(tag_name_tests(local_name), attribute_value_tests(attribute_value), CUSTOM_TESTS):
+                handler = \
+                    handle_general if name in general_attributes_with_priorities else \
+                    handle_periodic
+
+                handler(element, local_name, attribute_value, context_ref, name, priority, test, parse)
+
         general_attributes = tuple(
-            next((value for value in _general_attributes(xpath_expressions, attribute) if value is not None), None)
-            for (name, (xpath_expressions, attribute)) in GENERAL_XPATH_MAPPINGS.items()
+            general_attributes_with_priorities[name][1]
+            for name in GENERAL_XPATH_MAPPINGS.keys()
         )
 
-        periodical_attributes_by_date_and_name = {
-            (dates, name): value
-            for (name, (xpath_expressions, attribute)) in PERIODICAL_XPATH_MAPPINGS.items()
-            for (dates, value) in _periodical_attributes(xpath_expressions, attribute)
-        }
-        period_dates = reversed(sorted(list(set(dates for (dates, _) in periodical_attributes_by_date_and_name.keys()))))
-        periods = tuple((
+        periods = tuple(
             (datetime.date.fromisoformat(period_start_end[0]), datetime.date.fromisoformat(period_start_end[1]))
-            + tuple((
-                periodical_attributes_by_date_and_name.get((period_start_end, name))
-                for name, _ in PERIODICAL_XPATH_MAPPINGS.items()
-            ))
-            for period_start_end in period_dates
-        ))
+            + tuple(
+                periodic_attributes[name][1]
+                for name in PERIODICAL_XPATH_MAPPINGS.keys()
+            )
+            for period_start_end, periodic_attributes in periodic_attributes_with_priorities.items()
+        )
+        sorted_periods = sorted(periods, key=lambda period: (period[0], period[1]), reverse=True)
 
         yield from \
-            ((core_attributes + general_attributes + period) for period in periods) if periods else \
+            ((core_attributes + general_attributes + period) for period in sorted_periods) if sorted_periods else \
             ((core_attributes + general_attributes + (None,) * (2 + len(PERIODICAL_XPATH_MAPPINGS))),)
 
     return tuple(columns), (
         row
         for name, _, chunks in stream_unzip(zip_bytes_iter)
         for row in xbrl_to_rows(name.decode(), BytesIO(b''.join(chunks)))
     )
 
 
 @contextmanager
 def stream_read_xbrl_daily_all(
     url='http://download.companieshouse.gov.uk/en_accountsdata.html',
     get_client=lambda: httpx.Client(transport=httpx.HTTPTransport(retries=3)),
+    allow_404=True,
 ):
     with get_client() as client:
         all_links = BeautifulSoup(httpx.get(url).content, "html.parser").find_all('a')
         zip_urls = [
             link.attrs['href'] if link.attrs['href'].strip().startswith('http://') or link.attrs['href'].strip().startswith('https://') else
             urllib.parse.urljoin(url, link.attrs['href'])
             for link in all_links
             if link.attrs.get('href', '').endswith('.zip')
         ]
 
         def rows():
             for zip_url in zip_urls:
                 with client.stream('GET', zip_url) as r:
+                    try:
+                        r.raise_for_status()
+                    except httpx.HTTPStatusError:
+                        if r.status_code != 404 or not allow_404:
+                            raise
+                        else:
+                            for _ in r.iter_bytes(chunk_size=65536):
+                                pass
+                            continue
+
                     _, rows = stream_read_xbrl_zip(r.iter_bytes(chunk_size=65536))
                     yield from rows
 
         # Allows us to get the columns before actually iterating the real data
         columns, _ = stream_read_xbrl_zip(())
 
         yield columns, rows()
```

### Comparing `stream_read_xbrl-0.0.8/.gitignore` & `stream_read_xbrl-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stream_read_xbrl-0.0.8/LICENSE` & `stream_read_xbrl-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stream_read_xbrl-0.0.8/README.md` & `stream_read_xbrl-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <!-- --8<-- [start:intro] -->
 # stream-read-xbrl
 
 [![PyPI version](https://badge.fury.io/py/stream-read-xbrl.svg)](https://pypi.org/project/stream-read-xbrl/) [![Tests](https://github.com/uktrade/stream-read-xbrl/actions/workflows/tests.yml/badge.svg)](https://github.com/uktrade/stream-read-xbrl/actions/workflows/tests.yml) [![Test Coverage](https://api.codeclimate.com/v1/badges/02144f986cd3eecf4a0b/test_coverage)](https://codeclimate.com/github/uktrade/stream-read-xbrl/badges)
 
 
 Python package to parse Companies House accounts data in a streaming way. It converts the zipped XBRL format that Companies House supplies into a single data frame of 37 columns.
+
+It takes approximately 60 to 90 seconds to convert a single day of Companies House accounts data using stream-read-xbrl. 
 <!-- --8<-- [end:intro] -->
 
 
 <!-- --8<-- [start:features] -->
 <!-- --8<-- [end:features] -->
 
 ---
```

### Comparing `stream_read_xbrl-0.0.8/pyproject.toml` & `stream_read_xbrl-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stream-read-xbrl"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python package to parse Companies House accounts data in a streaming way"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `stream_read_xbrl-0.0.8/PKG-INFO` & `stream_read_xbrl-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stream-read-xbrl
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package to parse Companies House accounts data in a streaming way
 Project-URL: Documentation, https://stream-read-xbrl.docs.data.trade.gov.uk/
 Project-URL: Source, https://github.com/uktrade/stream-read-xbrl
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,14 +24,16 @@
 <!-- --8<-- [start:intro] -->
 # stream-read-xbrl
 
 [![PyPI version](https://badge.fury.io/py/stream-read-xbrl.svg)](https://pypi.org/project/stream-read-xbrl/) [![Tests](https://github.com/uktrade/stream-read-xbrl/actions/workflows/tests.yml/badge.svg)](https://github.com/uktrade/stream-read-xbrl/actions/workflows/tests.yml) [![Test Coverage](https://api.codeclimate.com/v1/badges/02144f986cd3eecf4a0b/test_coverage)](https://codeclimate.com/github/uktrade/stream-read-xbrl/badges)
 
 
 Python package to parse Companies House accounts data in a streaming way. It converts the zipped XBRL format that Companies House supplies into a single data frame of 37 columns.
+
+It takes approximately 60 to 90 seconds to convert a single day of Companies House accounts data using stream-read-xbrl. 
 <!-- --8<-- [end:intro] -->
 
 
 <!-- --8<-- [start:features] -->
 <!-- --8<-- [end:features] -->
 
 ---
```

