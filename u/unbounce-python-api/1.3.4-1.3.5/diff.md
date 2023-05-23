# Comparing `tmp/unbounce-python-api-1.3.4.tar.gz` & `tmp/unbounce-python-api-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unbounce-python-api-1.3.4.tar", last modified: Mon Jul  5 03:56:40 2021, max compression
+gzip compressed data, was "unbounce-python-api-1.3.5.tar", last modified: Tue May 23 03:11:38 2023, max compression
```

## Comparing `unbounce-python-api-1.3.4.tar` & `unbounce-python-api-1.3.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     9437 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/PKG-INFO
-drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     9437 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)      453 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       16 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/requires.txt
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       12 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/top_level.txt
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)        1 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounce_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7220 2021-06-21 06:34:08.000000 unbounce-python-api-1.3.4/README.md
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     1028 2021-07-05 03:56:11.000000 unbounce-python-api-1.3.4/setup.py
-drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/unbounceapi/
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     4534 2020-09-17 02:10:05.000000 unbounce-python-api-1.3.4/unbounceapi/users.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    11762 2020-09-17 02:15:38.000000 unbounce-python-api-1.3.4/unbounceapi/accounts.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    15173 2020-09-17 02:16:06.000000 unbounce-python-api-1.3.4/unbounceapi/client.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7633 2020-09-17 02:15:21.000000 unbounce-python-api-1.3.4/unbounceapi/domains.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)      110 2021-07-05 03:56:10.000000 unbounce-python-api-1.3.4/unbounceapi/__init__.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     6102 2020-09-17 02:14:54.000000 unbounce-python-api-1.3.4/unbounceapi/page_groups.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     4209 2020-09-17 02:15:06.000000 unbounce-python-api-1.3.4/unbounceapi/leads.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    21063 2020-09-17 02:14:40.000000 unbounce-python-api-1.3.4/unbounceapi/pages.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    14365 2020-09-17 02:11:31.000000 unbounce-python-api-1.3.4/unbounceapi/sub_accounts.py
--rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       79 2021-07-05 03:56:40.000000 unbounce-python-api-1.3.4/setup.cfg
+drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2023-05-23 03:11:38.513698 unbounce-python-api-1.3.5/
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     1071 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/LICENSE.txt
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7979 2023-05-23 03:11:38.513822 unbounce-python-api-1.3.5/PKG-INFO
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7220 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/README.md
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       79 2023-05-23 03:11:38.514263 unbounce-python-api-1.3.5/setup.cfg
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     1038 2023-05-23 03:09:20.000000 unbounce-python-api-1.3.5/setup.py
+drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2023-05-23 03:11:38.505364 unbounce-python-api-1.3.5/tests/
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     1369 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/tests/test_unbounceapi.py
+drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2023-05-23 03:11:38.507836 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7979 2023-05-23 03:11:38.000000 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)      491 2023-05-23 03:11:38.000000 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)        1 2023-05-23 03:11:38.000000 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       16 2023-05-23 03:11:38.000000 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/requires.txt
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)       12 2023-05-23 03:11:38.000000 unbounce-python-api-1.3.5/unbounce_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 yoshiohasegawa   (501) staff       (20)        0 2023-05-23 03:11:38.513072 unbounce-python-api-1.3.5/unbounceapi/
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)      110 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/__init__.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    11762 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/accounts.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    15173 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/client.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     7633 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/domains.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     4209 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/leads.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     6102 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/page_groups.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    21063 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/pages.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)    14365 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/sub_accounts.py
+-rw-r--r--   0 yoshiohasegawa   (501) staff       (20)     4534 2023-05-23 03:03:59.000000 unbounce-python-api-1.3.5/unbounceapi/users.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `unbounce-python-api-1.3.4/PKG-INFO` & `unbounce-python-api-1.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,203 @@
 Metadata-Version: 2.1
 Name: unbounce-python-api
-Version: 1.3.4
+Version: 1.3.5
 Summary: An Unbounce API wrapper written in python.
 Home-page: https://github.com/yoshiohasegawa/unbounce-python-api
+Download-URL: https://github.com/yoshiohasegawa/unbounce-python-api/archive/refs/tags/v1.3.5.tar.gz
 Author: Yoshio Hasegawa
 Author-email: yoshio.seisuke.hasegawa@gmail.com
 License: MIT
-Download-URL: https://github.com/yoshiohasegawa/unbounce-python-api/archive/v1.3.4.tar.gz
-Description: # Unbounce API
-        An [Unbounce API](https://developer.unbounce.com/api_reference/) wrapper written in Python.
-        
-        ## Getting Started
-        Find more information on authorization, managing API keys, using OAuth, permissions, rate limits, errors, and more on the [Unbounce API webpage](https://developer.unbounce.com/getting_started/). Find the project on the Python Package Index website here: [unbounce-python-api](https://pypi.org/project/unbounce-python-api/).
-        
-        To get started, install the package:
-        ```console
-        user@machine:~/$ pip install unbounce-python-api
-        ```
-        
-        Then, import it into your project:
-        ```python
-        from unbounceapi.client import Unbounce
-        ub = Unbounce('YOUR_API_KEY')
-        ```
-        
-        ## Global API
-        Read the docs here: [Global API](https://developer.unbounce.com/api_reference/).
-        
-        **Available Methods**
-        
-        - `ub.get_global()`
-        
-        ## Accounts
-        Read the docs here: [Accounts API](https://developer.unbounce.com/api_reference/#id_accounts).
-        
-        **Available Methods**
-        
-        - `ub.accounts.get_accounts(account_id=None, **kwargs)`
-            - account_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-        
-        - `ub.accounts.get_sub_accounts(account_id, **kwargs)`
-            - accounts_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.accounts.get_account_pages(account_id, **kwargs)`
-            - account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Sub Accounts
-        Read the docs here: [Sub Accounts API](https://developer.unbounce.com/api_reference/#id_sub_accounts__sub_account_id_).
-        
-        **Available Methods**
-        
-        - `ub.sub_accounts.get_sub_account(sub_account_id)`
-            - sub_account_id (required)
-        
-        - `ub.sub_accounts.get_sub_account_domains(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or ' desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.sub_accounts.get_sub_account_page_groups(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.sub_accounts.get_sub_accounts_pages(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Domains
-        Read the docs here: [Domains API](https://developer.unbounce.com/api_reference/#id_domains__domain_id_).
-        
-        **Available Methods**
-        
-        - `ub.domains.get_domain(domain_id)`
-            - domain_id (required)
-        
-        - `ub.domains.get_domain_pages(domain_id, kwargs**)`
-            - domain_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Pages
-        Read the docs here: [Pages API](https://developer.unbounce.com/api_reference/#id_pages).
-        
-        **Available Methods**
-        
-        - `ub.pages.get_pages(page_id=None, **kwargs)`
-            - page_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-            - with_stats (optional) [Default: 'False', Options: 'True' or 'False']
-            - role (optional) [Default: 'author', Options: 'author' or 'viewer']
-        
-        - `ub.pages.get_form_fields(page_id, **kwargs)`
-            - page_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - include_sub_pages [Default: 'False', Options: 'True' or 'False']
-        
-        - `ub.pages.get_page_leads(page_id, lead_id=None, **kwargs)`
-            - page_id (required)
-            - lead_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.pages.create_page_lead(page_id)`
-            - page_id (required)
-        
-        - `ub.pages.delete_page_lead(page_id, lead_id)`
-            - page_id (required)
-            - lead_id (required)
-        
-        - `ub.pages.post_lead_deletion_request(page_id)`
-            - page_id (required)
-        
-        - `ub.pages.get_lead_deletion_request_status(page_id, lead_deletion_request_id)`
-            - page_id (required)
-            - lead_deletion_request_id (required)
-        
-        ## Page Groups
-        Read the docs here: [Page Groups API](https://developer.unbounce.com/api_reference/#id_page_groups__page_group_id__pages).
-        
-        **Available Methods**
-        
-        - `ub.page_groups.get_page_group_pages(page_group_id, **kwargs)`
-            - page_group_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', Ex: '10']
-        
-        ## Leads
-        Read the docs here: [Leads API](https://developer.unbounce.com/api_reference/#id_leads__lead_id_).
-        
-        **Available Methods**
-        
-        - `ub.leads.get_lead(lead_id)`
-            - lead_id (required)
-        
-        ## Users
-        Read the docs here: [Users API](https://developer.unbounce.com/api_reference/#id_users).
-        
-        - `ub.users.get_user(user_id=None)`
-            - user_id (optional)
-        
-        
-        ## Contact
-        For support, feedback or, to report a bug, you may contact the maintainer:
-        - Yoshio Hasegawa: [GitHub](https://github.com/yoshiohasegawa), [LinkedIn](https://www.linkedin.com/in/yoshiohasegawa/)
-        
-        ### License
-        Distributed under the MIT License.
 Keywords: Unbounce,API,Wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Unbounce API
+An [Unbounce API](https://developer.unbounce.com/api_reference/) wrapper written in Python.
+
+## Getting Started
+Find more information on authorization, managing API keys, using OAuth, permissions, rate limits, errors, and more on the [Unbounce API webpage](https://developer.unbounce.com/getting_started/). Find the project on the Python Package Index website here: [unbounce-python-api](https://pypi.org/project/unbounce-python-api/).
+
+To get started, install the package:
+```console
+user@machine:~/$ pip install unbounce-python-api
+```
+
+Then, import it into your project:
+```python
+from unbounceapi.client import Unbounce
+ub = Unbounce('YOUR_API_KEY')
+```
+
+## Global API
+Read the docs here: [Global API](https://developer.unbounce.com/api_reference/).
+
+**Available Methods**
+
+- `ub.get_global()`
+
+## Accounts
+Read the docs here: [Accounts API](https://developer.unbounce.com/api_reference/#id_accounts).
+
+**Available Methods**
+
+- `ub.accounts.get_accounts(account_id=None, **kwargs)`
+    - account_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+
+- `ub.accounts.get_sub_accounts(account_id, **kwargs)`
+    - accounts_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.accounts.get_account_pages(account_id, **kwargs)`
+    - account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Sub Accounts
+Read the docs here: [Sub Accounts API](https://developer.unbounce.com/api_reference/#id_sub_accounts__sub_account_id_).
+
+**Available Methods**
+
+- `ub.sub_accounts.get_sub_account(sub_account_id)`
+    - sub_account_id (required)
+
+- `ub.sub_accounts.get_sub_account_domains(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or ' desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.sub_accounts.get_sub_account_page_groups(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.sub_accounts.get_sub_accounts_pages(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Domains
+Read the docs here: [Domains API](https://developer.unbounce.com/api_reference/#id_domains__domain_id_).
+
+**Available Methods**
+
+- `ub.domains.get_domain(domain_id)`
+    - domain_id (required)
+
+- `ub.domains.get_domain_pages(domain_id, kwargs**)`
+    - domain_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Pages
+Read the docs here: [Pages API](https://developer.unbounce.com/api_reference/#id_pages).
+
+**Available Methods**
+
+- `ub.pages.get_pages(page_id=None, **kwargs)`
+    - page_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+    - with_stats (optional) [Default: 'False', Options: 'True' or 'False']
+    - role (optional) [Default: 'author', Options: 'author' or 'viewer']
+
+- `ub.pages.get_form_fields(page_id, **kwargs)`
+    - page_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - include_sub_pages [Default: 'False', Options: 'True' or 'False']
+
+- `ub.pages.get_page_leads(page_id, lead_id=None, **kwargs)`
+    - page_id (required)
+    - lead_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.pages.create_page_lead(page_id)`
+    - page_id (required)
+
+- `ub.pages.delete_page_lead(page_id, lead_id)`
+    - page_id (required)
+    - lead_id (required)
+
+- `ub.pages.post_lead_deletion_request(page_id)`
+    - page_id (required)
+
+- `ub.pages.get_lead_deletion_request_status(page_id, lead_deletion_request_id)`
+    - page_id (required)
+    - lead_deletion_request_id (required)
+
+## Page Groups
+Read the docs here: [Page Groups API](https://developer.unbounce.com/api_reference/#id_page_groups__page_group_id__pages).
+
+**Available Methods**
+
+- `ub.page_groups.get_page_group_pages(page_group_id, **kwargs)`
+    - page_group_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', Ex: '10']
+
+## Leads
+Read the docs here: [Leads API](https://developer.unbounce.com/api_reference/#id_leads__lead_id_).
+
+**Available Methods**
+
+- `ub.leads.get_lead(lead_id)`
+    - lead_id (required)
+
+## Users
+Read the docs here: [Users API](https://developer.unbounce.com/api_reference/#id_users).
+
+- `ub.users.get_user(user_id=None)`
+    - user_id (optional)
+
+
+## Contact
+For support, feedback or, to report a bug, you may contact the maintainer:
+- Yoshio Hasegawa: [GitHub](https://github.com/yoshiohasegawa), [LinkedIn](https://www.linkedin.com/in/yoshiohasegawa/)
+
+### License
+Distributed under the MIT License.
```

### Comparing `unbounce-python-api-1.3.4/unbounce_python_api.egg-info/PKG-INFO` & `unbounce-python-api-1.3.5/unbounce_python_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,203 @@
 Metadata-Version: 2.1
 Name: unbounce-python-api
-Version: 1.3.4
+Version: 1.3.5
 Summary: An Unbounce API wrapper written in python.
 Home-page: https://github.com/yoshiohasegawa/unbounce-python-api
+Download-URL: https://github.com/yoshiohasegawa/unbounce-python-api/archive/refs/tags/v1.3.5.tar.gz
 Author: Yoshio Hasegawa
 Author-email: yoshio.seisuke.hasegawa@gmail.com
 License: MIT
-Download-URL: https://github.com/yoshiohasegawa/unbounce-python-api/archive/v1.3.4.tar.gz
-Description: # Unbounce API
-        An [Unbounce API](https://developer.unbounce.com/api_reference/) wrapper written in Python.
-        
-        ## Getting Started
-        Find more information on authorization, managing API keys, using OAuth, permissions, rate limits, errors, and more on the [Unbounce API webpage](https://developer.unbounce.com/getting_started/). Find the project on the Python Package Index website here: [unbounce-python-api](https://pypi.org/project/unbounce-python-api/).
-        
-        To get started, install the package:
-        ```console
-        user@machine:~/$ pip install unbounce-python-api
-        ```
-        
-        Then, import it into your project:
-        ```python
-        from unbounceapi.client import Unbounce
-        ub = Unbounce('YOUR_API_KEY')
-        ```
-        
-        ## Global API
-        Read the docs here: [Global API](https://developer.unbounce.com/api_reference/).
-        
-        **Available Methods**
-        
-        - `ub.get_global()`
-        
-        ## Accounts
-        Read the docs here: [Accounts API](https://developer.unbounce.com/api_reference/#id_accounts).
-        
-        **Available Methods**
-        
-        - `ub.accounts.get_accounts(account_id=None, **kwargs)`
-            - account_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-        
-        - `ub.accounts.get_sub_accounts(account_id, **kwargs)`
-            - accounts_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.accounts.get_account_pages(account_id, **kwargs)`
-            - account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Sub Accounts
-        Read the docs here: [Sub Accounts API](https://developer.unbounce.com/api_reference/#id_sub_accounts__sub_account_id_).
-        
-        **Available Methods**
-        
-        - `ub.sub_accounts.get_sub_account(sub_account_id)`
-            - sub_account_id (required)
-        
-        - `ub.sub_accounts.get_sub_account_domains(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or ' desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.sub_accounts.get_sub_account_page_groups(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.sub_accounts.get_sub_accounts_pages(sub_account_id, **kwargs)`
-            - sub_account_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Domains
-        Read the docs here: [Domains API](https://developer.unbounce.com/api_reference/#id_domains__domain_id_).
-        
-        **Available Methods**
-        
-        - `ub.domains.get_domain(domain_id)`
-            - domain_id (required)
-        
-        - `ub.domains.get_domain_pages(domain_id, kwargs**)`
-            - domain_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        ## Pages
-        Read the docs here: [Pages API](https://developer.unbounce.com/api_reference/#id_pages).
-        
-        **Available Methods**
-        
-        - `ub.pages.get_pages(page_id=None, **kwargs)`
-            - page_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-            - with_stats (optional) [Default: 'False', Options: 'True' or 'False']
-            - role (optional) [Default: 'author', Options: 'author' or 'viewer']
-        
-        - `ub.pages.get_form_fields(page_id, **kwargs)`
-            - page_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - include_sub_pages [Default: 'False', Options: 'True' or 'False']
-        
-        - `ub.pages.get_page_leads(page_id, lead_id=None, **kwargs)`
-            - page_id (required)
-            - lead_id (optional)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', ex: '10']
-        
-        - `ub.pages.create_page_lead(page_id)`
-            - page_id (required)
-        
-        - `ub.pages.delete_page_lead(page_id, lead_id)`
-            - page_id (required)
-            - lead_id (required)
-        
-        - `ub.pages.post_lead_deletion_request(page_id)`
-            - page_id (required)
-        
-        - `ub.pages.get_lead_deletion_request_status(page_id, lead_deletion_request_id)`
-            - page_id (required)
-            - lead_deletion_request_id (required)
-        
-        ## Page Groups
-        Read the docs here: [Page Groups API](https://developer.unbounce.com/api_reference/#id_page_groups__page_group_id__pages).
-        
-        **Available Methods**
-        
-        - `ub.page_groups.get_page_group_pages(page_group_id, **kwargs)`
-            - page_group_id (required)
-            - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
-            - count (optional) [Default: 'False', Options: 'True' or 'False']
-            - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
-            - to (optional) [ex: '2018-12-31T00:00:00.000Z']
-            - offset (optional) [ex: '3']
-            - limit (optional) [Default: '50', Max: '1000', Ex: '10']
-        
-        ## Leads
-        Read the docs here: [Leads API](https://developer.unbounce.com/api_reference/#id_leads__lead_id_).
-        
-        **Available Methods**
-        
-        - `ub.leads.get_lead(lead_id)`
-            - lead_id (required)
-        
-        ## Users
-        Read the docs here: [Users API](https://developer.unbounce.com/api_reference/#id_users).
-        
-        - `ub.users.get_user(user_id=None)`
-            - user_id (optional)
-        
-        
-        ## Contact
-        For support, feedback or, to report a bug, you may contact the maintainer:
-        - Yoshio Hasegawa: [GitHub](https://github.com/yoshiohasegawa), [LinkedIn](https://www.linkedin.com/in/yoshiohasegawa/)
-        
-        ### License
-        Distributed under the MIT License.
 Keywords: Unbounce,API,Wrapper
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Unbounce API
+An [Unbounce API](https://developer.unbounce.com/api_reference/) wrapper written in Python.
+
+## Getting Started
+Find more information on authorization, managing API keys, using OAuth, permissions, rate limits, errors, and more on the [Unbounce API webpage](https://developer.unbounce.com/getting_started/). Find the project on the Python Package Index website here: [unbounce-python-api](https://pypi.org/project/unbounce-python-api/).
+
+To get started, install the package:
+```console
+user@machine:~/$ pip install unbounce-python-api
+```
+
+Then, import it into your project:
+```python
+from unbounceapi.client import Unbounce
+ub = Unbounce('YOUR_API_KEY')
+```
+
+## Global API
+Read the docs here: [Global API](https://developer.unbounce.com/api_reference/).
+
+**Available Methods**
+
+- `ub.get_global()`
+
+## Accounts
+Read the docs here: [Accounts API](https://developer.unbounce.com/api_reference/#id_accounts).
+
+**Available Methods**
+
+- `ub.accounts.get_accounts(account_id=None, **kwargs)`
+    - account_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+
+- `ub.accounts.get_sub_accounts(account_id, **kwargs)`
+    - accounts_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.accounts.get_account_pages(account_id, **kwargs)`
+    - account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Sub Accounts
+Read the docs here: [Sub Accounts API](https://developer.unbounce.com/api_reference/#id_sub_accounts__sub_account_id_).
+
+**Available Methods**
+
+- `ub.sub_accounts.get_sub_account(sub_account_id)`
+    - sub_account_id (required)
+
+- `ub.sub_accounts.get_sub_account_domains(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or ' desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.sub_accounts.get_sub_account_page_groups(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.sub_accounts.get_sub_accounts_pages(sub_account_id, **kwargs)`
+    - sub_account_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Domains
+Read the docs here: [Domains API](https://developer.unbounce.com/api_reference/#id_domains__domain_id_).
+
+**Available Methods**
+
+- `ub.domains.get_domain(domain_id)`
+    - domain_id (required)
+
+- `ub.domains.get_domain_pages(domain_id, kwargs**)`
+    - domain_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+## Pages
+Read the docs here: [Pages API](https://developer.unbounce.com/api_reference/#id_pages).
+
+**Available Methods**
+
+- `ub.pages.get_pages(page_id=None, **kwargs)`
+    - page_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+    - with_stats (optional) [Default: 'False', Options: 'True' or 'False']
+    - role (optional) [Default: 'author', Options: 'author' or 'viewer']
+
+- `ub.pages.get_form_fields(page_id, **kwargs)`
+    - page_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - include_sub_pages [Default: 'False', Options: 'True' or 'False']
+
+- `ub.pages.get_page_leads(page_id, lead_id=None, **kwargs)`
+    - page_id (required)
+    - lead_id (optional)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', ex: '10']
+
+- `ub.pages.create_page_lead(page_id)`
+    - page_id (required)
+
+- `ub.pages.delete_page_lead(page_id, lead_id)`
+    - page_id (required)
+    - lead_id (required)
+
+- `ub.pages.post_lead_deletion_request(page_id)`
+    - page_id (required)
+
+- `ub.pages.get_lead_deletion_request_status(page_id, lead_deletion_request_id)`
+    - page_id (required)
+    - lead_deletion_request_id (required)
+
+## Page Groups
+Read the docs here: [Page Groups API](https://developer.unbounce.com/api_reference/#id_page_groups__page_group_id__pages).
+
+**Available Methods**
+
+- `ub.page_groups.get_page_group_pages(page_group_id, **kwargs)`
+    - page_group_id (required)
+    - sort_order (optional) [Default: 'asc', Options: 'asc' or 'desc']
+    - count (optional) [Default: 'False', Options: 'True' or 'False']
+    - _from (optional) [ex: '2018-01-01T00:00:00.000Z']
+    - to (optional) [ex: '2018-12-31T00:00:00.000Z']
+    - offset (optional) [ex: '3']
+    - limit (optional) [Default: '50', Max: '1000', Ex: '10']
+
+## Leads
+Read the docs here: [Leads API](https://developer.unbounce.com/api_reference/#id_leads__lead_id_).
+
+**Available Methods**
+
+- `ub.leads.get_lead(lead_id)`
+    - lead_id (required)
+
+## Users
+Read the docs here: [Users API](https://developer.unbounce.com/api_reference/#id_users).
+
+- `ub.users.get_user(user_id=None)`
+    - user_id (optional)
+
+
+## Contact
+For support, feedback or, to report a bug, you may contact the maintainer:
+- Yoshio Hasegawa: [GitHub](https://github.com/yoshiohasegawa), [LinkedIn](https://www.linkedin.com/in/yoshiohasegawa/)
+
+### License
+Distributed under the MIT License.
```

### Comparing `unbounce-python-api-1.3.4/README.md` & `unbounce-python-api-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/setup.py` & `unbounce-python-api-1.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
   name = 'unbounce-python-api',
   packages = ['unbounceapi'],
-  version = '1.3.4',
+  version = '1.3.5',
   license='MIT',
   description = 'An Unbounce API wrapper written in python.',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Yoshio Hasegawa',
   author_email = 'yoshio.seisuke.hasegawa@gmail.com',
   url = 'https://github.com/yoshiohasegawa/unbounce-python-api',
-  download_url = 'https://github.com/yoshiohasegawa/unbounce-python-api/archive/v1.3.4.tar.gz',
+  download_url = 'https://github.com/yoshiohasegawa/unbounce-python-api/archive/refs/tags/v1.3.5.tar.gz',
   keywords = ['Unbounce', 'API', 'Wrapper'],
   install_requires=[
           'requests',
           'pytest'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

### Comparing `unbounce-python-api-1.3.4/unbounceapi/users.py` & `unbounce-python-api-1.3.5/unbounceapi/users.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/accounts.py` & `unbounce-python-api-1.3.5/unbounceapi/accounts.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/client.py` & `unbounce-python-api-1.3.5/unbounceapi/client.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/domains.py` & `unbounce-python-api-1.3.5/unbounceapi/domains.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/page_groups.py` & `unbounce-python-api-1.3.5/unbounceapi/page_groups.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/leads.py` & `unbounce-python-api-1.3.5/unbounceapi/leads.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/pages.py` & `unbounce-python-api-1.3.5/unbounceapi/pages.py`

 * *Files identical despite different names*

### Comparing `unbounce-python-api-1.3.4/unbounceapi/sub_accounts.py` & `unbounce-python-api-1.3.5/unbounceapi/sub_accounts.py`

 * *Files identical despite different names*

