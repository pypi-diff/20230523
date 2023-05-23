# Comparing `tmp/python-tss-sdk-1.2.0.tar.gz` & `tmp/python_tss_sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tss-sdk-1.2.0.tar", last modified: Mon Aug 22 17:56:46 2022, max compression
+gzip compressed data, was "python_tss_sdk-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `python-tss-sdk-1.2.0.tar` & `python_tss_sdk-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      332 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      582 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      489 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/ISSUE_TEMPLATE/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      742 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      536 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      612 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      824 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     1984 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/.gitignore
--rw-r--r--   0        0        0     1051 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/LICENSE
--rw-r--r--   0        0        0     6206 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/README.md
--rw-r--r--   0        0        0      761 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/conftest.py
--rw-r--r--   0        0        0       69 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/delinea/__init__.py
--rw-r--r--   0        0        0        0 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/delinea/secrets/__init__.py
--rw-r--r--   0        0        0    14169 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/delinea/secrets/server.py
--rw-r--r--   0        0        0      664 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/example.py
--rw-r--r--   0        0        0      623 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       53 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/requirements.txt
--rw-r--r--   0        0        0     1558 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/tests/test_server.py
--rw-r--r--   0        0        0      568 2022-08-22 17:56:38.859546 python-tss-sdk-1.2.0/tox.ini
--rw-r--r--   0        0        0     6768 1970-01-01 00:00:00.000000 python-tss-sdk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      332 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      582 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      489 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      742 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      536 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      612 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      895 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0     1984 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.gitignore
+-rw-r--r--   0        0        0      541 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/.whitesource
+-rw-r--r--   0        0        0     1051 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/LICENSE
+-rw-r--r--   0        0        0     6252 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/README.md
+-rw-r--r--   0        0        0      818 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/conftest.py
+-rw-r--r--   0        0        0       69 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/secrets/__init__.py
+-rw-r--r--   0        0        0    15995 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/delinea/secrets/server.py
+-rw-r--r--   0        0        0      965 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/example.py
+-rw-r--r--   0        0        0      638 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/renovate.json
+-rw-r--r--   0        0        0       53 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/requirements.txt
+-rw-r--r--   0        0        0     1774 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/tests/test_server.py
+-rw-r--r--   0        0        0      621 2023-05-23 15:36:48.111132 python_tss_sdk-1.2.1/tox.ini
+-rw-r--r--   0        0        0     6829 1970-01-01 00:00:00.000000 python_tss_sdk-1.2.1/PKG-INFO
```

### Comparing `python-tss-sdk-1.2.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md` & `python_tss_sdk-1.2.1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `python-tss-sdk-1.2.0/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md` & `python_tss_sdk-1.2.1/.github/PULL_REQUEST_TEMPLATE/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `python-tss-sdk-1.2.0/.github/workflows/lint.yml` & `python_tss_sdk-1.2.1/.github/workflows/lint.yml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   lint:
     name: Run black linter
     runs-on: ubuntu-latest
     steps:
       - name: Check out Git repository
         uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
       - name: Install Python dependencies
         run: pip install black
       - name: Run black
         uses: wearerequired/lint-action@v2
         with:
            black: true
            auto_fix: true
```

### Comparing `python-tss-sdk-1.2.0/.github/workflows/release.yml` & `python_tss_sdk-1.2.1/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
       - 'v*'
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install flit
```

### Comparing `python-tss-sdk-1.2.0/.github/workflows/run_tests.yml` & `python_tss_sdk-1.2.1/.github/workflows/run_tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Run Tests
 
 on: [pull_request]
 
 jobs:
-  
+
   build:
     runs-on: ubuntu-latest
     environment: testing
     strategy:
       matrix:
