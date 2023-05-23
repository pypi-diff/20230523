# Comparing `tmp/huntflow_api_client-0.0.6.tar.gz` & `tmp/huntflow_api_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-0.0.6.tar", last modified: Fri May 19 07:40:45 2023, max compression
+gzip compressed data, was "huntflow_api_client-0.0.7.tar", last modified: Tue May 23 12:27:28 2023, max compression
```

## Comparing `huntflow_api_client-0.0.6.tar` & `huntflow_api_client-0.0.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1065 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/LICENSE
--rw-r--r--   0        0        0      488 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/README.md
--rw-r--r--   0        0        0       76 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     5578 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/api.py
--rw-r--r--   0        0        0     1293 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0     1760 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/account_vacancy_request.py
--rw-r--r--   0        0        0     1434 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/accounts.py
--rw-r--r--   0        0        0     2903 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/applicant_on_vacancy.py
--rw-r--r--   0        0        0      730 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0     8317 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/applicants.py
--rw-r--r--   0        0        0      941 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     2651 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/coworkers.py
--rw-r--r--   0        0        0      743 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/delayed_tasks.py
--rw-r--r--   0        0        0     3002 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/dictionaries.py
--rw-r--r--   0        0        0     2538 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/divisions.py
--rw-r--r--   0        0        0     6720 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/production_calendars.py
--rw-r--r--   0        0        0      713 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/rejection_reason.py
--rw-r--r--   0        0        0     2456 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0     9379 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/vacancies.py
--rw-r--r--   0        0        0     2918 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/vacancy_requests.py
--rw-r--r--   0        0        0     1789 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/entities/webhooks.py
--rw-r--r--   0        0        0      553 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/errors/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/errors/errors.py
--rw-r--r--   0        0        0     3732 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/errors/handlers.py
--rw-r--r--   0        0        0      361 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/errors/response_hooks.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0     6501 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0     2277 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/consts.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0     3614 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/applicant_on_vacancy.py
--rw-r--r--   0        0        0     6196 2023-05-19 07:40:32.077568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/applicants.py
--rw-r--r--   0        0        0     1492 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/dictionaries.py
--rw-r--r--   0        0        0      691 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/divisions.py
--rw-r--r--   0        0        0      921 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/production_calendars.py
--rw-r--r--   0        0        0      259 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0     3123 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/vacancies.py
--rw-r--r--   0        0        0     1407 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/vacancy_requests.py
--rw-r--r--   0        0        0      482 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/request/webhooks.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0     2102 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/account_vacancy_request.py
--rw-r--r--   0        0        0     1595 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/accounts.py
--rw-r--r--   0        0        0     1054 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicant_on_vacancy.py
--rw-r--r--   0        0        0      773 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicant_on_vacancy_status.py
--rw-r--r--   0        0        0    12930 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicants.py
--rw-r--r--   0        0        0     1262 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/coworkers.py
--rw-r--r--   0        0        0     1299 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/delayed_tasks.py
--rw-r--r--   0        0        0     2261 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/dictionaries.py
--rw-r--r--   0        0        0     1507 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/divisions.py
--rw-r--r--   0        0        0      330 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/offers.py
--rw-r--r--   0        0        0     1525 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/production_calendars.py
--rw-r--r--   0        0        0      476 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/rejection_reason.py
--rw-r--r--   0        0        0      781 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/survey.py
--rw-r--r--   0        0        0      241 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0     6182 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/vacancies.py
--rw-r--r--   0        0        0     2973 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/vacancy_requests.py
--rw-r--r--   0        0        0      719 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/models/response/webhooks.py
--rw-r--r--   0        0        0       53 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      548 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1597 2023-05-19 07:40:45.653282 huntflow_api_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     4744 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/api.py
--rw-r--r--   0        0        0       79 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      176 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/fixtures/server.py
--rw-r--r--   0        0        0      856 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/fixtures/tokens.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/__init__.py
--rw-r--r--   0        0        0     3161 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_account_divisions.py
--rw-r--r--   0        0        0     2590 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_account_tags.py
--rw-r--r--   0        0        0     3782 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_account_vacancy_request.py
--rw-r--r--   0        0        0     2279 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_accounts.py
--rw-r--r--   0        0        0     3614 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_applicant_on_vacancy.py
--rw-r--r--   0        0        0     1214 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_applicant_on_vacancy_statuses.py
--rw-r--r--   0        0        0    16569 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_applicants.py
--rw-r--r--   0        0        0     2815 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_coworkers.py
--rw-r--r--   0        0        0     1323 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_delayed_tasks.py
--rw-r--r--   0        0        0     4417 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_dictionaries.py
--rw-r--r--   0        0        0     7692 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_production_calendar.py
--rw-r--r--   0        0        0     1039 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_rejection_reasons.py
--rw-r--r--   0        0        0    14337 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_vacancies.py
--rw-r--r--   0        0        0     4266 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_vacancy_request.py
--rw-r--r--   0        0        0     2534 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_entities/test_webhooks.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_errors/__init__.py
--rw-r--r--   0        0        0     8007 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_errors/test_error_handlers.py
--rw-r--r--   0        0        0        0 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_tokens/__init__.py
--rw-r--r--   0        0        0     5630 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_tokens/test_access_token.py
--rw-r--r--   0        0        0     1973 2023-05-19 07:40:32.081568 huntflow_api_client-0.0.6/tests/test_tokens/test_huntflow_token_proxy.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0      488 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/README.md
+-rw-r--r--   0        0        0       76 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     5578 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/huntflow_api_client/api.py
+-rw-r--r--   0        0        0     1293 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/huntflow_api_client/entities/account_vacancy_request.py
+-rw-r--r--   0        0        0     1434 2023-05-23 12:27:15.405881 huntflow_api_client-0.0.7/huntflow_api_client/entities/accounts.py
+-rw-r--r--   0        0        0     2903 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      730 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     8554 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/applicants.py
+-rw-r--r--   0        0        0      941 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     2651 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/coworkers.py
+-rw-r--r--   0        0        0      743 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/delayed_tasks.py
+-rw-r--r--   0        0        0     3002 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/dictionaries.py
+-rw-r--r--   0        0        0     2554 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/divisions.py
+-rw-r--r--   0        0        0     6720 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/production_calendars.py
+-rw-r--r--   0        0        0      713 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/rejection_reason.py
+-rw-r--r--   0        0        0     2456 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0     9379 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/vacancies.py
+-rw-r--r--   0        0        0     2918 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/vacancy_requests.py
+-rw-r--r--   0        0        0     1789 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/entities/webhooks.py
+-rw-r--r--   0        0        0      553 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/errors/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/errors/errors.py
+-rw-r--r--   0        0        0     3732 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/errors/handlers.py
+-rw-r--r--   0        0        0      361 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/errors/response_hooks.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0     6501 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0     2394 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/consts.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0     3614 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/applicant_on_vacancy.py
+-rw-r--r--   0        0        0     6196 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/applicants.py
+-rw-r--r--   0        0        0     1492 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/dictionaries.py
+-rw-r--r--   0        0        0      691 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/divisions.py
+-rw-r--r--   0        0        0      921 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/production_calendars.py
+-rw-r--r--   0        0        0      259 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0     3123 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/vacancies.py
+-rw-r--r--   0        0        0     1407 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/vacancy_requests.py
+-rw-r--r--   0        0        0      482 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/request/webhooks.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0     2102 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/account_vacancy_request.py
+-rw-r--r--   0        0        0     1595 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/accounts.py
+-rw-r--r--   0        0        0     1054 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      773 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0    12930 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicants.py
+-rw-r--r--   0        0        0     1262 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/coworkers.py
+-rw-r--r--   0        0        0     1299 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/delayed_tasks.py
+-rw-r--r--   0        0        0     2261 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/dictionaries.py
+-rw-r--r--   0        0        0     1507 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/divisions.py
+-rw-r--r--   0        0        0      330 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/offers.py
+-rw-r--r--   0        0        0     1525 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/production_calendars.py
+-rw-r--r--   0        0        0      476 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/rejection_reason.py
+-rw-r--r--   0        0        0      781 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/survey.py
+-rw-r--r--   0        0        0      241 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0     6182 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/vacancies.py
+-rw-r--r--   0        0        0     2901 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/vacancy_requests.py
+-rw-r--r--   0        0        0      719 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/models/response/webhooks.py
+-rw-r--r--   0        0        0       53 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      548 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1597 2023-05-23 12:27:28.742031 huntflow_api_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     4744 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/api.py
+-rw-r--r--   0        0        0       79 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      176 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/fixtures/server.py
+-rw-r--r--   0        0        0      856 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/fixtures/tokens.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_account_divisions.py
+-rw-r--r--   0        0        0     2590 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_account_tags.py
+-rw-r--r--   0        0        0     3782 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_account_vacancy_request.py
+-rw-r--r--   0        0        0     2279 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_accounts.py
+-rw-r--r--   0        0        0     3614 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_applicant_on_vacancy.py
+-rw-r--r--   0        0        0     1214 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_applicant_on_vacancy_statuses.py
+-rw-r--r--   0        0        0    16778 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_applicants.py
+-rw-r--r--   0        0        0     2815 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_coworkers.py
+-rw-r--r--   0        0        0     1323 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_delayed_tasks.py
+-rw-r--r--   0        0        0     4417 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_dictionaries.py
+-rw-r--r--   0        0        0     7692 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_production_calendar.py
+-rw-r--r--   0        0        0     1039 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_rejection_reasons.py
+-rw-r--r--   0        0        0    14337 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_vacancies.py
+-rw-r--r--   0        0        0     4266 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_vacancy_request.py
+-rw-r--r--   0        0        0     2534 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_entities/test_webhooks.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_errors/__init__.py
+-rw-r--r--   0        0        0     8007 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_errors/test_error_handlers.py
+-rw-r--r--   0        0        0        0 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_tokens/__init__.py
+-rw-r--r--   0        0        0     5630 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_tokens/test_access_token.py
+-rw-r--r--   0        0        0     1973 2023-05-23 12:27:15.409881 huntflow_api_client-0.0.7/tests/test_tokens/test_huntflow_token_proxy.py
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.7/PKG-INFO
```

### Comparing `huntflow_api_client-0.0.6/LICENSE` & `huntflow_api_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/api.py` & `huntflow_api_client-0.0.7/huntflow_api_client/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/__init__.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/account_vacancy_request.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/accounts.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/applicant_on_vacancy.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/applicant_on_vacancy_status.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/applicants.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/applicants.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,17 +206,22 @@
         :param applicant_id: Applicant ID
         :param type_: Log type
         :param vacancy: If supplied, only logs related to the specified vacancy will be returned
         :param personal: If supplied, only logs not related to any vacancy will be returned
         :param count: Number of items per page
         :param page: Page number
 
