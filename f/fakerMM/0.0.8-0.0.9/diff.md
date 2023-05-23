# Comparing `tmp/fakerMM-0.0.8.tar.gz` & `tmp/fakerMM-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakerMM-0.0.8.tar", last modified: Tue Jan 10 08:57:00 2023, max compression
+gzip compressed data, was "fakerMM-0.0.9.tar", last modified: Fri Jan 27 08:48:57 2023, max compression
```

## Comparing `fakerMM-0.0.8.tar` & `fakerMM-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 08:57:00.812438 fakerMM-0.0.8/
--rw-rw-rw-   0        0        0     1066 2022-08-09 07:37:06.000000 fakerMM-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-08-09 07:40:00.000000 fakerMM-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      553 2023-01-10 08:57:00.811442 fakerMM-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       31 2022-08-22 07:19:16.000000 fakerMM-0.0.8/README.txt
-drwxrwxrwx   0        0        0        0 2023-01-10 08:57:00.795909 fakerMM-0.0.8/fakerMM/
--rw-rw-rw-   0        0        0    10014 2023-01-09 14:28:50.000000 fakerMM-0.0.8/fakerMM/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-10 08:57:00.809429 fakerMM-0.0.8/fakerMM.egg-info/
--rw-rw-rw-   0        0        0      553 2023-01-10 08:57:00.000000 fakerMM-0.0.8/fakerMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-01-10 08:57:00.000000 fakerMM-0.0.8/fakerMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 08:57:00.000000 fakerMM-0.0.8/fakerMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-01-10 08:57:00.000000 fakerMM-0.0.8/fakerMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-10 08:57:00.000000 fakerMM-0.0.8/fakerMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-10 08:57:00.812438 fakerMM-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-01-10 08:56:18.000000 fakerMM-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-27 08:48:57.556952 fakerMM-0.0.9/
+-rw-rw-rw-   0        0        0     1066 2022-08-09 07:37:06.000000 fakerMM-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2022-08-09 07:40:00.000000 fakerMM-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2023-01-27 08:48:57.555957 fakerMM-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2022-08-22 07:19:16.000000 fakerMM-0.0.9/README.txt
+drwxrwxrwx   0        0        0        0 2023-01-27 08:48:57.544857 fakerMM-0.0.9/fakerMM/
+-rw-rw-rw-   0        0        0    11313 2023-01-20 12:15:12.000000 fakerMM-0.0.9/fakerMM/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-27 08:48:57.554709 fakerMM-0.0.9/fakerMM.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-01-27 08:48:57.000000 fakerMM-0.0.9/fakerMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-01-27 08:48:57.000000 fakerMM-0.0.9/fakerMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-27 08:48:57.000000 fakerMM-0.0.9/fakerMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-01-27 08:48:57.000000 fakerMM-0.0.9/fakerMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-01-27 08:48:57.000000 fakerMM-0.0.9/fakerMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-27 08:48:57.556952 fakerMM-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-01-27 08:48:19.000000 fakerMM-0.0.9/setup.py
```

### Comparing `fakerMM-0.0.8/LICENSE.txt` & `fakerMM-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fakerMM-0.0.8/PKG-INFO` & `fakerMM-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakerMM
-Version: 0.0.8
+Version: 0.0.9
 Summary: datos sinteticos personalizados
 Home-page: UNKNOWN
 Author: Patricia Perez Villegas
 Author-email: 
 License: MIT
 Keywords: faker
 Platform: UNKNOWN
```

### Comparing `fakerMM-0.0.8/fakerMM/__init__.py` & `fakerMM-0.0.9/fakerMM/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -264,22 +264,73 @@
 #Contraseña sintetica
 
 def password(row):
     random_str_seq = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz@?!._-#" 
     res = ''.join(random.choices(random_str_seq, k=15))
     return (res)
 
-#    CUENTA CORRIENTE
+#    CUENTA CORRIENTE 
 #----------------------------------------------------------------------
-#Cuenta corriente fija
+#Cuenta corriente completa fija
 
-def current_account(row):
+def current_account_complete(row):
     campo='99999999509999999999'
     return (campo)
 
-#     IBAN
+#Campo cuenta corriente
+def current_account(row):
+    campo='9999999999'
+    return (campo)
+
+#     IBAN 
 #---------------------------------------------------------------------
-#Iban fijo
+#Iban completo fijo
 
-def iban(row):
+def iban_complete(row):
     campo='ES1299999999509999999999'
-    return (campo)
+    return (campo)
+
+#Iban
+def iban(row):
+    campo='ES12'
+    return (campo)
+
+# OTRAS COMPONENTES CUENTA CORRIENTE
+#----------------------------------------
+#Banco
+def bank(row):
+    campo='9999'
+    return (campo)
+#Sucursal
+def bank_office(row):
+    campo='9999'
+    return (campo)
+#Digito de control completo
+def DC_complete(row):
+    campo='50'
+    return (campo)
+#Digito de control 1
+def DC1(row):
+    campo='5'
+    return (campo)
+#Digito de control 2
+def DC2(row):
+    campo='0'
+    return (campo)
+
+#    COORDENADA X (LONGITUD)
+#----------------------------------------------------------------------
+#Valor de la coordenada x que se corresponde con la longitud cuyo valor debe oscilar entre -180 y 180
+
+def coordinateX(row):
+    #valor de la longitud entre -180 y 180
+    x = np.random.randint(-180, 180) 
+    return (x)
+
+#   COORDENADA Y (LATITUD)
+#------------------------------------------------------------------------
+#Valor de la coordenada y que se corresponde con la longitud cuyo valor debe oscilar entre -90 y 90
+
+def coordinateY(row):
+    #Valor latitud entre -90 y 90
+    y = np.random.randint(-90, 90) 
+    return (y)
```

### Comparing `fakerMM-0.0.8/fakerMM.egg-info/PKG-INFO` & `fakerMM-0.0.9/fakerMM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakerMM
-Version: 0.0.8
+Version: 0.0.9
 Summary: datos sinteticos personalizados
 Home-page: UNKNOWN
 Author: Patricia Perez Villegas
 Author-email: 
 License: MIT
 Keywords: faker
 Platform: UNKNOWN
```

### Comparing `fakerMM-0.0.8/setup.py` & `fakerMM-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='fakerMM',
-  version='0.0.8',
+  version='0.0.9',
   description='datos sinteticos personalizados',
   long_description=open('README.txt').read() + '\n\n',
   url='',  
   author='Patricia Perez Villegas',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

