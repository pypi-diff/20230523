# Comparing `tmp/supertokens_python-0.9.0.tar.gz` & `tmp/supertokens_python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supertokens_python-0.9.0.tar", last modified: Sat Jun 25 14:07:31 2022, max compression
+gzip compressed data, was "supertokens_python-0.9.1.tar", last modified: Mon Jun 27 17:24:58 2022, max compression
```

## Comparing `supertokens_python-0.9.0.tar` & `supertokens_python-0.9.1.tar`

### file list

```diff
@@ -1,427 +1,450 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/
--rw-r--r--   0 root         (0) root         (0)    10921 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1959 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      967 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)      125 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       76 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2949 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python/
--rw-r--r--   0 root         (0) root         (0)     1555 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1156 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/async_to_sync_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python/asyncio/
--rw-r--r--   0 root         (0) root         (0)     1722 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1154 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/constants.py
--rw-r--r--   0 root         (0) root         (0)     1248 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python/framework/
--rw-r--r--   0 root         (0) root         (0)      798 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python/framework/django/
--rw-r--r--   0 root         (0) root         (0)      781 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/django/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3746 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/django/django_middleware.py
--rw-r--r--   0 root         (0) root         (0)     2408 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/django/django_request.py
--rw-r--r--   0 root         (0) root         (0)     2912 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/django/django_response.py
--rw-r--r--   0 root         (0) root         (0)     1097 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/django/framework.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python/framework/fastapi/
--rw-r--r--   0 root         (0) root         (0)      802 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/fastapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2956 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_middleware.py
--rw-r--r--   0 root         (0) root         (0)     2194 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_request.py
--rw-r--r--   0 root         (0) root         (0)     3437 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_response.py
--rw-r--r--   0 root         (0) root         (0)     1089 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/fastapi/framework.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/framework/flask/
--rw-r--r--   0 root         (0) root         (0)      787 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3588 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/flask/flask_middleware.py
--rw-r--r--   0 root         (0) root         (0)     2575 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/flask/flask_request.py
--rw-r--r--   0 root         (0) root         (0)     3744 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/flask/flask_response.py
--rw-r--r--   0 root         (0) root         (0)     1086 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/flask/framework.py
--rw-r--r--   0 root         (0) root         (0)     2038 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/request.py
--rw-r--r--   0 root         (0) root         (0)     1811 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/response.py
--rw-r--r--   0 root         (0) root         (0)     1082 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/framework/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/ingredients/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)     1166 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3205 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/services/smtp.py
--rw-r--r--   0 root         (0) root         (0)     2978 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/
--rw-r--r--   0 root         (0) root         (0)     1154 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      758 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/supertokens.py
--rw-r--r--   0 root         (0) root         (0)     1223 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/twilio.py
--rw-r--r--   0 root         (0) root         (0)     3221 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/types.py
--rw-r--r--   0 root         (0) root         (0)     2237 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/logger.py
--rw-r--r--   0 root         (0) root         (0)     2707 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/normalised_url_domain.py
--rw-r--r--   0 root         (0) root         (0)     3366 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/normalised_url_path.py
--rw-r--r--   0 root         (0) root         (0)     1502 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/process_state.py
--rw-r--r--   0 root         (0) root         (0)     8900 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/querier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/recipe/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.993614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/
--rw-r--r--   0 root         (0) root         (0)     2236 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/
--rw-r--r--   0 root         (0) root         (0)     1034 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/email_exists.py
--rw-r--r--   0 root         (0) root         (0)     1862 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/generate_password_reset_token.py
--rw-r--r--   0 root         (0) root         (0)     7041 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     2093 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/password_reset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/signin.py
--rw-r--r--   0 root         (0) root         (0)     1753 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/signup.py
--rw-r--r--   0 root         (0) root         (0)     3551 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/asyncio/
--rw-r--r--   0 root         (0) root         (0)     5188 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      968 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     5698 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     2600 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1603 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset.py
--rw-r--r--   0 root         (0) root         (0)    20788 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset_email.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/
--rw-r--r--   0 root         (0) root         (0)     2704 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1780 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py
--rw-r--r--   0 root         (0) root         (0)     1564 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9727 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/interfaces.py
--rw-r--r--   0 root         (0) root         (0)    10518 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/recipe.py
--rw-r--r--   0 root         (0) root         (0)     6097 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/syncio/
--rw-r--r--   0 root         (0) root         (0)     4334 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3378 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/types.py
--rw-r--r--   0 root         (0) root         (0)    16977 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/
--rw-r--r--   0 root         (0) root         (0)     1371 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/
--rw-r--r--   0 root         (0) root         (0)      850 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2016 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/email_verify.py
--rw-r--r--   0 root         (0) root         (0)     1228 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/generate_email_verify_token.py
--rw-r--r--   0 root         (0) root         (0)     4309 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/asyncio/
--rw-r--r--   0 root         (0) root         (0)     2585 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      776 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     2915 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     1899 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify.py
--rw-r--r--   0 root         (0) root         (0)    20810 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify_email.py
--rw-r--r--   0 root         (0) root         (0)     1495 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/service_implementation.py
--rw-r--r--   0 root         (0) root         (0)      935 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5438 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     6771 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/recipe.py
--rw-r--r--   0 root         (0) root         (0)     3790 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.997614 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/syncio/
--rw-r--r--   0 root         (0) root         (0)     2483 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1922 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/types.py
--rw-r--r--   0 root         (0) root         (0)     5238 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/emailverification/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/jwt/
--rw-r--r--   0 root         (0) root         (0)     1163 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1136 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1256 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/jwks_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/jwt/asyncio/
--rw-r--r--   0 root         (0) root         (0)     1686 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/constants.py
--rw-r--r--   0 root         (0) root         (0)      833 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     4926 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/recipe.py
--rw-r--r--   0 root         (0) root         (0)     2680 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/jwt/syncio/
--rw-r--r--   0 root         (0) root         (0)     1489 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2021 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/jwt/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/openid/
--rw-r--r--   0 root         (0) root         (0)     1229 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/openid/api/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1263 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1448 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/api/open_id_discovery_configuration_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/openid/asyncio/
--rw-r--r--   0 root         (0) root         (0)     1978 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      746 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/constants.py
--rw-r--r--   0 root         (0) root         (0)      836 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2841 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     5860 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/recipe.py
--rw-r--r--   0 root         (0) root         (0)     2896 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/openid/syncio/
--rw-r--r--   0 root         (0) root         (0)     1669 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3049 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/openid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.001614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/
--rw-r--r--   0 root         (0) root         (0)     3078 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/
--rw-r--r--   0 root         (0) root         (0)      968 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/consume_code.py
--rw-r--r--   0 root         (0) root         (0)     3925 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/create_code.py
--rw-r--r--   0 root         (0) root         (0)     1420 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/email_exists.py
--rw-r--r--   0 root         (0) root         (0)    11935 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/phone_number_exists.py
--rw-r--r--   0 root         (0) root         (0)     1704 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/resend_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/asyncio/
--rw-r--r--   0 root         (0) root         (0)     8928 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      909 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     3614 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     1966 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2405 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login.py
--rw-r--r--   0 root         (0) root         (0)    66078 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login_email.py
--rw-r--r--   0 root         (0) root         (0)     1519 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/service_implementation.py
--rw-r--r--   0 root         (0) root         (0)      842 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13954 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/interfaces.py
--rw-r--r--   0 root         (0) root         (0)    11203 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/recipe.py
--rw-r--r--   0 root         (0) root         (0)    17638 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/
--rw-r--r--   0 root         (0) root         (0)      813 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     4434 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/
--rw-r--r--   0 root         (0) root         (0)     2599 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/
--rw-r--r--   0 root         (0) root         (0)     2451 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2474 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/passwordless_login.py
--rw-r--r--   0 root         (0) root         (0)     2091 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/service_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/syncio/
--rw-r--r--   0 root         (0) root         (0)     7290 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4251 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/types.py
--rw-r--r--   0 root         (0) root         (0)    11515 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/passwordless/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/session/
--rw-r--r--   0 root         (0) root         (0)     2202 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3204 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/access_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/session/api/
--rw-r--r--   0 root         (0) root         (0)      794 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2928 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     1379 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/api/refresh.py
--rw-r--r--   0 root         (0) root         (0)     1406 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/api/signout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.005614 supertokens_python-0.9.0/supertokens_python/recipe/session/asyncio/
--rw-r--r--   0 root         (0) root         (0)     7110 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1143 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/constants.py
--rw-r--r--   0 root         (0) root         (0)     6549 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/cookie_and_header.py
--rw-r--r--   0 root         (0) root         (0)     1772 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/asyncio/
--rw-r--r--   0 root         (0) root         (0)     2623 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/syncio/
--rw-r--r--   0 root         (0) root         (0)     2669 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/syncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/fastapi/
--rw-r--r--   0 root         (0) root         (0)     1789 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/fastapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/flask/
--rw-r--r--   0 root         (0) root         (0)     2109 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/framework/flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9417 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     2577 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/jwt.py
--rw-r--r--   0 root         (0) root         (0)    11232 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/recipe.py
--rw-r--r--   0 root         (0) root         (0)    13933 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/recipe_implementation.py
--rw-r--r--   0 root         (0) root         (0)     3589 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/session_class.py
--rw-r--r--   0 root         (0) root         (0)    12467 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/session_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/syncio/
--rw-r--r--   0 root         (0) root         (0)     5943 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14257 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/
--rw-r--r--   0 root         (0) root         (0)      811 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      897 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7159 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/recipe_implementation.py
--rw-r--r--   0 root         (0) root         (0)     3852 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/session_class.py
--rw-r--r--   0 root         (0) root         (0)     3741 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/utills.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/
--rw-r--r--   0 root         (0) root         (0)     2040 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/
--rw-r--r--   0 root         (0) root         (0)      888 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1418 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/apple_redirect.py
--rw-r--r--   0 root         (0) root         (0)     1943 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/authorisation_url.py
--rw-r--r--   0 root         (0) root         (0)     7971 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     3265 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/signinup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/asyncio/
--rw-r--r--   0 root         (0) root         (0)     4619 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      888 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     2842 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.009614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     1606 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      840 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5340 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1752 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/
--rw-r--r--   0 root         (0) root         (0)      965 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7144 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/apple.py
--rw-r--r--   0 root         (0) root         (0)     3904 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/discord.py
--rw-r--r--   0 root         (0) root         (0)     3449 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/facebook.py
--rw-r--r--   0 root         (0) root         (0)     4308 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/github.py
--rw-r--r--   0 root         (0) root         (0)     4122 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/google.py
--rw-r--r--   0 root         (0) root         (0)     5021 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/google_workspaces.py
--rw-r--r--   0 root         (0) root         (0)     3913 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/okta.py
--rw-r--r--   0 root         (0) root         (0)     8918 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/recipe.py
--rw-r--r--   0 root         (0) root         (0)     4317 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/syncio/
--rw-r--r--   0 root         (0) root         (0)     3490 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3080 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/types.py
--rw-r--r--   0 root         (0) root         (0)    11762 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/
--rw-r--r--   0 root         (0) root         (0)     2619 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3816 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/emailpassword_api_impementation.py
--rw-r--r--   0 root         (0) root         (0)     7773 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     3000 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/thirdparty_api_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/asyncio/
--rw-r--r--   0 root         (0) root         (0)     6293 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     4247 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     1679 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      853 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9415 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/interfaces.py
--rw-r--r--   0 root         (0) root         (0)    15167 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4310 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/email_password_recipe_implementation.py
--rw-r--r--   0 root         (0) root         (0)     9545 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/implementation.py
--rw-r--r--   0 root         (0) root         (0)     3362 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/third_party_recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/syncio/
--rw-r--r--   0 root         (0) root         (0)     5469 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1899 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/types.py
--rw-r--r--   0 root         (0) root         (0)     9809 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/
--rw-r--r--   0 root         (0) root         (0)     3366 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8537 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/implementation.py
--rw-r--r--   0 root         (0) root         (0)     3595 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/passwordless_api_impementation.py
--rw-r--r--   0 root         (0) root         (0)     3191 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/thirdparty_api_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/asyncio/
--rw-r--r--   0 root         (0) root         (0)    11969 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/asyncio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.013614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/
--rw-r--r--   0 root         (0) root         (0)      734 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     3965 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/
--rw-r--r--   0 root         (0) root         (0)     2804 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/
--rw-r--r--   0 root         (0) root         (0)     3338 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1752 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py
--rw-r--r--   0 root         (0) root         (0)     1700 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/passwordless_implementation.py
--rw-r--r--   0 root         (0) root         (0)      852 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12463 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/interfaces.py
--rw-r--r--   0 root         (0) root         (0)    19894 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14239 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/implementation.py
--rw-r--r--   0 root         (0) root         (0)     7204 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/passwordless_recipe_implementation.py
--rw-r--r--   0 root         (0) root         (0)     3279 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/third_party_recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/
--rw-r--r--   0 root         (0) root         (0)      813 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/
--rw-r--r--   0 root         (0) root         (0)     1920 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/
--rw-r--r--   0 root         (0) root         (0)     1410 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/
--rw-r--r--   0 root         (0) root         (0)     1629 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/syncio/
--rw-r--r--   0 root         (0) root         (0)     8833 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2778 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/types.py
--rw-r--r--   0 root         (0) root         (0)    12538 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/
--rw-r--r--   0 root         (0) root         (0)     1100 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/asyncio/
--rw-r--r--   0 root         (0) root         (0)      997 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/asyncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      738 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/interfaces.py
--rw-r--r--   0 root         (0) root         (0)     3935 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/recipe.py
--rw-r--r--   0 root         (0) root         (0)     2066 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/recipe_implementation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/syncio/
--rw-r--r--   0 root         (0) root         (0)      874 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2000 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/utils.py
--rw-r--r--   0 root         (0) root         (0)     2873 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/recipe_module.py
--rw-r--r--   0 root         (0) root         (0)    18052 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/supertokens.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/supertokens_python/syncio/
--rw-r--r--   0 root         (0) root         (0)     1762 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/syncio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1973 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/types.py
--rw-r--r--   0 root         (0) root         (0)     6630 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/supertokens_python/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.989614 supertokens_python-0.9.0/supertokens_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1959 2022-06-25 14:07:30.000000 supertokens_python-0.9.0/supertokens_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17845 2022-06-25 14:07:30.000000 supertokens_python-0.9.0/supertokens_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-25 14:07:30.000000 supertokens_python-0.9.0/supertokens_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      474 2022-06-25 14:07:30.000000 supertokens_python-0.9.0/supertokens_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-06-25 14:07:30.000000 supertokens_python-0.9.0/supertokens_python.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:30.985614 supertokens_python-0.9.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/tests/Django/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Django/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Django/settings.py
--rw-r--r--   0 root         (0) root         (0)    14025 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Django/test_django.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/tests/Fastapi/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Fastapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19631 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Fastapi/test_fastapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.017614 supertokens_python-0.9.0/tests/Flask/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Flask/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17664 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Flask/test_flask.py
--rw-r--r--   0 root         (0) root         (0)     1424 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/Flask/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/emailpassword/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28196 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/test_emaildelivery.py
--rw-r--r--   0 root         (0) root         (0)    10636 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/test_emailexists.py
--rw-r--r--   0 root         (0) root         (0)    35138 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/test_emailverify.py
--rw-r--r--   0 root         (0) root         (0)    11544 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/test_passwordreset.py
--rw-r--r--   0 root         (0) root         (0)    18320 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/emailpassword/test_signin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/frontendIntegration/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/frontendIntegration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/frontendIntegration/fastapi-server/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/frontendIntegration/fastapi-server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16206 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/frontendIntegration/fastapi-server/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/frontendIntegration/flask-server/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/frontendIntegration/flask-server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17144 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/frontendIntegration/flask-server/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/input_validation/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/input_validation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26009 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/input_validation/test_input_validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/jwt/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2213 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/jwt/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5244 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/jwt/test_create_jwt_feature.py
--rw-r--r--   0 root         (0) root         (0)     3095 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/jwt/test_get_JWKS.py
--rw-r--r--   0 root         (0) root         (0)     5029 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/jwt/test_override.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/passwordless/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/passwordless/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13596 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/passwordless/test_emaildelivery.py
--rw-r--r--   0 root         (0) root         (0)    16869 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/passwordless/test_smsdelivery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/playground/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/playground/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1331 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/playground/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/telemetry/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5154 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/telemetry/test_telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/thirdparty/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdparty/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16692 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdparty/test_emaildelivery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/thirdpartyemailpassword/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdpartyemailpassword/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30348 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdpartyemailpassword/test_email_delivery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-25 14:07:31.021614 supertokens_python-0.9.0/tests/thirdpartypasswordless/
--rw-r--r--   0 root         (0) root         (0)       74 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdpartypasswordless/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29151 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdpartypasswordless/test_emaildelivery.py
--rw-r--r--   0 root         (0) root         (0)    14687 2022-06-25 14:06:56.000000 supertokens_python-0.9.0/tests/thirdpartypasswordless/test_smsdelivery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.242741 supertokens_python-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)    10921 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1959 2022-06-27 17:24:58.242741 supertokens_python-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      967 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      125 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       76 2022-06-27 17:24:58.242741 supertokens_python-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2949 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python/
+-rw-r--r--   0 root         (0) root         (0)     1555 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/async_to_sync_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     1722 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1162 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python/framework/
+-rw-r--r--   0 root         (0) root         (0)      798 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python/framework/django/
+-rw-r--r--   0 root         (0) root         (0)      781 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/django/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/django/django_middleware.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/django/django_request.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/django/django_response.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/django/framework.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python/framework/fastapi/
+-rw-r--r--   0 root         (0) root         (0)      802 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/fastapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_middleware.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_request.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_response.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/fastapi/framework.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/framework/flask/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3588 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/flask/flask_middleware.py
+-rw-r--r--   0 root         (0) root         (0)     2575 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/flask/flask_request.py
+-rw-r--r--   0 root         (0) root         (0)     3744 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/flask/flask_response.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/flask/framework.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/request.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/response.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/framework/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/ingredients/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)     1166 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/services/smtp.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/
+-rw-r--r--   0 root         (0) root         (0)     1154 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      758 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/supertokens.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/twilio.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/types.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/normalised_url_domain.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/normalised_url_path.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/process_state.py
+-rw-r--r--   0 root         (0) root         (0)     8900 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/querier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/
+-rw-r--r--   0 root         (0) root         (0)     2236 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/
+-rw-r--r--   0 root         (0) root         (0)     1034 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/email_exists.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/generate_password_reset_token.py
+-rw-r--r--   0 root         (0) root         (0)     7041 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/password_reset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/signin.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/signup.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     5188 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      968 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.158740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     5698 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     2600 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset.py
+-rw-r--r--   0 root         (0) root         (0)    20788 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset_email.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/
+-rw-r--r--   0 root         (0) root         (0)     2704 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9727 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    10518 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     6097 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/syncio/
+-rw-r--r--   0 root         (0) root         (0)     4334 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/types.py
+-rw-r--r--   0 root         (0) root         (0)    16977 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/
+-rw-r--r--   0 root         (0) root         (0)     1371 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/
+-rw-r--r--   0 root         (0) root         (0)      850 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/email_verify.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/generate_email_verify_token.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     2585 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      776 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     2915 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1899 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify.py
+-rw-r--r--   0 root         (0) root         (0)    20810 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify_email.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/service_implementation.py
+-rw-r--r--   0 root         (0) root         (0)      935 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5438 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     6771 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/syncio/
+-rw-r--r--   0 root         (0) root         (0)     2483 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/types.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/emailverification/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.162740 supertokens_python-0.9.1/supertokens_python/recipe/jwt/
+-rw-r--r--   0 root         (0) root         (0)     1163 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.166741 supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/jwks_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.166741 supertokens_python-0.9.1/supertokens_python/recipe/jwt/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     1686 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/constants.py
+-rw-r--r--   0 root         (0) root         (0)      833 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.166741 supertokens_python-0.9.1/supertokens_python/recipe/jwt/syncio/
+-rw-r--r--   0 root         (0) root         (0)     1489 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/jwt/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.186740 supertokens_python-0.9.1/supertokens_python/recipe/openid/
+-rw-r--r--   0 root         (0) root         (0)     1229 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.186740 supertokens_python-0.9.1/supertokens_python/recipe/openid/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/api/open_id_discovery_configuration_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.186740 supertokens_python-0.9.1/supertokens_python/recipe/openid/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      746 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/constants.py
+-rw-r--r--   0 root         (0) root         (0)      836 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     2896 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/openid/syncio/
+-rw-r--r--   0 root         (0) root         (0)     1669 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/openid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/
+-rw-r--r--   0 root         (0) root         (0)     3078 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/
+-rw-r--r--   0 root         (0) root         (0)      968 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/consume_code.py
+-rw-r--r--   0 root         (0) root         (0)     3925 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/create_code.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/email_exists.py
+-rw-r--r--   0 root         (0) root         (0)    11935 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/phone_number_exists.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/resend_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     8928 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      909 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     3614 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1966 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2405 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login.py
+-rw-r--r--   0 root         (0) root         (0)    66078 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login_email.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/service_implementation.py
+-rw-r--r--   0 root         (0) root         (0)      842 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13954 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    11203 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/recipe.py
+-rw-r--r--   0 root         (0) root         (0)    17638 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      813 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     4434 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/
+-rw-r--r--   0 root         (0) root         (0)     2599 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/
+-rw-r--r--   0 root         (0) root         (0)     2451 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/passwordless_login.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/service_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.190741 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/syncio/
+-rw-r--r--   0 root         (0) root         (0)     7290 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/types.py
+-rw-r--r--   0 root         (0) root         (0)    11515 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/passwordless/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/
+-rw-r--r--   0 root         (0) root         (0)     2202 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3204 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/access_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/api/
+-rw-r--r--   0 root         (0) root         (0)      794 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2928 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/api/refresh.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/api/signout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     7110 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6549 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/cookie_and_header.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     2623 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/syncio/
+-rw-r--r--   0 root         (0) root         (0)     2669 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/syncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/fastapi/
+-rw-r--r--   0 root         (0) root         (0)     1789 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/fastapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/flask/
+-rw-r--r--   0 root         (0) root         (0)     2109 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/framework/flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9417 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/jwt.py
+-rw-r--r--   0 root         (0) root         (0)    11232 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/recipe.py
+-rw-r--r--   0 root         (0) root         (0)    13933 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/recipe_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/session_class.py
+-rw-r--r--   0 root         (0) root         (0)    12467 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/session_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/syncio/
+-rw-r--r--   0 root         (0) root         (0)     5943 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14257 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/
+-rw-r--r--   0 root         (0) root         (0)      811 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      897 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/recipe_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/session_class.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/utills.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.194741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/
+-rw-r--r--   0 root         (0) root         (0)     2040 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.198741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/
+-rw-r--r--   0 root         (0) root         (0)      888 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/apple_redirect.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/authorisation_url.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3265 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/signinup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.198741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     4619 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      888 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.198741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.198741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     2842 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1606 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      840 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/
+-rw-r--r--   0 root         (0) root         (0)      965 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/apple.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/discord.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/facebook.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/github.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/google.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/google_workspaces.py
+-rw-r--r--   0 root         (0) root         (0)     3913 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/okta.py
+-rw-r--r--   0 root         (0) root         (0)     8918 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     4317 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/syncio/
+-rw-r--r--   0 root         (0) root         (0)     3490 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/types.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/
+-rw-r--r--   0 root         (0) root         (0)     2619 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/emailpassword_api_impementation.py
+-rw-r--r--   0 root         (0) root         (0)     7773 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/thirdparty_api_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     6293 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     4247 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     1679 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      853 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9415 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    15167 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4310 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/email_password_recipe_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/third_party_recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/syncio/
+-rw-r--r--   0 root         (0) root         (0)     5469 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/types.py
+-rw-r--r--   0 root         (0) root         (0)     9809 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.206741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/
+-rw-r--r--   0 root         (0) root         (0)     3366 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8537 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/passwordless_api_impementation.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/thirdparty_api_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/asyncio/
+-rw-r--r--   0 root         (0) root         (0)    11969 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/asyncio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      734 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     3965 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.210741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/
+-rw-r--r--   0 root         (0) root         (0)     2804 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/
+-rw-r--r--   0 root         (0) root         (0)     3338 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/passwordless_implementation.py
+-rw-r--r--   0 root         (0) root         (0)      852 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    19894 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14239 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/implementation.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/passwordless_recipe_implementation.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/third_party_recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/
+-rw-r--r--   0 root         (0) root         (0)      813 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/
+-rw-r--r--   0 root         (0) root         (0)     1920 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/
+-rw-r--r--   0 root         (0) root         (0)     1410 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/
+-rw-r--r--   0 root         (0) root         (0)     1629 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/syncio/
+-rw-r--r--   0 root         (0) root         (0)     8833 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/types.py
+-rw-r--r--   0 root         (0) root         (0)    12538 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/
+-rw-r--r--   0 root         (0) root         (0)     1100 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/asyncio/
+-rw-r--r--   0 root         (0) root         (0)      997 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      738 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     3935 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/syncio/
+-rw-r--r--   0 root         (0) root         (0)      874 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.222741 supertokens_python-0.9.1/supertokens_python/recipe/userroles/
+-rw-r--r--   0 root         (0) root         (0)     1094 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/supertokens_python/recipe/userroles/asyncio/
+-rw-r--r--   0 root         (0) root         (0)     4247 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/asyncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      804 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/recipe.py
+-rw-r--r--   0 root         (0) root         (0)     5672 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/recipe_implementation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/supertokens_python/recipe/userroles/syncio/
+-rw-r--r--   0 root         (0) root         (0)     4037 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe/userroles/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/recipe_module.py
+-rw-r--r--   0 root         (0) root         (0)    18052 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/supertokens.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/supertokens_python/syncio/
+-rw-r--r--   0 root         (0) root         (0)     1762 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/syncio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/types.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/supertokens_python/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.154740 supertokens_python-0.9.1/supertokens_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1959 2022-06-27 17:24:58.000000 supertokens_python-0.9.1/supertokens_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18742 2022-06-27 17:24:58.000000 supertokens_python-0.9.1/supertokens_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-06-27 17:24:58.000000 supertokens_python-0.9.1/supertokens_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-27 17:24:58.000000 supertokens_python-0.9.1/supertokens_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-06-27 17:24:58.000000 supertokens_python-0.9.1/supertokens_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.150740 supertokens_python-0.9.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/Django/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Django/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Django/settings.py
+-rw-r--r--   0 root         (0) root         (0)    14025 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Django/test_django.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/Fastapi/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Fastapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19631 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Fastapi/test_fastapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/Flask/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Flask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17664 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Flask/test_flask.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/Flask/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/emailpassword/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28196 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/test_emaildelivery.py
+-rw-r--r--   0 root         (0) root         (0)    10636 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/test_emailexists.py
+-rw-r--r--   0 root         (0) root         (0)    35352 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/test_emailverify.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/test_passwordreset.py
+-rw-r--r--   0 root         (0) root         (0)    18320 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/emailpassword/test_signin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/frontendIntegration/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/frontendIntegration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/frontendIntegration/fastapi-server/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/frontendIntegration/fastapi-server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16206 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/frontendIntegration/fastapi-server/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/frontendIntegration/flask-server/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/frontendIntegration/flask-server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17144 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/frontendIntegration/flask-server/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/input_validation/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/input_validation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26009 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/input_validation/test_input_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/jwt/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/jwt/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5244 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/jwt/test_create_jwt_feature.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/jwt/test_get_JWKS.py
+-rw-r--r--   0 root         (0) root         (0)     5029 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/jwt/test_override.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/passwordless/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/passwordless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13596 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/passwordless/test_emaildelivery.py
+-rw-r--r--   0 root         (0) root         (0)    16869 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/passwordless/test_smsdelivery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/playground/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/playground/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/playground/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.226741 supertokens_python-0.9.1/tests/telemetry/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/telemetry/test_telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.230741 supertokens_python-0.9.1/tests/thirdparty/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdparty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16692 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdparty/test_emaildelivery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.230741 supertokens_python-0.9.1/tests/thirdpartyemailpassword/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdpartyemailpassword/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30348 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdpartyemailpassword/test_email_delivery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.242741 supertokens_python-0.9.1/tests/thirdpartypasswordless/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdpartypasswordless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29151 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdpartypasswordless/test_emaildelivery.py
+-rw-r--r--   0 root         (0) root         (0)    14687 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/thirdpartypasswordless/test_smsdelivery.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-27 17:24:58.242741 supertokens_python-0.9.1/tests/userroles/
+-rw-r--r--   0 root         (0) root         (0)       74 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_add_role_to_user.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     6995 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_create_new_role_or_add_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3730 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_delete_role.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_get_permissions_for_role.py
+-rw-r--r--   0 root         (0) root         (0)     2550 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_get_roles_for_user.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_get_roles_that_have_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_get_users_that_have_role.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_remove_permissions_from_role.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2022-06-27 17:24:23.000000 supertokens_python-0.9.1/tests/userroles/test_remove_user_role.py
```

### Comparing `supertokens_python-0.9.0/LICENSE.md` & `supertokens_python-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/PKG-INFO` & `supertokens_python-0.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supertokens_python
-Version: 0.9.0
+Version: 0.9.1
 Summary: SuperTokens SDK for Python
 Home-page: https://github.com/supertokens/supertokens-python
 Author: SuperTokens
 Author-email: team@supertokens.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supertokens_python Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: supertokens_python Version: 0.9.1 Summary:
 SuperTokens SDK for Python Home-page: https://github.com/supertokens/
 supertokens-python Author: SuperTokens Author-email: team@supertokens.com
 License: Apache 2.0 Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
