# Comparing `tmp/relativedate-1.1.0.tar.gz` & `tmp/relativedate-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relativedate-1.1.0.tar", last modified: Tue May 23 15:18:04 2023, max compression
+gzip compressed data, was "relativedate-1.2.0.tar", last modified: Tue May 23 18:34:23 2023, max compression
```

## Comparing `relativedate-1.1.0.tar` & `relativedate-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 15:18:04.442003 relativedate-1.1.0/
--rw-rw-rw-   0        0        0     2406 2023-05-23 15:18:04.441006 relativedate-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2246 2023-05-23 10:51:04.000000 relativedate-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 15:18:04.422056 relativedate-1.1.0/relativedate/
--rw-rw-rw-   0        0        0     1221 2023-05-23 15:07:26.000000 relativedate-1.1.0/relativedate/__init__.py
--rw-rw-rw-   0        0        0     1369 2023-05-23 15:07:39.000000 relativedate-1.1.0/relativedate/dtmath.py
-drwxrwxrwx   0        0        0        0 2023-05-23 15:18:04.440009 relativedate-1.1.0/relativedate.egg-info/
--rw-rw-rw-   0        0        0     2406 2023-05-23 15:18:04.000000 relativedate-1.1.0/relativedate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-23 15:18:04.000000 relativedate-1.1.0/relativedate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 15:18:04.000000 relativedate-1.1.0/relativedate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 15:18:04.000000 relativedate-1.1.0/relativedate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 15:18:04.442003 relativedate-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      455 2023-05-23 11:28:58.000000 relativedate-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.039123 relativedate-1.2.0/
+-rw-rw-rw-   0        0        0     2387 2023-05-23 18:34:23.038125 relativedate-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2227 2023-05-23 18:33:38.000000 relativedate-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.024163 relativedate-1.2.0/relativedate/
+-rw-rw-rw-   0        0        0     1427 2023-05-23 18:25:53.000000 relativedate-1.2.0/relativedate/__init__.py
+-rw-rw-rw-   0        0        0      394 2023-05-23 18:27:39.000000 relativedate-1.2.0/relativedate/dtget.py
+-rw-rw-rw-   0        0        0     1369 2023-05-23 15:07:39.000000 relativedate-1.2.0/relativedate/dtmath.py
+drwxrwxrwx   0        0        0        0 2023-05-23 18:34:23.037132 relativedate-1.2.0/relativedate.egg-info/
+-rw-rw-rw-   0        0        0     2387 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 18:34:22.000000 relativedate-1.2.0/relativedate.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 18:34:23.039123 relativedate-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      455 2023-05-23 18:34:19.000000 relativedate-1.2.0/setup.py
```

### Comparing `relativedate-1.1.0/PKG-INFO` & `relativedate-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
     Biblioteca Python relacionada a datas, onde é criado um objeto "RelativeDate" que possui o atributo datetime, onde é retornado um objeto datetime.
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
-<u><b>Links</b></u> <br>
-    <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-    <b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-    <b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>Links</b> <br>
+<b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
+<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.1.0 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.2.0 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

### Comparing `relativedate-1.1.0/README.md` & `relativedate-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     Biblioteca Python relacionada a datas, onde é criado um objeto "RelativeDate" que possui o atributo datetime, onde é retornado um objeto datetime.
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
-<u><b>Links</b></u> <br>
-    <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-    <b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-    <b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>Links</b> <br>
+<b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
+<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

### Comparing `relativedate-1.1.0/relativedate/dtmath.py` & `relativedate-1.2.0/relativedate/dtmath.py`

 * *Files identical despite different names*

### Comparing `relativedate-1.1.0/relativedate.egg-info/PKG-INFO` & `relativedate-1.2.0/relativedate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: relativedate
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pacote Python para tabalhar com Datas Relativas
 Description-Content-Type: text/markdown
 
 <h1>Python Package: relativedate</h1>
 
 <b>Descrição:</b>
 <p>
     Biblioteca Python relacionada a datas, onde é criado um objeto "RelativeDate" que possui o atributo datetime, onde é retornado um objeto datetime.
 </p>
 <p>
     O objetivo desta biblioteca é facilitar a manipulação de datas relativas e calculos com datas, em sua primeira versão estamos trabalhando apenas com a data relativa baseado em mês, onde pode se passar o argumento de meses (positivo e negativo) e retornará a data relativa ao mês desejado
 </p>
 
 <hr>
-<u><b>Links</b></u> <br>
-    <b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
-    <b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
-    <b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
+<b>Links</b> <br>
+<b>GitHub:</b> <a href="https://github.com/jmiante/relativedate/" target="_blank">https://github.com/jmiante/relativedate</a> <br>
+<b>PyPI:</b> <a href="https://pypi.org/project/relativedate/" target="_blank">https://pypi.org/project/relativedate</a> <br>
+<b>Site:</b> <a href="https://jmiante.github.io/relativedate/" target="_blank">https://jmiante.github.io/relativedate</a> <br>
 
 <hr>
 <b>Instalação:</b>
 <p>pip install relativedate</p>
 <hr>
 
 <hr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: relativedate Version: 1.1.0 Summary: Pacote Python
+Metadata-Version: 2.1 Name: relativedate Version: 1.2.0 Summary: Pacote Python
 para tabalhar com Datas Relativas Description-Content-Type: text/markdown
 ****** Python Package: relativedate ******
 DescriÃ§Ã£o:
 Biblioteca Python relacionada a datas, onde Ã© criado um objeto "RelativeDate"
 que possui o atributo datetime, onde Ã© retornado um objeto datetime.
 O objetivo desta biblioteca Ã© facilitar a manipulaÃ§Ã£o de datas relativas e
 calculos com datas, em sua primeira versÃ£o estamos trabalhando apenas com a
```

