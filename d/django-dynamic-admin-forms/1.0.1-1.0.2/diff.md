# Comparing `tmp/django-dynamic-admin-forms-1.0.1.tar.gz` & `tmp/django-dynamic-admin-forms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-admin-forms-1.0.1.tar", last modified: Tue May 23 08:53:26 2023, max compression
+gzip compressed data, was "django-dynamic-admin-forms-1.0.2.tar", last modified: Tue May 23 14:13:09 2023, max compression
```

## Comparing `django-dynamic-admin-forms-1.0.1.tar` & `django-dynamic-admin-forms-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     6307 2023-05-23 08:48:07.314355 django-dynamic-admin-forms-1.0.1/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.1/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.1/.editorconfig
--rw-r--r--   0        0        0     1700 2023-05-23 08:48:07.316367 django-dynamic-admin-forms-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      889 2023-05-23 08:48:07.317358 django-dynamic-admin-forms-1.0.1/.gitignore
--rw-r--r--   0        0        0     1850 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        6 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.1/.python-version
--rw-r--r--   0        0        0      551 2023-05-23 08:48:07.319356 django-dynamic-admin-forms-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0      487 2023-05-23 08:52:57.777351 django-dynamic-admin-forms-1.0.1/CHANGES.md
--rw-r--r--   0        0        0      512 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.1/Dockerfile
--rw-r--r--   0        0        0     1107 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.1/LICENSE.md
--rw-r--r--   0        0        0      145 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0     9894 2023-05-23 08:48:07.322359 django-dynamic-admin-forms-1.0.1/README.md
--rw-r--r--   0        0        0       98 2023-05-23 08:52:57.777351 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-23 08:48:07.323355 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/admin.py
--rw-r--r--   0        0        0      112 2023-05-23 08:48:07.324357 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/apps.py
--rw-r--r--   0        0        0     2330 2023-05-23 08:48:07.325356 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/static/js/dynamic_admin.js
--rw-r--r--   0        0        0     1638 2023-05-23 08:48:07.326356 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/templates/admin/change_form.html
--rw-r--r--   0        0        0      166 2023-05-23 08:52:12.885647 django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/urls.py
--rw-r--r--   0        0        0      654 2023-05-23 08:48:07.328355 django-dynamic-admin-forms-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     2847 2023-05-23 08:48:07.328864 django-dynamic-admin-forms-1.0.1/docs/conf.py
--rw-r--r--   0        0        0   946599 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/docs/demo.gif
--rw-r--r--   0        0        0       31 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.1/docs/features/changelog.rst
--rw-r--r--   0        0        0      112 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.1/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-23 08:48:07.330876 django-dynamic-admin-forms-1.0.1/docs/make.bat
--rw-r--r--   0        0        0      151 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/cypress.json
--rw-r--r--   0        0        0     1388 2023-05-23 08:48:07.331876 django-dynamic-admin-forms-1.0.1/e2e/cypress/integration/dynamic-select.spec.js
--rw-r--r--   0        0        0      783 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0      863 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/cypress/support/commands.js
--rw-r--r--   0        0        0      690 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/cypress/support/index.js
--rw-r--r--   0        0        0      135 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/cypress/support/paths.js
--rw-r--r--   0        0        0      278 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.1/e2e/package.json
--rw-r--r--   0        0        0    49959 2023-05-22 13:58:14.266926 django-dynamic-admin-forms-1.0.1/e2e/yarn.lock
--rw-r--r--   0        0        0     9275 2023-05-23 08:48:07.332876 django-dynamic-admin-forms-1.0.1/fixtures/fixtures-dev.json
--rw-r--r--   0        0        0      677 2023-05-23 08:48:07.333878 django-dynamic-admin-forms-1.0.1/manage.py
--rw-r--r--   0        0        0     3715 2023-05-23 08:48:07.335878 django-dynamic-admin-forms-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-23 08:48:07.337426 django-dynamic-admin-forms-1.0.1/pytest.init
--rw-r--r--   0        0        0     3706 2023-05-23 08:48:07.338499 django-dynamic-admin-forms-1.0.1/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-23 08:48:07.340480 django-dynamic-admin-forms-1.0.1/scripts/publish_to_pypi.ps1
--rw-r--r--   0        0        0       50 2023-05-23 08:48:07.341477 django-dynamic-admin-forms-1.0.1/scripts/publish_to_pypi.sh
--rw-r--r--   0        0        0     2579 2023-05-23 08:48:07.342529 django-dynamic-admin-forms-1.0.1/settings.py
--rw-r--r--   0        0        0       69 2023-05-23 08:48:07.342529 django-dynamic-admin-forms-1.0.1/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-23 08:48:07.343558 django-dynamic-admin-forms-1.0.1/testapp/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-23 08:48:07.344555 django-dynamic-admin-forms-1.0.1/testapp/admin.py
--rw-r--r--   0        0        0      152 2023-05-23 08:48:07.345558 django-dynamic-admin-forms-1.0.1/testapp/apps.py
--rw-r--r--   0        0        0     3002 2023-05-23 08:48:07.347565 django-dynamic-admin-forms-1.0.1/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0      593 2023-05-23 08:48:07.348555 django-dynamic-admin-forms-1.0.1/testapp/migrations/0002_extend_example.py
--rw-r--r--   0        0        0      594 2023-05-23 08:48:07.350554 django-dynamic-admin-forms-1.0.1/testapp/migrations/0003_example_file_field.py
--rw-r--r--   0        0        0        0 2023-05-23 08:48:07.351563 django-dynamic-admin-forms-1.0.1/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     1219 2023-05-23 08:48:07.352560 django-dynamic-admin-forms-1.0.1/testapp/models.py
--rw-r--r--   0        0        0      220 2023-05-22 13:58:14.270434 django-dynamic-admin-forms-1.0.1/tox.ini
--rw-r--r--   0        0        0      849 2023-05-23 08:48:07.353554 django-dynamic-admin-forms-1.0.1/urls.py
--rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 django-dynamic-admin-forms-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6307 2023-05-23 08:48:07.314355 django-dynamic-admin-forms-1.0.2/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.2/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.2/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-23 08:48:07.316367 django-dynamic-admin-forms-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      889 2023-05-23 08:48:07.317358 django-dynamic-admin-forms-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1850 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        6 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.2/.python-version
+-rw-r--r--   0        0        0      551 2023-05-23 08:48:07.319356 django-dynamic-admin-forms-1.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0      487 2023-05-23 08:52:57.777351 django-dynamic-admin-forms-1.0.2/CHANGES.md
+-rw-r--r--   0        0        0      512 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.2/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0      145 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     9894 2023-05-23 08:48:07.322359 django-dynamic-admin-forms-1.0.2/README.md
+-rw-r--r--   0        0        0      101 2023-05-23 14:12:37.984785 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-23 08:48:07.323355 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/admin.py
+-rw-r--r--   0        0        0      119 2023-05-23 14:12:37.984785 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/apps.py
+-rw-r--r--   0        0        0     2330 2023-05-23 08:48:07.325356 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/static/js/dynamic_admin.js
+-rw-r--r--   0        0        0     1638 2023-05-23 08:48:07.326356 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/templates/admin/change_form.html
+-rw-r--r--   0        0        0      175 2023-05-23 14:12:37.984785 django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/urls.py
+-rw-r--r--   0        0        0      654 2023-05-23 08:48:07.328355 django-dynamic-admin-forms-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     2847 2023-05-23 08:48:07.328864 django-dynamic-admin-forms-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0   946599 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/docs/demo.gif
+-rw-r--r--   0        0        0       31 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.2/docs/features/changelog.rst
+-rw-r--r--   0        0        0      112 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.2/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-23 08:48:07.330876 django-dynamic-admin-forms-1.0.2/docs/make.bat
+-rw-r--r--   0        0        0      151 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/cypress.json
+-rw-r--r--   0        0        0     1388 2023-05-23 08:48:07.331876 django-dynamic-admin-forms-1.0.2/e2e/cypress/integration/dynamic-select.spec.js
+-rw-r--r--   0        0        0      783 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0      863 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/cypress/support/commands.js
+-rw-r--r--   0        0        0      690 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      135 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/cypress/support/paths.js
+-rw-r--r--   0        0        0      278 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.2/e2e/package.json
+-rw-r--r--   0        0        0    49959 2023-05-22 13:58:14.266926 django-dynamic-admin-forms-1.0.2/e2e/yarn.lock
+-rw-r--r--   0        0        0     9275 2023-05-23 08:48:07.332876 django-dynamic-admin-forms-1.0.2/fixtures/fixtures-dev.json
+-rw-r--r--   0        0        0      677 2023-05-23 08:48:07.333878 django-dynamic-admin-forms-1.0.2/manage.py
+-rw-r--r--   0        0        0     3715 2023-05-23 08:48:07.335878 django-dynamic-admin-forms-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-23 08:48:07.337426 django-dynamic-admin-forms-1.0.2/pytest.init
+-rw-r--r--   0        0        0     3706 2023-05-23 08:48:07.338499 django-dynamic-admin-forms-1.0.2/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-23 08:48:07.340480 django-dynamic-admin-forms-1.0.2/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-05-23 08:48:07.341477 django-dynamic-admin-forms-1.0.2/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     2587 2023-05-23 14:12:37.984785 django-dynamic-admin-forms-1.0.2/settings.py
+-rw-r--r--   0        0        0       69 2023-05-23 08:48:07.342529 django-dynamic-admin-forms-1.0.2/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-23 08:48:07.343558 django-dynamic-admin-forms-1.0.2/testapp/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-23 08:48:07.344555 django-dynamic-admin-forms-1.0.2/testapp/admin.py
+-rw-r--r--   0        0        0      152 2023-05-23 08:48:07.345558 django-dynamic-admin-forms-1.0.2/testapp/apps.py
+-rw-r--r--   0        0        0     3002 2023-05-23 08:48:07.347565 django-dynamic-admin-forms-1.0.2/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      593 2023-05-23 08:48:07.348555 django-dynamic-admin-forms-1.0.2/testapp/migrations/0002_extend_example.py
+-rw-r--r--   0        0        0      594 2023-05-23 08:48:07.350554 django-dynamic-admin-forms-1.0.2/testapp/migrations/0003_example_file_field.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:48:07.351563 django-dynamic-admin-forms-1.0.2/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     1219 2023-05-23 08:48:07.352560 django-dynamic-admin-forms-1.0.2/testapp/models.py
+-rw-r--r--   0        0        0      856 2023-05-23 14:12:37.984785 django-dynamic-admin-forms-1.0.2/testapp/urls.py
+-rw-r--r--   0        0        0      220 2023-05-22 13:58:14.270434 django-dynamic-admin-forms-1.0.2/tox.ini
+-rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 django-dynamic-admin-forms-1.0.2/PKG-INFO
```

### Comparing `django-dynamic-admin-forms-1.0.1/.ambient-package-update/metadata.py` & `django-dynamic-admin-forms-1.0.2/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/.github/workflows/ci.yml` & `django-dynamic-admin-forms-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/.gitignore` & `django-dynamic-admin-forms-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/.gitlab-ci.yml` & `django-dynamic-admin-forms-1.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/.pre-commit-config.yaml` & `django-dynamic-admin-forms-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/.readthedocs.yml` & `django-dynamic-admin-forms-1.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/Dockerfile` & `django-dynamic-admin-forms-1.0.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/LICENSE.md` & `django-dynamic-admin-forms-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/README.md` & `django-dynamic-admin-forms-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/admin.py` & `django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/static/js/dynamic_admin.js` & `django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/static/js/dynamic_admin.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/django_dynamic_admin_forms/templates/admin/change_form.html` & `django-dynamic-admin-forms-1.0.2/django_dynamic_admin_forms/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/docs/Makefile` & `django-dynamic-admin-forms-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/docs/conf.py` & `django-dynamic-admin-forms-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/docs/demo.gif` & `django-dynamic-admin-forms-1.0.2/docs/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/docs/make.bat` & `django-dynamic-admin-forms-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/e2e/cypress/integration/dynamic-select.spec.js` & `django-dynamic-admin-forms-1.0.2/e2e/cypress/integration/dynamic-select.spec.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/e2e/cypress/plugins/index.js` & `django-dynamic-admin-forms-1.0.2/e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/e2e/cypress/support/commands.js` & `django-dynamic-admin-forms-1.0.2/e2e/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/e2e/cypress/support/index.js` & `django-dynamic-admin-forms-1.0.2/e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/e2e/yarn.lock` & `django-dynamic-admin-forms-1.0.2/e2e/yarn.lock`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/fixtures/fixtures-dev.json` & `django-dynamic-admin-forms-1.0.2/fixtures/fixtures-dev.json`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/manage.py` & `django-dynamic-admin-forms-1.0.2/manage.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/pyproject.toml` & `django-dynamic-admin-forms-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/requirements.txt` & `django-dynamic-admin-forms-1.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/settings.py` & `django-dynamic-admin-forms-1.0.2/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 SECRET_KEY = "7t!88vton98+=cb#=&4_5en37480c7+5qu9u=1@vfz#esaen0e"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = ["localhost"]
 