```

### Comparing `supertokens_python-0.9.0/README.md` & `supertokens_python-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/setup.py` & `supertokens_python-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     "Makefile",
     ".pylintrc",
     "dev-requirements.txt"
 ]
 
 setup(
     name="supertokens_python",
-    version="0.9.0",
+    version="0.9.1",
     author="SuperTokens",
     license="Apache 2.0",
     author_email="team@supertokens.com",
     description="SuperTokens SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/supertokens/supertokens-python",
```

### Comparing `supertokens_python-0.9.0/supertokens_python/__init__.py` & `supertokens_python-0.9.1/supertokens_python/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/async_to_sync_wrapper.py` & `supertokens_python-0.9.1/supertokens_python/async_to_sync_wrapper.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/constants.py` & `supertokens_python-0.9.1/supertokens_python/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 # obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-SUPPORTED_CDI_VERSIONS = ['2.9', '2.10', '2.11', '2.12', '2.13']
-VERSION = '0.9.0'
+SUPPORTED_CDI_VERSIONS = ['2.9', '2.10', '2.11', '2.12', '2.13', '2.14']
+VERSION = '0.9.1'
 TELEMETRY = '/telemetry'
 USER_COUNT = '/users/count'
 USER_DELETE = '/user/remove'
 USERS = '/users'
 TELEMETRY_SUPERTOKENS_API_URL = 'https://api.supertokens.io/0/st/telemetry'
 TELEMETRY_SUPERTOKENS_API_VERSION = '2'
 ERROR_MESSAGE_KEY = 'message'
```

### Comparing `supertokens_python-0.9.0/supertokens_python/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/__init__.py` & `supertokens_python-0.9.1/supertokens_python/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/django/__init__.py` & `supertokens_python-0.9.1/supertokens_python/framework/django/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/django/django_middleware.py` & `supertokens_python-0.9.1/supertokens_python/framework/django/django_middleware.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/django/django_request.py` & `supertokens_python-0.9.1/supertokens_python/framework/django/django_request.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/django/django_response.py` & `supertokens_python-0.9.1/supertokens_python/framework/django/django_response.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/django/framework.py` & `supertokens_python-0.9.1/supertokens_python/framework/django/framework.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/fastapi/__init__.py` & `supertokens_python-0.9.1/supertokens_python/framework/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_middleware.py` & `supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_middleware.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_request.py` & `supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_request.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/fastapi/fastapi_response.py` & `supertokens_python-0.9.1/supertokens_python/framework/fastapi/fastapi_response.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/fastapi/framework.py` & `supertokens_python-0.9.1/supertokens_python/framework/fastapi/framework.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/flask/__init__.py` & `supertokens_python-0.9.1/supertokens_python/framework/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/flask/flask_middleware.py` & `supertokens_python-0.9.1/supertokens_python/framework/flask/flask_middleware.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/flask/flask_request.py` & `supertokens_python-0.9.1/supertokens_python/framework/flask/flask_request.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/flask/flask_response.py` & `supertokens_python-0.9.1/supertokens_python/framework/flask/flask_response.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/flask/framework.py` & `supertokens_python-0.9.1/supertokens_python/framework/flask/framework.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/request.py` & `supertokens_python-0.9.1/supertokens_python/framework/request.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/response.py` & `supertokens_python-0.9.1/supertokens_python/framework/response.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/framework/types.py` & `supertokens_python-0.9.1/supertokens_python/framework/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/__init__.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/services/smtp.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/services/smtp.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/emaildelivery/types.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/emaildelivery/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/supertokens.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/supertokens.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/services/twilio.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/services/twilio.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/ingredients/smsdelivery/types.py` & `supertokens_python-0.9.1/supertokens_python/ingredients/smsdelivery/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/logger.py` & `supertokens_python-0.9.1/supertokens_python/logger.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/normalised_url_domain.py` & `supertokens_python-0.9.1/supertokens_python/normalised_url_domain.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/normalised_url_path.py` & `supertokens_python-0.9.1/supertokens_python/normalised_url_path.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/process_state.py` & `supertokens_python-0.9.1/supertokens_python/process_state.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/querier.py` & `supertokens_python-0.9.1/supertokens_python/querier.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/email_exists.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/email_exists.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/generate_password_reset_token.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/generate_password_reset_token.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/password_reset.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/password_reset.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/signin.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/signin.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/signup.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/signup.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/api/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/api/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset_email.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/password_reset_email.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailpassword/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailpassword/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/email_verify.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/email_verify.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/generate_email_verify_token.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/generate_email_verify_token.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify_email.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/email_verify_email.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/service_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/emaildelivery/services/smtp/service_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/emailverification/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/emailverification/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/api/jwks_get.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/api/jwks_get.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/jwt/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/api/open_id_discovery_configuration_get.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/api/open_id_discovery_configuration_get.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/openid/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/openid/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/consume_code.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/consume_code.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/create_code.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/create_code.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/email_exists.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/email_exists.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/phone_number_exists.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/phone_number_exists.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/api/resend_code.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/api/resend_code.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login_email.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/pless_login_email.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/service_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/emaildelivery/services/smtp/service_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/supertokens/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/passwordless_login.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/passwordless_login.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/service_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/smsdelivery/services/twilio/service_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/passwordless/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/passwordless/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/access_token.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/access_token.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/api/refresh.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/api/refresh.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/api/signout.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/api/signout.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/cookie_and_header.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/cookie_and_header.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/django/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/django/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/fastapi/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/framework/flask/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/framework/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/jwt.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/jwt.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/session_class.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/session_class.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/session_functions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/session_functions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/session_class.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/session_class.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/session/with_jwt/utills.py` & `supertokens_python-0.9.1/supertokens_python/recipe/session/with_jwt/utills.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/apple_redirect.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/apple_redirect.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/authorisation_url.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/authorisation_url.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/api/signinup.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/api/signinup.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/constants.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/constants.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/provider.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/provider.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/apple.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/apple.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/discord.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/discord.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/facebook.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/facebook.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/github.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/github.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/google.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/google.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/google_workspaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/google_workspaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/providers/okta.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/providers/okta.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdparty/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdparty/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/emailpassword_api_impementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/emailpassword_api_impementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/api/thirdparty_api_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/api/thirdparty_api_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/email_password_recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/email_password_recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/third_party_recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/recipeimplementation/third_party_recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartyemailpassword/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartyemailpassword/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/passwordless_api_impementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/passwordless_api_impementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/api/thirdparty_api_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/api/thirdparty_api_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/email_verification_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/passwordless_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/emaildelivery/services/smtp/service_implementation/passwordless_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/passwordless_recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/passwordless_recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/third_party_recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/recipeimplementation/third_party_recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/backward_compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/supertokens/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/smsdelivery/services/twilio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/types.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/thirdpartypasswordless/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/thirdpartypasswordless/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/asyncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/exceptions.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/interfaces.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/interfaces.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/recipe.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/recipe.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/recipe_implementation.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/recipe_implementation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe/usermetadata/utils.py` & `supertokens_python-0.9.1/supertokens_python/recipe/usermetadata/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/recipe_module.py` & `supertokens_python-0.9.1/supertokens_python/recipe_module.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/supertokens.py` & `supertokens_python-0.9.1/supertokens_python/supertokens.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/syncio/__init__.py` & `supertokens_python-0.9.1/supertokens_python/syncio/__init__.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/types.py` & `supertokens_python-0.9.1/supertokens_python/types.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python/utils.py` & `supertokens_python-0.9.1/supertokens_python/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/supertokens_python.egg-info/PKG-INFO` & `supertokens_python-0.9.1/supertokens_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supertokens-python
-Version: 0.9.0
+Version: 0.9.1
 Summary: SuperTokens SDK for Python
 Home-page: https://github.com/supertokens/supertokens-python
 Author: SuperTokens
 Author-email: team@supertokens.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: supertokens-python Version: 0.9.0 Summary:
+Metadata-Version: 2.1 Name: supertokens-python Version: 0.9.1 Summary:
 SuperTokens SDK for Python Home-page: https://github.com/supertokens/
 supertokens-python Author: SuperTokens Author-email: team@supertokens.com
 License: Apache 2.0 Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Intended Audience ::
```

### Comparing `supertokens_python-0.9.0/supertokens_python.egg-info/SOURCES.txt` & `supertokens_python-0.9.1/supertokens_python.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -263,14 +263,22 @@
 supertokens_python/recipe/usermetadata/exceptions.py
 supertokens_python/recipe/usermetadata/interfaces.py
 supertokens_python/recipe/usermetadata/recipe.py
 supertokens_python/recipe/usermetadata/recipe_implementation.py
 supertokens_python/recipe/usermetadata/utils.py
 supertokens_python/recipe/usermetadata/asyncio/__init__.py
 supertokens_python/recipe/usermetadata/syncio/__init__.py
+supertokens_python/recipe/userroles/__init__.py
+supertokens_python/recipe/userroles/exceptions.py
+supertokens_python/recipe/userroles/interfaces.py
+supertokens_python/recipe/userroles/recipe.py
+supertokens_python/recipe/userroles/recipe_implementation.py
+supertokens_python/recipe/userroles/utils.py
+supertokens_python/recipe/userroles/asyncio/__init__.py
+supertokens_python/recipe/userroles/syncio/__init__.py
 supertokens_python/syncio/__init__.py
 tests/Django/__init__.py
 tests/Django/settings.py
 tests/Django/test_django.py
 tests/Fastapi/__init__.py
 tests/Fastapi/test_fastapi.py
 tests/Flask/__init__.py
@@ -303,8 +311,19 @@
 tests/telemetry/test_telemetry.py
 tests/thirdparty/__init__.py
 tests/thirdparty/test_emaildelivery.py
 tests/thirdpartyemailpassword/__init__.py
 tests/thirdpartyemailpassword/test_email_delivery.py
 tests/thirdpartypasswordless/__init__.py
 tests/thirdpartypasswordless/test_emaildelivery.py
-tests/thirdpartypasswordless/test_smsdelivery.py
+tests/thirdpartypasswordless/test_smsdelivery.py
+tests/userroles/__init__.py
+tests/userroles/test_add_role_to_user.py
+tests/userroles/test_config.py
+tests/userroles/test_create_new_role_or_add_permissions.py
+tests/userroles/test_delete_role.py
+tests/userroles/test_get_permissions_for_role.py
+tests/userroles/test_get_roles_for_user.py
+tests/userroles/test_get_roles_that_have_permissions.py
+tests/userroles/test_get_users_that_have_role.py
+tests/userroles/test_remove_permissions_from_role.py
+tests/userroles/test_remove_user_role.py
```

### Comparing `supertokens_python-0.9.0/tests/Django/settings.py` & `supertokens_python-0.9.1/tests/Django/settings.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/Django/test_django.py` & `supertokens_python-0.9.1/tests/Django/test_django.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/Fastapi/test_fastapi.py` & `supertokens_python-0.9.1/tests/Fastapi/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/Flask/test_flask.py` & `supertokens_python-0.9.1/tests/Flask/test_flask.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/Flask/utils.py` & `supertokens_python-0.9.1/tests/Flask/utils.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/emailpassword/test_emaildelivery.py` & `supertokens_python-0.9.1/tests/emailpassword/test_emaildelivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/emailpassword/test_emailexists.py` & `supertokens_python-0.9.1/tests/emailpassword/test_emailexists.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/emailpassword/test_emailverify.py` & `supertokens_python-0.9.1/tests/emailpassword/test_emailverify.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     EmailVerifyPostOkResult, VerifyEmailUsingTokenInvalidTokenError)
 from supertokens_python.recipe.emailverification.types import User as EVUser
 from supertokens_python.recipe.emailverification.utils import OverrideConfig
 from supertokens_python.recipe.session import SessionContainer
 from supertokens_python.recipe.session.asyncio import (create_new_session,
                                                        get_session,
                                                        refresh_session)
