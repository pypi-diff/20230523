# Comparing `tmp/aa_moonmining-1.9.0.tar.gz` & `tmp/aa_moonmining-1.9.1.tar.gz`

## Comparing `aa_moonmining-1.9.0.tar` & `aa_moonmining-1.9.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/__init__.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/admin.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/app_settings.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/apps.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/auth_hooks.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/constants.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/core.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/forms.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/helpers.py
--rw-r--r--   0        0        0    14543 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/managers.py
--rw-r--r--   0        0        0    57269 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/models.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/providers.py
--rw-r--r--   0        0        0   881820 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/swagger.json
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tasks.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/urls.py
--rw-r--r--   0        0        0    39111 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/views.py
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/django.pot
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19962 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_calculate_all.py
--rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_import_moons.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonmining_load_eve.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/management/commands/moonstuff_export_moons.py
--rw-r--r--   0        0        0    17813 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0001_initial.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0003_mining_ledger_reports.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0004_add_permission_moon_ledgers.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0005_make_pricing_more_flexible.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0006_add_labels.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/0007_add_localization.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/migrations/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/extractions.css
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/global.css
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/moonmining.css
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/moons.css
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/css/reports.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/_generic_modal_page.html
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/base.html
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/extractions.html
--rw-r--r--   0        0        0     8913 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/moons.html
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/reports.html
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/tests.html
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/base.html
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/content_base.html
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/extraction_details.html
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/extraction_ledger.html
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/loader_body.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/moon_details.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/upload_survey.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details.html
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head.html
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head_base.html
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_products.html
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger.html
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_head.html
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extractions_tab.html
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/global_js.html
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/location.html
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/menu.html
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details.html
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_moon.html
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_products.html
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moons_tab.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/upload_survey.html
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/value_estimate_legend.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templatetags/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/templatetags/moonmining.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/helpers.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_admin.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_commands.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_core.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_helpers.py
--rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_integration.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_managers.py
--rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_models.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_templatetags.py
--rw-r--r--   0        0        0    27002 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/test_views.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/allianceauth.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/esi.json
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0  1283587 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    17156 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/factories.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_many_moons.py
--rw-r--r--   0        0        0    99565 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.json
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/load_allianceauth.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_ids.csv
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_2.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_3.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/moons_for_import.csv
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/notification_details.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/notifications_full.json
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tests/testdata/survey_data.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tools/drop_tables.sql
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/moonmining/tools/esi_notes.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/LICENSE
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/README.md
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 aa_moonmining-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/__init__.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/admin.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/app_settings.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/apps.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/auth_hooks.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/constants.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/core.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/forms.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/helpers.py
+-rw-r--r--   0        0        0    14543 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/managers.py
+-rw-r--r--   0        0        0    57269 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/models.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/providers.py
+-rw-r--r--   0        0        0   881820 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/swagger.json
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tasks.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/urls.py
+-rw-r--r--   0        0        0    38642 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/views.py
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/django.pot
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19818 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19771 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19962 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    20049 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    19811 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/management/commands/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/management/commands/moonmining_calculate_all.py
+-rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/management/commands/moonmining_import_moons.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/management/commands/moonmining_load_eve.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/management/commands/moonstuff_export_moons.py
+-rw-r--r--   0        0        0    17813 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0003_mining_ledger_reports.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0004_add_permission_moon_ledgers.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0005_make_pricing_more_flexible.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0006_add_labels.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/0007_add_localization.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/migrations/__init__.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/css/extractions.css
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/css/global.css
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/css/moonmining.css
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/css/moons.css
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/_generic_modal_page.html
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/base.html
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/extractions.html
+-rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/moons.html
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/reports.html
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/tests.html
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/base.html
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/content_base.html
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/extraction_details.html
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/extraction_ledger.html
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/loader_body.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/moon_details.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/upload_survey.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details.html
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_head.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_head_base.html
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_products.html
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger.html
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_characters.html
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_head.html
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extractions_tab.html
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/global_js.html
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/location.html
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/menu.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moon_details.html
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moon_details_moon.html
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moon_details_products.html
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moons_tab.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_owned_value_tab.html
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_user_mining_tab.html
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/upload_survey.html
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/value_estimate_legend.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templatetags/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/templatetags/moonmining.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/helpers.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_admin.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_commands.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_core.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_helpers.py
+-rw-r--r--   0        0        0     8354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_integration.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_managers.py
+-rw-r--r--   0        0        0    47598 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_models.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_templatetags.py
+-rw-r--r--   0        0        0    26354 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/test_views.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/allianceauth.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    29013 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/esi.json
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0  1283587 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    17156 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/factories.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/generate_many_moons.py
+-rw-r--r--   0        0        0    99565 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/generate_moons.json
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/generate_moons.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/load_allianceauth.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/moon_ids.csv
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/moon_survey_input_2.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/moon_survey_input_3.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/moons_for_import.csv
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/notification_details.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/notifications_full.json
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tests/testdata/survey_data.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tools/drop_tables.sql
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/moonmining/tools/esi_notes.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/LICENSE
+-rw-r--r--   0        0        0    13099 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/README.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    14517 2020-02-02 00:00:00.000000 aa_moonmining-1.9.1/PKG-INFO
```

### Comparing `aa_moonmining-1.9.0/moonmining/admin.py` & `aa_moonmining-1.9.1/moonmining/admin.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/app_settings.py` & `aa_moonmining-1.9.1/moonmining/app_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from app_utils.django import clean_setting
+from app_utils.app_settings import clean_setting
 
-# Number of hours an extractions that has passed its ready time is still shown
-# on the upcoming extractions tab
 MOONMINING_COMPLETED_EXTRACTIONS_HOURS_UNTIL_STALE = clean_setting(
     "MOONMINING_COMPLETED_EXTRACTIONS_HOURS_UNTIL_STALE", 12
 )
+"""Number of hours an extractions that has passed its ready time is still shown
+on the upcoming extractions tab.
+"""
 
-# Reprocessing yield used for calculating reprocess prices
 MOONMINING_REPROCESSING_YIELD = clean_setting("MOONMINING_REPROCESSING_YIELD", 0.85)
+"""Reprocessing yield used for calculating reprocess prices."""
 
-# Whether to calculate prices from reprocessed materials or not.
-# Will use direct ore prices when switched off
 MOONMINING_USE_REPROCESS_PRICING = clean_setting(
     "MOONMINING_USE_REPROCESS_PRICING", False
 )