-ROOT_URLCONF = "urls"
+ROOT_URLCONF = "testapp.urls"
 
 INSTALLED_APPS = [
     "django_dynamic_admin_forms",
     # "jazzmin",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
```

### Comparing `django-dynamic-admin-forms-1.0.1/testapp/admin.py` & `django-dynamic-admin-forms-1.0.2/testapp/admin.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/testapp/migrations/0001_initial.py` & `django-dynamic-admin-forms-1.0.2/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/testapp/migrations/0002_extend_example.py` & `django-dynamic-admin-forms-1.0.2/testapp/migrations/0002_extend_example.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/testapp/migrations/0003_example_file_field.py` & `django-dynamic-admin-forms-1.0.2/testapp/migrations/0003_example_file_field.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/testapp/models.py` & `django-dynamic-admin-forms-1.0.2/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-1.0.1/urls.py` & `django-dynamic-admin-forms-1.0.2/testapp/urls.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,9 +14,9 @@
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
 from django.urls import include, path
 
 urlpatterns = [
     path("admin/", admin.site.urls),
-    path("dynamic-admin-form/", include("dynamic_admin_forms.urls")),
+    path("dynamic-admin-form/", include("django_dynamic_admin_forms.urls")),
 ]
```

### Comparing `django-dynamic-admin-forms-1.0.1/PKG-INFO` & `django-dynamic-admin-forms-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dynamic-admin-forms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Add simple dynamic interaction to the otherwise static django admin.
 Author-email: Ambient Digital <hello@ambient.digital>, Fabian Binz <fabian.binz@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

