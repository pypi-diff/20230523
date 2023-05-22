# Comparing `tmp/alicat-0.5.0.tar.gz` & `tmp/alicat-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alicat-0.5.0.tar", last modified: Tue Apr 25 18:14:39 2023, max compression
+gzip compressed data, was "alicat-0.5.1.tar", last modified: Mon May 22 22:08:39 2023, max compression
```

## Comparing `alicat-0.5.0.tar` & `alicat-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202353 alicat-0.5.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       51 2023-04-12 17:39:23.000000 alicat-0.5.0/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2023-04-12 01:08:23.000000 alicat-0.5.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-04-25 18:14:39.202454 alicat-0.5.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4894 2023-04-12 17:39:23.000000 alicat-0.5.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.201067 alicat-0.5.0/alicat/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4570 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18579 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2881 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     7932 2023-04-25 18:10:43.000000 alicat-0.5.0/alicat/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202090 alicat-0.5.0/alicat.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      332 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      126 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-04-25 18:14:39.000000 alicat-0.5.0/alicat.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      136 2023-04-25 18:14:39.202704 alicat-0.5.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1536 2023-04-25 18:10:43.000000 alicat-0.5.0/setup.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:14:39.202218 alicat-0.5.0/tests/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2142 2023-04-25 18:10:19.000000 alicat-0.5.0/tests/test_driver.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-22 22:08:39.813779 alicat-0.5.1/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       61 2023-04-25 18:35:30.000000 alicat-0.5.1/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18027 2023-04-12 01:08:23.000000 alicat-0.5.1/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-05-22 22:08:39.813895 alicat-0.5.1/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4894 2023-04-12 17:39:23.000000 alicat-0.5.1/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-22 22:08:39.811622 alicat-0.5.1/alicat/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4570 2023-05-22 22:05:57.000000 alicat-0.5.1/alicat/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18769 2023-05-22 22:07:23.000000 alicat-0.5.1/alicat/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2882 2023-04-27 18:39:33.000000 alicat-0.5.1/alicat/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-25 18:10:43.000000 alicat-0.5.1/alicat/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     7944 2023-04-28 19:46:52.000000 alicat-0.5.1/alicat/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-22 22:08:39.812686 alicat-0.5.1/alicat.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     5725 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      332 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       47 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      126 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        7 2023-05-22 22:08:39.000000 alicat-0.5.1/alicat.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      201 2023-05-22 22:08:39.814312 alicat-0.5.1/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1536 2023-05-22 22:08:19.000000 alicat-0.5.1/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-22 22:08:39.813202 alicat-0.5.1/tests/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2142 2023-05-21 14:20:12.000000 alicat-0.5.1/tests/test_driver.py
```

### Comparing `alicat-0.5.0/LICENSE` & `alicat-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alicat-0.5.0/PKG-INFO` & `alicat-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `alicat-0.5.0/README.md` & `alicat-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `alicat-0.5.0/alicat/__init__.py` & `alicat-0.5.1/alicat/__init__.py`

 * *Files identical despite different names*

### Comparing `alicat-0.5.0/alicat/driver.py` & `alicat-0.5.1/alicat/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         self.unit = unit
         self.keys = ['pressure', 'temperature', 'volumetric_flow', 'mass_flow',
                      'setpoint', 'gas']
         self.open = True
         self.firmware: Union[str, None] = None
 
-    async def __aenter__(self, *args: Any) -> Any:
+    async def __aenter__(self, *args: Any) -> 'FlowMeter':
         """Provide async enter to context manager."""
         return self
 
     async def __aexit__(self, *args: Any) -> None:
         """Provide async exit to context manager."""
         return
 
@@ -276,15 +276,15 @@
         """Close the flow meter. Call this on program termination.
 
         Also closes the serial port if no other FlowMeter object has
         a reference to the port.
         """
         if not self.open:
             return
-        self.hw.close
+        await self.hw.close()
         self.open = False
 
 
 class FlowController(FlowMeter):
     """Python driver for Alicat Flow Controllers.
 
     [Reference](http://www.alicat.com/products/mass-flow-meters-and-
@@ -297,27 +297,31 @@
     that the "Input" option is set to "Serial".
     """
 
     registers = {'mass flow': 0b00100101, 'vol flow': 0b00100100,
                  'abs pressure': 0b00100010, 'gauge pressure': 0b00100110,
                  'diff pressure': 0b00100111}
 
