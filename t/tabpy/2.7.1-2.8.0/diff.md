# Comparing `tmp/tabpy-2.7.1.tar.gz` & `tmp/tabpy-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabpy-2.7.1.tar", last modified: Tue May  9 13:32:33 2023, max compression
+gzip compressed data, was "tabpy-2.8.0.tar", last modified: Tue May 23 12:42:09 2023, max compression
```

## Comparing `tabpy-2.7.1.tar` & `tabpy-2.8.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.929614 tabpy-2.7.1/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.146024 tabpy-2.7.1/.github/
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.373766 tabpy-2.7.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/ISSUE_TEMPLATE/tabpy-issue-report.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.376766 tabpy-2.7.1/.github/PULL_REQUEST_TEMPLATE/
--rw-rw-rw-   0        0        0     1400 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.390766 tabpy-2.7.1/.github/workflows/
--rw-rw-rw-   0        0        0      971 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/workflows/coverage.yml
--rw-rw-rw-   0        0        0     1439 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/workflows/docker-publish.yml
--rw-rw-rw-   0        0        0     1138 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/workflows/lint.yml
--rw-rw-rw-   0        0        0      758 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/workflows/pull_request.yml
--rw-rw-rw-   0        0        0      752 2023-05-02 13:24:30.000000 tabpy-2.7.1/.github/workflows/push.yml
--rw-rw-rw-   0        0        0     1659 2023-05-02 13:24:30.000000 tabpy-2.7.1/.gitignore
--rw-rw-rw-   0        0        0       66 2023-05-02 13:24:30.000000 tabpy-2.7.1/.pep8speaks.yml
--rw-rw-rw-   0        0        0      831 2023-05-02 13:24:30.000000 tabpy-2.7.1/.scrutinizer.yml
--rw-rw-rw-   0        0        0     5217 2023-05-02 13:24:30.000000 tabpy-2.7.1/CHANGELOG
--rw-rw-rw-   0        0        0     3969 2023-05-02 13:24:30.000000 tabpy-2.7.1/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      272 2023-05-02 13:24:30.000000 tabpy-2.7.1/Dockerfile
--rw-rw-rw-   0        0        0     1099 2023-05-02 13:24:30.000000 tabpy-2.7.1/LICENSE
--rw-rw-rw-   0        0        0      549 2023-05-02 13:24:30.000000 tabpy-2.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6773 2023-05-09 13:32:33.929614 tabpy-2.7.1/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-05-02 13:24:30.000000 tabpy-2.7.1/Procfile
--rw-rw-rw-   0        0        0     3334 2023-05-02 13:24:30.000000 tabpy-2.7.1/README.md
--rw-rw-rw-   0        0        0       27 2023-05-02 13:24:30.000000 tabpy-2.7.1/_config.yml
--rw-rw-rw-   0        0        0      765 2023-05-02 13:24:30.000000 tabpy-2.7.1/app.json
--rw-rw-rw-   0        0        0     2523 2023-05-02 13:24:30.000000 tabpy-2.7.1/codeql-analysis.yml
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.442102 tabpy-2.7.1/docs/
--rw-rw-rw-   0        0        0     7688 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/TableauConfiguration.md
--rw-rw-rw-   0        0        0      887 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/about.md
--rw-rw-rw-   0        0        0      426 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/deploy-to-heroku.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.452945 tabpy-2.7.1/docs/img/
--rw-rw-rw-   0        0        0   136889 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/img/Example1-SimpleFunctionCall.png
--rw-rw-rw-   0        0        0   188230 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/img/Example2-MultipleFunctionCalls.png
--rw-rw-rw-   0        0        0    43399 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/img/python-calculated-field.png
--rw-rw-rw-   0        0        0     1229 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/security.md
--rw-rw-rw-   0        0        0    13360 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/server-config.md
--rw-rw-rw-   0        0        0     1422 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/server-install.md
--rw-rw-rw-   0        0        0     4268 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/server-rest.md
--rw-rw-rw-   0        0        0    17022 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/tabpy-tools.md
--rw-rw-rw-   0        0        0     2174 2023-05-02 13:24:30.000000 tabpy-2.7.1/docs/tabpy-virtualenv.md
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.459944 tabpy-2.7.1/misc/
--rw-rw-rw-   0        0        0     3747 2023-05-02 13:24:30.000000 tabpy-2.7.1/misc/TabPy.postman_collection.json
--rw-rw-rw-   0        0        0     7855 2023-05-02 13:24:30.000000 tabpy-2.7.1/misc/TabPy.yml
--rw-rw-rw-   0        0        0       90 2023-05-02 13:24:30.000000 tabpy-2.7.1/requirements.txt
--rw-rw-rw-   0        0        0        6 2023-05-02 13:24:30.000000 tabpy-2.7.1/requirements_dev.txt
--rw-rw-rw-   0        0        0      337 2023-05-09 13:32:33.933615 tabpy-2.7.1/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-05-02 13:24:30.000000 tabpy-2.7.1/setup.py
--rw-rw-rw-   0        0        0      512 2023-05-02 13:24:30.000000 tabpy-2.7.1/start.sh
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.475940 tabpy-2.7.1/tabpy/
--rw-rw-rw-   0        0        0        7 2023-05-09 13:25:50.000000 tabpy-2.7.1/tabpy/VERSION
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.506197 tabpy-2.7.1/tabpy/models/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/__init__.py
--rw-rw-rw-   0        0        0      820 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/deploy_models.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.521195 tabpy-2.7.1/tabpy/models/scripts/
--rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/scripts/ANOVA.py
--rw-rw-rw-   0        0        0     2258 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/scripts/PCA.py
--rw-rw-rw-   0        0        0     1476 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/scripts/SentimentAnalysis.py
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/scripts/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/scripts/tTest.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.528196 tabpy-2.7.1/tabpy/models/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/utils/__init__.py
--rw-rw-rw-   0        0        0     1789 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/models/utils/setup_utils.py
--rw-rw-rw-   0        0        0      889 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.534195 tabpy-2.7.1/tabpy/tabpy_server/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.550194 tabpy-2.7.1/tabpy/tabpy_server/app/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/app/__init__.py
--rw-rw-rw-   0        0        0    20043 2023-05-09 13:25:50.000000 tabpy-2.7.1/tabpy/tabpy_server/app/app.py
--rw-rw-rw-   0        0        0     1560 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/app/app_parameters.py
--rw-rw-rw-   0        0        0     5396 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/app/arrow_server.py
--rw-rw-rw-   0        0        0     2723 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/app/util.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.569198 tabpy-2.7.1/tabpy/tabpy_server/common/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/common/__init__.py
--rw-rw-rw-   0        0        0     1985 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/common/default.conf
--rw-rw-rw-   0        0        0     3010 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/common/endpoint_file_mgr.py
--rw-rw-rw-   0        0        0     3828 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/common/messages.py
--rw-rw-rw-   0        0        0      107 2023-05-02 13:24:30.000000 tabpy-2.7.1/tabpy/tabpy_server/common/util.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.610194 tabpy-2.7.1/tabpy/tabpy_server/handlers/
--rw-rw-rw-   0        0        0     1014 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/__init__.py
--rw-rw-rw-   0        0        0    15551 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/base_handler.py
--rw-rw-rw-   0        0        0     1735 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
--rw-rw-rw-   0        0        0     5068 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/endpoint_handler.py
--rw-rw-rw-   0        0        0     2598 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/endpoints_handler.py
--rw-rw-rw-   0        0        0     8200 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
--rw-rw-rw-   0        0        0     5840 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/management_handler.py
--rw-rw-rw-   0        0        0      211 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/no_op_auth_handler.py
--rw-rw-rw-   0        0        0     8294 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/query_plane_handler.py
--rw-rw-rw-   0        0        0      998 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/service_info_handler.py
--rw-rw-rw-   0        0        0      921 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/status_handler.py
--rw-rw-rw-   0        0        0      721 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/upload_destination_handler.py
--rw-rw-rw-   0        0        0     1005 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/handlers/util.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.623193 tabpy-2.7.1/tabpy/tabpy_server/management/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/management/__init__.py
--rw-rw-rw-   0        0        0    21331 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/management/state.py
--rw-rw-rw-   0        0        0     1524 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/management/util.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.647742 tabpy-2.7.1/tabpy/tabpy_server/psws/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/psws/__init__.py
--rw-rw-rw-   0        0        0     7364 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/psws/callbacks.py
--rw-rw-rw-   0        0        0     9732 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/psws/python_service.py
--rw-rw-rw-   0        0        0      269 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/state.ini.template
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.666743 tabpy-2.7.1/tabpy/tabpy_server/static/
--rw-rw-rw-   0        0        0     1768 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/static/TabPy_logo.png
--rw-rw-rw-   0        0        0     1619 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/static/index.html
--rw-rw-rw-   0        0        0    33575 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_server/static/tableau.png
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.703742 tabpy-2.7.1/tabpy/tabpy_tools/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/__init__.py
--rw-rw-rw-   0        0        0    12171 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/client.py
--rw-rw-rw-   0        0        0     2429 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/custom_query_object.py
--rw-rw-rw-   0        0        0     3052 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/query_object.py
--rw-rw-rw-   0        0        0    13521 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/rest.py
--rw-rw-rw-   0        0        0     7283 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/rest_client.py
--rw-rw-rw-   0        0        0     4241 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/tabpy_tools/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.717742 tabpy-2.7.1/tabpy/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2023-05-02 13:24:31.000000 tabpy-2.7.1/tabpy/utils/tabpy_user.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.500670 tabpy-2.7.1/tabpy.egg-info/
--rw-rw-rw-   0        0        0     6773 2023-05-09 13:32:32.000000 tabpy-2.7.1/tabpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4829 2023-05-09 13:32:33.000000 tabpy-2.7.1/tabpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 13:32:32.000000 tabpy-2.7.1/tabpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-05-09 13:32:32.000000 tabpy-2.7.1/tabpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      218 2023-05-09 13:32:32.000000 tabpy-2.7.1/tabpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-09 13:32:32.000000 tabpy-2.7.1/tabpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.720743 tabpy-2.7.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.820474 tabpy-2.7.1/tests/integration/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/__init__.py
--rw-rw-rw-   0        0        0    10362 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/integ_test_base.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.856107 tabpy-2.7.1/tests/integration/resources/
--rw-rw-rw-   0        0        0     1398 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/2019_04_24_to_3018_08_25.crt
--rw-rw-rw-   0        0        0     1706 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/2019_04_24_to_3018_08_25.key
--rw-rw-rw-   0        0        0     1347 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/data.csv
--rw-rw-rw-   0        0        0     1569 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/deploy_and_evaluate_model.conf
--rw-rw-rw-   0        0        0     1582 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/deploy_and_evaluate_model_auth.conf
--rw-rw-rw-   0        0        0      136 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/resources/pwdfile.txt
--rw-rw-rw-   0        0        0     2246 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_arrow_server.py
--rw-rw-rw-   0        0        0     2461 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_auth.py
--rw-rw-rw-   0        0        0     1261 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_custom_evaluate_timeout.py
--rw-rw-rw-   0        0        0     1067 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model.py
--rw-rw-rw-   0        0        0     1267 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model_auth_on.py
--rw-rw-rw-   0        0        0     1506 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model_ssl.py
--rw-rw-rw-   0        0        0      736 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_model_ssl_off_auth_off.py
--rw-rw-rw-   0        0        0      950 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_model_ssl_off_auth_on.py
--rw-rw-rw-   0        0        0     1112 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_model_ssl_on_auth_off.py
--rw-rw-rw-   0        0        0     3045 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_deploy_model_ssl_on_auth_on.py
--rw-rw-rw-   0        0        0     3295 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_evaluate.py
--rw-rw-rw-   0        0        0     3376 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_gzip.py
--rw-rw-rw-   0        0        0      725 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_url.py
--rw-rw-rw-   0        0        0      986 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/integration/test_url_ssl.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.863110 tabpy-2.7.1/tests/unit/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.903616 tabpy-2.7.1/tests/unit/server_tests/
--rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.913614 tabpy-2.7.1/tests/unit/server_tests/resources/
--rw-rw-rw-   0        0        0      758 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/resources/expired.crt
--rw-rw-rw-   0        0        0     4330 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/resources/future.crt
--rw-rw-rw-   0        0        0     1410 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/resources/valid.crt
--rw-rw-rw-   0        0        0    13712 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_config.py
--rw-rw-rw-   0        0        0      486 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_endpoint_file_manager.py
--rw-rw-rw-   0        0        0     5347 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_endpoint_handler.py
--rw-rw-rw-   0        0        0     4729 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_endpoints_handler.py
--rw-rw-rw-   0        0        0    16279 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_evaluation_plane_handler.py
--rw-rw-rw-   0        0        0     5711 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_pwd_file.py
--rw-rw-rw-   0        0        0     5519 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/server_tests/test_service_info_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-09 13:32:33.927613 tabpy-2.7.1/tests/unit/tools_tests/
--rw-rw-rw-   0        0        0      100 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/tools_tests/__init__.py
--rw-rw-rw-   0        0        0     3262 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/tools_tests/test_client.py
--rw-rw-rw-   0        0        0     7665 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/tools_tests/test_rest.py
--rw-rw-rw-   0        0        0     1959 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/tools_tests/test_rest_object.py
--rw-rw-rw-   0        0        0     1082 2023-05-02 13:24:31.000000 tabpy-2.7.1/tests/unit/tools_tests/test_schema.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.526171 tabpy-2.8.0/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.411565 tabpy-2.8.0/.github/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.613079 tabpy-2.8.0/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.613079 tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-rw-rw-   0        0        0     1400 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.659955 tabpy-2.8.0/.github/workflows/
+-rw-rw-rw-   0        0        0      971 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/coverage.yml
+-rw-rw-rw-   0        0        0     1439 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/docker-publish.yml
+-rw-rw-rw-   0        0        0     1138 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/lint.yml
+-rw-rw-rw-   0        0        0      758 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/pull_request.yml
+-rw-rw-rw-   0        0        0      752 2023-05-02 13:24:30.000000 tabpy-2.8.0/.github/workflows/push.yml
+-rw-rw-rw-   0        0        0     1659 2023-05-02 13:24:30.000000 tabpy-2.8.0/.gitignore
+-rw-rw-rw-   0        0        0       66 2023-05-02 13:24:30.000000 tabpy-2.8.0/.pep8speaks.yml
+-rw-rw-rw-   0        0        0      831 2023-05-02 13:24:30.000000 tabpy-2.8.0/.scrutinizer.yml
+-rw-rw-rw-   0        0        0     5351 2023-05-23 12:40:10.000000 tabpy-2.8.0/CHANGELOG
+-rw-rw-rw-   0        0        0     3969 2023-05-02 13:24:30.000000 tabpy-2.8.0/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      272 2023-05-02 13:24:30.000000 tabpy-2.8.0/Dockerfile
+-rw-rw-rw-   0        0        0     1099 2023-05-02 13:24:30.000000 tabpy-2.8.0/LICENSE
+-rw-rw-rw-   0        0        0      549 2023-05-02 13:24:30.000000 tabpy-2.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6907 2023-05-23 12:42:09.526171 tabpy-2.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-05-02 13:24:30.000000 tabpy-2.8.0/Procfile
+-rw-rw-rw-   0        0        0     3334 2023-05-02 13:24:30.000000 tabpy-2.8.0/README.md
+-rw-rw-rw-   0        0        0       27 2023-05-02 13:24:30.000000 tabpy-2.8.0/_config.yml
+-rw-rw-rw-   0        0        0      765 2023-05-02 13:24:30.000000 tabpy-2.8.0/app.json
+-rw-rw-rw-   0        0        0     2523 2023-05-02 13:24:30.000000 tabpy-2.8.0/codeql-analysis.yml
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.722367 tabpy-2.8.0/docs/
+-rw-rw-rw-   0        0        0     7688 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/TableauConfiguration.md
+-rw-rw-rw-   0        0        0      887 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/about.md
+-rw-rw-rw-   0        0        0      426 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/deploy-to-heroku.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.738080 tabpy-2.8.0/docs/img/
+-rw-rw-rw-   0        0        0   136889 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/Example1-SimpleFunctionCall.png
+-rw-rw-rw-   0        0        0   188230 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/Example2-MultipleFunctionCalls.png
+-rw-rw-rw-   0        0        0    43399 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/img/python-calculated-field.png
+-rw-rw-rw-   0        0        0     1229 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/security.md
+-rw-rw-rw-   0        0        0    13360 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-config.md
+-rw-rw-rw-   0        0        0     1422 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-install.md
+-rw-rw-rw-   0        0        0     4268 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/server-rest.md
+-rw-rw-rw-   0        0        0    17022 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/tabpy-tools.md
+-rw-rw-rw-   0        0        0     2174 2023-05-02 13:24:30.000000 tabpy-2.8.0/docs/tabpy-virtualenv.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.753703 tabpy-2.8.0/misc/
+-rw-rw-rw-   0        0        0     3747 2023-05-02 13:24:30.000000 tabpy-2.8.0/misc/TabPy.postman_collection.json
+-rw-rw-rw-   0        0        0     7855 2023-05-02 13:24:30.000000 tabpy-2.8.0/misc/TabPy.yml
+-rw-rw-rw-   0        0        0       90 2023-05-02 13:24:30.000000 tabpy-2.8.0/requirements.txt
+-rw-rw-rw-   0        0        0        6 2023-05-02 13:24:30.000000 tabpy-2.8.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0      337 2023-05-23 12:42:09.526171 tabpy-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3708 2023-05-02 13:24:30.000000 tabpy-2.8.0/setup.py
+-rw-rw-rw-   0        0        0      512 2023-05-02 13:24:30.000000 tabpy-2.8.0/start.sh
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.769235 tabpy-2.8.0/tabpy/
+-rw-rw-rw-   0        0        0        7 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/VERSION
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.831833 tabpy-2.8.0/tabpy/models/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/__init__.py
+-rw-rw-rw-   0        0        0      820 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/deploy_models.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.863090 tabpy-2.8.0/tabpy/models/scripts/
+-rw-rw-rw-   0        0        0      715 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/ANOVA.py
+-rw-rw-rw-   0        0        0     2258 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/PCA.py
+-rw-rw-rw-   0        0        0     1476 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/SentimentAnalysis.py
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1416 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/scripts/tTest.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.878705 tabpy-2.8.0/tabpy/models/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/utils/__init__.py
+-rw-rw-rw-   0        0        0     1789 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/models/utils/setup_utils.py
+-rw-rw-rw-   0        0        0      889 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.894383 tabpy-2.8.0/tabpy/tabpy_server/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.925580 tabpy-2.8.0/tabpy/tabpy_server/app/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/__init__.py
+-rw-rw-rw-   0        0        0    20759 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/app/app.py
+-rw-rw-rw-   0        0        0     1560 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/app_parameters.py
+-rw-rw-rw-   0        0        0     5396 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/arrow_server.py
+-rw-rw-rw-   0        0        0     2723 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/app/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.956884 tabpy-2.8.0/tabpy/tabpy_server/common/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/__init__.py
+-rw-rw-rw-   0        0        0     1985 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/default.conf
+-rw-rw-rw-   0        0        0     3010 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/endpoint_file_mgr.py
+-rw-rw-rw-   0        0        0     3828 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/messages.py
+-rw-rw-rw-   0        0        0      107 2023-05-02 13:24:30.000000 tabpy-2.8.0/tabpy/tabpy_server/common/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.069768 tabpy-2.8.0/tabpy/tabpy_server/handlers/
+-rw-rw-rw-   0        0        0     1014 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/__init__.py
+-rw-rw-rw-   0        0        0    16470 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1735 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py
+-rw-rw-rw-   0        0        0     5068 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoint_handler.py
+-rw-rw-rw-   0        0        0     2598 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoints_handler.py
+-rw-rw-rw-   0        0        0     8376 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5840 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/management_handler.py
+-rw-rw-rw-   0        0        0      211 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/no_op_auth_handler.py
+-rw-rw-rw-   0        0        0     8448 2023-05-23 12:40:10.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/query_plane_handler.py
+-rw-rw-rw-   0        0        0      998 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/service_info_handler.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/status_handler.py
+-rw-rw-rw-   0        0        0      721 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/upload_destination_handler.py
+-rw-rw-rw-   0        0        0     1005 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/handlers/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.085290 tabpy-2.8.0/tabpy/tabpy_server/management/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/__init__.py
+-rw-rw-rw-   0        0        0    21331 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/state.py
+-rw-rw-rw-   0        0        0     1524 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/management/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.116642 tabpy-2.8.0/tabpy/tabpy_server/psws/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/__init__.py
+-rw-rw-rw-   0        0        0     7364 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/callbacks.py
+-rw-rw-rw-   0        0        0     9732 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/psws/python_service.py
+-rw-rw-rw-   0        0        0      269 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/state.ini.template
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.147893 tabpy-2.8.0/tabpy/tabpy_server/static/
+-rw-rw-rw-   0        0        0     1768 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/TabPy_logo.png
+-rw-rw-rw-   0        0        0     1619 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/index.html
+-rw-rw-rw-   0        0        0    33575 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_server/static/tableau.png
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.179046 tabpy-2.8.0/tabpy/tabpy_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/__init__.py
+-rw-rw-rw-   0        0        0    12171 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/client.py
+-rw-rw-rw-   0        0        0     2429 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/custom_query_object.py
+-rw-rw-rw-   0        0        0     3052 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/query_object.py
+-rw-rw-rw-   0        0        0    13521 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/rest.py
+-rw-rw-rw-   0        0        0     7283 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/rest_client.py
+-rw-rw-rw-   0        0        0     4241 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/tabpy_tools/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.194671 tabpy-2.8.0/tabpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-05-02 13:24:31.000000 tabpy-2.8.0/tabpy/utils/tabpy_user.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:08.816209 tabpy-2.8.0/tabpy.egg-info/
+-rw-rw-rw-   0        0        0     6907 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4829 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      218 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 12:42:08.000000 tabpy-2.8.0/tabpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.210302 tabpy-2.8.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.335501 tabpy-2.8.0/tests/integration/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/__init__.py
+-rw-rw-rw-   0        0        0    10362 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/integ_test_base.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.382165 tabpy-2.8.0/tests/integration/resources/
+-rw-rw-rw-   0        0        0     1398 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt
+-rw-rw-rw-   0        0        0     1706 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.key
+-rw-rw-rw-   0        0        0     1347 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/data.csv
+-rw-rw-rw-   0        0        0     1569 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model.conf
+-rw-rw-rw-   0        0        0     1582 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf
+-rw-rw-rw-   0        0        0      136 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/resources/pwdfile.txt
+-rw-rw-rw-   0        0        0     2246 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_arrow_server.py
+-rw-rw-rw-   0        0        0     2461 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_auth.py
+-rw-rw-rw-   0        0        0     1261 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_custom_evaluate_timeout.py
+-rw-rw-rw-   0        0        0     1067 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model.py
+-rw-rw-rw-   0        0        0     1267 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py
+-rw-rw-rw-   0        0        0     1506 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_ssl.py
+-rw-rw-rw-   0        0        0      736 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_off.py
+-rw-rw-rw-   0        0        0      950 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_on.py
+-rw-rw-rw-   0        0        0     1112 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_off.py
+-rw-rw-rw-   0        0        0     3045 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_on.py
+-rw-rw-rw-   0        0        0     3295 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_evaluate.py
+-rw-rw-rw-   0        0        0     3376 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_gzip.py
+-rw-rw-rw-   0        0        0      725 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_url.py
+-rw-rw-rw-   0        0        0      986 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/integration/test_url_ssl.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.397890 tabpy-2.8.0/tests/unit/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.460385 tabpy-2.8.0/tests/unit/server_tests/
+-rw-rw-rw-   0        0        0        0 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.491659 tabpy-2.8.0/tests/unit/server_tests/resources/
+-rw-rw-rw-   0        0        0      758 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/expired.crt
+-rw-rw-rw-   0        0        0     4330 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/future.crt
+-rw-rw-rw-   0        0        0     1410 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/resources/valid.crt
+-rw-rw-rw-   0        0        0    13712 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_config.py
+-rw-rw-rw-   0        0        0      486 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoint_file_manager.py
+-rw-rw-rw-   0        0        0     5347 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoint_handler.py
+-rw-rw-rw-   0        0        0     4729 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_endpoints_handler.py
+-rw-rw-rw-   0        0        0    18446 2023-05-23 12:40:10.000000 tabpy-2.8.0/tests/unit/server_tests/test_evaluation_plane_handler.py
+-rw-rw-rw-   0        0        0     5711 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_pwd_file.py
+-rw-rw-rw-   0        0        0     5519 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/server_tests/test_service_info_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:42:09.526171 tabpy-2.8.0/tests/unit/tools_tests/
+-rw-rw-rw-   0        0        0      100 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/__init__.py
+-rw-rw-rw-   0        0        0     3262 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_client.py
+-rw-rw-rw-   0        0        0     7665 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_rest.py
+-rw-rw-rw-   0        0        0     1959 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_rest_object.py
+-rw-rw-rw-   0        0        0     1082 2023-05-02 13:24:31.000000 tabpy-2.8.0/tests/unit/tools_tests/test_schema.py
```

### Comparing `tabpy-2.7.1/.github/ISSUE_TEMPLATE/tabpy-issue-report.md` & `tabpy-2.8.0/.github/ISSUE_TEMPLATE/tabpy-issue-report.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `tabpy-2.8.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/workflows/coverage.yml` & `tabpy-2.8.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/workflows/docker-publish.yml` & `tabpy-2.8.0/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/workflows/lint.yml` & `tabpy-2.8.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/workflows/pull_request.yml` & `tabpy-2.8.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.github/workflows/push.yml` & `tabpy-2.8.0/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.gitignore` & `tabpy-2.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/.scrutinizer.yml` & `tabpy-2.8.0/.scrutinizer.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/CHANGELOG` & `tabpy-2.8.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v2.8.0
+
+### Improvements
+
+- Returns 413 error code when request payload exceeds 
+TABPY_MAX_REQUEST_SIZE_MB config setting.
+
 ## v2.7.0
 
 ### Improvements
 
 - Adds support for data streaming in Arrow columnar format via Apache
 Arrow Flight.
```

