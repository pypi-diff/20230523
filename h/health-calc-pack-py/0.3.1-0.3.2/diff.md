# Comparing `tmp/health_calc_pack_py-0.3.1.tar.gz` & `tmp/health_calc_pack_py-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health_calc_pack_py-0.3.1.tar", max compression
+gzip compressed data, was "health_calc_pack_py-0.3.2.tar", max compression
```

## Comparing `health_calc_pack_py-0.3.1.tar` & `health_calc_pack_py-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.3.1/health_calc_pack_py/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.3.1/health_calc_pack_py/app.py
--rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.3.1/health_calc_pack_py/imc.py
--rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.3.1/health_calc_pack_py/macronutrientes.py
--rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.3.1/health_calc_pack_py/static/swagger.json
--rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.3.1/health_calc_pack_py/test_imc.py
--rw-r--r--   0        0        0      510 2023-05-17 10:48:39.394796 health_calc_pack_py-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1626 2023-05-17 10:47:52.230226 health_calc_pack_py-0.3.1/README.md
--rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 health_calc_pack_py-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-17 01:13:19.681769 health_calc_pack_py-0.3.2/health_calc_pack_py/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-17 02:07:50.108989 health_calc_pack_py-0.3.2/health_calc_pack_py/app.py
+-rw-r--r--   0        0        0      114 2023-05-17 01:13:20.285768 health_calc_pack_py-0.3.2/health_calc_pack_py/imc.py
+-rw-r--r--   0        0        0      869 2023-05-17 01:29:17.749957 health_calc_pack_py-0.3.2/health_calc_pack_py/macronutrientes.py
+-rw-r--r--   0        0        0     2988 2023-05-17 01:52:51.016461 health_calc_pack_py-0.3.2/health_calc_pack_py/static/swagger.json
+-rw-r--r--   0        0        0      234 2023-05-17 01:13:21.222773 health_calc_pack_py-0.3.2/health_calc_pack_py/test_imc.py
+-rw-r--r--   0        0        0      568 2023-05-22 22:23:53.511991 health_calc_pack_py-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1602 2023-05-22 22:24:08.055486 health_calc_pack_py-0.3.2/README.md
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 health_calc_pack_py-0.3.2/PKG-INFO
```

### Comparing `health_calc_pack_py-0.3.1/health_calc_pack_py/app.py` & `health_calc_pack_py-0.3.2/health_calc_pack_py/app.py`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.3.1/health_calc_pack_py/macronutrientes.py` & `health_calc_pack_py-0.3.2/health_calc_pack_py/macronutrientes.py`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.3.1/health_calc_pack_py/static/swagger.json` & `health_calc_pack_py-0.3.2/health_calc_pack_py/static/swagger.json`

 * *Files identical despite different names*

### Comparing `health_calc_pack_py-0.3.1/README.md` & `health_calc_pack_py-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,14 @@
 
 ## Testes unitários
 
 python -m unittest discover tests
 
 Isso executará todos os testes unitários definidos na pasta tests e exibirá os resultados.
 
-## Testes unitários
-
 Endpoints
 
 A API fornece os seguintes endpoints:
 
 /imc: Recebe um JSON contendo altura e peso, e retorna o IMC calculado.
 
 /macronutrientes: Recebe um JSON contendo peso e objetivo nutricional, e retorna os macronutrientes calculados.
```

### Comparing `health_calc_pack_py-0.3.1/PKG-INFO` & `health_calc_pack_py-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: health-calc-pack-py
-Version: 0.3.1
+Version: 0.3.2
 Summary: Uma API para calcular IMC e macronutrientes
 Author: Angelo Diniz
 Author-email: angelo.jose.7l@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -55,16 +55,14 @@
 
 ## Testes unitários
 
 python -m unittest discover tests
 
 Isso executará todos os testes unitários definidos na pasta tests e exibirá os resultados.
 
-## Testes unitários
-
 Endpoints
 
 A API fornece os seguintes endpoints:
 
 /imc: Recebe um JSON contendo altura e peso, e retorna o IMC calculado.
 
 /macronutrientes: Recebe um JSON contendo peso e objetivo nutricional, e retorna os macronutrientes calculados.
```

