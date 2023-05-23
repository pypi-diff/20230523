# Comparing `tmp/httpie-oauth2-client-credentials-0.1.2.tar.gz` & `tmp/httpie-oauth2-client-credentials-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpie-oauth2-client-credentials-0.1.2.tar", last modified: Mon May  8 16:10:48 2023, max compression
+gzip compressed data, was "httpie-oauth2-client-credentials-0.2.0.tar", last modified: Tue May 23 07:10:23 2023, max compression
```

## Comparing `httpie-oauth2-client-credentials-0.1.2.tar` & `httpie-oauth2-client-credentials-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 16:10:48.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:10:48.127634 httpie-oauth2-client-credentials-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-08 16:10:37.000000 httpie-oauth2-client-credentials-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:10:23.175233 httpie-oauth2-client-credentials-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 07:10:09.000000 httpie-oauth2-client-credentials-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-23 07:10:23.175233 httpie-oauth2-client-credentials-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-23 07:10:09.000000 httpie-oauth2-client-credentials-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:10:23.175233 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 07:10:23.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-23 07:10:09.000000 httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 07:10:23.175233 httpie-oauth2-client-credentials-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 07:10:09.000000 httpie-oauth2-client-credentials-0.2.0/setup.py
```

### Comparing `httpie-oauth2-client-credentials-0.1.2/LICENSE` & `httpie-oauth2-client-credentials-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `httpie-oauth2-client-credentials-0.1.2/PKG-INFO` & `httpie-oauth2-client-credentials-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: httpie-oauth2-client-credentials
-Version: 0.1.2
-Summary: httpie auth plugin for OAuth2.0 client credentials flow.
-Home-page: https://github.com/satodoc/httpie-oauth2-client-credentials
-Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
-Author: satdoc
-Author-email: satodoc-develop-public@outlook.com
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: Environment :: Plugins
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hca-httpie-auth
 
 As an auth plugin for httpie, it obtains a token with the OAuth2.0 client_credentials flow before executing http, and adds the `Authorization: Bearer ${token}` header to the executed request.  
 
 ## Token request patterns
 
 Token request patterns are supported for the following:
@@ -119,14 +99,43 @@
     "client_id": "${client_id}",
     "client_secret": "${client_secret}",
     "grant_type": "client_credentials",
     "scope": "${SCOPE}"
 }
 ```
 
+## Supported .netrc
+
+Supported `.netrc`.  
+Please check the [httpie documentation](https://httpie.io/docs/cli/netrc) for usage instructions.
+
+### Important Notes before Use
+
+The value for "machine" in the ".netrc" file is the TARGET_ENDPOINT host, not the TOKEN_ENDPOINT host.
+It should be TOKEN_ENDPOINT, but the main body of httpie is designed to extract authentication information from the TARGET_ENDPOINT host.
+
+```bash
+# Create(or add) .netrc file.
+cat <<EOF>> ~/.netrc
+
+machine   {TARGET_ENDPOINT_HOST}
+login     {Your Client ID}
+password  {Your Client Secret}
+EOF
+
+# Change permission.
+chmod 600 ~/.netrc
+# Example request.
+http --auth-type=oauth2-client-credentials \
+     --token-endpoint="${TOKEN_ENDPOINT_URL}" \
+     --token-request-type="form" \
+     --scope="${SCOPE}" \
+     ${TARGET_ENDPOINT_URL}
+```
+
 ## Options
 
 - `--print-token-response`  
   Output the token acquisition response to the console
 
 ## Note
```

### Comparing `httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.egg-info/PKG-INFO` & `httpie-oauth2-client-credentials-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpie-oauth2-client-credentials
-Version: 0.1.2
+Version: 0.2.0
 Summary: httpie auth plugin for OAuth2.0 client credentials flow.
 Home-page: https://github.com/satodoc/httpie-oauth2-client-credentials
 Download-URL: https://github.com/satodoc/httpie-oauth2-client-credentials
 Author: satdoc
 Author-email: satodoc-develop-public@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
@@ -119,14 +119,43 @@
     "client_id": "${client_id}",
     "client_secret": "${client_secret}",
     "grant_type": "client_credentials",
     "scope": "${SCOPE}"
 }
 ```
 
+## Supported .netrc
+
+Supported `.netrc`.  
+Please check the [httpie documentation](https://httpie.io/docs/cli/netrc) for usage instructions.
+
+### Important Notes before Use
+
+The value for "machine" in the ".netrc" file is the TARGET_ENDPOINT host, not the TOKEN_ENDPOINT host.
+It should be TOKEN_ENDPOINT, but the main body of httpie is designed to extract authentication information from the TARGET_ENDPOINT host.
+
+```bash
+# Create(or add) .netrc file.
+cat <<EOF>> ~/.netrc
+
+machine   {TARGET_ENDPOINT_HOST}
+login     {Your Client ID}
+password  {Your Client Secret}
+EOF
+
+# Change permission.
+chmod 600 ~/.netrc
+# Example request.
+http --auth-type=oauth2-client-credentials \
+     --token-endpoint="${TOKEN_ENDPOINT_URL}" \
+     --token-request-type="form" \
+     --scope="${SCOPE}" \
+     ${TARGET_ENDPOINT_URL}
+```
+
 ## Options
 
 - `--print-token-response`  
   Output the token acquisition response to the console
 
 ## Note
```

### Comparing `httpie-oauth2-client-credentials-0.1.2/httpie_oauth2_client_credentials.py` & `httpie-oauth2-client-credentials-0.2.0/httpie_oauth2_client_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
                     sys.stderr.write(f'error_response: \n========== \n{res_body}\n==========\n')
             raise e
 
 class OAuth2ClientCredentialsPlugin(AuthPlugin):
 
     name = 'OAuth2.0 client credentilas flow.'
     auth_type = 'oauth2-client-credentials'
+    netrc_parse = True
     description = 'Set the Bearer token obtained in the OAuth2.0 client_credentials flow to the Authorization header.'
 
     params = httpie_args_parser.add_argument_group(title='OAuth2.0 client credentilas flow options')
     params.add_argument(
         '--token-endpoint',
         default=None,
         metavar='TOKEN_ENDPOINT_URL',
```

### Comparing `httpie-oauth2-client-credentials-0.1.2/setup.py` & `httpie-oauth2-client-credentials-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 setup(
     name="httpie-oauth2-client-credentials",
     description="httpie auth plugin for OAuth2.0 client credentials flow.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    version="0.1.2",
+    version="0.2.0",
     author='satdoc',
     author_email='satodoc-develop-public@outlook.com',
     license='MIT',
     url='https://github.com/satodoc/httpie-oauth2-client-credentials',
     download_url='https://github.com/satodoc/httpie-oauth2-client-credentials',
     py_modules=['httpie_oauth2_client_credentials'],
-    install_requires=['httpie>=2.0.0'],
+    install_requires=['httpie>=3.2.2'],
     entry_points={
         'httpie.plugins.auth.v1': [
             'httpie_oauth2_client_credentials = httpie_oauth2_client_credentials:OAuth2ClientCredentialsPlugin'
         ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',
```