-    def __init__(self, address: str='/dev/ttyUSB0', unit: str='A') -> None:
+    def __init__(self, address: str='/dev/ttyUSB0', unit: str='A', **kwargs: Any) -> None:
         """Connect this driver with the appropriate USB / serial port.
 
         Args:
             address: The serial port or TCP address:port. Default '/dev/ttyUSB0'.
             unit: The Alicat-specified unit ID, A-Z. Default 'A'.
         """
-        FlowMeter.__init__(self, address, unit)
+        FlowMeter.__init__(self, address, unit, **kwargs)
         self.control_point = None
         async def _init_control_point() -> None:
             self.control_point = await self._get_control_point()
         self._init_task = asyncio.create_task(_init_control_point())
 
+    async def __aenter__(self, *args: Any) -> 'FlowController':
+        """Provide async enter to context manager."""
+        return self
+
     async def _write_and_read(self, command: str) -> Optional[str]:
         """Wrap the communicator request.
 
         (1) Ensure _init_task is called once before the first request
         (2) Call _test_controller_open() before any request
         """
         if 'R122' not in command:
@@ -468,15 +472,15 @@
             raise OSError("Could not read control point.")
         value = int(line.split('=')[-1])
         try:
             cp = next(p for p, r in self.registers.items() if value == r)
             self.control_point = cp
             return cp
         except StopIteration:
-            raise ValueError(f"Unexpected register value: {value:d}")
+            raise ValueError(f"Unexpected register value: {value:d}") from None
 
     async def _set_control_point(self, point: str) -> None:
         """Set whether to control on mass flow or pressure.
 
         Args:
             point: Either "flow" or "pressure".
         """
```

### Comparing `alicat-0.5.0/alicat/mock.py` & `alicat-0.5.1/alicat/mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .driver import FlowController as RealFlowController
 
 
 class AsyncClientMock(MagicMock):
     """Magic mock that works with async methods."""
 
-    async def __call__(self, *args, **kwargs): # type: ignore [no-untyped-def]
+    async def __call__(self, *args, **kwargs):  # type: ignore [no-untyped-def]
         """Convert regular mocks into into an async coroutine."""
         return super().__call__(*args, **kwargs)
 
 
 class FlowController(RealFlowController):
     """Mocks an Alicat MFC for offline testing."""
```

### Comparing `alicat-0.5.0/alicat/util.py` & `alicat-0.5.1/alicat/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,16 +103,16 @@
     """
 
     def __init__(self, address: str, timeout: float=1.0):
         """Communicator using a TCP/IP<=>serial gateway."""
         super().__init__(timeout)
         try:
             self.address, self.port = address.split(':')
-        except ValueError:
-            raise ValueError('address must be hostname:port')
+        except ValueError as e:
+            raise ValueError('address must be hostname:port') from e
 
     async def __aenter__(self) -> Client:
         """Provide async entrance to context manager.
 
         Contrasting synchronous access, this will connect on initialization.
         """
         await self._handle_connection()
```

### Comparing `alicat-0.5.0/alicat.egg-info/PKG-INFO` & `alicat-0.5.1/alicat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alicat
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python driver for Alicat mass flow controllers.
 Home-page: https://github.com/numat/alicat/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `alicat-0.5.0/setup.py` & `alicat-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="alicat",
-    version="0.5.0",
+    version="0.5.1",
     description="Python driver for Alicat mass flow controllers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/alicat/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     packages=["alicat"],
@@ -18,16 +18,16 @@
     install_requires=["pyserial"],
     extras_require={
             'test': [
                 'pytest>=6,<8',
                 'pytest-cov>=4,<5',
                 'pytest-asyncio==0.*',
                 'pytest-xdist==3.*',
-                'ruff==0.0.263',
-                'mypy==1.2.0',
+                'ruff==0.0.269',
+                'mypy==1.3.0',
                 'types-pyserial',
             ],
         },
     entry_points={
         "console_scripts": [("alicat = alicat:command_line")]
     },
     license="GPLv2",
```

### Comparing `alicat-0.5.0/tests/test_driver.py` & `alicat-0.5.1/tests/test_driver.py`

 * *Files identical despite different names*