### Comparing `tabpy-2.7.1/CONTRIBUTING.md` & `tabpy-2.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/LICENSE` & `tabpy-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/MANIFEST.in` & `tabpy-2.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/PKG-INFO` & `tabpy-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpy
-Version: 2.7.1
+Version: 2.8.0
 Summary: Web server Tableau uses to run Python scripts.
 Home-page: https://github.com/tableau/TabPy
 Download-URL: https://pypi.org/project/tabpy
 Author: Tableau
 Author-email: github@tableau.com
 Maintainer: Tableau
 Maintainer-email: github@tableau.com
@@ -37,14 +37,21 @@
 
 TabPy (the Tableau Python Server) is an external service implementation
 which expands Tableau's capabilities by allowing users to execute Python
 scripts and saved functions via Tableau's table calculations.
 
 # Changelog
 
+## v2.8.0
+
+### Improvements
+
+- Returns 413 error code when request payload exceeds 
+TABPY_MAX_REQUEST_SIZE_MB config setting.
+
 ## v2.7.0
 
 ### Improvements
 
 - Adds support for data streaming in Arrow columnar format via Apache
 Arrow Flight.
```

### Comparing `tabpy-2.7.1/README.md` & `tabpy-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/app.json` & `tabpy-2.8.0/app.json`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/codeql-analysis.yml` & `tabpy-2.8.0/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/TableauConfiguration.md` & `tabpy-2.8.0/docs/TableauConfiguration.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/about.md` & `tabpy-2.8.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/img/Example1-SimpleFunctionCall.png` & `tabpy-2.8.0/docs/img/Example1-SimpleFunctionCall.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/img/Example2-MultipleFunctionCalls.png` & `tabpy-2.8.0/docs/img/Example2-MultipleFunctionCalls.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/img/python-calculated-field.png` & `tabpy-2.8.0/docs/img/python-calculated-field.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/security.md` & `tabpy-2.8.0/docs/security.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/server-config.md` & `tabpy-2.8.0/docs/server-config.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/server-install.md` & `tabpy-2.8.0/docs/server-install.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/server-rest.md` & `tabpy-2.8.0/docs/server-rest.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/tabpy-tools.md` & `tabpy-2.8.0/docs/tabpy-tools.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/docs/tabpy-virtualenv.md` & `tabpy-2.8.0/docs/tabpy-virtualenv.md`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/misc/TabPy.postman_collection.json` & `tabpy-2.8.0/misc/TabPy.postman_collection.json`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/misc/TabPy.yml` & `tabpy-2.8.0/misc/TabPy.yml`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/setup.py` & `tabpy-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/start.sh` & `tabpy-2.8.0/start.sh`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/deploy_models.py` & `tabpy-2.8.0/tabpy/models/deploy_models.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/scripts/ANOVA.py` & `tabpy-2.8.0/tabpy/models/scripts/ANOVA.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/scripts/PCA.py` & `tabpy-2.8.0/tabpy/models/scripts/PCA.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/scripts/SentimentAnalysis.py` & `tabpy-2.8.0/tabpy/models/scripts/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/scripts/tTest.py` & `tabpy-2.8.0/tabpy/models/scripts/tTest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/models/utils/setup_utils.py` & `tabpy-2.8.0/tabpy/models/utils/setup_utils.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy.py` & `tabpy-2.8.0/tabpy/tabpy.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/app/app.py` & `tabpy-2.8.0/tabpy/tabpy_server/app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 import configparser
 import logging
 import multiprocessing
 import os
 import shutil
 import signal
 import sys
+import _thread
+
+import tornado
+from tornado.http1connection import HTTP1Connection
+
 import tabpy
+import tabpy.tabpy_server.app.arrow_server as pa
 from tabpy.tabpy import __version__
 from tabpy.tabpy_server.app.app_parameters import ConfigParameters, SettingsParameters
 from tabpy.tabpy_server.app.util import parse_pwd_file
 from tabpy.tabpy_server.handlers.basic_auth_server_middleware_factory import BasicAuthServerMiddlewareFactory
 from tabpy.tabpy_server.handlers.no_op_auth_handler import NoOpAuthHandler
 from tabpy.tabpy_server.management.state import TabPyState
 from tabpy.tabpy_server.management.util import _get_state_from_file
@@ -22,17 +28,14 @@
     EvaluationPlaneHandler,
     EvaluationPlaneDisabledHandler,
     QueryPlaneHandler,
     ServiceInfoHandler,
     StatusHandler,
     UploadDestinationHandler,
 )
-import tornado
-import tabpy.tabpy_server.app.arrow_server as pa
-import _thread
 
 logger = logging.getLogger(__name__)
 
 def _init_asyncio_patch():
     """
     Select compatible event loop for Tornado 5+.
     As of Python 3.8, the default event loop on Windows is `proactor`,
@@ -58,14 +61,15 @@
 
     settings = {}
     subdirectory = ""
     tabpy_state = None
     python_service = None
     credentials = {}
     arrow_server = None
+    max_request_size = None
 
     def __init__(self, config_file):
         if config_file is None:
             config_file = os.path.join(
                 os.path.dirname(__file__), os.path.pardir, "common", "default.conf"
             )
 
@@ -112,19 +116,15 @@
                             tls_certificates=tls_certificates,
                             verify_client=verify_client, auth_handler=NoOpAuthHandler(),
                             middleware=auth_middleware)
         return server
 
     def run(self):
         application = self._create_tornado_web_app()
-        max_request_size = (
-            int(self.settings[SettingsParameters.MaxRequestSizeInMb]) * 1024 * 1024
-        )
-        logger.info(f"Setting max request size to {max_request_size} bytes")
-
+        
         init_model_evaluator(self.settings, self.tabpy_state, self.python_service)
 
         protocol = self.settings[SettingsParameters.TransferProtocol]
         ssl_options = None
         if protocol == "https":
             ssl_options = {
                 "certfile": self.settings[SettingsParameters.CertificateFile],
@@ -138,16 +138,16 @@
         settings = {}
         if self.settings[SettingsParameters.GzipEnabled] is True:
             settings["decompress_request"] = True
 
         application.listen(
             self.settings[SettingsParameters.Port],
             ssl_options=ssl_options,
-            max_buffer_size=max_request_size,
-            max_body_size=max_request_size,
+            max_buffer_size=self.max_request_size,
+            max_body_size=self.max_request_size,
             **settings,
         ) 
 
         logger.info(
             "Web service listening on port "
             f"{str(self.settings[SettingsParameters.Port])}"
         )
@@ -350,14 +350,20 @@
 
         # set and validate transfer protocol
         self.settings[SettingsParameters.TransferProtocol] = self.settings[
             SettingsParameters.TransferProtocol
         ].lower()
 
         self._validate_transfer_protocol_settings()
+        
+        # Set max request size in bytes
+        self.max_request_size = (
+            int(self.settings[SettingsParameters.MaxRequestSizeInMb]) * 1024 * 1024
+        )
+        logger.info(f"Setting max request size to {self.max_request_size} bytes")
 
         # if state.ini does not exist try and create it - remove
         # last dependence on batch/shell script
         self.settings[SettingsParameters.StateFilePath] = os.path.realpath(
             os.path.normpath(
                 os.path.expanduser(self.settings[SettingsParameters.StateFilePath])
             )
@@ -493,7 +499,20 @@
                 f"template {state_file_template_path}..."
             )
             shutil.copy(state_file_template_path, state_file_path)
 
         logger.info(f"Loading state from state file {state_file_path}")
         tabpy_state = _get_state_from_file(state_file_dir)
         return tabpy_state, TabPyState(config=tabpy_state, settings=self.settings)
+
+
+# Override _read_body to allow content with size exceeding max_body_size
+# This enables proper handling of 413 errors in base_handler
+def _read_body_allow_max_size(self, code, headers, delegate):
+    if "Content-Length" in headers:
+        content_length = int(headers["Content-Length"])
+        if content_length > self._max_body_size:
+            return
+    return self.original_read_body(code, headers, delegate)
+
+HTTP1Connection.original_read_body = HTTP1Connection._read_body
+HTTP1Connection._read_body = _read_body_allow_max_size
```

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/app/app_parameters.py` & `tabpy-2.8.0/tabpy/tabpy_server/app/app_parameters.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/app/arrow_server.py` & `tabpy-2.8.0/tabpy/tabpy_server/app/arrow_server.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/app/util.py` & `tabpy-2.8.0/tabpy/tabpy_server/app/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/common/default.conf` & `tabpy-2.8.0/tabpy/tabpy_server/common/default.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/common/endpoint_file_mgr.py` & `tabpy-2.8.0/tabpy/tabpy_server/common/endpoint_file_mgr.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/common/messages.py` & `tabpy-2.8.0/tabpy/tabpy_server/common/messages.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/__init__.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/base_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/base_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         self.protocol = self.settings[SettingsParameters.TransferProtocol]
         self.port = self.settings[SettingsParameters.Port]
         self.python_service = app.python_service
         self.credentials = app.credentials
         self.username = None
         self.password = None
         self.eval_timeout = self.settings[SettingsParameters.EvaluateTimeout]