+"""Whether to calculate prices from reprocessed materials or not.
+Will use direct ore prices when switched off.
+"""
 
-# Total ore volume per month used for calculating moon values.
 MOONMINING_VOLUME_PER_DAY = clean_setting("MOONMINING_VOLUME_PER_DAY", 960_400)
 MOONMINING_DAYS_PER_MONTH = clean_setting("MOONMINING_DAYS_PER_MONTH", 30.4)
 MOONMINING_VOLUME_PER_MONTH = MOONMINING_VOLUME_PER_DAY * MOONMINING_DAYS_PER_MONTH
+"""Total ore volume per month used for calculating moon values."""
 
-# whether admins will get notifications about important events like
-# when someone adds a new owner
 MOONMINING_ADMIN_NOTIFICATIONS_ENABLED = clean_setting(
     "MOONMINING_ADMIN_NOTIFICATIONS_ENABLED", True
 )
+"""Whether admins will get notifications about important events like
+when someone adds a new owner.
+"""
 
-# whether uploaded survey are automatically overwritten by product estimates from
-# extractions to keep the moon values current
 MOONMINING_OVERWRITE_SURVEYS_WITH_ESTIMATES = clean_setting(
     "MOONMINING_OVERWRITE_SURVEYS_WITH_ESTIMATES", False
 )
+"""whether uploaded survey are automatically overwritten by product estimates from
+extractions to keep the moon values current."""
```

### Comparing `aa_moonmining-1.9.0/moonmining/auth_hooks.py` & `aa_moonmining-1.9.1/moonmining/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/constants.py` & `aa_moonmining-1.9.1/moonmining/constants.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/core.py` & `aa_moonmining-1.9.1/moonmining/core.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/managers.py` & `aa_moonmining-1.9.1/moonmining/managers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/models.py` & `aa_moonmining-1.9.1/moonmining/models.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/swagger.json` & `aa_moonmining-1.9.1/moonmining/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tasks.py` & `aa_moonmining-1.9.1/moonmining/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/urls.py` & `aa_moonmining-1.9.1/moonmining/urls.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/views.py` & `aa_moonmining-1.9.1/moonmining/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime as dt
 from enum import Enum
 from typing import Union
 
 from django_datatables_view.base_datatable_view import BaseDatatableView
 
+from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.auth.mixins import LoginRequiredMixin, PermissionRequiredMixin
 from django.contrib.auth.models import User
 from django.db import models
 from django.db.models import (
     Case,
     Count,
@@ -20,43 +21,41 @@
     Q,
     Subquery,
     Sum,
     Value,
     When,
 )
 from django.db.models.functions import Coalesce, Concat
-from django.http import HttpResponseNotFound, JsonResponse
-from django.shortcuts import redirect, render
+from django.http import JsonResponse
+from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
 from django.utils.html import format_html, strip_tags
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.cache import cache_page
 from esi.decorators import token_required
 
-from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.eveonline.evelinks import dotlan
 from allianceauth.eveonline.models import EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.allianceauth import notify_admins
 from app_utils.logging import LoggerAddTag
-from app_utils.messages import messages_plus
 from app_utils.views import fontawesome_modal_button_html, link_html, yesno_str
 
 from . import __title__, helpers, tasks
 from .app_settings import (
     MOONMINING_ADMIN_NOTIFICATIONS_ENABLED,
     MOONMINING_COMPLETED_EXTRACTIONS_HOURS_UNTIL_STALE,
     MOONMINING_REPROCESSING_YIELD,
     MOONMINING_USE_REPROCESS_PRICING,
     MOONMINING_VOLUME_PER_MONTH,
 )
 from .constants import DATE_FORMAT, DATETIME_FORMAT, EveGroupId
 from .forms import MoonScanForm
-from .helpers import HttpResponseUnauthorized
+from .helpers import user_perms_lookup
 from .models import EveOreType, Extraction, Moon, Owner, Refinery
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class ExtractionsCategory(str, helpers.EnumToDict, Enum):
     UPCOMING = "upcoming"
@@ -243,31 +242,27 @@
         )
     return JsonResponse(data, safe=False)
 
 
 @login_required
 @permission_required(["moonmining.extractions_access", "moonmining.basic_access"])
 def extraction_details(request, extraction_pk: int):
-    try:
-        extraction = (
-            Extraction.objects.annotate_volume()
-            .select_related(
-                "refinery",
-                "refinery__moon",
-                "refinery__moon__eve_moon",
-                "refinery__moon__eve_moon__eve_planet__eve_solar_system",
-                "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
-                "canceled_by",
-                "fractured_by",
-                "started_by",
-            )
-            .get(pk=extraction_pk)
-        )
-    except Extraction.DoesNotExist:
-        return HttpResponseNotFound()
+    extraction = get_object_or_404(
+        Extraction.objects.annotate_volume().select_related(
+            "refinery",
+            "refinery__moon",
+            "refinery__moon__eve_moon",
+            "refinery__moon__eve_moon__eve_planet__eve_solar_system",
+            "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
+            "canceled_by",
+            "fractured_by",
+            "started_by",
+        ),
+        pk=extraction_pk,
+    )
     context = {
         "page_title": (
             f"{extraction.refinery.moon} "
             f"| {extraction.chunk_arrival_at.strftime(DATE_FORMAT)}"
         ),
         "extraction": extraction,
     }
@@ -284,27 +279,23 @@
     [
         "moonmining.extractions_access",
         "moonmining.basic_access",
         "moonmining.view_moon_ledgers",
     ]
 )
 def extraction_ledger(request, extraction_pk: int):
