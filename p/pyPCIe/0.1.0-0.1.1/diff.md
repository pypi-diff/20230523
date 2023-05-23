# Comparing `tmp/pyPCIe-0.1.0.tar.gz` & `tmp/pyPCIe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPCIe-0.1.0.tar", last modified: Fri Mar 11 16:17:37 2022, max compression
+gzip compressed data, was "pyPCIe-0.1.1.tar", last modified: Tue May 23 14:37:23 2023, max compression
```

## Comparing `pyPCIe-0.1.0.tar` & `pyPCIe-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-03-11 16:17:37.046409 pyPCIe-0.1.0/
--rw-r--r--   0 user      (1000) user      (1000)     1068 2021-09-19 12:44:49.000000 pyPCIe-0.1.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1271 2022-03-11 16:17:37.046409 pyPCIe-0.1.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      736 2022-03-11 16:13:08.000000 pyPCIe-0.1.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-03-11 16:17:37.045409 pyPCIe-0.1.0/pyPCIe.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1271 2022-03-11 16:17:36.000000 pyPCIe-0.1.0/pyPCIe.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      196 2022-03-11 16:17:37.000000 pyPCIe-0.1.0/pyPCIe.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2022-03-11 16:17:36.000000 pyPCIe-0.1.0/pyPCIe.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2022-03-11 16:17:36.000000 pyPCIe-0.1.0/pyPCIe.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-03-11 16:17:37.046409 pyPCIe-0.1.0/pypcie/
--rw-r--r--   0 user      (1000) user      (1000)       48 2021-09-19 14:33:57.000000 pyPCIe-0.1.0/pypcie/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     2272 2021-10-19 18:11:57.000000 pyPCIe-0.1.0/pypcie/bar.py
--rw-r--r--   0 user      (1000) user      (1000)     2373 2021-09-19 15:33:37.000000 pyPCIe-0.1.0/pypcie/device.py
--rw-r--r--   0 user      (1000) user      (1000)       38 2022-03-11 16:17:37.046409 pyPCIe-0.1.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      822 2022-03-11 16:16:36.000000 pyPCIe-0.1.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-23 14:37:23.854783 pyPCIe-0.1.1/
+-rw-r--r--   0 user      (1000) user      (1000)     1068 2021-09-19 12:44:49.000000 pyPCIe-0.1.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     1237 2023-05-23 14:37:23.854783 pyPCIe-0.1.1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      739 2022-03-11 16:30:19.000000 pyPCIe-0.1.1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-23 14:37:23.851783 pyPCIe-0.1.1/pyPCIe.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1237 2023-05-23 14:37:23.000000 pyPCIe-0.1.1/pyPCIe.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      196 2023-05-23 14:37:23.000000 pyPCIe-0.1.1/pyPCIe.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-23 14:37:23.000000 pyPCIe-0.1.1/pyPCIe.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-23 14:37:23.000000 pyPCIe-0.1.1/pyPCIe.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-23 14:37:23.853783 pyPCIe-0.1.1/pypcie/
+-rw-r--r--   0 user      (1000) user      (1000)       48 2021-09-19 14:33:57.000000 pyPCIe-0.1.1/pypcie/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2293 2023-05-20 20:34:57.000000 pyPCIe-0.1.1/pypcie/bar.py
+-rw-r--r--   0 user      (1000) user      (1000)     2373 2021-09-19 15:33:37.000000 pyPCIe-0.1.1/pypcie/device.py
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-23 14:37:23.854783 pyPCIe-0.1.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      822 2023-05-23 14:25:34.000000 pyPCIe-0.1.1/setup.py
```

### Comparing `pyPCIe-0.1.0/LICENSE` & `pyPCIe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPCIe-0.1.0/PKG-INFO` & `pyPCIe-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: pyPCIe
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple Python module to access PCIe devices
 Home-page: https://github.com/heikoengel/pyPCIe
 Author: Heiko Engel
 Author-email: <heikoengel@users.noreply.github.com>
-License: UNKNOWN
 Keywords: python,pcie
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyPCIe: Simple Python Module to access PCIe Endpoint BARs
 
-PyCIe provides a quick way to read/write registers in PCIe Base
+pyPCIe provides a quick way to read/write registers in PCIe Base
 Address Register (BAR) regions.
 