+        :raises ValueError: Only one parameter from `vacancy` and `personal` must be specified
+
         :return: List of applicant's worklog
         """
         path = f"/accounts/{account_id}/applicants/{applicant_id}/logs"
+        if vacancy is not None and personal:
+            raise ValueError("Only one parameter from vacancy and personal must be specified")
+
         params: Dict[str, Any] = {
             "personal": personal,
             "count": count,
             "page": page,
         }
         if type_:
             params["type"] = type_.value
```

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/base.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/base.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/coworkers.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/delayed_tasks.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/dictionaries.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/divisions.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/divisions.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,16 @@
             https://api.huntflow.ai/v2/docs#get-/accounts/-account_id-/coworkers/-coworker_id-/divisions
 
         :param account_id: Organization ID
         :param coworker_id: If specified - will be returned divisions for specified coworker
         :param only_available:	If True,
             then only divisions available to the current user will be returned
 
-        :raises ValueError: Only one parameter from coworker_id and only_available must be specified
+        :raises ValueError:
+            Only one parameter from `coworker_id` and `only_available` must be specified
 
         :return: List of company divisions.
         """
         if coworker_id is not None and only_available:
             raise ValueError(
                 "Only one parameter from coworker_id and only_available must be specified",
             )
```

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/production_calendars.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/rejection_reason.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/rejection_reason.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/tags.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/vacancies.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/vacancy_requests.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/entities/webhooks.py` & `huntflow_api_client-0.0.7/huntflow_api_client/entities/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/errors/__init__.py` & `huntflow_api_client-0.0.7/huntflow_api_client/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/errors/errors.py` & `huntflow_api_client-0.0.7/huntflow_api_client/errors/errors.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/errors/handlers.py` & `huntflow_api_client-0.0.7/huntflow_api_client/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/common.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/common.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/consts.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,20 @@
 
 
 class Transparency(str, Enum):
     busy = "busy"
     free = "free"
 
 
+class VacancyRequestStatus(str, Enum):
+    pending = "pending"
+    approved = "approved"
+    rejected = "rejected"
+
+
 class EventReminderMultiplier(str, Enum):
     minutes = "minutes"
     hours = "hours"
     days = "days"
     weeks = "weeks"
```

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/applicant_on_vacancy.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/applicants.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/dictionaries.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/divisions.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/production_calendars.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/vacancies.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/request/vacancy_requests.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/request/vacancy_requests.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/account_vacancy_request.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/accounts.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicant_on_vacancy.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicant_on_vacancy_status.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicant_on_vacancy_status.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/applicants.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/applicants.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/coworkers.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/delayed_tasks.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/dictionaries.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/divisions.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/production_calendars.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/production_calendars.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/survey.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/survey.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/vacancies.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/vacancy_requests.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/vacancy_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from __future__ import annotations
 
 import datetime
 import typing as t
