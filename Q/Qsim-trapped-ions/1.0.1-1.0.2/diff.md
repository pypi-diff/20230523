# Comparing `tmp/Qsim_trapped_ions-1.0.1.tar.gz` & `tmp/Qsim_trapped_ions-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Qsim_trapped_ions-1.0.1.tar", last modified: Tue May 23 09:30:49 2023, max compression
+gzip compressed data, was "Qsim_trapped_ions-1.0.2.tar", last modified: Tue May 23 09:39:05 2023, max compression
```

## Comparing `Qsim_trapped_ions-1.0.1.tar` & `Qsim_trapped_ions-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.889487 Qsim_trapped_ions-1.0.1/
--rw-rw-rw-   0        0        0      246 2023-05-23 09:30:49.889487 Qsim_trapped_ions-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.834761 Qsim_trapped_ions-1.0.1/Qsim/
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.843782 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.848190 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/eigendiagram/
--rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/eigendiagram/exci_diagram.py
--rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/eigendiagram/init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.853763 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/__init__.py
--rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/pure_spin.py
--rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/spin_phonon.py
--rw-rw-rw-   0        0        0    30482 2023-05-23 08:53:03.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ion_system.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.858472 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/ising_c.py
--rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/ising_ps.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.875752 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/__init__.py
--rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
--rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/anharmonic_transfer.py
--rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/chaos.py
--rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/elec_transfer.py
--rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/exci_operators.py
--rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/exci_transfer.py
--rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/multi_core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.880360 Qsim_trapped_ions-1.0.1/Qsim/operator/
--rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.1/Qsim/operator/__init__.py
--rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.1/Qsim/operator/phonon.py
--rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.1/Qsim/operator/spin.py
-drwxrwxrwx   0        0        0        0 2023-05-23 09:30:49.887457 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/
--rw-rw-rw-   0        0        0      246 2023-05-23 09:30:49.000000 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      986 2023-05-23 09:30:49.000000 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 09:30:49.000000 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-23 09:30:49.000000 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-23 09:30:49.000000 Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4035 2023-05-23 09:08:47.000000 Qsim_trapped_ions-1.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-23 09:30:49.889487 Qsim_trapped_ions-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1189 2023-05-23 09:30:40.000000 Qsim_trapped_ions-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.826034 Qsim_trapped_ions-1.0.2/
+-rw-rw-rw-   0        0        0      246 2023-05-23 09:39:05.826034 Qsim_trapped_ions-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.784133 Qsim_trapped_ions-1.0.2/Qsim/
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.790135 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.793136 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/eigendiagram/
+-rw-rw-rw-   0        0        0     7825 2023-04-22 20:45:12.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/eigendiagram/exci_diagram.py
+-rw-rw-rw-   0        0        0      111 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/eigendiagram/init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.797137 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/__init__.py
+-rw-rw-rw-   0        0        0     2853 2023-03-27 05:10:36.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/pure_spin.py
+-rw-rw-rw-   0        0        0     7440 2023-02-19 21:26:44.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/spin_phonon.py
+-rw-rw-rw-   0        0        0    30482 2023-05-23 08:53:03.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ion_system.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.801525 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/ising_c.py
+-rw-rw-rw-   0        0        0     4045 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/ising_ps.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.812031 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/__init__.py
+-rw-rw-rw-   0        0        0    15712 2023-03-07 21:30:48.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py
+-rw-rw-rw-   0        0        0    15800 2023-03-08 00:56:56.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/anharmonic_transfer.py
+-rw-rw-rw-   0        0        0     3037 2023-02-20 05:11:39.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/chaos.py
+-rw-rw-rw-   0        0        0     3063 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/elec_transfer.py
+-rw-rw-rw-   0        0        0    13991 2023-03-05 19:12:10.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/exci_operators.py
+-rw-rw-rw-   0        0        0     4323 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/exci_transfer.py
+-rw-rw-rw-   0        0        0     5700 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/multi_core.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.817032 Qsim_trapped_ions-1.0.2/Qsim/operator/
+-rw-rw-rw-   0        0        0      131 2023-01-25 04:42:42.000000 Qsim_trapped_ions-1.0.2/Qsim/operator/__init__.py
+-rw-rw-rw-   0        0        0     7121 2023-03-05 17:06:10.000000 Qsim_trapped_ions-1.0.2/Qsim/operator/phonon.py
+-rw-rw-rw-   0        0        0     6429 2023-02-27 23:34:30.000000 Qsim_trapped_ions-1.0.2/Qsim/operator/spin.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:39:05.824033 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/
+-rw-rw-rw-   0        0        0      246 2023-05-23 09:39:05.000000 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2023-05-23 09:39:05.000000 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:39:05.000000 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 09:39:05.000000 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-23 09:39:05.000000 Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4035 2023-05-23 09:08:47.000000 Qsim_trapped_ions-1.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:39:05.826034 Qsim_trapped_ions-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-05-23 09:38:53.000000 Qsim_trapped_ions-1.0.2/setup.py
```

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/eigendiagram/exci_diagram.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/eigendiagram/exci_diagram.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/pure_spin.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/pure_spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/interaction/spin_phonon.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/interaction/spin_phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ion_system.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ion_system.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/ising_c.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/ising_c.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/ising/ising_ps.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/ising/ising_ps.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/anharmonic_transfer - 副本.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/anharmonic_transfer.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/anharmonic_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/chaos.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/chaos.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/elec_transfer.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/elec_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/exci_operators.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/exci_operators.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/exci_transfer.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/exci_transfer.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/ion_chain/transfer/multi_core.py` & `Qsim_trapped_ions-1.0.2/Qsim/ion_chain/transfer/multi_core.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/operator/phonon.py` & `Qsim_trapped_ions-1.0.2/Qsim/operator/phonon.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim/operator/spin.py` & `Qsim_trapped_ions-1.0.2/Qsim/operator/spin.py`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/Qsim_trapped_ions.egg-info/SOURCES.txt` & `Qsim_trapped_ions-1.0.2/Qsim_trapped_ions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/README.rst` & `Qsim_trapped_ions-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Qsim_trapped_ions-1.0.1/setup.py` & `Qsim_trapped_ions-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 @author: zhumj
 """
 
 from setuptools import setup
 
 def readme_file():
-    with open('README.rst') as rf:
+    with open("C:\\Users\\zhumj\\.ipython\README.rst") as rf:
         return rf.read()
     
 setup(name = 'Qsim_trapped_ions', 
-      version = '1.0.1', 
+      version = '1.0.2', 
       description = 'Numerical simulation of trapped ion quantum dynamics',
       package_dir = {
             'Qsim': 'Qsim',
             'Qsim.ion_chain': 'Qsim/ion_chain',
             'Qsim.operator': 'Qsim/operator',
             'Qsim.ion_chain.eigendiagram': 'Qsim/ion_chain/eigendiagram',
             'Qsim.ion_chain.interaction': 'Qsim/ion_chain/interaction',
```

