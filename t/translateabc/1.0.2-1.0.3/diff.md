# Comparing `tmp/translateabc-1.0.2.tar.gz` & `tmp/translateabc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translateabc-1.0.2.tar", last modified: Tue May 23 12:31:33 2023, max compression
+gzip compressed data, was "translateabc-1.0.3.tar", last modified: Tue May 23 12:43:02 2023, max compression
```

## Comparing `translateabc-1.0.2.tar` & `translateabc-1.0.3.tar`

### file list

```diff
@@ -1,53 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.201017 translateabc-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.168428 translateabc-1.0.2/.idea/
--rw-rw-rw-   0        0        0      184 2023-05-23 11:40:39.000000 translateabc-1.0.2/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.169429 translateabc-1.0.2/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      174 2023-05-23 11:40:38.000000 translateabc-1.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      182 2023-05-23 11:48:08.000000 translateabc-1.0.2/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-05-23 11:40:38.000000 translateabc-1.0.2/.idea/modules.xml
--rw-rw-rw-   0        0        0      318 2023-05-23 11:48:08.000000 translateabc-1.0.2/.idea/translateabc.iml
--rw-rw-rw-   0        0        0     4010 2023-05-23 12:31:12.000000 translateabc-1.0.2/.idea/workspace.xml
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-23 12:30:23.000000 translateabc-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      491 2023-05-23 12:31:33.201017 translateabc-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.173456 translateabc-1.0.2/dist/
--rw-rw-rw-   0        0        0  1675410 2023-05-23 12:31:15.000000 translateabc-1.0.2/dist/translateabc-1.0.2.tar.gz
--rw-rw-rw-   0        0        0   531223 2023-05-23 12:31:15.000000 translateabc-1.0.2/dist/translateabc-1.0.2.win-amd64.zip
--rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 12:31:33.201535 translateabc-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-23 12:31:12.000000 translateabc-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.155399 translateabc-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.175958 translateabc-1.0.2/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.156901 translateabc-1.0.2/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.156400 translateabc-1.0.2/src/translateabc/READMEhh/ai35/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.187475 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/
--rw-rw-rw-   0        0        0     2469 2023-05-22 14:26:06.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/1.ipynb
--rw-rw-rw-   0        0        0     5078 2023-05-22 14:26:04.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/2.ipynb
--rw-rw-rw-   0        0        0     2661 2023-05-22 14:30:18.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/3.ipynb
--rw-rw-rw-   0        0        0    12943 2023-05-22 14:36:23.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/4.ipynb
--rw-rw-rw-   0        0        0     4965 2023-05-22 14:48:13.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/5.ipynb
--rw-rw-rw-   0        0        0     3570 2023-05-22 15:10:05.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/6.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.188984 translateabc-1.0.2/src/translateabc/READMEhh/ai35/02/
--rw-rw-rw-   0        0        0        0 2023-05-22 14:53:43.000000 translateabc-1.0.2/src/translateabc/READMEhh/ai35/02/01.ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.189985 translateabc-1.0.2/src/translateabc/READMEhh/moni/
--rw-rw-rw-   0        0        0  4928289 2022-08-06 03:19:14.000000 translateabc-1.0.2/src/translateabc/READMEhh/moni/bankmarketing.csv
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.199013 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/
--rw-rw-rw-   0        0        0      124 2023-05-22 15:56:25.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/1.csv
--rw-rw-rw-   0        0        0     5625 2023-05-22 16:09:33.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/1.ipynb
--rw-rw-rw-   0        0        0       53 2023-05-22 15:56:19.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/2.csv
--rw-rw-rw-   0        0        0      167 2023-05-22 15:59:00.000000 translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/output.csv
--rw-rw-rw-   0        0        0       69 2023-05-23 11:44:44.000000 translateabc-1.0.2/src/translateabc/__init__.py
--rw-rw-rw-   0        0        0      386 2023-05-23 11:44:03.000000 translateabc-1.0.2/src/translateabc/translateabc.py
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:33.179962 translateabc-1.0.2/src/translateabc.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-23 12:31:33.000000 translateabc-1.0.2/src/translateabc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.232976 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.233980 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/
-drwxrwxrwx   0        0        0        0 2023-05-23 12:31:15.276650 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/
--r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.255659 translateabc-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.220548 translateabc-1.0.3/.idea/
+-rw-rw-rw-   0        0        0      184 2023-05-23 11:40:39.000000 translateabc-1.0.3/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.222057 translateabc-1.0.3/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      174 2023-05-23 11:40:38.000000 translateabc-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      182 2023-05-23 11:48:08.000000 translateabc-1.0.3/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-05-23 11:40:38.000000 translateabc-1.0.3/.idea/modules.xml
+-rw-rw-rw-   0        0        0      318 2023-05-23 11:48:08.000000 translateabc-1.0.3/.idea/translateabc.iml
+-rw-rw-rw-   0        0        0     4010 2023-05-23 12:43:00.000000 translateabc-1.0.3/.idea/workspace.xml
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:45.000000 translateabc-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-23 12:30:23.000000 translateabc-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      491 2023-05-23 12:43:02.255159 translateabc-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-23 11:45:51.000000 translateabc-1.0.3/README.md
+-rw-rw-rw-   0        0        0       88 2023-05-23 11:45:30.000000 translateabc-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 12:43:02.255659 translateabc-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-23 12:43:00.000000 translateabc-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.202501 translateabc-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.224559 translateabc-1.0.3/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.205003 translateabc-1.0.3/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.204002 translateabc-1.0.3/src/translateabc/READMEhh/ai35/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.237095 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/
+-rw-rw-rw-   0        0        0     2469 2023-05-22 14:26:06.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/1.ipynb
+-rw-rw-rw-   0        0        0     5078 2023-05-22 14:26:04.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/2.ipynb
+-rw-rw-rw-   0        0        0     2661 2023-05-22 14:30:18.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/3.ipynb
+-rw-rw-rw-   0        0        0    12943 2023-05-22 14:36:23.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/4.ipynb
+-rw-rw-rw-   0        0        0     4965 2023-05-22 14:48:13.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/5.ipynb
+-rw-rw-rw-   0        0        0     3570 2023-05-22 15:10:05.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/6.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.238096 translateabc-1.0.3/src/translateabc/READMEhh/ai35/02/
+-rw-rw-rw-   0        0        0        0 2023-05-22 14:53:43.000000 translateabc-1.0.3/src/translateabc/READMEhh/ai35/02/01.ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.244123 translateabc-1.0.3/src/translateabc/READMEhh/moni/
+-rw-rw-rw-   0        0        0  4928289 2022-08-06 03:19:14.000000 translateabc-1.0.3/src/translateabc/READMEhh/moni/bankmarketing.csv
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.3/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.249127 translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/
+-rw-rw-rw-   0        0        0      124 2023-05-22 15:56:25.000000 translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/1.csv
+-rw-rw-rw-   0        0        0     5625 2023-05-22 16:09:33.000000 translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/1.ipynb
+-rw-rw-rw-   0        0        0       53 2023-05-22 15:56:19.000000 translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/2.csv
+-rw-rw-rw-   0        0        0      167 2023-05-22 15:59:00.000000 translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/output.csv
+-rw-rw-rw-   0        0        0       85 2023-05-23 12:42:24.000000 translateabc-1.0.3/src/translateabc/__init__.py
+-rw-rw-rw-   0        0        0      386 2023-05-23 11:44:03.000000 translateabc-1.0.3/src/translateabc/translateabc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.229063 translateabc-1.0.3/src/translateabc.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-23 12:43:02.000000 translateabc-1.0.3/src/translateabc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2023-05-23 12:43:02.000000 translateabc-1.0.3/src/translateabc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:43:02.000000 translateabc-1.0.3/src/translateabc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 12:43:02.000000 translateabc-1.0.3/src/translateabc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.205504 translateabc-1.0.3/translateabc-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.206004 translateabc-1.0.3/translateabc-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.206004 translateabc-1.0.3/translateabc-1.0.1/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.206504 translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.250655 translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/moni/
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.208506 translateabc-1.0.3/translateabc-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.207506 translateabc-1.0.3/translateabc-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.207506 translateabc-1.0.3/translateabc-1.0.2/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.208006 translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.252156 translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/moni/
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.3/translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.208506 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.209006 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.209006 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.209006 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:43:02.253658 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/
+-r--r--r--   0        0        0   236578 2023-05-22 16:01:29.000000 translateabc-1.0.3/translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
```

### Comparing `translateabc-1.0.2/.idea/workspace.xml` & `translateabc-1.0.3/.idea/workspace.xml`

 * *Files 1% similar despite different names*

#### Comparing `translateabc-1.0.2/.idea/workspace.xml` & `translateabc-1.0.3/.idea/workspace.xml`

```diff
@@ -65,15 +65,15 @@
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="abbb2ca3-9882-4039-a5c1-346b705212b6" name="Changes" comment=""/>
       <created>1684841815866</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1684841815866</updated>