+        self.max_request_size = app.max_request_size
 
         self.logger = ContextLoggerWrapper(self.request)
         self.logger.enable_context_logging(
             app.settings[SettingsParameters.LogRequestContext]
         )
         self.logger.log(logging.DEBUG, "Checking if need to handle authentication")
         self.auth_error = self.handle_authentication("v1")
@@ -438,7 +439,29 @@
             self.set_status(406)
             self.set_header("WWW-Authenticate", f'Basic realm="{self.tabpy_state.name}"')
             self.error_out(
                 406,
                 info="Not Acceptable",
                 log_message="Username or password provided when authentication not available.",
             )
+
+    def request_body_size_within_limit(self):
+        """
+        Determines if the request body size is within the specified limit.
+        
+        Returns
+        -------
+        bool
+            True if the request body size is within the limit, False otherwise.
+        """
+        if self.max_request_size is not None:
+            if "Content-Length" in self.request.headers:
+                content_length = int(self.request.headers["Content-Length"])
+                if content_length > self.max_request_size:
+                    self.error_out(
+                        413,
+                        info="Request Entity Too Large",
+                        log_message=f"Request with size {content_length} exceeded limit of {self.max_request_size} (bytes).",
+                    )
+                    return False
+
+        return True
```

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/basic_auth_server_middleware_factory.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/endpoint_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoint_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/endpoints_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/evaluation_plane_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/evaluation_plane_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         self.executor = executor
 
     @gen.coroutine
     def post(self):
         if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
             self.fail_with_auth_error()
             return
+
+        if not self.request_body_size_within_limit():
+            return
+            
         self.error_out(404, "Ad-hoc scripts have been disabled on this analytics extension, please contact your "
                             "administrator.")
 
 
 class EvaluationPlaneHandler(BaseHandler):
     """
     EvaluationPlaneHandler is responsible for running arbitrary python scripts.
@@ -161,14 +165,17 @@
         self.arrow_server.flights[key] = my_table
 
     @gen.coroutine
     def post(self):
         if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
             self.fail_with_auth_error()
             return
+        
+        if not self.request_body_size_within_limit():
+            return
 
         self._add_CORS_header()
         try:
             yield self._post_impl()
         except Exception as e:
             import traceback
             self.logger.log(logging.ERROR, traceback.format_exc())
```

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/management_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/management_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/query_plane_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/query_plane_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,22 +213,28 @@
 
     @gen.coroutine
     def get(self, endpoint_name):
         if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
             self.fail_with_auth_error()
             return
 
