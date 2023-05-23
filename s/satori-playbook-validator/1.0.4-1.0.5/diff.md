# Comparing `tmp/satori_playbook_validator-1.0.4.tar.gz` & `tmp/satori_playbook_validator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_playbook_validator-1.0.4.tar", last modified: Sat May 20 05:48:16 2023, max compression
+gzip compressed data, was "satori_playbook_validator-1.0.5.tar", last modified: Tue May 23 21:03:34 2023, max compression
```

## Comparing `satori_playbook_validator-1.0.4.tar` & `satori_playbook_validator-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       30 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/README.md
--rw-r--r--   0        0        0      433 2023-05-20 05:48:16.012914 satori_playbook_validator-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      163 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/__init__.py
--rw-r--r--   0        0        0     3114 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/_validator.py
--rw-r--r--   0        0        0       51 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/exceptions.py
--rw-r--r--   0        0        0      267 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/command.json
--rw-r--r--   0        0        0      251 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/import.json
--rw-r--r--   0        0        0     2197 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/input.json
--rw-r--r--   0        0        0     1025 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/settings.json
--rw-r--r--   0        0        0     1743 2023-05-20 05:47:58.876425 satori_playbook_validator-1.0.4/src/satorici/validator/schemas/test.json
--rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/README.md
+-rw-r--r--   0        0        0      433 2023-05-23 21:03:34.134093 satori_playbook_validator-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/__init__.py
+-rw-r--r--   0        0        0     3268 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/_validator.py
+-rw-r--r--   0        0        0      223 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/exceptions.py
+-rw-r--r--   0        0        0      267 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/command.json
+-rw-r--r--   0        0        0      251 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/import.json
+-rw-r--r--   0        0        0     2197 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/input.json
+-rw-r--r--   0        0        0     1025 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/settings.json
+-rw-r--r--   0        0        0     1743 2023-05-23 21:03:15.885929 satori_playbook_validator-1.0.5/src/satorici/validator/schemas/test.json
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 satori_playbook_validator-1.0.5/PKG-INFO
```

### Comparing `satori_playbook_validator-1.0.4/src/satorici/validator/_validator.py` & `satori_playbook_validator-1.0.5/src/satorici/validator/_validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 from flatdict import FlatDict
 from jsonschema import Draft7Validator, FormatChecker
 from jsonschema.exceptions import ValidationError
 from jsonschema.validators import RefResolver
 
-from .exceptions import PlaybookValidationError
+from .exceptions import PlaybookValidationError, PlaybookVariableError
 
 INPUT_REGEX = re.compile(r"\$\(([\w-]+)\)")
 
 SCHEMAS = Path(__file__).parent / "schemas"
 
 with (
     open(SCHEMAS / "command.json") as commands,
@@ -61,27 +61,30 @@
 
             found_prefix = prefix
 
             for key, value in flat_config.items():
                 if key.startswith(prefix) and input_schema.is_valid(value):
                     break
             else:
-                raise PlaybookValidationError(
-                    f"No valid inputs for variable: {variable}"
+                raise PlaybookVariableError(
+                    f"No valid inputs for variable: {variable}", parameter=variable
                 )
 
         if not found_prefix:
-            raise PlaybookValidationError(f"Can't resolve variable: {variable}")
+            raise PlaybookVariableError(
+                f"Can't resolve variable: {variable}", parameter=variable
+            )
 
 
 def validate_playbook(config: dict):
     """
     Validate yaml loaded playbook config and return corresponding dict
 
     Raises `PlaybookValidationError` on invalid playbook
+    Raises `PlaybookVariableError` on invalid playbook variables
     """
 
     if not isinstance(config, dict):
         raise TypeError("config must be a dict")
 
     config_copy = deepcopy(config)
```

### Comparing `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/input.json` & `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/input.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/settings.json` & `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/settings.json`

 * *Files identical despite different names*

### Comparing `satori_playbook_validator-1.0.4/src/satorici/validator/schemas/test.json` & `satori_playbook_validator-1.0.5/src/satorici/validator/schemas/test.json`

 * *Files identical despite different names*