-      <workItem from="1684841953267" duration="3087000"/>
+      <workItem from="1684841953267" duration="3785000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
```

### Comparing `translateabc-1.0.2/setup.py` & `translateabc-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="translateabc",
-    version="1.0.2",
+    version="1.0.3",
     author="Linvery",
     author_email="1253445120@qq.com",
     description="translateabc",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="https://github.com/pypa/sampleproject",
```

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/1.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/1.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/2.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/2.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/3.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/3.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/4.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/4.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/5.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/5.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/ai35/01/6.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/ai35/01/6.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/moni/bankmarketing.csv` & `translateabc-1.0.3/src/translateabc/READMEhh/moni/bankmarketing.csv`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc/READMEhh/pandas-exercise/1.ipynb` & `translateabc-1.0.3/src/translateabc/READMEhh/pandas-exercise/1.ipynb`

 * *Files identical despite different names*

### Comparing `translateabc-1.0.2/src/translateabc.egg-info/SOURCES.txt` & `translateabc-1.0.3/src/translateabc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 setup.py
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
 .idea/translateabc.iml
 .idea/workspace.xml
 .idea/inspectionProfiles/profiles_settings.xml
-dist/translateabc-1.0.2.tar.gz
-dist/translateabc-1.0.2.win-amd64.zip
 src/translateabc/__init__.py
 src/translateabc/translateabc.py
 src/translateabc.egg-info/PKG-INFO
 src/translateabc.egg-info/SOURCES.txt
 src/translateabc.egg-info/dependency_links.txt
 src/translateabc.egg-info/top_level.txt
 src/translateabc/READMEhh/ai35/01/1.ipynb
@@ -26,8 +24,10 @@
 src/translateabc/READMEhh/ai35/02/01.ipynb
 src/translateabc/READMEhh/moni/bankmarketing.csv
 src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
 src/translateabc/READMEhh/pandas-exercise/1.csv
 src/translateabc/READMEhh/pandas-exercise/1.ipynb
 src/translateabc/READMEhh/pandas-exercise/2.csv
 src/translateabc/READMEhh/pandas-exercise/output.csv
-translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+translateabc-1.0.2/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
+translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb
```

### Comparing `translateabc-1.0.2/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb` & `translateabc-1.0.3/translateabc-1.0.1/src/translateabc/READMEhh/moni/bigdata01-8(1).ipynb`

 * *Files identical despite different names*

