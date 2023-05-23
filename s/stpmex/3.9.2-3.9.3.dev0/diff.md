# Comparing `tmp/stpmex-3.9.2.tar.gz` & `tmp/stpmex-3.9.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpmex-3.9.2.tar", last modified: Tue Oct 25 17:44:48 2022, max compression
+gzip compressed data, was "stpmex-3.9.3.dev0.tar", last modified: Thu Oct 27 22:23:51 2022, max compression
```

## Comparing `stpmex-3.9.2.tar` & `stpmex-3.9.3.dev0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:48.646308 stpmex-3.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-25 17:44:40.000000 stpmex-3.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-10-25 17:44:48.646308 stpmex-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-10-25 17:44:40.000000 stpmex-3.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-10-25 17:44:48.646308 stpmex-3.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-10-25 17:44:40.000000 stpmex-3.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:48.642308 stpmex-3.9.2/stpmex/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/business_days.py
--rw-r--r--   0 runner    (1001) docker     (121)     6390 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/exc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:48.642308 stpmex-3.9.2/stpmex/resources/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/resources/cuentas.py
--rw-r--r--   0 runner    (1001) docker     (121)     7483 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/resources/ordenes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/resources/saldos.py
--rw-r--r--   0 runner    (1001) docker     (121)    15092 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 17:44:40.000000 stpmex-3.9.2/stpmex/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:48.642308 stpmex-3.9.2/stpmex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3177 2022-10-25 17:44:48.000000 stpmex-3.9.2/stpmex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-25 17:44:48.000000 stpmex-3.9.2/stpmex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 17:44:48.000000 stpmex-3.9.2/stpmex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-25 17:44:48.000000 stpmex-3.9.2/stpmex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-25 17:44:48.000000 stpmex-3.9.2/stpmex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:48.646308 stpmex-3.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/test_business_days.py
--rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-10-25 17:44:40.000000 stpmex-3.9.2/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2658 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2022-10-27 22:23:51.968201 stpmex-3.9.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/stpmex/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1760 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/business_days.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6517 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/exc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/stpmex/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/resources/cuentas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7483 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/resources/ordenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/resources/saldos.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15092 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/stpmex/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/stpmex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3182 2022-10-27 22:23:51.000000 stpmex-3.9.3.dev0/stpmex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-27 22:23:51.000000 stpmex-3.9.3.dev0/stpmex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 22:23:51.000000 stpmex-3.9.3.dev0/stpmex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-10-27 22:23:51.000000 stpmex-3.9.3.dev0/stpmex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-27 22:23:51.000000 stpmex-3.9.3.dev0/stpmex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:51.964202 stpmex-3.9.3.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/test_business_days.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6120 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-10-27 22:23:42.000000 stpmex-3.9.3.dev0/tests/test_validations.py
```

### Comparing `stpmex-3.9.2/LICENSE` & `stpmex-3.9.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/PKG-INFO` & `stpmex-3.9.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpmex
-Version: 3.9.2
+Version: 3.9.3.dev0
 Summary: Client library for stpmex.com
 Home-page: https://github.com/cuenca-mx/stpmex-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `stpmex-3.9.2/README.md` & `stpmex-3.9.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/setup.cfg` & `stpmex-3.9.3.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/setup.py` & `stpmex-3.9.3.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/auth.py` & `stpmex-3.9.3.dev0/stpmex/auth.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/business_days.py` & `stpmex-3.9.3.dev0/stpmex/business_days.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/client.py` & `stpmex-3.9.3.dev0/stpmex/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     InvalidAmount,
     InvalidField,
     InvalidInstitution,
     InvalidPassphrase,
     InvalidRfcOrCurp,
     InvalidTrackingKey,
     MandatoryField,
+    NoEntityFound,
     NoOrdenesEncontradas,
     NoServiceResponse,
     PldRejected,
     SameAccount,
     SignatureValidationError,
     StpmexException,
 )
