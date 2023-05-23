# Comparing `tmp/dimm_utils-0.1.2.tar.gz` & `tmp/dimm_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimm_utils-0.1.2.tar", max compression
+gzip compressed data, was "dimm_utils-0.1.3.tar", max compression
```

## Comparing `dimm_utils-0.1.2.tar` & `dimm_utils-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       91 2023-05-23 14:36:01.477822 dimm_utils-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:04:10.404588 dimm_utils-0.1.2/dimm_utils/__init__.py
--rw-r--r--   0        0        0       21 2023-05-23 14:08:51.294332 dimm_utils-0.1.2/dimm_utils/constants.py
--rw-r--r--   0        0        0     4675 2023-05-23 15:11:13.102036 dimm_utils-0.1.2/dimm_utils/core.py
--rw-r--r--   0        0        0      323 2023-05-23 15:11:21.626130 dimm_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-05-23 14:36:01.477822 dimm_utils-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:04:10.404588 dimm_utils-0.1.3/dimm_utils/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 14:08:51.294332 dimm_utils-0.1.3/dimm_utils/constants.py
+-rw-r--r--   0        0        0     4617 2023-05-23 15:15:47.131179 dimm_utils-0.1.3/dimm_utils/core.py
+-rw-r--r--   0        0        0      323 2023-05-23 15:15:50.591000 dimm_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.3/PKG-INFO
```

### Comparing `dimm_utils-0.1.2/dimm_utils/core.py` & `dimm_utils-0.1.3/dimm_utils/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,17 @@
 def get_secret(client, secret_name: str) -> str:
     try:
         # Retrieve the secret value
         response = client.get_secret_value(SecretId=secret_name)
 
         # Parse the secret value as JSON
         return response["SecretString"]
-    except client.exceptions.ParameterNotFound:
-        raise Exception(f"Secret {secret_name} not found in AWS SSM")
+    except Exception as e:
+        print(e)
+        raise e
 
 
 def store_secret_from_local(client, secret_name: str, secret_value: str):
     authenticate_local()
     # Create or update the secret
     try:
         secret = get_secret(client, secret_name)
```