-    try:
-        extraction = (
-            Extraction.objects.all()
-            .select_related(
-                "refinery",
-                "refinery__moon",
-                "refinery__moon__eve_moon__eve_planet__eve_solar_system",
-                "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
-            )
-            .get(pk=extraction_pk)
-        )
-    except Extraction.DoesNotExist:
-        return HttpResponseNotFound()
+    extraction = get_object_or_404(
+        Extraction.objects.all().select_related(
+            "refinery",
+            "refinery__moon",
+            "refinery__moon__eve_moon__eve_planet__eve_solar_system",
+            "refinery__moon__eve_moon__eve_planet__eve_solar_system__eve_constellation__eve_region",
+        ),
+        pk=extraction_pk,
+    )
     ledger = extraction.ledger.select_related(
         "character", "corporation", "user__profile__main_character", "ore_type"
     )
     total_value = ledger.aggregate(Sum(F("total_price")))["total_price__sum"]
     total_volume = ledger.aggregate(Sum(F("total_volume")))["total_volume__sum"]
     sum_price = ExpressionWrapper(
         F("quantity") * Coalesce(F("unit_price"), 0), output_field=FloatField()
@@ -349,20 +340,24 @@
         return render(request, "moonmining/_generic_modal_page.html", context)
     return render(request, "moonmining/modals/extraction_ledger.html", context)
 
 
 @login_required()
 @permission_required("moonmining.basic_access")
 def moons(request):
+    user_perms = user_perms_lookup(
+        request.user, ["moonmining.extractions_access", "moonmining.view_all_moons"]
+    )
     context = {
         "page_title": _("Moons"),
         "MoonsCategory": MoonsCategory.to_dict(),
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
+        "user_perms": user_perms,
     }
     return render(request, "moonmining/moons.html", context)
 
 
 class MoonListJson(PermissionRequiredMixin, LoginRequiredMixin, BaseDatatableView):
     model = Moon
     permission_required = "moonmining.basic_access"
@@ -450,22 +445,20 @@
             )
             .annotate(
                 rarity_class_str=Concat(
                     Value("R"), F("rarity_class"), output_field=models.CharField()
                 )
             )
         )
-        if (
-            category == MoonsCategory.ALL
-            and user.has_perm("moonmining.extractions_access")
-            and user.has_perm("moonmining.view_all_moons")
-        ):
+        if category == MoonsCategory.ALL and user.has_perm("moonmining.view_all_moons"):
             pass
