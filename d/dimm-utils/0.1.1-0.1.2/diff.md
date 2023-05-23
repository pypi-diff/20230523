# Comparing `tmp/dimm_utils-0.1.1.tar.gz` & `tmp/dimm_utils-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimm_utils-0.1.1.tar", max compression
+gzip compressed data, was "dimm_utils-0.1.2.tar", max compression
```

## Comparing `dimm_utils-0.1.1.tar` & `dimm_utils-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       91 2023-05-23 14:36:01.477822 dimm_utils-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 14:04:10.404588 dimm_utils-0.1.1/dimm_utils/__init__.py
--rw-r--r--   0        0        0       21 2023-05-23 14:08:51.294332 dimm_utils-0.1.1/dimm_utils/constants.py
--rw-r--r--   0        0        0     4674 2023-05-23 14:52:27.997058 dimm_utils-0.1.1/dimm_utils/core.py
--rw-r--r--   0        0        0      323 2023-05-23 14:53:02.549797 dimm_utils-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 dimm_utils-0.1.1/setup.py
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2023-05-23 14:36:01.477822 dimm_utils-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 14:04:10.404588 dimm_utils-0.1.2/dimm_utils/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 14:08:51.294332 dimm_utils-0.1.2/dimm_utils/constants.py
+-rw-r--r--   0        0        0     4675 2023-05-23 15:11:13.102036 dimm_utils-0.1.2/dimm_utils/core.py
+-rw-r--r--   0        0        0      323 2023-05-23 15:11:21.626130 dimm_utils-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 dimm_utils-0.1.2/PKG-INFO
```

### Comparing `dimm_utils-0.1.1/dimm_utils/core.py` & `dimm_utils-0.1.2/dimm_utils/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,19 +67,30 @@
         "aws_secret_access_key": aws_secret_access_key,
         "aws_session_token": aws_session_token,
         "region_name": aws_region,
     }
     return credentials
 
 
+def get_secret(client, secret_name: str) -> str:
+    try:
+        # Retrieve the secret value
+        response = client.get_secret_value(SecretId=secret_name)
+
+        # Parse the secret value as JSON
+        return response["SecretString"]
+    except client.exceptions.ParameterNotFound:
+        raise Exception(f"Secret {secret_name} not found in AWS SSM")
+
+
 def store_secret_from_local(client, secret_name: str, secret_value: str):
     authenticate_local()
     # Create or update the secret
     try:
-        secret = client.get_secret(secret_name)
+        secret = get_secret(client, secret_name)
         if secret == secret_value:
             print("Secret already exists")
             return
         client.create_secret(
             Name=secret_name,
             SecretString=secret_value,
         )
@@ -98,25 +109,14 @@
 
     if status == 200:
         return response.get("Body")
     else:
         print(f"Unsuccessful S3 get_object response. Status - {status}")
 
 
-def get_secret(client, secret_name: str) -> str:
-    try:
-        # Retrieve the secret value
-        response = client.get_secret_value(SecretId=secret_name)
-
-        # Parse the secret value as JSON
-        return response["SecretString"]
-    except client.exceptions.ParameterNotFound:
-        raise Exception(f"Secret {secret_name} not found in AWS SSM")
-
-
 def upload_file_to_s3(client, bucket_name: str, key: str, file_path: str):
     try:
         # Check if the parent directory exists
         parent_dir = "/".join(key.split("/")[:-1])
         response = client.list_objects_v2(Bucket=bucket_name, Prefix=parent_dir)
         parent_dir_exists = response.get("KeyCount", 0) > 0
```

