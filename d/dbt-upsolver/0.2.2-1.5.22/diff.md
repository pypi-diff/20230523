# Comparing `tmp/dbt-upsolver-0.2.2.tar.gz` & `tmp/dbt-upsolver-1.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-0.2.2.tar", last modified: Mon May 22 18:07:53 2023, max compression
+gzip compressed data, was "dbt-upsolver-1.5.22.tar", last modified: Tue May 23 13:07:01 2023, max compression
```

## Comparing `dbt-upsolver-0.2.2.tar` & `dbt-upsolver-1.5.22.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/target_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.366083 dbt-upsolver-1.5.22/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.366083 dbt-upsolver-1.5.22/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.370083 dbt-upsolver-1.5.22/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.374083 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-23 13:07:01.000000 dbt-upsolver-1.5.22/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:07:01.378083 dbt-upsolver-1.5.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-23 13:06:47.000000 dbt-upsolver-1.5.22/setup.py
```

### Comparing `dbt-upsolver-0.2.2/LICENSE` & `dbt-upsolver-1.5.22/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/PKG-INFO` & `dbt-upsolver-1.5.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.2
+Version: 1.5.22
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.2/README.md` & `dbt-upsolver-1.5.22/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/target_options.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/target_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-1.5.22/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/incremental.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-1.5.22/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-1.5.22/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.2
+Version: 1.5.22
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.2/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-1.5.22/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.2/setup.py` & `dbt-upsolver-1.5.22/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 package_name = "dbt-upsolver"
 package_version = _dbt_upsolver_version()
 description = """The Upsolver adapter plugin for dbt"""
-dbt_version = '1.4.5'
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -63,15 +62,15 @@
             "include/upsolver/profile_template.yml",
             "include/upsolver/macros/*.sql",
             "include/upsolver/macros/*/*.sql"
         ]
     },
     include_package_data=True,
     install_requires = [
-        "dbt-core~=1.4.6",
+        "dbt-core~=1.5.0",
         "upsolver-sdk-python"
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
```