+from supertokens_python.utils import is_version_gte
 from tests.utils import (TEST_ACCESS_TOKEN_MAX_AGE_CONFIG_KEY, clean_st,
                          email_verify_token_request, extract_all_cookies,
                          reset, set_key_value_in_config, setup_st,
                          sign_up_request, start_st)
 
 
 def setup_function(_):
@@ -934,15 +935,17 @@
         recipe_list=[session.init(
             anti_csrf='VIA_TOKEN'
         ), emailpassword.init()]
     )
     start_st()
 
     version = await Querier.get_instance().get_api_version()
-    assert version in ('2.9', '2.10', '2.11', '2.12', '2.13')
+    if not is_version_gte(version, "2.9"):
+        # If the version less than 2.9, the recipe doesn't exist. So skip the test
+        return
 
     response_1 = sign_up_request(
         driver_config_client,
         "test@gmail.com",
         "testPass123")
     assert response_1.status_code == 200
     dict_response = json.loads(response_1.text)
@@ -973,15 +976,17 @@
         recipe_list=[session.init(
             anti_csrf='VIA_TOKEN'
         ), emailpassword.init()]
     )
     start_st()
 
     version = await Querier.get_instance().get_api_version()
-    assert version in ('2.9', '2.10', '2.11', '2.12', '2.13')
+    if not is_version_gte(version, "2.9"):
+        # If the version is less than 2.9, the recipe doesn't exist. So skip the test.
+        return
 
     response_1 = sign_up_request(
         driver_config_client,
         "test@gmail.com",
         "testPass123")
     assert response_1.status_code == 200
     dict_response = json.loads(response_1.text)
