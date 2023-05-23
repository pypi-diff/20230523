# Comparing `tmp/digitalguide_reader-0.0.8.tar.gz` & `tmp/digitalguide_reader-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalguide_reader-0.0.8.tar", last modified: Wed Oct 19 17:23:53 2022, max compression
+gzip compressed data, was "digitalguide_reader-0.0.9.tar", last modified: Wed Oct 19 17:50:54 2022, max compression
```

## Comparing `digitalguide_reader-0.0.8.tar` & `digitalguide_reader-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:53.276610 digitalguide_reader-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-19 17:23:53.276610 digitalguide_reader-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:53.272610 digitalguide_reader-0.0.8/digitalguide_reader/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/gsheet2actions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:53.276610 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/
--rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Action.py
--rw-r--r--   0 runner    (1001) docker     (121)    18970 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Interaktion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Route.py
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/wegInteraktion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:23:53.272610 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-19 17:23:53.000000 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-19 17:23:53.000000 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 17:23:53.000000 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-19 17:23:53.000000 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-19 17:23:53.000000 digitalguide_reader-0.0.8/digitalguide_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 17:23:53.276610 digitalguide_reader-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-19 17:23:26.000000 digitalguide_reader-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/digitalguide_reader/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/gsheet2actions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/
+-rw-r--r--   0 runner    (1001) docker     (121)     8301 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Action.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19068 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Interaktion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1823 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Route.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Trigger.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/wegInteraktion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-10-19 17:50:54.000000 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-10-19 17:50:54.000000 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 17:50:54.000000 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-10-19 17:50:54.000000 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-19 17:50:54.000000 digitalguide_reader-0.0.9/digitalguide_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-19 17:50:54.978403 digitalguide_reader-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-19 17:50:32.000000 digitalguide_reader-0.0.9/setup.py
```

### Comparing `digitalguide_reader-0.0.8/LICENSE` & `digitalguide_reader-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/gsheet2actions.py` & `digitalguide_reader-0.0.9/digitalguide_reader/gsheet2actions.py`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Action.py` & `digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Action.py`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Interaktion.py` & `digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Interaktion.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,22 +181,22 @@
 
             for aktion, aktion_list in interaktion_dict.items():
                 if aktion.startswith("antwort_"):
                     actions["{}_{}".format(poi_name, aktion)] = [{"type": "function",
                                                                   "func": "loop_list",
                                                                   "key": poi_name,
                                                                   "value": aktion.replace("antwort_", ""),
-                                                                  "doppelte_antwort": interaktion_dict["doppelte Antwort"][0][1]}]\
+                                                                  "doppelte_antwort": readActions(interaktion_dict["doppelte Antwort"], messanger=messanger, asset_url=asset_url)}]\
                         + readActions(aktion_list, messanger=messanger, asset_url=asset_url) \
                         + readActions(interaktion_dict["richtig Antwort"], messanger=messanger, asset_url=asset_url) \
                         + [{"type": "function",
                             "func": "loop_list_fertig",
                             "key": poi_name,
                             "answer_id_list": answer_id_list,
-                            "fertig_antwort": interaktion_dict["fertig Antwort"][0][1]}]
+                            "fertig_antwort": readActions(interaktion_dict["fertig Antwort"], messanger=messanger, asset_url=asset_url)}]
                     
                     actions["{}_{}_re".format(poi_name, aktion)] = readActions(aktion_list, messanger=messanger, asset_url=asset_url) \
                                                                         + readActions(interaktion_dict["richtig Antwort"], messanger=messanger, asset_url=asset_url)
 
                 elif aktion.startswith("trigger_"):
                     if aktion != "trigger_weiter":
                         states["{}_FRAGE".format(poi_name.upper())] += readTriggers(
```

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Route.py` & `digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Route.py`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/Trigger.py` & `digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/Trigger.py`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader/standardinteraktion/wegInteraktion.py` & `digitalguide_reader-0.0.9/digitalguide_reader/standardinteraktion/wegInteraktion.py`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/digitalguide_reader.egg-info/SOURCES.txt` & `digitalguide_reader-0.0.9/digitalguide_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalguide_reader-0.0.8/setup.py` & `digitalguide_reader-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='digitalguide_reader',
     packages=find_packages(),
-    version='0.0.8',
+    version='0.0.9',
     description='A Python Library to read in a google sheet and turn it into states and actions',
     author='Soeren Etler',
     license='MIT',
     install_requires=["openpyxl",
                       "PyYAML",
                       "requests",
                       "gunicorn",
```