@@ -135,14 +136,16 @@
 
     if id == 0 and error == 'No se recibió respuesta del servicio':
         raise NoServiceResponse(**resp['resultado'])
     elif id == 0 and error == 'Error validando la firma':
         raise SignatureValidationError(**resp['resultado'])
     elif id == 0 and re.match(r'El campo .+ es obligatorio', error):
         raise MandatoryField(**resp['resultado'])
+    elif id == 0 and 'No entity found for query' in error:
+        raise NoEntityFound(**resp['resultado'])
     elif id == -1 and re.match(
         r'La clave de rastreo .+ ya fue utilizada', error
     ):
         raise ClaveRastreoAlreadyInUse(**resp['resultado'])
     elif id == -7 and re.match(r'La cuenta .+ no existe', error):
         raise AccountDoesNotExist(**resp['resultado'])
     elif id == -9 and re.match(r'La Institucion \d+ no es valida', error):
```

### Comparing `stpmex-3.9.2/stpmex/exc.py` & `stpmex-3.9.3.dev0/stpmex/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,7 +92,11 @@
 
 
 class BlockedInstitutionError(PydanticValueError):
     """Institución bloqueada"""
 
     code = 'clabe.bank_code'
     msg_template = '{bank_name} has been blocked by STP.'
+
+
+class NoEntityFound(StpmexException):
+    """No se encuentra una transacción"""
```

### Comparing `stpmex-3.9.2/stpmex/resources/base.py` & `stpmex-3.9.3.dev0/stpmex/resources/base.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/resources/cuentas.py` & `stpmex-3.9.3.dev0/stpmex/resources/cuentas.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/resources/ordenes.py` & `stpmex-3.9.3.dev0/stpmex/resources/ordenes.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/resources/saldos.py` & `stpmex-3.9.3.dev0/stpmex/resources/saldos.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex/types.py` & `stpmex-3.9.3.dev0/stpmex/types.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/stpmex.egg-info/PKG-INFO` & `stpmex-3.9.3.dev0/stpmex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpmex
-Version: 3.9.2
+Version: 3.9.3.dev0
 Summary: Client library for stpmex.com
 Home-page: https://github.com/cuenca-mx/stpmex-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `stpmex-3.9.2/stpmex.egg-info/SOURCES.txt` & `stpmex-3.9.3.dev0/stpmex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/tests/conftest.py` & `stpmex-3.9.3.dev0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/tests/test_auth.py` & `stpmex-3.9.3.dev0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/tests/test_business_days.py` & `stpmex-3.9.3.dev0/tests/test_business_days.py`

 * *Files identical despite different names*

### Comparing `stpmex-3.9.2/tests/test_client.py` & `stpmex-3.9.3.dev0/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     InvalidAmount,
     InvalidField,
     InvalidInstitution,
     InvalidPassphrase,
     InvalidRfcOrCurp,
     InvalidTrackingKey,
     MandatoryField,
+    NoEntityFound,
     NoServiceResponse,
     PldRejected,
     SameAccount,
     SignatureValidationError,
     StpmexException,
 )
 
@@ -168,14 +169,19 @@
                 descripcion='El campo Apellido materno '
                 'obligatorio 6461801500000000',
                 id=5,
             ),
             CUENTA_ENDPOINT,
             MandatoryField,
         ),
+        (
+            _desc_error('Firma invalida No entity found for query', 0),
+            ORDEN_PAGO_ENDPOINT,
+            NoEntityFound,
+        ),
     ],
     indirect=['client_mock'],
 )
 def test_errors(
     client_mock: Client, endpoint: str, expected_exc: type
 ) -> None:
     with pytest.raises(expected_exc) as exc_info:
```

### Comparing `stpmex-3.9.2/tests/test_validations.py` & `stpmex-3.9.3.dev0/tests/test_validations.py`

 * *Files identical despite different names*

