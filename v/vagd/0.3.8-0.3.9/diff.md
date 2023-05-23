# Comparing `tmp/vagd-0.3.8.tar.gz` & `tmp/vagd-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.3.8.tar", last modified: Wed May 17 09:43:09 2023, max compression
+gzip compressed data, was "vagd-0.3.9.tar", last modified: Tue May 23 10:34:26 2023, max compression
```

## Comparing `vagd-0.3.8.tar` & `vagd-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.3.8/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-17 09:43:09.142420 vagd-0.3.8/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2282 2023-03-21 08:25:45.000000 vagd-0.3.8/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-05-17 09:40:53.000000 vagd-0.3.8/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-05-17 09:43:09.142420 vagd-0.3.8/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.135753 vagd-0.3.8/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.139087 vagd-0.3.8/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.3.8/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      900 2023-04-15 11:40:48.000000 vagd-0.3.8/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.3.8/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.3.8/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.3.8/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.3.8/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      753 2023-03-20 15:06:29.000000 vagd-0.3.8/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      734 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4202 2023-03-21 09:12:24.000000 vagd-0.3.8/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10244 2023-05-17 09:35:51.000000 vagd-0.3.8/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.3.8/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.3.8/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.3.8/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.139087 vagd-0.3.8/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-05-17 09:43:09.000000 vagd-0.3.8/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-17 09:43:09.142420 vagd-0.3.8/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.3.8/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.3.9/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-23 10:34:26.716432 vagd-0.3.9/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2282 2023-03-21 08:25:45.000000 vagd-0.3.9/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-05-23 10:33:24.000000 vagd-0.3.9/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-05-23 10:34:26.716432 vagd-0.3.9/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.709766 vagd-0.3.9/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.713099 vagd-0.3.9/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.3.9/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      900 2023-04-15 11:40:48.000000 vagd-0.3.9/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.3.9/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.3.9/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.3.9/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      755 2023-05-23 10:32:45.000000 vagd-0.3.9/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      734 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4202 2023-03-21 09:12:24.000000 vagd-0.3.9/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10244 2023-05-17 09:35:51.000000 vagd-0.3.9/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.3.9/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.3.9/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.713099 vagd-0.3.9/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.3.9/test/test.py
```

### Comparing `vagd-0.3.8/LICENSE` & `vagd-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/PKG-INFO` & `vagd-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.8
+Version: 0.3.9
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.3.8/README.md` & `vagd-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/pyproject.toml` & `vagd-0.3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.3.8/src/vagd/box.py` & `vagd-0.3.9/src/vagd/box.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/gdb/__init__.pyi` & `vagd-0.3.9/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/gdb/events.pyi` & `vagd-0.3.9/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/gdb/printing.pyi` & `vagd-0.3.9/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/gdb/types.pyi` & `vagd-0.3.9/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/gdb/xmethod.pyi` & `vagd-0.3.9/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/helper.py` & `vagd-0.3.9/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/template.txt` & `vagd-0.3.9/src/vagd/template.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,14 @@
     if args.REMOTE:
         context.log_level = 'debug'
         return remote(IP, PORT)
 
     if not vm:
         vm = Vagd(exe.path, vbox=Box.UBUNTU_FOCAL64, ex=True, fast=True)
         # vm = Qegd(exe.path, img=Box.CLOUDIMAGE_FOCAL, user='ubuntu', ex=True, fast=True)
-        # vm = Dogd(exe.path, img=Box.DOCKER_FOCAL, ex=True, fast=True)
+        # vm = Dogd(exe.path, image=Box.DOCKER_FOCAL, ex=True, fast=True)
     return vm.start(argv=ARGS, env=ENV, gdbscript=GDB, **kw)
 
 
 t = get_target()
 
 t.interactive()
```

### Comparing `vagd-0.3.8/src/vagd/templates.py` & `vagd-0.3.9/src/vagd/templates.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/virts/dogd.py` & `vagd-0.3.9/src/vagd/virts/dogd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/virts/pwngd.py` & `vagd-0.3.9/src/vagd/virts/pwngd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/virts/qegd.py` & `vagd-0.3.9/src/vagd/virts/qegd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/virts/shgd.py` & `vagd-0.3.9/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/virts/vagd.py` & `vagd-0.3.9/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd/wrapper.py` & `vagd-0.3.9/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/src/vagd.egg-info/PKG-INFO` & `vagd-0.3.9/src/vagd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.8
+Version: 0.3.9
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vagd-0.3.8/src/vagd.egg-info/SOURCES.txt` & `vagd-0.3.9/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vagd-0.3.8/test/test.py` & `vagd-0.3.9/test/test.py`

 * *Files identical despite different names*

