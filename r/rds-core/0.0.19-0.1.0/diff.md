# Comparing `tmp/rds-core-0.0.19.tar.gz` & `tmp/rds-core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.0.19.tar", last modified: Tue May 23 00:32:29 2023, max compression
+gzip compressed data, was "rds-core-0.1.0.tar", last modified: Tue May 23 00:39:01 2023, max compression
```

## Comparing `rds-core-0.0.19.tar` & `rds-core-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.638781 rds-core-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 00:32:06.000000 rds-core-0.0.19/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-23 00:32:29.638781 rds-core-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 00:32:06.000000 rds-core-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.630781 rds-core-0.0.19/rds_core/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.634781 rds-core-0.0.19/rds_core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.634781 rds-core-0.0.19/rds_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.638781 rds-core-0.0.19/rds_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/helpers/cnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.638781 rds-core-0.0.19/rds_core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.626781 rds-core-0.0.19/rds_core/transformers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.638781 rds-core-0.0.19/rds_core/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.638781 rds-core-0.0.19/rds_core/transformers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-23 00:32:06.000000 rds-core-0.0.19/rds_core/transformers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:32:29.634781 rds-core-0.0.19/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-23 00:32:29.000000 rds-core-0.0.19/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 00:32:29.000000 rds-core-0.0.19/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:32:29.000000 rds-core-0.0.19/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-23 00:32:29.000000 rds-core-0.0.19/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 00:32:29.000000 rds-core-0.0.19/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 00:32:29.642781 rds-core-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-23 00:32:06.000000 rds-core-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 00:38:37.000000 rds-core-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-23 00:39:01.592189 rds-core-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 00:38:37.000000 rds-core-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.588189 rds-core-0.1.0/rds_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/helpers/cnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.584189 rds-core-0.1.0/rds_core/transformers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.592189 rds-core-0.1.0/rds_core/transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-23 00:38:37.000000 rds-core-0.1.0/rds_core/transformers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:39:01.588189 rds-core-0.1.0/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-23 00:39:01.000000 rds-core-0.1.0/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 00:39:01.000000 rds-core-0.1.0/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:39:01.000000 rds-core-0.1.0/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-23 00:39:01.000000 rds-core-0.1.0/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 00:39:01.000000 rds-core-0.1.0/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 00:39:01.596189 rds-core-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-23 00:38:37.000000 rds-core-0.1.0/setup.py
```

### Comparing `rds-core-0.0.19/PKG-INFO` & `rds-core-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-core
-Version: 0.0.19
+Version: 0.1.0
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Keywords: rds,cache,config,helper,searchengine
```

### Comparing `rds-core-0.0.19/README.md` & `rds-core-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/cache/__init__.py` & `rds-core-0.1.0/rds_core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/cache/base.py` & `rds-core-0.1.0/rds_core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/cache/nocache.py` & `rds-core-0.1.0/rds_core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/cache/search_engine.py` & `rds-core-0.1.0/rds_core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/helpers/__init__.py` & `rds-core-0.1.0/rds_core/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/helpers/http_client.py` & `rds-core-0.1.0/rds_core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/searchengine/__init__.py` & `rds-core-0.1.0/rds_core/searchengine/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core/transformers/fields/__init__.py` & `rds-core-0.1.0/rds_core/transformers/fields/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         source_dict: Dict[str, Any],
         dest_dict: Dict[str, Any],
         dest_fieldname: str,
     ):
         if self.source_field is None:
             dest_dict[dest_fieldname] = None
         else:
-            dest_dict[dest_fieldname] = self.cast(
+            dest_dict[dest_fieldname] = self.cast_source_value(
                 get_dict_by_pathname(source_dict, self.source_field)
             )
 
     def cast_source_value(self, source_value: Union[str, int, bool, float]):
         return source_value
 
 
@@ -65,15 +65,18 @@
         self,
         source_dict: Dict[str, Any],
         dest_dict: Dict[str, Any],
         dest_fieldname: str,
     ) -> str:
         if self.fields is not None:
             dest_dict[dest_fieldname] = self.separator.join(
-                [self.cast(get_dict_by_pathname(source_dict, f)) for f in self.fields]
+                [
+                    self.cast_source_value(get_dict_by_pathname(source_dict, f))
+                    for f in self.fields
+                ]
             )
 
 
 class SubModelField(Field):
     def transform_to_dict(
         self,
         source_dict: Dict[str, Any],
```

### Comparing `rds-core-0.0.19/rds_core/transformers/models/__init__.py` & `rds-core-0.1.0/rds_core/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/rds_core.egg-info/PKG-INFO` & `rds-core-0.1.0/rds_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rds-core
-Version: 0.0.19
+Version: 0.1.0
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Keywords: rds,cache,config,helper,searchengine
```

### Comparing `rds-core-0.0.19/rds_core.egg-info/SOURCES.txt` & `rds-core-0.1.0/rds_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rds-core-0.0.19/setup.py` & `rds-core-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.0.19",
+    version="0.1.0",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
```

