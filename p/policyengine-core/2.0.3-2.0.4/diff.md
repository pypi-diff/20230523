# Comparing `tmp/policyengine-core-2.0.3.tar.gz` & `tmp/policyengine-core-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-core-2.0.3.tar", last modified: Fri Apr 14 10:08:15 2023, max compression
+gzip compressed data, was "policyengine-core-2.0.4.tar", last modified: Tue May 23 07:36:48 2023, max compression
```

## Comparing `policyengine-core-2.0.3.tar` & `policyengine-core-2.0.4.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.406809 policyengine-core-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 10:08:15.406809 policyengine-core-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.374809 policyengine-core-2.0.3/policyengine_core/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/charts/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/commons/formulas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/commons/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/commons/rates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/data/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/data/datasets/country_template_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/modelled_policies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.370809 policyengine-core-2.0.3/policyengine_core/country_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/parenting_allowance/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/parenting_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/parameters/general/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/general/age_of_majority.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/general/age_of_retirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core/country_template/parameters/taxes/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/taxes/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/taxes/income_tax_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/parameters/taxes/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.382809 policyengine-core-2.0.3/policyengine_core/country_template/reforms/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/add_dynamic_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/add_new_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/flat_social_security_contribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/modify_social_security_taxation.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/reforms/removal_basic_income.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.382809 policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/couple.json
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/housing.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/single.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.382809 policyengine-core-2.0.3/policyengine_core/country_template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/age.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/disposable_income.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.382809 policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/add_dynamic_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/add_new_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/modify_social_security_taxation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.382809 policyengine-core-2.0.3/policyengine_core/country_template/tests/situations/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/situations/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/situations/parenting_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/social_security_contribution.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/tests/test_microsimulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/country_template/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/benefits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/demographics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/housing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/income.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/country_template/variables/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_storage/in_memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_storage/on_disk_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_structures/parameter_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_structures/parameter_node_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_structures/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/data_structures/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/entities/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/entities/group_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/entities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/entities/role.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.386809 policyengine-core-2.0.3/policyengine_core/enums/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/enums/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/enums/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/enums/enum_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/cycle_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/empty_argument_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/nan_creation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/parameter_not_found_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/parameter_parsing_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/period_mismatch_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/situation_parsing_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/spiral_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/variable_name_conflict_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/errors/variable_not_found_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/experimental/memory_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/extension_template/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/local_benefit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.374809 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/local_town/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/local_town/child_allowance/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/local_town/child_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/local_town/child_allowance/index.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/parameters/local_town/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/extension_template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/extension_template/tests/local_benefit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.390809 policyengine-core-2.0.3/policyengine_core/holders/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/holders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/holders/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/holders/holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/model_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.394809 policyengine-core-2.0.3/policyengine_core/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/at_instant_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.394809 policyengine-core-2.0.3/policyengine_core/parameters/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/homogenize_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/interpolate_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/propagate_parameter_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/operations/uprate_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter_at_instant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter_node_at_instant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/parameter_scale_bracket.py
--rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/parameters/vectorial_parameter_node_at_instant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.394809 policyengine-core-2.0.3/policyengine_core/periods/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/periods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/periods/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/periods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/periods/instant_.py
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/periods/period_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.394809 policyengine-core-2.0.3/policyengine_core/populations/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/populations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/populations/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/populations/group_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/populations/population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/projectors/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/entity_to_person_projector.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/first_person_to_entity_projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/projectors/unique_role_to_entity_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/reforms/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/reforms/reform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/scripts/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/policyengine_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/run_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/run_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/scripts/simulation_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/simulations/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/individual_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/microsimulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43029 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32284 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/simulations/simulation_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.398809 policyengine-core-2.0.3/policyengine_core/taxbenefitsystems/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxbenefitsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxbenefitsystems/tax_benefit_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/taxscales/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/abstract_rate_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/abstract_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/amount_tax_scale_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/linear_average_rate_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/marginal_amount_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/marginal_rate_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/rate_tax_scale_like.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/single_amount_tax_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/taxscales/tax_scale_like.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tools/simulation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tools/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/tracers/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/computation_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/flat_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/full_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/performance_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/simple_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/trace_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/tracers/tracing_parameter_node_at_instant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/types/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/types/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/types/data_types/arrays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.402809 policyengine-core-2.0.3/policyengine_core/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/defined_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.406809 policyengine-core-2.0.3/policyengine_core/warnings/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/warnings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/warnings/libyaml_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/warnings/memory_config_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/policyengine_core/warnings/tempfile_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:08:15.378809 policyengine-core-2.0.3/policyengine_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-14 10:08:14.000000 policyengine-core-2.0.3/policyengine_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-04-14 10:08:15.000000 policyengine-core-2.0.3/policyengine_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:08:15.000000 policyengine-core-2.0.3/policyengine_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 10:08:15.000000 policyengine-core-2.0.3/policyengine_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-14 10:08:15.000000 policyengine-core-2.0.3/policyengine_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 10:08:15.000000 policyengine-core-2.0.3/policyengine_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:08:15.406809 policyengine-core-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-14 10:07:04.000000 policyengine-core-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/charts/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/commons/formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/commons/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/commons/rates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/data/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/data/datasets/country_template_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/modelled_policies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.671939 policyengine-core-2.0.4/policyengine_core/country_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/parenting_allowance/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/parenting_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/parameters/general/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/general/age_of_majority.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/general/age_of_retirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/parameters/taxes/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/taxes/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/taxes/income_tax_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/parameters/taxes/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/reforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/add_dynamic_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/add_new_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/flat_social_security_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/modify_social_security_taxation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/reforms/removal_basic_income.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/couple.json
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/housing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/single.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/country_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/disposable_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/add_dynamic_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/add_new_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/modify_social_security_taxation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/country_template/tests/situations/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/situations/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/situations/parenting_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/social_security_contribution.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/tests/test_microsimulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/country_template/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/housing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/income.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/country_template/variables/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_storage/in_memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_storage/on_disk_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_structures/parameter_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_structures/parameter_node_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_structures/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/data_structures/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/entities/group_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/entities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/entities/role.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.679939 policyengine-core-2.0.4/policyengine_core/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/enums/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/enums/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/enums/enum_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/cycle_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/empty_argument_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/nan_creation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/parameter_not_found_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/parameter_parsing_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/period_mismatch_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/situation_parsing_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/spiral_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/variable_name_conflict_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/errors/variable_not_found_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/experimental/memory_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/extension_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/local_benefit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.671939 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/local_town/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/local_town/child_allowance/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/local_town/child_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/local_town/child_allowance/index.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/parameters/local_town/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/extension_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/extension_template/tests/local_benefit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/holders/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/holders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/holders/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/holders/holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/model_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/at_instant_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.683939 policyengine-core-2.0.4/policyengine_core/parameters/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/homogenize_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/interpolate_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/propagate_parameter_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/operations/uprate_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter_at_instant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter_node_at_instant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/parameter_scale_bracket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9654 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/parameters/vectorial_parameter_node_at_instant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/periods/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/periods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/periods/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/periods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/periods/instant_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/periods/period_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/populations/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/populations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/populations/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/populations/group_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/populations/population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/projectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/entity_to_person_projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/first_person_to_entity_projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/projectors/unique_role_to_entity_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/reforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/reforms/reform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/scripts/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/policyengine_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/run_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/scripts/simulation_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/individual_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/microsimulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43029 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/simulations/simulation_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/taxbenefitsystems/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxbenefitsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxbenefitsystems/tax_benefit_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/taxscales/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/abstract_rate_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/abstract_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/amount_tax_scale_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/linear_average_rate_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/marginal_amount_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/marginal_rate_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/rate_tax_scale_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/single_amount_tax_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/taxscales/tax_scale_like.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.687940 policyengine-core-2.0.4/policyengine_core/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tools/simulation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tools/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/policyengine_core/tracers/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/computation_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/flat_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/full_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/performance_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/simple_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/trace_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/tracers/tracing_parameter_node_at_instant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/policyengine_core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/policyengine_core/types/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/types/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/types/data_types/arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/policyengine_core/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/defined_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20365 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/policyengine_core/warnings/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/warnings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/warnings/libyaml_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/warnings/memory_config_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/policyengine_core/warnings/tempfile_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:36:48.675939 policyengine-core-2.0.4/policyengine_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 07:36:48.000000 policyengine-core-2.0.4/policyengine_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:36:48.691939 policyengine-core-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-23 07:35:53.000000 policyengine-core-2.0.4/setup.py
```

### Comparing `policyengine-core-2.0.3/LICENSE` & `policyengine-core-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/PKG-INFO` & `policyengine-core-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-core
-Version: 2.0.3
+Version: 2.0.4
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-core-2.0.3/README.md` & `policyengine-core-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/charts/formatting.py` & `policyengine-core-2.0.4/policyengine_core/charts/formatting.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/commons/formulas.py` & `policyengine-core-2.0.4/policyengine_core/commons/formulas.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/commons/misc.py` & `policyengine-core-2.0.4/policyengine_core/commons/misc.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/commons/rates.py` & `policyengine-core-2.0.4/policyengine_core/commons/rates.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/__init__.py` & `policyengine-core-2.0.4/policyengine_core/country_template/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/data/datasets/country_template_dataset.py` & `policyengine-core-2.0.4/policyengine_core/country_template/data/datasets/country_template_dataset.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/entities.py` & `policyengine-core-2.0.4/policyengine_core/country_template/entities.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/parameters/taxes/social_security_contribution.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/parameters/taxes/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/reforms/add_dynamic_variable.py` & `policyengine-core-2.0.4/policyengine_core/country_template/reforms/add_dynamic_variable.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/reforms/add_new_tax.py` & `policyengine-core-2.0.4/policyengine_core/country_template/reforms/add_new_tax.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/reforms/flat_social_security_contribution.py` & `policyengine-core-2.0.4/policyengine_core/country_template/reforms/flat_social_security_contribution.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/reforms/modify_social_security_taxation.py` & `policyengine-core-2.0.4/policyengine_core/country_template/reforms/modify_social_security_taxation.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/reforms/removal_basic_income.py` & `policyengine-core-2.0.4/policyengine_core/country_template/reforms/removal_basic_income.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/situation_examples/couple.json` & `policyengine-core-2.0.4/policyengine_core/country_template/situation_examples/couple.json`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/age.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/age.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/basic_income.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/basic_income.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/disposable_income.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/disposable_income.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/housing_tax.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/housing_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/add_new_tax.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/add_new_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/reforms/modify_social_security_taxation.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/reforms/modify_social_security_taxation.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/situations/income_tax.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/situations/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/situations/parenting_allowance.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/situations/parenting_allowance.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/tests/social_security_contribution.yaml` & `policyengine-core-2.0.4/policyengine_core/country_template/tests/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/benefits.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/benefits.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/demographics.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/demographics.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/housing.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/housing.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/ids.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/ids.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/income.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/income.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/stats.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/stats.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/country_template/variables/taxes.py` & `policyengine-core-2.0.4/policyengine_core/country_template/variables/taxes.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/data/dataset.py` & `policyengine-core-2.0.4/policyengine_core/data/dataset.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/data_storage/in_memory_storage.py` & `policyengine-core-2.0.4/policyengine_core/data_storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/data_storage/on_disk_storage.py` & `policyengine-core-2.0.4/policyengine_core/data_storage/on_disk_storage.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/data_structures/parameter_metadata.py` & `policyengine-core-2.0.4/policyengine_core/data_structures/parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/data_structures/parameter_node_metadata.py` & `policyengine-core-2.0.4/policyengine_core/data_structures/parameter_node_metadata.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/entities/entity.py` & `policyengine-core-2.0.4/policyengine_core/entities/entity.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/entities/group_entity.py` & `policyengine-core-2.0.4/policyengine_core/entities/group_entity.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/entities/helpers.py` & `policyengine-core-2.0.4/policyengine_core/entities/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/entities/role.py` & `policyengine-core-2.0.4/policyengine_core/entities/role.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/enums/enum.py` & `policyengine-core-2.0.4/policyengine_core/enums/enum.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/enums/enum_array.py` & `policyengine-core-2.0.4/policyengine_core/enums/enum_array.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/__init__.py` & `policyengine-core-2.0.4/policyengine_core/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/empty_argument_error.py` & `policyengine-core-2.0.4/policyengine_core/errors/empty_argument_error.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/parameter_not_found_error.py` & `policyengine-core-2.0.4/policyengine_core/errors/parameter_not_found_error.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/parameter_parsing_error.py` & `policyengine-core-2.0.4/policyengine_core/errors/parameter_parsing_error.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/situation_parsing_error.py` & `policyengine-core-2.0.4/policyengine_core/errors/situation_parsing_error.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/errors/variable_not_found_error.py` & `policyengine-core-2.0.4/policyengine_core/errors/variable_not_found_error.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/experimental/memory_config.py` & `policyengine-core-2.0.4/policyengine_core/experimental/memory_config.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/extension_template/local_benefit.py` & `policyengine-core-2.0.4/policyengine_core/extension_template/local_benefit.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/extension_template/tests/local_benefit.yaml` & `policyengine-core-2.0.4/policyengine_core/extension_template/tests/local_benefit.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/holders/helpers.py` & `policyengine-core-2.0.4/policyengine_core/holders/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/holders/holder.py` & `policyengine-core-2.0.4/policyengine_core/holders/holder.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/model_api.py` & `policyengine-core-2.0.4/policyengine_core/model_api.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/__init__.py` & `policyengine-core-2.0.4/policyengine_core/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/at_instant_like.py` & `policyengine-core-2.0.4/policyengine_core/parameters/at_instant_like.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/config.py` & `policyengine-core-2.0.4/policyengine_core/parameters/config.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/helpers.py` & `policyengine-core-2.0.4/policyengine_core/parameters/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/operations/get_parameter.py` & `policyengine-core-2.0.4/policyengine_core/parameters/operations/get_parameter.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/operations/homogenize_parameters.py` & `policyengine-core-2.0.4/policyengine_core/parameters/operations/homogenize_parameters.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/operations/interpolate_parameters.py` & `policyengine-core-2.0.4/policyengine_core/parameters/operations/interpolate_parameters.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/operations/propagate_parameter_metadata.py` & `policyengine-core-2.0.4/policyengine_core/parameters/operations/propagate_parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/operations/uprate_parameters.py` & `policyengine-core-2.0.4/policyengine_core/parameters/operations/uprate_parameters.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/parameter.py` & `policyengine-core-2.0.4/policyengine_core/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/parameter_at_instant.py` & `policyengine-core-2.0.4/policyengine_core/parameters/parameter_at_instant.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/parameter_node.py` & `policyengine-core-2.0.4/policyengine_core/parameters/parameter_node.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/parameter_node_at_instant.py` & `policyengine-core-2.0.4/policyengine_core/parameters/parameter_node_at_instant.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/parameter_scale.py` & `policyengine-core-2.0.4/policyengine_core/parameters/parameter_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/parameters/vectorial_parameter_node_at_instant.py` & `policyengine-core-2.0.4/policyengine_core/parameters/vectorial_parameter_node_at_instant.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/periods/helpers.py` & `policyengine-core-2.0.4/policyengine_core/periods/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/periods/instant_.py` & `policyengine-core-2.0.4/policyengine_core/periods/instant_.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/periods/period_.py` & `policyengine-core-2.0.4/policyengine_core/periods/period_.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/populations/group_population.py` & `policyengine-core-2.0.4/policyengine_core/populations/group_population.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/populations/population.py` & `policyengine-core-2.0.4/policyengine_core/populations/population.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/projectors/entity_to_person_projector.py` & `policyengine-core-2.0.4/policyengine_core/projectors/entity_to_person_projector.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/projectors/first_person_to_entity_projector.py` & `policyengine-core-2.0.4/policyengine_core/projectors/first_person_to_entity_projector.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/projectors/helpers.py` & `policyengine-core-2.0.4/policyengine_core/projectors/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/projectors/projector.py` & `policyengine-core-2.0.4/policyengine_core/projectors/projector.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/reforms/reform.py` & `policyengine-core-2.0.4/policyengine_core/reforms/reform.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/__init__.py` & `policyengine-core-2.0.4/policyengine_core/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/assets/index.html` & `policyengine-core-2.0.4/policyengine_core/scripts/assets/index.html`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/policyengine_command.py` & `policyengine-core-2.0.4/policyengine_core/scripts/policyengine_command.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/run_data.py` & `policyengine-core-2.0.4/policyengine_core/scripts/run_data.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/run_test.py` & `policyengine-core-2.0.4/policyengine_core/scripts/run_test.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/scripts/simulation_generator.py` & `policyengine-core-2.0.4/policyengine_core/scripts/simulation_generator.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/simulations/helpers.py` & `policyengine-core-2.0.4/policyengine_core/simulations/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/simulations/individual_sim.py` & `policyengine-core-2.0.4/policyengine_core/simulations/individual_sim.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/simulations/microsimulation.py` & `policyengine-core-2.0.4/policyengine_core/simulations/microsimulation.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/simulations/simulation.py` & `policyengine-core-2.0.4/policyengine_core/simulations/simulation.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/simulations/simulation_builder.py` & `policyengine-core-2.0.4/policyengine_core/simulations/simulation_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,29 +700,31 @@
         for entity_name in self.entity_counts.keys():
             # Adjust counts
             self.axes_entity_counts[entity_name] = (
                 self.get_count(entity_name) * cell_count
             )
             # Adjust ids
             original_ids = self.get_ids(entity_name) * cell_count