-from enum import Enum
 
 from pydantic import BaseModel, EmailStr, Field, PositiveInt
 
 from huntflow_api_client.models.common import File, PaginatedResponse
-
-
-class VacancyRequestStatus(str, Enum):
-    pending = "pending"
-    approved = "approved"
-    rejected = "rejected"
+from huntflow_api_client.models.consts import VacancyRequestStatus
 
 
 class UserInfo(BaseModel):
     id: PositiveInt = Field(
         ...,
         description="Coworker who create the vacancy request",
     )
```

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/models/response/webhooks.py` & `huntflow_api_client-0.0.7/huntflow_api_client/models/response/webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-0.0.7/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-0.0.7/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-0.0.7/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/huntflow_api_client/tokens/token.py` & `huntflow_api_client-0.0.7/huntflow_api_client/tokens/token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/pyproject.toml` & `huntflow_api_client-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "huntflow-api-client"
-version = "0.0.6"
+version = "0.0.7"
 description = "Huntflow API Client for Python"
 authors = [
     { name = "Developers huntflow", email = "developer@huntflow.ru" },
 ]
 dependencies = [
     "httpx>=0.23.3",
     "email-validator>=1.3.1",
```

### Comparing `huntflow_api_client-0.0.6/tests/api.py` & `huntflow_api_client-0.0.7/tests/api.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/fixtures/tokens.py` & `huntflow_api_client-0.0.7/tests/fixtures/tokens.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_account_divisions.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_account_divisions.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_account_tags.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_account_tags.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_account_vacancy_request.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_account_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_accounts.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_accounts.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_applicant_on_vacancy.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_applicant_on_vacancy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_applicant_on_vacancy_statuses.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_applicant_on_vacancy_statuses.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_applicants.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_applicants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict
 