```

### Comparing `supertokens_python-0.9.0/tests/emailpassword/test_passwordreset.py` & `supertokens_python-0.9.1/tests/emailpassword/test_passwordreset.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/emailpassword/test_signin.py` & `supertokens_python-0.9.1/tests/emailpassword/test_signin.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/frontendIntegration/fastapi-server/app.py` & `supertokens_python-0.9.1/tests/frontendIntegration/fastapi-server/app.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/frontendIntegration/flask-server/app.py` & `supertokens_python-0.9.1/tests/frontendIntegration/flask-server/app.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/input_validation/test_input_validation.py` & `supertokens_python-0.9.1/tests/input_validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/jwt/test_config.py` & `supertokens_python-0.9.1/tests/jwt/test_config.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/jwt/test_create_jwt_feature.py` & `supertokens_python-0.9.1/tests/jwt/test_create_jwt_feature.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/jwt/test_get_JWKS.py` & `supertokens_python-0.9.1/tests/jwt/test_get_JWKS.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/jwt/test_override.py` & `supertokens_python-0.9.1/tests/jwt/test_override.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/passwordless/test_emaildelivery.py` & `supertokens_python-0.9.1/tests/passwordless/test_emaildelivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/passwordless/test_smsdelivery.py` & `supertokens_python-0.9.1/tests/passwordless/test_smsdelivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/playground/app.py` & `supertokens_python-0.9.1/tests/playground/app.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/telemetry/test_telemetry.py` & `supertokens_python-0.9.1/tests/telemetry/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/thirdparty/test_emaildelivery.py` & `supertokens_python-0.9.1/tests/thirdparty/test_emaildelivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/thirdpartyemailpassword/test_email_delivery.py` & `supertokens_python-0.9.1/tests/thirdpartyemailpassword/test_email_delivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/thirdpartypasswordless/test_emaildelivery.py` & `supertokens_python-0.9.1/tests/thirdpartypasswordless/test_emaildelivery.py`

 * *Files identical despite different names*

### Comparing `supertokens_python-0.9.0/tests/thirdpartypasswordless/test_smsdelivery.py` & `supertokens_python-0.9.1/tests/thirdpartypasswordless/test_smsdelivery.py`

 * *Files identical despite different names*