+        if not self.request_body_size_within_limit():
+            return
+
         start = time.time()
         endpoint_name = urllib.parse.unquote(endpoint_name)
         self._process_query(endpoint_name, start)
 
     @gen.coroutine
     def post(self, endpoint_name):
         self.logger.log(logging.DEBUG, f"Processing POST for /query/{endpoint_name}...")
 
         if self.should_fail_with_auth_error() != AuthErrorStates.NONE:
             self.fail_with_auth_error()
             return
 
+        if not self.request_body_size_within_limit():
+            return
+
         start = time.time()
         endpoint_name = urllib.parse.unquote(endpoint_name)
         self._process_query(endpoint_name, start)
```

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/service_info_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/service_info_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/status_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/status_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/upload_destination_handler.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/upload_destination_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/handlers/util.py` & `tabpy-2.8.0/tabpy/tabpy_server/handlers/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/management/state.py` & `tabpy-2.8.0/tabpy/tabpy_server/management/state.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/management/util.py` & `tabpy-2.8.0/tabpy/tabpy_server/management/util.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/psws/callbacks.py` & `tabpy-2.8.0/tabpy/tabpy_server/psws/callbacks.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/psws/python_service.py` & `tabpy-2.8.0/tabpy/tabpy_server/psws/python_service.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/static/TabPy_logo.png` & `tabpy-2.8.0/tabpy/tabpy_server/static/TabPy_logo.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/static/index.html` & `tabpy-2.8.0/tabpy/tabpy_server/static/index.html`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_server/static/tableau.png` & `tabpy-2.8.0/tabpy/tabpy_server/static/tableau.png`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/client.py` & `tabpy-2.8.0/tabpy/tabpy_tools/client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/custom_query_object.py` & `tabpy-2.8.0/tabpy/tabpy_tools/custom_query_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/query_object.py` & `tabpy-2.8.0/tabpy/tabpy_tools/query_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/rest.py` & `tabpy-2.8.0/tabpy/tabpy_tools/rest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/rest_client.py` & `tabpy-2.8.0/tabpy/tabpy_tools/rest_client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/tabpy_tools/schema.py` & `tabpy-2.8.0/tabpy/tabpy_tools/schema.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy/utils/tabpy_user.py` & `tabpy-2.8.0/tabpy/utils/tabpy_user.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tabpy.egg-info/PKG-INFO` & `tabpy-2.8.0/tabpy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpy
-Version: 2.7.1
+Version: 2.8.0
 Summary: Web server Tableau uses to run Python scripts.
 Home-page: https://github.com/tableau/TabPy
 Download-URL: https://pypi.org/project/tabpy
 Author: Tableau
 Author-email: github@tableau.com
 Maintainer: Tableau
 Maintainer-email: github@tableau.com
@@ -37,14 +37,21 @@
 
 TabPy (the Tableau Python Server) is an external service implementation
 which expands Tableau's capabilities by allowing users to execute Python
 scripts and saved functions via Tableau's table calculations.
 
 # Changelog
 
+## v2.8.0
+
+### Improvements
+
+- Returns 413 error code when request payload exceeds 
+TABPY_MAX_REQUEST_SIZE_MB config setting.
+
 ## v2.7.0
 
 ### Improvements
 
 - Adds support for data streaming in Arrow columnar format via Apache
 Arrow Flight.
```