+import pytest
 from pytest_httpx import HTTPXMock
 
 from huntflow_api_client import HuntflowAPI
 from huntflow_api_client.entities.applicants import Applicant
 from huntflow_api_client.models.consts import ApplicantLogType
 from huntflow_api_client.models.request.applicants import (
     ApplicantCreateRequest,
@@ -522,7 +523,15 @@
     response = await applicants.log_list(
         account_id=ACCOUNT_ID,
         applicant_id=1,
         vacancy=1,
         type_=ApplicantLogType.ADD,
     )
     assert response == ApplicantLogResponse.parse_obj(APPLICANT_LOG_LIST_RESPONSE)
+
+    with pytest.raises(ValueError):
+        await applicants.log_list(
+            account_id=ACCOUNT_ID,
+            applicant_id=1,
+            vacancy=1,
+            personal=True,
+        )
```

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_coworkers.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_coworkers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_delayed_tasks.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_delayed_tasks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_dictionaries.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_dictionaries.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_production_calendar.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_production_calendar.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_rejection_reasons.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_rejection_reasons.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_vacancies.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_vacancies.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_vacancy_request.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_vacancy_request.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_entities/test_webhooks.py` & `huntflow_api_client-0.0.7/tests/test_entities/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_errors/test_error_handlers.py` & `huntflow_api_client-0.0.7/tests/test_errors/test_error_handlers.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_tokens/test_access_token.py` & `huntflow_api_client-0.0.7/tests/test_tokens/test_access_token.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/tests/test_tokens/test_huntflow_token_proxy.py` & `huntflow_api_client-0.0.7/tests/test_tokens/test_huntflow_token_proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.6/PKG-INFO` & `huntflow_api_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huntflow-api-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Huntflow API Client for Python
 Author-Email: Developers huntflow <developer@huntflow.ru>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