-PyCIe `mmap`s PCIe device BARs via the `resourceX` files in
+pyPCIe `mmap`s PCIe device BARs via the `resourceX` files in
 `/sys/bus/pci/devices/[bus_id]` for read/write and provides functions
 for 32 bit read/write requests.
 
 *Note: the `resourceX` files in sysfs are typically only accessible as
-root. The python scripts using PyCIe might need to be run as root.*
+root. The python scripts using pyPCIe might need to be run as root.*
 
 ## Example
 
 ```python
 from pypcie import Device
 
 # Bind to PCI device at "0000:03:00.0"
@@ -39,9 +37,7 @@
 
 # write 0xdeadbeef to BAR 0, offset 0x1000
 bar.write(0x1000, 0xdeadbeef)
 
 # read BAR 0, offset 0x1004
 ret = bar.read(0x1004)
 ```
-
-
```

### Comparing `pyPCIe-0.1.0/README.md` & `pyPCIe-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyPCIe: Simple Python Module to access PCIe Endpoint BARs
 
-PyCIe provides a quick way to read/write registers in PCIe Base
+pyPCIe provides a quick way to read/write registers in PCIe Base
 Address Register (BAR) regions.
 
-PyCIe `mmap`s PCIe device BARs via the `resourceX` files in
+pyPCIe `mmap`s PCIe device BARs via the `resourceX` files in
 `/sys/bus/pci/devices/[bus_id]` for read/write and provides functions
 for 32 bit read/write requests.
 
 *Note: the `resourceX` files in sysfs are typically only accessible as
-root. The python scripts using PyCIe might need to be run as root.*
+root. The python scripts using pyPCIe might need to be run as root.*
 
 ## Example
 
 ```python
 from pypcie import Device
 
 # Bind to PCI device at "0000:03:00.0"
```

### Comparing `pyPCIe-0.1.0/pyPCIe.egg-info/PKG-INFO` & `pyPCIe-0.1.1/pyPCIe.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: pyPCIe
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple Python module to access PCIe devices
 Home-page: https://github.com/heikoengel/pyPCIe
 Author: Heiko Engel
 Author-email: <heikoengel@users.noreply.github.com>
-License: UNKNOWN
 Keywords: python,pcie
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyPCIe: Simple Python Module to access PCIe Endpoint BARs
 
-PyCIe provides a quick way to read/write registers in PCIe Base
+pyPCIe provides a quick way to read/write registers in PCIe Base
 Address Register (BAR) regions.
 
-PyCIe `mmap`s PCIe device BARs via the `resourceX` files in
+pyPCIe `mmap`s PCIe device BARs via the `resourceX` files in
 `/sys/bus/pci/devices/[bus_id]` for read/write and provides functions
 for 32 bit read/write requests.
 
 *Note: the `resourceX` files in sysfs are typically only accessible as
-root. The python scripts using PyCIe might need to be run as root.*
+root. The python scripts using pyPCIe might need to be run as root.*
 
 ## Example
 
 ```python
 from pypcie import Device
 
 # Bind to PCI device at "0000:03:00.0"
@@ -39,9 +37,7 @@
 
 # write 0xdeadbeef to BAR 0, offset 0x1000
 bar.write(0x1000, 0xdeadbeef)
 
 # read BAR 0, offset 0x1004
 ret = bar.read(0x1004)
 ```
-
-
```

### Comparing `pyPCIe-0.1.0/pypcie/bar.py` & `pyPCIe-0.1.1/pypcie/bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     """
 
     def __init__(self, filename: str):
         self.__map = None
         self.__stat = os.stat(filename)
         fd = os.open(filename, os.O_RDWR)
         self.__map = mmap(fd, 0, prot=PROT_READ | PROT_WRITE)
+        os.close(fd)
 
     def __del__(self):
         if self.__map is not None:
             self.__map.close()
 
     def __check_offset(self, offset: int):
         """ Check if the given offset is properly DW-aligned and the access
```

### Comparing `pyPCIe-0.1.0/pypcie/device.py` & `pyPCIe-0.1.1/pypcie/device.py`

 * *Files identical despite different names*

### Comparing `pyPCIe-0.1.0/setup.py` & `pyPCIe-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Simple Python module to access PCIe devices'
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Setting up
 setup(
     name="pyPCIe",
```