### Comparing `tabpy-2.7.1/tabpy.egg-info/SOURCES.txt` & `tabpy-2.8.0/tabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/integ_test_base.py` & `tabpy-2.8.0/tests/integration/integ_test_base.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/resources/2019_04_24_to_3018_08_25.crt` & `tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/resources/2019_04_24_to_3018_08_25.key` & `tabpy-2.8.0/tests/integration/resources/2019_04_24_to_3018_08_25.key`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/resources/data.csv` & `tabpy-2.8.0/tests/integration/resources/data.csv`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/resources/deploy_and_evaluate_model.conf` & `tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/resources/deploy_and_evaluate_model_auth.conf` & `tabpy-2.8.0/tests/integration/resources/deploy_and_evaluate_model_auth.conf`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_arrow_server.py` & `tabpy-2.8.0/tests/integration/test_arrow_server.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_auth.py` & `tabpy-2.8.0/tests/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_custom_evaluate_timeout.py` & `tabpy-2.8.0/tests/integration/test_custom_evaluate_timeout.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model.py` & `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model_auth_on.py` & `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_and_evaluate_model_ssl.py` & `tabpy-2.8.0/tests/integration/test_deploy_and_evaluate_model_ssl.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_model_ssl_off_auth_off.py` & `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_off.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_model_ssl_off_auth_on.py` & `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_off_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_model_ssl_on_auth_off.py` & `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_off.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_deploy_model_ssl_on_auth_on.py` & `tabpy-2.8.0/tests/integration/test_deploy_model_ssl_on_auth_on.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_evaluate.py` & `tabpy-2.8.0/tests/integration/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_gzip.py` & `tabpy-2.8.0/tests/integration/test_gzip.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_url.py` & `tabpy-2.8.0/tests/integration/test_url.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/integration/test_url_ssl.py` & `tabpy-2.8.0/tests/integration/test_url_ssl.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/resources/expired.crt` & `tabpy-2.8.0/tests/unit/server_tests/resources/expired.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/resources/future.crt` & `tabpy-2.8.0/tests/unit/server_tests/resources/future.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/resources/valid.crt` & `tabpy-2.8.0/tests/unit/server_tests/resources/valid.crt`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_config.py` & `tabpy-2.8.0/tests/unit/server_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_endpoint_handler.py` & `tabpy-2.8.0/tests/unit/server_tests/test_endpoint_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_endpoints_handler.py` & `tabpy-2.8.0/tests/unit/server_tests/test_endpoints_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_evaluation_plane_handler.py` & `tabpy-2.8.0/tests/unit/server_tests/test_evaluation_plane_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import base64
+import json
 import os
 import tempfile