-        python: [3.7, 3.8, 3.9, "3.10"]
+        python: [3.8, 3.9, "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
       - name: Install Tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
@@ -26,9 +26,10 @@
       - name: Run Tox
         # Run tox using the version of Python in `PATH`
         run: tox -e py
         env:
           TSS_USERNAME: ${{ secrets.TSS_USERNAME }}
           TSS_PASSWORD: ${{ secrets.TSS_PASSWORD }}
           TSS_TENANT: ${{ secrets.TSS_TENANT }}
-          SECRET_ID: ${{ secrets.SECRET_ID }}
-          SECRET_PATH: ${{ secrets.SECRET_PATH }}
+          TSS_SECRET_ID: ${{ secrets.TSS_SECRET_ID }}
+          TSS_SECRET_PATH: ${{ secrets.TSS_SECRET_PATH }}
+          TSS_FOLDER_ID: ${{ secrets.TSS_FOLDER_ID }}
```

### Comparing `python-tss-sdk-1.2.0/.gitignore` & `python_tss_sdk-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python-tss-sdk-1.2.0/LICENSE` & `python_tss_sdk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tss-sdk-1.2.0/README.md` & `python_tss_sdk-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 #### Password Authorization
 
 If using traditional `username` and `password` authentication to log in to your Secret Server, you can pass the `PasswordGrantAuthorizer` into the `SecretServer` class at instantiation. The `PasswordGrantAuthorizer` requires a `base_url`, `username`, and `password`. It optionally takes a `token_path_uri`, but defaults to `/oauth2/token`.
 
 ```python
 from delinea.secrets.server import PasswordGrantAuthorizer
 
-authorizer = PasswordGrantAuthorizer("https://hostname/SecretServer", "myusername", "mypassword")
+authorizer = PasswordGrantAuthorizer("https://hostname/SecretServer", os.getenv("myusername"), os.getenv("password")")
 ```
 
 #### Domain Authorization
 
 To use a domain credential, use the `DomainPasswordGrantAuthorizer`. It requires a `base_url`, `username`, `domain`, and `password`. It optionally takes a `token_path_uri`, but defaults to `/oauth2/token`.
 
 ```python
 from delinea.secrets.server import DomainPasswordGrantAuthorizer
 
-authorizer = DomainPasswordGrantAuthorizer("https://hostname/SecretServer", "myusername", "mydomain", "mypassword")
+authorizer = DomainPasswordGrantAuthorizer("https://hostname/SecretServer", os.getenv("myusername"), os.getenv("mydomain"), os.getenv("password"))
 ```
 
 #### Access Token Authorization
 
 If you already have an `access_token`, you can pass directly via the `AccessTokenAuthorizer`.
 
 ```python
@@ -112,19 +112,19 @@
 print(f"username: {secret.fields['username'].value}\npassword: {secret.fields['password'].value}")
 ```
 
 > Note: The `path` must be the full folder path and name of the secret.
 
 ## Using Self-Signed Certificates
 
-When using a self-signed certificate for SSL, the `REQUESTS_CA_BUNDLE` environment variable should be set to the path of the certificate (in `.pem` format). This will negate the need to ignore SSL certificate verification, which makes your application vunerable. Please reference the [`requests` documentation](https://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification) for further details on the `REQUESTS_CA_BUNDLE` environment variable, should you require it.
+When using a self-signed certificate for SSL, the `REQUESTS_CA_BUNDLE` environment variable should be set to the path of the certificate (in `.pem` format). This will negate the need to ignore SSL certificate verification, which makes your application vunerable. Please reference the [`requests` documentation](https://docs.python.org/3/library/ssl.html) for further details on the `REQUESTS_CA_BUNDLE` environment variable, should you require it.
 
 ## Create a Build Environment (optional)
 
-The SDK requires [Python 3.7](https://www.python.org/downloads/) or higher.
+The SDK requires [Python 3.8](https://www.python.org/downloads/) or higher.
 
 First, ensure Python is in `$PATH`, then run:
 
 ```shell
 # Clone the repo
 git clone https://github.com/DelineaXPM/python-tss-sdk
 cd python-tss-sdk
@@ -140,16 +140,17 @@
 
 Valid credentials are required to run the unit tests. The credentials should be stored in environment variables or in a `.env` file:
 
 ```shell
 export TSS_USERNAME=myusername
 export TSS_PASSWORD=mysecretpassword
 export TSS_TENANT=mytenant
-export SECRET_ID=42
-export SECRET_PATH=\Test Secrets\SecretName
+export TSS_SECRET_ID=42
+export TSS_SECRET_PATH=\Test Secrets\SecretName
+export TSS_FOLDER_ID=1
 ```
 
 The tests assume that the user associated with the specified `TSS_USERNAME` and `TSS_PASSWORD` can read the secret to be fetched, and that the Secret itself contains `username` and `password` fields.
 
 To run the tests with `tox`:
 
 ```shell
```

### Comparing `python-tss-sdk-1.2.0/conftest.py` & `python_tss_sdk-1.2.1/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 @pytest.fixture
 def env_vars():
     return {
         "username": os.getenv("TSS_USERNAME"),
         "password": os.getenv("TSS_PASSWORD"),
         "tenant": os.getenv("TSS_TENANT"),
-        "secret_id": os.getenv("SECRET_ID"),
-        "secret_path": os.getenv("SECRET_PATH"),
+        "secret_id": os.getenv("TSS_SECRET_ID"),
+        "secret_path": os.getenv("TSS_SECRET_PATH"),
+        "folder_id": os.getenv("TSS_FOLDER_ID"),
     }
 
 
 @pytest.fixture
 def authorizer(env_vars):
     return PasswordGrantAuthorizer(
         f"https://{env_vars['tenant']}.secretservercloud.com",
```

### Comparing `python-tss-sdk-1.2.0/delinea/secrets/server.py` & `python_tss_sdk-1.2.1/delinea/secrets/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -365,24 +365,76 @@
         params = {"secretPath": path}
         return self.get_secret(
             id=0,
             fetch_file_attachments=fetch_file_attachments,
             query_params=params,
         )
 
+    def search_secrets(self, query_params=None):
+        """Get Secrets from Secret Server
+
+        :param query_params: query parameters to pass to the endpoint
+        :type query_params: dict
+        :return: a JSON formatted string representation of the secrets
+        :rtype: ``str``
+        :raise: :class:`SecretServerAccessError` when the caller does not have
+                permission to access the secret
+        :raise: :class:`SecretServerError` when the REST API call fails for
+                any other reason
+        """
+        endpoint_url = f"{self.api_url}/secrets"
+
+        if query_params is None:
+            return self.process(requests.get(endpoint_url, headers=self.headers())).text
+        else:
+            return self.process(
+                requests.get(
+                    endpoint_url,
+                    params=query_params,
+                    headers=self.headers(),
+                )
+            ).text
+
+    def get_secret_ids_by_folderid(self, folder_id):
+        """Gets a list of secrets ids by folder_id
+
+        :param folder_id: the id of the folder
+        :type id: int
+        :return: a ``list`` of the secret id's
+        :rtype: ``list``
+        :raise: :class:`SecretServerAccessError` when the caller does not have
+                permission to access the secret
+        :raise: :class:`SecretServerError` when the REST API call fails for
+                any other reason
+        """
+
+        params = {"filter.folderId": folder_id}
+        response = self.search_secrets(query_params=params)
+
+        try:
+            secrets = json.loads(response)
+        except json.JSONDecodeError:
+            raise SecretServerError(response)
+
+        secret_ids = []
+        for secret in secrets["records"]:
+            secret_ids.append(secret["id"])
+
+        return secret_ids
+
 
 class SecretServerV0(SecretServer):
     """A class that uses an *OAuth2 Bearer Token* to access the Secret Server
     REST API. It uses the :attr:`username` and :attr:`password` to access the
     Secret Server at :attr:`base_url`.
 
     It gets an ``access_token`` that it uses to create an *HTTP Authorization
     Header* which it includes in each REST API call.
 
-    This class maintains backwards compatability with v0.0.5
+    This class maintains backwards compatibility with v0.0.5
     """
 
     def __init__(
         self,
         base_url,
         username,
         password,
```

### Comparing `python-tss-sdk-1.2.0/pyproject.toml` & `python_tss_sdk-1.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.metadata]
 module = "delinea"
-author = "Adam Migus"
-author-email = "adam@migus.org"
+author = "Delinea Integrations"
+author-email = "GitHub@delinea.com"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 description-file = "README.md"
 requires = [
     "requests >= 2.12.5"
 ]
-requires-python=">=3.7"
+requires-python=">=3.8"
 dist-name = "python-tss-sdk"
```

### Comparing `python-tss-sdk-1.2.0/tests/test_server.py` & `python_tss_sdk-1.2.1/tests/test_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,60 @@
-import pytest
-
-from delinea.secrets.server import (
-    AccessTokenAuthorizer,
-    SecretServer,
-    SecretServerClientError,
-    SecretServerError,
-    ServerSecret,
-)
-
-
-def test_bad_url(env_vars, authorizer):
-    bad_server = SecretServer(
-        f"https://{env_vars['tenant']}.secretservercloud.com/nonexistent",
-        authorizer,
-    )
-    with pytest.raises(SecretServerError):
-        bad_server.get_secret(env_vars["secret_id"])
-
-
-def test_token_url(env_vars, authorizer):
-    assert (
-        authorizer.token_url
-        == f"https://{env_vars['tenant']}.secretservercloud.com/oauth2/token"
-    )
-
-
-def test_api_url(secret_server, env_vars):
-    assert (
-        secret_server.api_url
-        == f"https://{env_vars['tenant']}.secretservercloud.com/api/v1"
-    )
-
-
-def test_access_token_authorizer(env_vars, authorizer):
-    assert SecretServer(
-        f"https://{env_vars['tenant']}.secretservercloud.com/",
-        AccessTokenAuthorizer(authorizer.get_access_token()),
-    ).get_secret(env_vars["secret_id"])["id"] == int(env_vars["secret_id"])
-
-
-def test_server_secret(env_vars, secret_server):
-    assert ServerSecret(**secret_server.get_secret(env_vars["secret_id"])).id == int(
-        env_vars["secret_id"]
-    )
-
-
-def test_server_secret_by_path(env_vars, secret_server):
-    assert ServerSecret(
-        **secret_server.get_secret_by_path(env_vars["secret_path"])
-    ).id == int(env_vars["secret_id"])
-
-
-def test_nonexistent_secret(secret_server):
-    with pytest.raises(SecretServerClientError):
-        secret_server.get_secret(1000)
+import pytest
+
+from delinea.secrets.server import (
+    AccessTokenAuthorizer,
+    SecretServer,
+    SecretServerClientError,
+    SecretServerError,
+    ServerSecret,
+)
+
+
+def test_bad_url(env_vars, authorizer):
+    bad_server = SecretServer(
+        f"https://{env_vars['tenant']}.secretservercloud.com/nonexistent",
+        authorizer,
+    )
+    with pytest.raises(SecretServerError):
+        bad_server.get_secret(env_vars["secret_id"])
+
+
+def test_token_url(env_vars, authorizer):
+    assert (
+        authorizer.token_url
+        == f"https://{env_vars['tenant']}.secretservercloud.com/oauth2/token"
+    )
+
+
+def test_api_url(secret_server, env_vars):
+    assert (
+        secret_server.api_url
+        == f"https://{env_vars['tenant']}.secretservercloud.com/api/v1"
+    )
+
+
+def test_access_token_authorizer(env_vars, authorizer):
+    assert SecretServer(
+        f"https://{env_vars['tenant']}.secretservercloud.com/",
+        AccessTokenAuthorizer(authorizer.get_access_token()),
+    ).get_secret(env_vars["secret_id"])["id"] == int(env_vars["secret_id"])
+
+
+def test_server_secret(env_vars, secret_server):
+    assert ServerSecret(**secret_server.get_secret(env_vars["secret_id"])).id == int(
+        env_vars["secret_id"]
+    )
+
+
+def test_server_secret_by_path(env_vars, secret_server):
+    assert ServerSecret(
+        **secret_server.get_secret_by_path(env_vars["secret_path"])
+    ).id == int(env_vars["secret_id"])
+
+
+def test_nonexistent_secret(secret_server):
+    with pytest.raises(SecretServerClientError):
+        secret_server.get_secret(1000)
+
+
+def test_server_secret_ids_by_folderid(env_vars, secret_server):
+    assert type(secret_server.get_secret_ids_by_folderid(env_vars["folder_id"])) is list
```

### Comparing `python-tss-sdk-1.2.0/PKG-INFO` & `python_tss_sdk-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python-tss-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: The Delinea Secret Server Python SDK
-Author: Adam Migus
-Author-email: adam@migus.org
-Requires-Python: >=3.7
+Author: Delinea Integrations
+Author-email: GitHub@delinea.com
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests >= 2.12.5
 
 # The Delinea Secret Server Python SDK
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ![PyPI Version](https://img.shields.io/pypi/v/python-tss-sdk) ![License](https://img.shields.io/github/license/DelineaXPM/python-tss-sdk) ![Python Versions](https://img.shields.io/pypi/pyversions/python-tss-sdk)
@@ -41,25 +41,25 @@
 #### Password Authorization
 
 If using traditional `username` and `password` authentication to log in to your Secret Server, you can pass the `PasswordGrantAuthorizer` into the `SecretServer` class at instantiation. The `PasswordGrantAuthorizer` requires a `base_url`, `username`, and `password`. It optionally takes a `token_path_uri`, but defaults to `/oauth2/token`.
 
 ```python
 from delinea.secrets.server import PasswordGrantAuthorizer
 
-authorizer = PasswordGrantAuthorizer("https://hostname/SecretServer", "myusername", "mypassword")
+authorizer = PasswordGrantAuthorizer("https://hostname/SecretServer", os.getenv("myusername"), os.getenv("password")")
 ```
 
 #### Domain Authorization
 
 To use a domain credential, use the `DomainPasswordGrantAuthorizer`. It requires a `base_url`, `username`, `domain`, and `password`. It optionally takes a `token_path_uri`, but defaults to `/oauth2/token`.
 
 ```python
 from delinea.secrets.server import DomainPasswordGrantAuthorizer
 
-authorizer = DomainPasswordGrantAuthorizer("https://hostname/SecretServer", "myusername", "mydomain", "mypassword")
+authorizer = DomainPasswordGrantAuthorizer("https://hostname/SecretServer", os.getenv("myusername"), os.getenv("mydomain"), os.getenv("password"))
 ```
 
 #### Access Token Authorization
 
 If you already have an `access_token`, you can pass directly via the `AccessTokenAuthorizer`.
 
 ```python
@@ -128,19 +128,19 @@
 print(f"username: {secret.fields['username'].value}\npassword: {secret.fields['password'].value}")
 ```
 
 > Note: The `path` must be the full folder path and name of the secret.
 
 ## Using Self-Signed Certificates
 
-When using a self-signed certificate for SSL, the `REQUESTS_CA_BUNDLE` environment variable should be set to the path of the certificate (in `.pem` format). This will negate the need to ignore SSL certificate verification, which makes your application vunerable. Please reference the [`requests` documentation](https://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification) for further details on the `REQUESTS_CA_BUNDLE` environment variable, should you require it.
+When using a self-signed certificate for SSL, the `REQUESTS_CA_BUNDLE` environment variable should be set to the path of the certificate (in `.pem` format). This will negate the need to ignore SSL certificate verification, which makes your application vunerable. Please reference the [`requests` documentation](https://docs.python.org/3/library/ssl.html) for further details on the `REQUESTS_CA_BUNDLE` environment variable, should you require it.
 
 ## Create a Build Environment (optional)
 
-The SDK requires [Python 3.7](https://www.python.org/downloads/) or higher.
+The SDK requires [Python 3.8](https://www.python.org/downloads/) or higher.
 
 First, ensure Python is in `$PATH`, then run:
 
 ```shell
 # Clone the repo
 git clone https://github.com/DelineaXPM/python-tss-sdk
 cd python-tss-sdk
@@ -156,16 +156,17 @@
 
 Valid credentials are required to run the unit tests. The credentials should be stored in environment variables or in a `.env` file:
 
 ```shell
 export TSS_USERNAME=myusername
 export TSS_PASSWORD=mysecretpassword
 export TSS_TENANT=mytenant
-export SECRET_ID=42
-export SECRET_PATH=\Test Secrets\SecretName
+export TSS_SECRET_ID=42
+export TSS_SECRET_PATH=\Test Secrets\SecretName
+export TSS_FOLDER_ID=1
 ```
 
 The tests assume that the user associated with the specified `TSS_USERNAME` and `TSS_PASSWORD` can read the secret to be fetched, and that the Secret itself contains `username` and `password` fields.
 
 To run the tests with `tox`:
 
 ```shell
```

