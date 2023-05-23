# Comparing `tmp/zbuilder-0.0.8.tar.gz` & `tmp/zbuilder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zbuilder-0.0.8.tar", last modified: Fri Dec 13 21:34:10 2019, max compression
+gzip compressed data, was "dist/zbuilder-0.0.9.tar", last modified: Fri Dec 13 21:45:34 2019, max compression
```

## Comparing `zbuilder-0.0.8.tar` & `zbuilder-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (115)      864 2019-12-13 21:34:10.000000 zbuilder-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (115)     1092 2019-12-13 21:32:55.000000 zbuilder-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/
--rw-r--r--   0 runner    (1001) docker     (115)      797 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/cfg.py
--rw-r--r--   0 runner    (1001) docker     (115)     6269 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/helpers.py
--rw-r--r--   0 runner    (1001) docker     (115)      877 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/options.py
--rw-r--r--   0 runner    (1001) docker     (115)      436 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/dns/
--rw-r--r--   0 runner    (1001) docker     (115)     1385 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/do.py
--rw-r--r--   0 runner    (1001) docker     (115)      179 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/vagrant.py
--rw-r--r--   0 runner    (1001) docker     (115)     2538 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1688 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/azure.py
--rw-r--r--   0 runner    (1001) docker     (115)     2538 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/gcp.py
--rw-r--r--   0 runner    (1001) docker     (115)      744 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/dns/ansible.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/vm/
--rw-r--r--   0 runner    (1001) docker     (115)     6117 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/do.py
--rw-r--r--   0 runner    (1001) docker     (115)     2130 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/vagrant.py
--rw-r--r--   0 runner    (1001) docker     (115)     1589 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    11266 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/azure.py
--rw-r--r--   0 runner    (1001) docker     (115)     9538 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/gcp.py
--rw-r--r--   0 runner    (1001) docker     (115)     5685 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/vm/ganeti.py
--rw-r--r--   0 runner    (1001) docker     (115)     7264 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/assets/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder/assets/vagrant/
--rw-r--r--   0 runner    (1001) docker     (115)     2782 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/assets/vagrant/Vagrant.j2
--rw-r--r--   0 runner    (1001) docker     (115)      316 2019-12-13 21:32:55.000000 zbuilder-0.0.8/zbuilder/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)      864 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)       47 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        9 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     1187 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)      652 2019-12-13 21:34:10.000000 zbuilder-0.0.8/zbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)       16 2019-12-13 21:32:55.000000 zbuilder-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)    35147 2019-12-13 21:32:55.000000 zbuilder-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)      422 2019-12-13 21:34:10.000000 zbuilder-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)      471 2019-12-13 21:32:55.000000 zbuilder-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (115)     1096 2019-12-13 21:45:34.000000 zbuilder-0.0.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (115)     1092 2019-12-13 21:44:26.000000 zbuilder-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/
+-rw-r--r--   0 runner    (1001) docker     (115)      797 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6269 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (115)      877 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/options.py
+-rw-r--r--   0 runner    (1001) docker     (115)      436 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/dns/
+-rw-r--r--   0 runner    (1001) docker     (115)     1385 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/do.py
+-rw-r--r--   0 runner    (1001) docker     (115)      179 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/vagrant.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2538 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1688 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/azure.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2538 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (115)      744 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/dns/ansible.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/vm/
+-rw-r--r--   0 runner    (1001) docker     (115)     6117 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/do.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2130 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/vagrant.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1589 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11266 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/azure.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9538 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5685 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/vm/ganeti.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7264 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/assets/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder/assets/vagrant/
+-rw-r--r--   0 runner    (1001) docker     (115)     2782 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/assets/vagrant/Vagrant.j2
+-rw-r--r--   0 runner    (1001) docker     (115)      316 2019-12-13 21:44:26.000000 zbuilder-0.0.9/zbuilder/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     1096 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)       47 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        9 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)     1187 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      652 2019-12-13 21:45:34.000000 zbuilder-0.0.9/zbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       16 2019-12-13 21:44:26.000000 zbuilder-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)    35147 2019-12-13 21:44:26.000000 zbuilder-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)      422 2019-12-13 21:45:34.000000 zbuilder-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)      671 2019-12-13 21:44:26.000000 zbuilder-0.0.9/README.md
```

### Comparing `zbuilder-0.0.8/PKG-INFO` & `zbuilder-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: zbuilder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create VMs
 Home-page: https://github.com/hasiotis/zbuilder
 Author: Chasiotis Nikos
 Author-email: hasiotis@gmail.com
 License: GPLv3+
 Description: # Zbuilder: Building VMs and applying ansible playbooks
         
         [![Documentation Status](https://readthedocs.org/projects/zbuilder/badge/?version=latest)](https://zbuilder.readthedocs.io/en/latest/?badge=latest)
         
+        ZBuilder is a tool to help you build VMs ready to be transfered to ansible.
+        By using ansible as a library, it has access to all ansible variables. This
+        way it achieves high integration with ansible.
+        
         ## Installation
         
         Install and update using:
         ```
         pip3 install --user -U zbuilder
         ```
```

### Comparing `zbuilder-0.0.8/setup.py` & `zbuilder-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/cfg.py` & `zbuilder-0.0.9/zbuilder/cfg.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/helpers.py` & `zbuilder-0.0.9/zbuilder/helpers.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/options.py` & `zbuilder-0.0.9/zbuilder/options.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/dns/do.py` & `zbuilder-0.0.9/zbuilder/dns/do.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/dns/__init__.py` & `zbuilder-0.0.9/zbuilder/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/dns/azure.py` & `zbuilder-0.0.9/zbuilder/dns/azure.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/dns/gcp.py` & `zbuilder-0.0.9/zbuilder/dns/gcp.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/dns/ansible.py` & `zbuilder-0.0.9/zbuilder/dns/ansible.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/do.py` & `zbuilder-0.0.9/zbuilder/vm/do.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/vagrant.py` & `zbuilder-0.0.9/zbuilder/vm/vagrant.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/__init__.py` & `zbuilder-0.0.9/zbuilder/vm/__init__.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/azure.py` & `zbuilder-0.0.9/zbuilder/vm/azure.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/gcp.py` & `zbuilder-0.0.9/zbuilder/vm/gcp.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/vm/ganeti.py` & `zbuilder-0.0.9/zbuilder/vm/ganeti.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/cli.py` & `zbuilder-0.0.9/zbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder/assets/vagrant/Vagrant.j2` & `zbuilder-0.0.9/zbuilder/assets/vagrant/Vagrant.j2`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder.egg-info/PKG-INFO` & `zbuilder-0.0.9/zbuilder.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: zbuilder
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create VMs
 Home-page: https://github.com/hasiotis/zbuilder
 Author: Chasiotis Nikos
 Author-email: hasiotis@gmail.com
 License: GPLv3+
 Description: # Zbuilder: Building VMs and applying ansible playbooks
         
         [![Documentation Status](https://readthedocs.org/projects/zbuilder/badge/?version=latest)](https://zbuilder.readthedocs.io/en/latest/?badge=latest)
         
+        ZBuilder is a tool to help you build VMs ready to be transfered to ansible.
+        By using ansible as a library, it has access to all ansible variables. This
+        way it achieves high integration with ansible.
+        
         ## Installation
         
         Install and update using:
         ```
         pip3 install --user -U zbuilder
         ```
```

### Comparing `zbuilder-0.0.8/zbuilder.egg-info/requires.txt` & `zbuilder-0.0.9/zbuilder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/zbuilder.egg-info/SOURCES.txt` & `zbuilder-0.0.9/zbuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zbuilder-0.0.8/LICENSE` & `zbuilder-0.0.9/LICENSE`

 * *Files identical despite different names*