-        elif category == MoonsCategory.OURS and user.has_perm(
-            "moonmining.extractions_access"
+        elif (
+            category == MoonsCategory.OURS
+            and user.has_perm("moonmining.extractions_access")
+            or user.has_perm("moonmining.view_all_moons")
         ):
             moon_query = moon_query.filter(refinery__isnull=False)
         elif category == MoonsCategory.UPLOADS and user.has_perm(
             "moonmining.upload_moon_scan"
         ):
             moon_query = moon_query.filter(products_updated_by=user)
         else:
@@ -578,26 +571,23 @@
         if column == "region_name":
             return region.name
         if column == "constellation_name":
             return constellation.name
         return None
 
     def _render_details(self, row):
-        has_details_access = self.request.user.has_perm(
-            "moonmining.extractions_access"
-        ) or self.request.user.has_perm("moonmining.view_all_moons")
-        if has_details_access:
+        details_html = ""
+        if self.request.user.has_perm("moonmining.extractions_access"):
             details_html = (
                 extraction_details_button_html(row.extraction_pk) + " "
                 if row.extraction_pk
                 else ""
             )
-            details_html += moon_details_button_html(row)
-            return details_html
-        return ""
+        details_html += moon_details_button_html(row)
+        return details_html
 
     def _render_refinery(self, row, column) -> Union[str, dict]:
         if row.has_refinery:
             refinery = row.refinery
             refinery_html = refinery.name_html()
             refinery_name = refinery.name
             corporation_name = refinery.owner.name
@@ -654,30 +644,28 @@
             elif column == "label_name":
                 options = qs.exclude(label__isnull=True).values_list(
                     "label__name", flat=True
                 )
             elif column == "has_refinery_str":
                 options = qs.values_list("has_refinery_str", flat=True)
             elif column == "has_extraction_str":
-                options = qs.values_list("has_extraction_str", flat=True)
+                if request.user.has_perm("moonmining.extractions_access"):
+                    options = qs.values_list("has_extraction_str", flat=True)
+                else:
+                    options = []
             else:
                 options = [f"** ERROR: Invalid column name '{column}' **"]
             result[column] = sorted(list(set(options)), key=str.casefold)
     return JsonResponse(result, safe=False)
 
 
 @login_required
 @permission_required("moonmining.basic_access")
 def moon_details(request, moon_pk: int):
-    try:
-        moon = Moon.objects.selected_related_defaults().get(pk=moon_pk)
-    except Moon.DoesNotExist:
-        return HttpResponseNotFound()
-    if not request.user.has_perm("moonmining.extractions_access"):
-        return HttpResponseUnauthorized()
+    moon = get_object_or_404(Moon.objects.selected_related_defaults(), pk=moon_pk)
     context = {
         "page_title": moon.name,
         "moon": moon,
         "use_reprocess_pricing": MOONMINING_USE_REPROCESS_PRICING,
         "reprocessing_yield": MOONMINING_REPROCESSING_YIELD * 100,
         "total_volume_per_month": MOONMINING_VOLUME_PER_MONTH / 1000000,
     }
@@ -688,20 +676,18 @@
     return render(request, "moonmining/modals/moon_details.html", context)
 
 
 @permission_required(["moonmining.add_refinery_owner", "moonmining.basic_access"])
 @token_required(scopes=Owner.esi_scopes())  # type: ignore
 @login_required
 def add_owner(request, token):
-    try:
-        character_ownership = request.user.character_ownerships.select_related(
-            "character"
-        ).get(character__character_id=token.character_id)
-    except CharacterOwnership.DoesNotExist:
-        return HttpResponseNotFound()
+    character_ownership = get_object_or_404(
+        request.user.character_ownerships.select_related("character"),
+        character__character_id=token.character_id,
+    )
     try:
         corporation = EveCorporationInfo.objects.get(
             corporation_id=character_ownership.character.corporation_id
         )
     except EveCorporationInfo.DoesNotExist:
         corporation = EveCorporationInfo.objects.create_corporation(
             corp_id=character_ownership.character.corporation_id
@@ -709,15 +695,15 @@
         corporation.save()
 
     owner = Owner.objects.update_or_create(
         corporation=corporation,
         defaults={"character_ownership": character_ownership},
     )[0]
     tasks.update_owner.delay(owner.pk)
-    messages_plus.success(request, f"Update of refineries started for {owner}.")
+    messages.success(request, f"Update of refineries started for {owner}.")
     if MOONMINING_ADMIN_NOTIFICATIONS_ENABLED:
         notify_admins(
             message=_(
                 "%(corporation)s was added as new owner by %(user)s."
                 % {"corporation": owner, "user": request.user}
             ),
             title=f"{__title__}: Owner added: {owner}",
@@ -730,23 +716,23 @@
 def upload_survey(request):
     context = {"page_title": _("Upload Moon Surveys")}
     if request.method == "POST":
         form = MoonScanForm(request.POST)
         if form.is_valid():
             scans = request.POST["scan"]
             tasks.process_survey_input.delay(scans, request.user.pk)
-            messages_plus.success(
+            messages.success(
                 request,
                 _(
                     "Your scan has been submitted for processing. "
                     "You will receive a notification once processing is complete."
                 ),
             )
         else:
-            messages_plus.error(
+            messages.error(
                 request,
                 _(
                     "Oh No! Something went wrong with your moon scan submission. "
                     "Please try again."
                 ),
             )
         return redirect("moonmining:moons")
```

### Comparing `aa_moonmining-1.9.0/moonmining/locale/django.pot` & `aa_moonmining-1.9.1/moonmining/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/de/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/en/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/es/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/fr_FR/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/it_IT/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/ja/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/ko_KR/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/ru/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/uk/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_moonmining-1.9.1/moonmining/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_calculate_all.py` & `aa_moonmining-1.9.1/moonmining/management/commands/moonmining_calculate_all.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_import_moons.py` & `aa_moonmining-1.9.1/moonmining/management/commands/moonmining_import_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/management/commands/moonmining_load_eve.py` & `aa_moonmining-1.9.1/moonmining/management/commands/moonmining_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/management/commands/moonstuff_export_moons.py` & `aa_moonmining-1.9.1/moonmining/management/commands/moonstuff_export_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0001_initial.py` & `aa_moonmining-1.9.1/moonmining/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0002_add_mining_ledger.py` & `aa_moonmining-1.9.1/moonmining/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0003_mining_ledger_reports.py` & `aa_moonmining-1.9.1/moonmining/migrations/0003_mining_ledger_reports.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0004_add_permission_moon_ledgers.py` & `aa_moonmining-1.9.1/moonmining/migrations/0004_add_permission_moon_ledgers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0005_make_pricing_more_flexible.py` & `aa_moonmining-1.9.1/moonmining/migrations/0005_make_pricing_more_flexible.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0006_add_labels.py` & `aa_moonmining-1.9.1/moonmining/migrations/0006_add_labels.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/migrations/0007_add_localization.py` & `aa_moonmining-1.9.1/moonmining/migrations/0007_add_localization.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/css/extractions.css` & `aa_moonmining-1.9.1/moonmining/static/moonmining/css/extractions.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/css/global.css` & `aa_moonmining-1.9.1/moonmining/static/moonmining/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/css/moonmining.css` & `aa_moonmining-1.9.1/moonmining/static/moonmining/css/moonmining.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/css/reports.css` & `aa_moonmining-1.9.1/moonmining/static/moonmining/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif` & `aa_moonmining-1.9.1/moonmining/static/moonmining/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif` & `aa_moonmining-1.9.1/moonmining/static/moonmining/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js` & `aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js` & `aa_moonmining-1.9.1/moonmining/static/moonmining/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/base.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/extractions.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/extractions.html`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     {% include "moonmining/modals/base.html" with modal_id="modalExtractionDetails" modal_content_id="modalExtractionDetailsContent" %}
     {% include "moonmining/modals/base.html" with modal_id="modalExtractionLedger" modal_content_id="modalExtractionLedgerContent" modal_size="modal-xl" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {{ block.super }}
     <script type="text/javascript">
+        "use_strict";
         $(function() {
-            var def = {
+            let def = {
                 ajax: {
                     url: '',
                     dataSrc: '',
                     cache: true
                 },
                 columns: [
                     {
@@ -115,31 +116,31 @@
                             title: "{% translate 'Status' %}"
                         }
                     ],
                     bootstrap: true,
                     autoSize: false
                 },
                 footerCallback: function (row, data, start, end, display) {
-                    var api = this.api(), data;
+                    let api = this.api();
 
                     dataTableFooterSumColumn(api, 4);
                     dataTableFooterSumColumn(api, 5, 'isk');
                     dataTableFooterSumColumn(api, 6, 'isk');
                 }
             };
 
             /* upcoming extractions*/
             def.ajax.url = '{% url "moonmining:extractions_data" ExtractionsCategory.UPCOMING %}'
             def.order = [ [0, "asc"] ]
-            var table = $('#table_{{ ExtractionsCategory.UPCOMING }}').DataTable(def);
+            $('#table_{{ ExtractionsCategory.UPCOMING }}').DataTable(def);
 
             /* past extractions */
             def.ajax.url = '{% url "moonmining:extractions_data" ExtractionsCategory.PAST %}'
             def.order = [ [0, "desc"] ]
-            var table = $('#table_{{ ExtractionsCategory.PAST }}').DataTable(def);
+            $('#table_{{ ExtractionsCategory.PAST }}').DataTable(def);
 
             $('#myTabs a[href="#tab_{{ ExtractionsCategory.UPCOMING }}"]').tab('show')
 
             handle_modal_events("modalMoonDetails", "modalMoonDetailsContent")
             handle_modal_events("modalExtractionDetails", "modalExtractionDetailsContent")
             handle_modal_events("modalExtractionLedger", "modalExtractionLedgerContent")
         });
```

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/moons.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/moons.html`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                 {% translate "Upload Moon Surveys" %}
             </button>
         {% endif %}
     </span>
 
     <!-- Nav tabs -->
     <ul id="myTabs" class="nav nav-tabs" role="tablist">
-        {% if perms.moonmining.extractions_access %}
+        {% if perms.moonmining.extractions_access or perms.moonmining.view_all_moons %}
             <li role="presentation">
                 <a href="#tab_{{ MoonsCategory.OURS }}" aria-controls="tab_{{ MoonsCategory.OURS }}" role="tab" data-toggle="tab">{% translate "Owned Moons" %}</a>
             </li>
         {% endif %}
         {% if perms.moonmining.view_all_moons %}
             <li role="presentation">
                 <a href="#tab_{{ MoonsCategory.ALL }}" aria-controls="tab_{{ MoonsCategory.ALL }}" role="tab" data-toggle="tab">{% translate "All Moons" %}</a>
@@ -43,24 +43,77 @@
 
     {% if perms.moonmining.extractions_access or perms.moonmining.view_all_moons %}
         <script>var defaultTab = "tab_{{MoonsCategory.OURS}}";</script>
     {% elif perms.moonmining.upload_moon_scan %}
         <script>var defaultTab = "tab_{{MoonsCategory.UPLOADS}}";</script>
     {% endif %}
 
+    {{ user_perms|json_script:"user-perms" }}
+
     <!-- Modals -->
     {% include "moonmining/modals/base.html" with modal_id="modalUploadSurvey" modal_content_id="modalUploadSurveyContent" %}
     {% include "moonmining/modals/base.html" with modal_id="modalMoonDetails" modal_content_id="modalMoonDetailsContent" %}
     {% include "moonmining/modals/base.html" with modal_id="modalExtractionDetails" modal_content_id="modalExtractionDetailsContent" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {{ block.super }}
     <script type="text/javascript">
+        "use_strict";
+        const perms = JSON.parse(document.getElementById('user-perms').textContent);
         $(function(){
+            let dropDownColumns = [
+                {
+                    idx: 10,
+                    title: "{% translate 'Alliance' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 9,
+                    title: "{% translate 'Corporation' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 15,
+                    title: "{% translate 'Region' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 13,
+                    title: "{% translate 'Constellation' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 7,
+                    title: "{% translate 'System' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 11,
+                    title: "{% translate 'Rarity' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 14,
+                    title: "{% translate 'Label' %}",
+                    maxWidth: "10em"
+                },
+                {
+                    idx: 8,
+                    title: "{% translate 'Owned?' %}",
+                    maxWidth: "10em"
+                }
+            ];
+            if (perms.moonmining.extractions_access) {
+                dropDownColumns.push({
+                    idx: 12,
+                    title: "{% translate 'Extraction?' %}",
+                    maxWidth: "10em"
+                });
+            }
             const def = {
                 ajax: {
                     url: '',
                     dataSrc: 'data',
                     cache: true
                 },
                 columns: [
@@ -97,61 +150,15 @@
                 pageLength: DEFAULT_PAGE_LENGTH,
                 order: [ [0, "asc"] ],
                 columnDefs: [
                     { "orderable": false, "targets": [ 4, 6 ] },
                     { "visible": false, "targets": [ 7, 8, 9, 10, 11, 12, 13, 14, 15 ] },
                 ],
                 filterDropDown: {
-                    columns: [
-                        {
-                            idx: 10,
-                            title: "{% translate 'Alliance' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 9,
-                            title: "{% translate 'Corporation' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 15,
-                            title: "{% translate 'Region' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 13,
-                            title: "{% translate 'Constellation' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 7,
-                            title: "{% translate 'System' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 11,
-                            title: "{% translate 'Rarity' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 14,
-                            title: "{% translate 'Label' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 8,
-                            title: "{% translate 'Refinery?' %}",
-                            maxWidth: "10em"
-                        },
-                        {
-                            idx: 12,
-                            title: "{% translate 'Extraction?' %}",
-                            maxWidth: "10em"
-                        }
-                    ],
+                    columns: dropDownColumns,
                     bootstrap: true,
                     autoSize: false
                 }
             };
 
             /* our moons table */
             let def_ours = jQuery.extend(true, {}, def)
@@ -182,19 +189,19 @@
             let table_uploads = $('#table_{{ MoonsCategory.UPLOADS }}').DataTable(def_uploads);
             table_uploads.on( 'init', function () {
                 table_uploads.columns.adjust().draw();
                 $("#loader_{{ MoonsCategory.UPLOADS }}").hide();
                 $("#wrapper_{{ MoonsCategory.UPLOADS }}").show();
             } );
 
-            $('#myTabs a[href="#' + defaultTab + '"]').tab('show')
+            $('#myTabs a[href="#' + defaultTab + '"]').tab('show');
 
-            handle_modal_events("modalUploadSurvey", "modalUploadSurveyContent")
-            handle_modal_events("modalMoonDetails", "modalMoonDetailsContent")
-            handle_modal_events("modalExtractionDetails", "modalExtractionDetailsContent")
+            handle_modal_events("modalUploadSurvey", "modalUploadSurveyContent");
+            handle_modal_events("modalMoonDetails", "modalMoonDetailsContent");
+            handle_modal_events("modalExtractionDetails", "modalExtractionDetailsContent");
 
         });
     </script>
 {% endblock %}
 
 {% block extra_css %}
     {{ block.super }}
```

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/reports.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/reports.html`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     {% include "moonmining/modals/base.html" with modal_id="modalMoonDetails" modal_content_id="modalMoonDetailsContent" %}
 {% endblock %}
 
 {% block extra_javascript %}
     {{ block.super }}
     <script type="application/javascript" src="{% static 'moonmining/vendor/datatables/plugins/dataTables.rowGroup.min.js' %}"></script>
     <script type="text/javascript">
+        "use_strict";
         $(function() {
-            $('#table_owned_value').DataTable(
-                {
+            $('#table_owned_value').DataTable({
                 ajax: {
                     url: '{% url "moonmining:report_owned_value_data" %}',
                     dataSrc: '',
                     cache: true
                 },
                 columns: [
                     { data: 'corporation' },
@@ -91,16 +91,15 @@
                     const api = this.api();
 
                     dataTableFooterSumColumn(api, 5);
                     dataTableFooterSumColumn(api, 7, 'isk');
                 }
             });
 
-            $('#table_user_mining').DataTable(
-                {
+            $('#table_user_mining').DataTable({
                 ajax: {
                     url: '{% url "moonmining:report_user_mining_data" %}',
                     dataSrc: '',
                     cache: true
                 },
                 columns: [
                     { data: 'name' },
@@ -167,16 +166,15 @@
                     dataTableFooterSumColumn(api, 7);
                     dataTableFooterSumColumn(api, 8, 'isk');
                     dataTableFooterSumColumn(api, 9);
                     dataTableFooterSumColumn(api, 10, 'isk');
                 }
             });
 
-            $('#table_user_uploaded').DataTable(
-                {
+            $('#table_user_uploaded').DataTable({
                 ajax: {
                     url: '{% url "moonmining:report_user_uploaded_data" %}',
                     dataSrc: '',
                     cache: true
                 },
                 columns: [
                     { data: 'name' },
@@ -205,16 +203,15 @@
                     autoSize: false
                 },
                 footerCallback: function (row, data, start, end, display) {
                     dataTableFooterSumColumn(this.api(), 3);
                 }
             });
 
-            $('#table_ore_prices').DataTable(
-                {
+            $('#table_ore_prices').DataTable({
                 ajax: {
                     url: '{% url "moonmining:report_ore_prices_data" %}',
                     dataSrc: '',
                     cache: true
                 },
                 columns: [
                     { data: 'name' },
```

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/tests.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/tests.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/modals/content_base.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/modals/content_base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_head.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_head_base.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_head_base.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_details_products.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_details_products.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_characters.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_characters.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_head.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_head.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extraction_ledger_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/extractions_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/extractions_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/global_js.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/global_js.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 <!-- Global Javascript. Implemented as template, so we can use tags, filters and context. -->
 
 <script type="text/javascript">
+    "use strict";
     /* Global constants */
-    const DEFAULT_LENGTH_MENU = [[10, 25, 50, 100 -1], [10, 25, 50, 100, "All"]]
-    const DEFAULT_PAGE_LENGTH = 50
-    const B_DIVIDER = 9
+    const DEFAULT_LENGTH_MENU = [[10, 25, 50, 100 -1], [10, 25, 50, 100, "All"]];
+    const DEFAULT_PAGE_LENGTH = 50;
+    const B_DIVIDER = 9;
 
     // Format ISK values for output
     // magnitude: show value with given magnitude, else magnitude will be calculated
     function formatisk(data, magnitude=null) {
         if ( data != null ) {
             const power_map = {'t': 12, 'b': 9, 'm': 6, 'k': 3, '': 0}
             if (!power_map.hasOwnProperty(magnitude)) {
@@ -28,33 +29,34 @@
     // sum numbers in column and write result in footer row
     // Args:
     // - api: current api object
     // - columnIdx: Index number of columns to sum, starts with 0
     // - format: format of output. either 'number' or 'isk'
     function dataTableFooterSumColumn(api, columnIdx, format='number'){
         // Remove the formatting to get integer data for summation
-        var intVal = function (i) {
+        let intVal = function (i) {
             return typeof i === 'string' ?
                 i.replace(/[\$,]/g, '') * 1 :
                 typeof i === 'number' ?
                     i : 0;
         };
 
-        var columnTotal = api
+        let columnTotal = api
             .column(columnIdx)
             .data()
             .reduce(function (a, b) {
                     return intVal(a) + intVal(b);
                 },
                 0
             );
+        let result = "";
         if (format == 'isk'){
-            var result = formatisk(columnTotal)
+            result = formatisk(columnTotal)
         } else {
-            var result = columnTotal.toLocaleString('en-US', {maximumFractionDigits: 0})
+            result = columnTotal.toLocaleString('en-US', {maximumFractionDigits: 0})
         }
         $(api.column(columnIdx).footer()).html(result);
     }
 
     // DataTables renderer for ISK values
     $.fn.dataTable.render.formatisk = function(magnitude=null) {
         return function ( data, type, row ) {
@@ -66,13 +68,21 @@
         };
     };
 
     // wrap boiler plate code for handling modal events
     function handle_modal_events(modalId, modalContentId,) {
         $('#' + modalId ).on('show.bs.modal', function (event) {
             $(this).find('.modal-body').load("{% url 'moonmining:modal_loader_body' %}?is_night_mode={{NIGHT_MODE}}")
-            var button = $(event.relatedTarget)
-            var ajax_url = button.data('ajax_url');
-            $('#' + modalContentId).load(ajax_url)
+            let button = $(event.relatedTarget);
+            let ajax_url = button.data('ajax_url');
+            $('#' + modalContentId).load(ajax_url, function( response, status, xhr ) {
+                if ( status == "error" ) {
+                    let msg = `
+                        <p class="text-danger">
+                            Sorry but there was an error: ${xhr.status} ${xhr.statusText}
+                        </p>`;
+                    $(this).find('.modal-body').html(msg);
+                }
+            });
         });
     }
 </script>
```

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/location.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/location.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/menu.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_moon.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moon_details_moon.html`

 * *Files 21% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 
 <div class="row">
     <div class="col-md-2">
         <p><strong>{% translate 'Refinery:' %}</strong></p>
     </div>
     <div class="col-md-10">
     {% if moon.refinery %}
-        <p>{{ moon.refinery|default:"-" }}  / {{ moon.refinery.eve_type|default:"-" }}</p>
+        <p>{{ moon.refinery|default:"?" }}  / {{ moon.refinery.eve_type|default:"?" }}</p>
     {% else %}
-        -
+        ?
     {% endif %}
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
         <p><strong>{% translate 'Corporation:' %}</strong></p>
     </div>
     <div class="col-md-10">
-    <p>{{ moon.refinery.owner|default:"-" }}</p>
+    <p>{{ moon.refinery.owner|default:"?" }}</p>
     </div>
 </div>
 
 <div class="row">
     <div class="col-md-2">
         <p><strong>{% translate 'Est. Value:' %}</strong></p>
     </div>
```

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moon_details_products.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moon_details_products.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/moons_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/moons_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_ore_prices_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_owned_value_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_owned_value_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_mining_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_user_mining_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/reports_user_uploaded_tab.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templates/moonmining/partials/upload_survey.html` & `aa_moonmining-1.9.1/moonmining/templates/moonmining/partials/upload_survey.html`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/templatetags/moonmining.py` & `aa_moonmining-1.9.1/moonmining/templatetags/moonmining.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/helpers.py` & `aa_moonmining-1.9.1/moonmining/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_admin.py` & `aa_moonmining-1.9.1/moonmining/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_commands.py` & `aa_moonmining-1.9.1/moonmining/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_core.py` & `aa_moonmining-1.9.1/moonmining/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_helpers.py` & `aa_moonmining-1.9.1/moonmining/tests/test_helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime as dt
 
 from django.test import TestCase
 
 from .. import helpers
+from .testdata.factories import UserMainFactory
 
 
 class TestRoundDatetime(TestCase):
     def test_should_round_up(self):
         # given
         my_dt = dt.datetime(2021, 4, 6, 20, 15, 0, 567000)
         # when/then
@@ -25,7 +26,25 @@
     def test_should_do_nothing(self):
         # given
         my_dt = dt.datetime(2021, 4, 6, 20, 15, 0)
         # when/then
         self.assertEqual(
             dt.datetime(2021, 4, 6, 20, 15, 0), helpers.round_seconds(my_dt)
         )
+
+
+class TestUserPermLookup(TestCase):
+    def test_should_return_lookup(self):
+        # given
+        user = UserMainFactory(permissions=["moonmining.extractions_access"])
+        # when
+        result = helpers.user_perms_lookup(
+            user, ["moonmining.extractions_access", "moonmining.view_all_moons"]
+        )
+        # then
+        excepted = {
+            "moonmining": {
+                "extractions_access": True,
+                "view_all_moons": False,
+            }
+        }
+        self.assertDictEqual(result, excepted)
```

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_integration.py` & `aa_moonmining-1.9.1/moonmining/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_managers.py` & `aa_moonmining-1.9.1/moonmining/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_models.py` & `aa_moonmining-1.9.1/moonmining/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_templatetags.py` & `aa_moonmining-1.9.1/moonmining/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/test_views.py` & `aa_moonmining-1.9.1/moonmining/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime as dt
 from unittest.mock import Mock, patch
 
 import pytz
 
 from django.contrib.sessions.middleware import SessionMiddleware
+from django.http import Http404
 from django.test import RequestFactory, TestCase
 from django.urls import reverse
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveMarketPrice, EveMoon
 
 from allianceauth.eveonline.models import EveCorporationInfo
@@ -43,15 +44,15 @@
         cls.factory = RequestFactory()
         cls.user, cls.character_ownership = create_user_from_evecharacter(
             1001, permissions=["moonmining.add_refinery_owner"]
         )
 
     @patch(MODULE_PATH + ".notify_admins")
     @patch(MODULE_PATH + ".tasks.update_owner")
-    @patch(MODULE_PATH + ".messages_plus")
+    @patch(MODULE_PATH + ".messages")
     def test_should_add_new_owner(
         self, mock_messages, mock_update_owner, mock_notify_admins
     ):
         # given
         token = Mock(spec=Token)
         token.character_id = self.character_ownership.character.character_id
         request = self.factory.get(reverse("moonmining:add_owner"))
@@ -68,15 +69,15 @@
         self.assertTrue(mock_messages.success.called)
         self.assertTrue(mock_update_owner.delay.called)
         self.assertTrue(mock_notify_admins.called)
         obj = Owner.objects.get(corporation__corporation_id=2001)
         self.assertEqual(obj.character_ownership, self.character_ownership)
 
     @patch(MODULE_PATH + ".tasks.update_owner")
-    @patch(MODULE_PATH + ".messages_plus")
+    @patch(MODULE_PATH + ".messages")
     def test_should_update_existing_owner(self, mock_messages, mock_update_owner):
         # given
         Owner.objects.create(
             corporation=EveCorporationInfo.objects.get(corporation_id=2001),
             character_ownership=None,
         )
         token = Mock(spec=Token)
@@ -94,31 +95,30 @@
         self.assertEqual(response.url, reverse("moonmining:index"))
         self.assertTrue(mock_messages.success.called)
         self.assertTrue(mock_update_owner.delay.called)
         obj = Owner.objects.get(corporation__corporation_id=2001)
         self.assertEqual(obj.character_ownership, self.character_ownership)
 
     @patch(MODULE_PATH + ".tasks.update_owner")
-    @patch(MODULE_PATH + ".messages_plus")
+    @patch(MODULE_PATH + ".messages")
     def test_should_raise_404_if_character_ownership_not_found(
         self, mock_messages, mock_update_owner
     ):
         # given
         token = Mock(spec=Token)
         token.character_id = 1099
         request = self.factory.get(reverse("moonmining:add_owner"))
         request.user = self.user
         request.token = token
         middleware = SessionMiddleware(Mock())
         middleware.process_request(request)
         orig_view = views.add_owner.__wrapped__.__wrapped__.__wrapped__
         # when
-        response = orig_view(request, token)
-        # then
-        self.assertEqual(response.status_code, 404)
+        with self.assertRaises(Http404):
+            orig_view(request, token)
 
 
 class TestMoonsData(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         load_eveuniverse()
@@ -135,19 +135,15 @@
         data = helpers.json_response_to_python_2(response)
         return {int(obj[0]): obj for obj in data}
 
     def test_should_return_all_moons(self):
         # given
         user, _ = create_user_from_evecharacter(
             1001,
-            permissions=[
-                "moonmining.basic_access",
-                "moonmining.extractions_access",
-                "moonmining.view_all_moons",
-            ],
+            permissions=["moonmining.basic_access", "moonmining.view_all_moons"],
             scopes=Owner.esi_scopes(),
         )
         self.client.force_login(user)
         # when
         response = self.client.get(f"/moonmining/moons_data/{views.MoonsCategory.ALL}")
         # then
         self.assertEqual(response.status_code, 200)
@@ -169,61 +165,48 @@
         # when
         response = self.client.get(f"/moonmining/moons_data/{views.MoonsCategory.OURS}")
         # then
         self.assertEqual(response.status_code, 200)
         data = self._response_to_dict(response)
         self.assertSetEqual(set(data.keys()), {40131695})
 
-    def test_should_handle_empty_refineries(self):
+    def test_should_return_our_moons_when_all_moons_perm(self):
         # given
+        moon = Moon.objects.get(pk=40131695)
+        RefineryFactory(moon=moon)
         user, _ = create_user_from_evecharacter(
             1002,
             permissions=["moonmining.basic_access", "moonmining.extractions_access"],
             scopes=Owner.esi_scopes(),
         )
         self.client.force_login(user)
-        moon = Moon.objects.get(pk=40131695)
-        refinery = RefineryFactory(moon=moon)
-        RefineryFactory(owner=refinery.owner, moon=None)
         # when
         response = self.client.get(f"/moonmining/moons_data/{views.MoonsCategory.OURS}")
         # then
         self.assertEqual(response.status_code, 200)
         data = self._response_to_dict(response)
         self.assertSetEqual(set(data.keys()), {40131695})
 
-    def test_should_return_empty_list_for_all_moons(self):
+    def test_should_handle_empty_refineries(self):
         # given
         user, _ = create_user_from_evecharacter(
-            1001,
+            1002,
             permissions=["moonmining.basic_access", "moonmining.extractions_access"],
             scopes=Owner.esi_scopes(),
         )
         self.client.force_login(user)
-        # when
-        response = self.client.get(f"/moonmining/moons_data/{views.MoonsCategory.ALL}")
-        # then
-        self.assertEqual(response.status_code, 200)
-        data = self._response_to_dict(response)
-        self.assertEqual(len(data), 0)
-
-    def test_should_return_empty_list_for_our_moons(self):
-        # given
-        user, _ = create_user_from_evecharacter(
-            1001,
-            permissions=["moonmining.basic_access"],
-            scopes=Owner.esi_scopes(),
-        )
-        self.client.force_login(user)
+        moon = Moon.objects.get(pk=40131695)
+        refinery = RefineryFactory(moon=moon)
+        RefineryFactory(owner=refinery.owner, moon=None)
         # when
         response = self.client.get(f"/moonmining/moons_data/{views.MoonsCategory.OURS}")
         # then
         self.assertEqual(response.status_code, 200)
         data = self._response_to_dict(response)
-        self.assertEqual(len(data), 0)
+        self.assertSetEqual(set(data.keys()), {40131695})
 
     def test_should_return_uploaded_moons_only(self):
         # given
         user, _ = create_user_from_evecharacter(
             1001,
             permissions=["moonmining.basic_access", "moonmining.upload_moon_scan"],
             scopes=Owner.esi_scopes(),
@@ -240,19 +223,15 @@
         data = self._response_to_dict(response)
         self.assertSetEqual(set(data.keys()), {40161708})
 
     def test_should_return_fdd_for_all_moons(self):
         # given
         user, _ = create_user_from_evecharacter(
             1002,
-            permissions=[
-                "moonmining.basic_access",
-                "moonmining.extractions_access",
-                "moonmining.view_all_moons",
-            ],
+            permissions=["moonmining.basic_access", "moonmining.view_all_moons"],
             scopes=Owner.esi_scopes(),
         )
         moon = Moon.objects.get(pk=40131695)
         RefineryFactory(moon=moon)
         self.client.force_login(user)
         # when
         response = self.client.get(
@@ -268,15 +247,15 @@
         self.assertListEqual(data["corporation_name"], ["Wayne Technologies"])
         self.assertListEqual(data["region_name"], ["Heimatar", "Metropolis"])
         self.assertListEqual(data["constellation_name"], ["Aldodan", "Hed"])
         self.assertListEqual(data["solar_system_name"], ["Auga", "Helgatild"])
         self.assertListEqual(data["rarity_class_str"], ["R64"])
         self.assertListEqual(data["label_name"], ["Dummy"])
         self.assertListEqual(data["has_refinery_str"], ["no", "yes"])
-        self.assertListEqual(data["has_extraction_str"], ["no"])
+        self.assertListEqual(data["has_extraction_str"], [])
         self.assertIn("ERROR", data["invalid_column"][0])
 
 
 class TestMoonInfo(TestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
```

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/allianceauth.json` & `aa_moonmining-1.9.1/moonmining/tests/testdata/allianceauth.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/create_eveuniverse.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/esi.json` & `aa_moonmining-1.9.1/moonmining/tests/testdata/esi.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/esi_client_stub.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/eveuniverse.json` & `aa_moonmining-1.9.1/moonmining/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/factories.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_many_moons.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/generate_many_moons.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 
 from django.contrib.auth.models import User
 from django.utils.timezone import now
 from eveuniverse.core.esitools import is_esi_online
 from eveuniverse.models import EveMoon
 
 from moonmining.models import EveOreType, Moon, MoonProduct
+from moonmining.tests.testdata.factories import random_percentages
 
-from .factories import random_percentages
-
-MAX_MOONS = 1000
+MAX_MOONS = 100
 
 ORE_TYPES = {
     45490: "Zeolites",
     45491: "Sylvite",
     45492: "Bitumens",
     45493: "Coesite",
     45494: "Cobaltite",
```

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.json` & `aa_moonmining-1.9.1/moonmining/tests/testdata/generate_moons.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/generate_moons.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/generate_moons.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/load_allianceauth.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/load_eveuniverse.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/load_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/moon_ids.csv` & `aa_moonmining-1.9.1/moonmining/tests/testdata/moon_ids.csv`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/moon_survey_input_2.txt` & `aa_moonmining-1.9.1/moonmining/tests/testdata/moon_survey_input_2.txt`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/notification_details.py` & `aa_moonmining-1.9.1/moonmining/tests/testdata/notification_details.py`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/moonmining/tests/testdata/notifications_full.json` & `aa_moonmining-1.9.1/moonmining/tests/testdata/notifications_full.json`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/LICENSE` & `aa_moonmining-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_moonmining-1.9.0/README.md` & `aa_moonmining-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
 Name  | Description
 -- | --
 `moonmining.basic_access` | This is access permission, users without this permission will be unable to access the plugin.
 `moonmining.upload_moon_scan` | This permission allows users to upload moon scan data.
 `moonmining.extractions_access` | User can access extractions and view owned moons.
 `moonmining.reports_access` | User can access reports.
-`moonmining.view_all_moons` | User can view all moons in the database.
+`moonmining.view_all_moons` | User can view all moons in the database and see own moons.
 `moonmining.add_refinery_owner` | This permission is allows users to add their tokens to be pulled from when checking for new extraction events.
 `moonmining.view_moon_ledgers` | Users with this permission can view the mining ledgers from past extractions from moons they have access to.
 
 ## Settings
 
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
```

### Comparing `aa_moonmining-1.9.0/pyproject.toml` & `aa_moonmining-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
-    "allianceauth-app-utils>=1.14.2",
+    "allianceauth-app-utils>=1.18",
     "allianceauth>=3",
     "django-bootstrap-form",
     "django-datatables-view>=1.20",
     "django-eveuniverse>=0.18",
     "django-navhelper",
     "PyYAML",
 ]
```

### Comparing `aa_moonmining-1.9.0/PKG-INFO` & `aa_moonmining-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-moonmining
-Version: 1.9.0
+Version: 1.9.1
 Summary: Alliance Auth app for tracking moon extractions and scouting new moons.
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-moonmining
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-moonmining
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-moonmining/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-moonmining/-/issues
 Author-email: Erik Kalkoken <kaloken87@gmail.com>
 License-Expression: MIT
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-Requires-Dist: allianceauth-app-utils>=1.14.2
+Requires-Dist: allianceauth-app-utils>=1.18
 Requires-Dist: allianceauth>=3
 Requires-Dist: django-bootstrap-form
 Requires-Dist: django-datatables-view>=1.20
 Requires-Dist: django-eveuniverse>=0.18
 Requires-Dist: django-navhelper
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
@@ -237,15 +237,15 @@
 
 Name  | Description
 -- | --
 `moonmining.basic_access` | This is access permission, users without this permission will be unable to access the plugin.
 `moonmining.upload_moon_scan` | This permission allows users to upload moon scan data.
 `moonmining.extractions_access` | User can access extractions and view owned moons.
 `moonmining.reports_access` | User can access reports.
-`moonmining.view_all_moons` | User can view all moons in the database.
+`moonmining.view_all_moons` | User can view all moons in the database and see own moons.
 `moonmining.add_refinery_owner` | This permission is allows users to add their tokens to be pulled from when checking for new extraction events.
 `moonmining.view_moon_ledgers` | Users with this permission can view the mining ledgers from past extractions from moons they have access to.
 
 ## Settings
 
 Here is a list of available settings for this app. They can be configured by adding them to your AA settings file (`local.py`).
```