+import string
 
 from tornado.testing import AsyncHTTPTestCase
 
 from tabpy.tabpy_server.app.app import TabPyApp
 from tabpy.tabpy_server.handlers.util import hash_password
 
 
@@ -454,14 +456,75 @@
         response = self.fetch(
             "/evaluate",
             method="POST",
             body=self.script
         )
         self.assertEqual(200, response.code)
 
+class TestEvaluationPlaneHandlerMaxRequestSize(AsyncHTTPTestCase):
+    @classmethod
+    def setUpClass(cls):
+        prefix = "__TestEvaluationPlaneHandlerMaxRequestSize_"
+
+        # create config file
+        cls.config_file = tempfile.NamedTemporaryFile(
+            mode="w+t", prefix=prefix, suffix=".conf", delete=False
+        )
+        cls.config_file.write(
+            "[TabPy]\n"
+            "TABPY_MAX_REQUEST_SIZE_MB = 1"
+        )
+        cls.config_file.close()
+
+    @classmethod
+    def tearDownClass(cls):
+        os.remove(cls.config_file.name)
+
+    def get_app(self):
+        self.app = TabPyApp(self.config_file.name)
+        return self.app._create_tornado_web_app()
+
+    def create_large_payload(self):
+        num_chars = 2 * 1024 * 1024 # 2MB Size
+        large_string = string.printable * (num_chars // len(string.printable))
+        large_string += string.printable[:num_chars % len(string.printable)]
+        payload = {
+            "data": { "_arg1": [1, large_string] },
+            "script": "return _arg1"
+        }
+        return json.dumps(payload).encode('utf-8')
+
+    def test_evaluation_payload_exceeds_max_request_size(self):
+        response = self.fetch(
+            "/evaluate",
+            method="POST",
+            body=self.create_large_payload()
+        )
+        self.assertEqual(413, response.code)
+
+    def test_evaluation_max_request_size_not_applied(self):
+        self.app.max_request_size = None
+        response = self.fetch(
+            "/evaluate",
+            method="POST",
+            body=self.create_large_payload()
+        )
+        self.assertEqual(200, response.code)
+        self.assertEqual(1, json.loads(response.body)[0])
+
+    def test_no_content_length_header_present(self):
+        response = self.fetch(
+            "/evaluate",
+            method="POST",
+            allow_nonstandard_methods=True
+        )
+        message = json.loads(response.body)["message"]
+        # Ensure it reaches script processing stage in EvaluationPlaneHandler.post
+        self.assertEqual("Error processing script", message)
+
 
 class TestEvaluationPlaneHandlerDefault(AsyncHTTPTestCase):
     @classmethod
     def setUpClass(cls):
         prefix = "__TestEvaluationPlaneHandlerDefault_"
 
         # create config file
```

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_pwd_file.py` & `tabpy-2.8.0/tests/unit/server_tests/test_pwd_file.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/server_tests/test_service_info_handler.py` & `tabpy-2.8.0/tests/unit/server_tests/test_service_info_handler.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/tools_tests/test_client.py` & `tabpy-2.8.0/tests/unit/tools_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/tools_tests/test_rest.py` & `tabpy-2.8.0/tests/unit/tools_tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/tools_tests/test_rest_object.py` & `tabpy-2.8.0/tests/unit/tools_tests/test_rest_object.py`

 * *Files identical despite different names*

### Comparing `tabpy-2.7.1/tests/unit/tools_tests/test_schema.py` & `tabpy-2.8.0/tests/unit/tools_tests/test_schema.py`

 * *Files identical despite different names*