-            indices = np.arange(
-                0, cell_count * self.entity_counts[entity_name]
+            # indices should be [0, 0, 0, 1, 1, 1, 2, 2, 2, ...] where each number is repeated axis_entity_count times
+            indices = np.repeat(
+                np.arange(0, cell_count), self.entity_counts[entity_name]
             )
             adjusted_ids = [
                 id + str(ix) for id, ix in zip(original_ids, indices)
             ]
             self.axes_entity_ids[entity_name] = adjusted_ids
             # Adjust roles
             original_roles = self.get_roles(entity_name)
             adjusted_roles = np.repeat(original_roles, cell_count)
             self.axes_roles[entity_name] = adjusted_roles
             # Adjust memberships, for group entities only
             if entity_name != self.persons_plural:
                 original_memberships = self.get_memberships(entity_name)
-                repeated_memberships = np.repeat(
+                # repeat membership, e.g. [1, 0] -> [1, 0, 1, 0, ...]
+                repeated_memberships = np.tile(
                     original_memberships, cell_count
                 )
                 indices = (
                     np.repeat(
                         np.arange(0, cell_count), len(original_memberships)
                     )
                     * self.entity_counts[entity_name]
```

### Comparing `policyengine-core-2.0.3/policyengine_core/taxbenefitsystems/tax_benefit_system.py` & `policyengine-core-2.0.4/policyengine_core/taxbenefitsystems/tax_benefit_system.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/__init__.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/abstract_rate_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/abstract_rate_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/abstract_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/abstract_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/amount_tax_scale_like.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/amount_tax_scale_like.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/helpers.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/linear_average_rate_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/linear_average_rate_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/marginal_amount_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/marginal_amount_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/marginal_rate_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/marginal_rate_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/rate_tax_scale_like.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/rate_tax_scale_like.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/single_amount_tax_scale.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/single_amount_tax_scale.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/taxscales/tax_scale_like.py` & `policyengine-core-2.0.4/policyengine_core/taxscales/tax_scale_like.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tools/__init__.py` & `policyengine-core-2.0.4/policyengine_core/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tools/simulation_dumper.py` & `policyengine-core-2.0.4/policyengine_core/tools/simulation_dumper.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tools/test_runner.py` & `policyengine-core-2.0.4/policyengine_core/tools/test_runner.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/computation_log.py` & `policyengine-core-2.0.4/policyengine_core/tracers/computation_log.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/flat_trace.py` & `policyengine-core-2.0.4/policyengine_core/tracers/flat_trace.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/full_tracer.py` & `policyengine-core-2.0.4/policyengine_core/tracers/full_tracer.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/performance_log.py` & `policyengine-core-2.0.4/policyengine_core/tracers/performance_log.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/simple_tracer.py` & `policyengine-core-2.0.4/policyengine_core/tracers/simple_tracer.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/trace_node.py` & `policyengine-core-2.0.4/policyengine_core/tracers/trace_node.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/tracers/tracing_parameter_node_at_instant.py` & `policyengine-core-2.0.4/policyengine_core/tracers/tracing_parameter_node_at_instant.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/types/__init__.py` & `policyengine-core-2.0.4/policyengine_core/types/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/types/data_types/arrays.py` & `policyengine-core-2.0.4/policyengine_core/types/data_types/arrays.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/variables/config.py` & `policyengine-core-2.0.4/policyengine_core/variables/config.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/variables/defined_for.py` & `policyengine-core-2.0.4/policyengine_core/variables/defined_for.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/variables/helpers.py` & `policyengine-core-2.0.4/policyengine_core/variables/helpers.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/variables/typing.py` & `policyengine-core-2.0.4/policyengine_core/variables/typing.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core/variables/variable.py` & `policyengine-core-2.0.4/policyengine_core/variables/variable.py`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/policyengine_core.egg-info/PKG-INFO` & `policyengine-core-2.0.4/policyengine_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-core
-Version: 2.0.3
+Version: 2.0.4
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-core-2.0.3/policyengine_core.egg-info/SOURCES.txt` & `policyengine-core-2.0.4/policyengine_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `policyengine-core-2.0.3/setup.py` & `policyengine-core-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "types-requests==2.28.11.7",
     "types-setuptools==65.6.0.2",
     "types-urllib3==1.26.25.4",
 ]
 
 setup(
     name="policyengine-core",
-    version="2.0.3",
+    version="2.0.4",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

