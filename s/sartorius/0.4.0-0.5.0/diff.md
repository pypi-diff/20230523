# Comparing `tmp/sartorius-0.4.0.tar.gz` & `tmp/sartorius-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sartorius-0.4.0.tar", last modified: Wed Apr 26 21:17:17 2023, max compression
+gzip compressed data, was "sartorius-0.5.0.tar", last modified: Tue May 23 21:12:27 2023, max compression
```

## Comparing `sartorius-0.4.0.tar` & `sartorius-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.524237 sartorius-0.4.0/
--rw-r--r--   0 a.ruddick   (502) staff       (20)       74 2023-04-25 18:54:02.000000 sartorius-0.4.0/.gitignore
--rw-r--r--   0 a.ruddick   (502) staff       (20)    18092 2021-07-02 17:04:12.000000 sartorius-0.4.0/LICENSE
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-04-26 21:17:17.524309 sartorius-0.4.0/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)     2216 2021-07-02 17:04:12.000000 sartorius-0.4.0/README.md
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.523247 sartorius-0.4.0/sartorius/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1375 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/__init__.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3504 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/driver.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1282 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/mock.py
--rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/py.typed
--rw-r--r--   0 a.ruddick   (502) staff       (20)     4022 2023-04-26 21:07:55.000000 sartorius-0.4.0/sartorius/util.py
-drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:17:17.524127 sartorius-0.4.0/sartorius.egg-info/
--rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/PKG-INFO
--rw-r--r--   0 a.ruddick   (502) staff       (20)      344 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/SOURCES.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/dependency_links.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       53 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/entry_points.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       84 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/requires.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)       10 2023-04-26 21:17:17.000000 sartorius-0.4.0/sartorius.egg-info/top_level.txt
--rw-r--r--   0 a.ruddick   (502) staff       (20)      283 2023-04-26 21:17:17.524572 sartorius-0.4.0/setup.cfg
--rw-r--r--   0 a.ruddick   (502) staff       (20)     1370 2023-04-26 21:17:07.000000 sartorius-0.4.0/setup.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-23 21:12:27.709521 sartorius-0.5.0/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       74 2023-04-25 18:54:02.000000 sartorius-0.5.0/.gitignore
+-rw-r--r--   0 a.ruddick   (502) staff       (20)    18092 2021-07-02 17:04:12.000000 sartorius-0.5.0/LICENSE
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-05-23 21:12:27.709600 sartorius-0.5.0/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     2216 2021-07-02 17:04:12.000000 sartorius-0.5.0/README.md
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-23 21:12:27.708216 sartorius-0.5.0/sartorius/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1247 2023-05-23 21:11:11.000000 sartorius-0.5.0/sartorius/__init__.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     4507 2023-05-23 19:34:21.000000 sartorius-0.5.0/sartorius/driver.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1447 2023-05-23 19:36:04.000000 sartorius-0.5.0/sartorius/mock.py
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        0 2023-04-26 21:07:55.000000 sartorius-0.5.0/sartorius/py.typed
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     6139 2023-05-23 19:18:39.000000 sartorius-0.5.0/sartorius/util.py
+drwxr-xr-x   0 a.ruddick   (502) staff       (20)        0 2023-05-23 21:12:27.709378 sartorius-0.5.0/sartorius.egg-info/
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     3011 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/PKG-INFO
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      344 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/SOURCES.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)        1 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/dependency_links.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       53 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/entry_points.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      108 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/requires.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)       10 2023-05-23 21:12:27.000000 sartorius-0.5.0/sartorius.egg-info/top_level.txt
+-rw-r--r--   0 a.ruddick   (502) staff       (20)      309 2023-05-23 21:12:27.709906 sartorius-0.5.0/setup.cfg
+-rw-r--r--   0 a.ruddick   (502) staff       (20)     1437 2023-05-23 21:11:25.000000 sartorius-0.5.0/setup.py
```

### Comparing `sartorius-0.4.0/LICENSE` & `sartorius-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sartorius-0.4.0/PKG-INFO` & `sartorius-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sartorius
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python driver for Sartorius and Minebea Intec scales.
 Home-page: https://github.com/numat/sartorius/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sartorius-0.4.0/README.md` & `sartorius-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sartorius-0.4.0/sartorius/__init__.py` & `sartorius-0.5.0/sartorius/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 def command_line(args: Any = None) -> None:
     """Command line tool exposed through package install."""
     import argparse
     import asyncio
     import json
 
     parser = argparse.ArgumentParser(description="Read scale status.")
-    parser.add_argument('address', help="The IP address of the scale.")
-    parser.add_argument('-p', '--port', help="The port of the scale (default 49155)",
-                        type=int, default=49155)
+    parser.add_argument('address', help="The serial or IP address of the scale.")
     parser.add_argument('-n', '--no-info', action='store_true', help="Exclude "
                         "scale information. Reduces communication overhead.")
     parser.add_argument('-z', '--zero', action='store_true', help="Tares and "
                         "zeroes the scale.")
     args = parser.parse_args(args)
 
     async def get() -> None:
-        async with Scale(args.address, args.port) as scale:
+        async with Scale(address=args.address) as scale:
             if args.zero:
                 await scale.zero()
             d = await scale.get()
             if not args.no_info and d.get('on', True):
                 d['info'] = await scale.get_info()
             print(json.dumps(d, indent=4))
     asyncio.run(get())
```

### Comparing `sartorius-0.4.0/sartorius/driver.py` & `sartorius-0.5.0/sartorius/driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,69 @@
 """
 A Python driver for Sartorius and Minebea Intec ethernet scales.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2019 NuMat Technologies
 """
 import logging
+from typing import Any
 
-from sartorius.util import TcpClient
+from sartorius.util import Client, SerialClient, TcpClient
 
 logger = logging.getLogger('sartorius')
 
 
-class Scale(TcpClient):
+class Scale:
     """Driver for Sartorius and Minebea Intec ethernet scales.
 
     This implements a version of the Scale Manufacturers Association
     standardized communications protocol.
     """
 
-    def __init__(self, ip: str, port: int = 49155) -> None:
-        """Set up connection parameters, IP address and port."""
+    def __init__(self, address: str = '', ip: str = '', port: int = 49155,
+                 **kwargs: Any) -> None:
+        """Set up connection parameters, IP address and port.
+
+        Accepts either an address string (TCP or serial), or combination
+        of port & ip (TCP, backwards compatible)
+        """
+        if ip != '':
+            if ":" in ip:
+                port = int(ip.split(":")[1])
+                ip = ip.split(':')[0]
+                address = ip
+            address = f'{ip}:{port}'
         self.units: str = ""
-        if ":" in ip:
-            port = int(ip.split(":")[1])
-            ip = ip.split(':')[0]
-        super().__init__(ip, port)
+        if address.startswith('/dev') or address.startswith('COM'):  # serial
+            self.hw: Client = SerialClient(address=address, **kwargs)
+        else:
+            if ':' not in address:
+                address = f'{address}:{port}'
+            self.hw = TcpClient(address=address, **kwargs)
+
+    async def __aenter__(self, *args: Any) -> 'Scale':
+        """Provide async enter to context manager."""
+        return self
+
+    async def __aexit__(self, *args: Any) -> None:
+        """Provide async exit to context manager."""
+        return
 
     async def get(self) -> dict:
         """Get scale reading."""
-        response = await self._write_and_read('\x1bP')
+        response = await self.hw._write_and_read('\x1bP')
         if not response:
             raise OSError("Unable to get reading from scale.")
         return self._parse(response)
 
     async def get_info(self) -> dict:
         """Get scale model, serial, and software version numbers."""
-        model = await self._write_and_read('\x1bx1_')
-        serial = await self._write_and_read('\x1bx2_')
-        software = await self._write_and_read('\x1bx3_')
+        model = await self.hw._write_and_read('\x1bx1_')
+        serial = await self.hw._write_and_read('\x1bx2_')
+        software = await self.hw._write_and_read('\x1bx3_')
         if not (model and serial and software):
             raise OSError("Unable to get information from scale.")
         response = {
             'model': model.strip(),
             'serial': serial.strip(),
             'software': software.strip(),
         }
@@ -49,15 +71,15 @@
             if (' + ' in item or ' kg' in item):
                 logger.error(f"Received malformed data: {response}")
                 return {}
         return response
 
     async def zero(self) -> None:
         """Tare and zero the scale."""
-        await self._write_and_read('\x1bT')
+        await self.hw._write_and_read('\x1bT')
 
     def _parse(self, response: str) -> dict:
         """Parse a scale response.
 
         Scale weight is returned according to the SMA communication standard:
             K K K K K K + * A A A A A A A A * E E E CR LF
         K: ID code character
@@ -82,22 +104,27 @@
             logger.error(f"Received malformed data: {response}")
             return {'on': False}
         id = response[:6].strip()
         if id == 'Stat':
             error = response[9:14].strip()
             logger.warning(f'Could not read: {error}')
             return {'on': False}
-        elif id != 'N':
-            raise ValueError("This driver only supports net weight.")
+        elif id == 'N':
+            measurement = 'net'
+        elif id == 'G':
+            measurement = 'gross'
+        else:
+            raise ValueError("This driver only supports net/gross weight.")
         mass = float(response[6:16].replace(' ', ''))
         units = response[17:20].strip()
         if units:
             self.units = units
             stable = True
         else:
             units = self.units
             stable = False
         return {
             'mass': mass,
             'units': units,
             'stable': stable,
+            'measurement': measurement,
         }
```

### Comparing `sartorius-0.4.0/sartorius/util.py` & `sartorius-0.5.0/sartorius/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,72 +1,38 @@
-"""Base functionality for async TCP communication.
+"""Base functionality for async communication.
 
 Distributed under the GNU General Public License v2
 Copyright (C) 2019 NuMat Technologies
 """
 
 import asyncio
 import logging
-from typing import Any, Dict, Optional
+from abc import ABC, abstractmethod
+from typing import Any, Dict, Optional, Union
 
-logger = logging.getLogger('sartorius')
+import serial
 
+logger = logging.getLogger('sartorius')
 
-class TcpClient():
-    """A generic reconnecting asyncio TCP client.
 
-    This base functionality can be used by any industrial control device
-    communicating over TCP.
-    """
+class Client(ABC):
+    """Base class for a generic reconnecting client."""
 
-    def __init__(self, ip: str, port: int, eol: str = '\r\n'):
-        """Set connection parameters.
-
-        Connection is handled asynchronously, either using `async with` or
-        behind the scenes on the first `await` call.
-        """
-        self.ip = ip
-        self.port = port
-        self.eol = eol.encode()
+    def __init__(self, timeout: float) -> None:
+        """Initialize the client."""
+        self.eol = b'\r\n'
         self.open = False
-        self.reconnecting = False
-        self.timeouts = 0
+        self.timeout = timeout
         self.max_timeouts = 10
-        self.connection: Dict[str, Any] = {}
         self.lock: Optional[asyncio.Lock] = None
 
-    async def __aenter__(self) -> Any:
-        """Provide async entrance to context manager.
-
-        Contrasting synchronous access, this will connect on initialization.
-        """
-        await self._handle_connection()
-        return self
-
-    def __exit__(self, *args: Any) -> None:
-        """Provide exit to context manager."""
-        self.close()
-
-    async def __aexit__(self, *args: Any) -> None:
-        """Provide async exit to context manager."""
-        self.close()
-
     def close(self) -> None:
-        """Close the TCP connection."""
-        if self.open:
-            self.connection['writer'].close()
+        """Close the connection."""
         self.open = False
 
-    async def _connect(self) -> None:
-        """Asynchronously open a TCP connection with the server."""
-        self.close()
-        reader, writer = await asyncio.open_connection(self.ip, self.port)
-        self.connection = {'reader': reader, 'writer': writer}
-        self.open = True
-
     async def _write_and_read(self, command: str) -> Optional[str]:
         """Write a command and read a response.
 
         As industrial devices are commonly unplugged, this has been expanded to
         handle recovering from disconnects.  A lock is used to queue multiple requests.
         """
         if not self.lock:
@@ -80,34 +46,123 @@
                 except asyncio.exceptions.IncompleteReadError:
                     logger.error('IncompleteReadError.  Are there multiple connections?')
                     return None
             else:
                 response = None
         return response
 
+    @abstractmethod
+    async def _handle_connection(self) -> None:
+        """Automatically maintain the connection."""
+        ...
+
+    @abstractmethod
+    async def _handle_communication(self, command: str) -> Optional[str]:
+        """Manage communication, including timeouts and logging."""
+        ...
+
+
+class SerialClient(Client):
+    """Client using a directly-connected RS232 serial device."""
+
+    def __init__(self, address: str, baudrate: int = 9600, timeout: float = .15,
+                 bytesize: int = serial.EIGHTBITS,
+                 stopbits: Union[float, int] = serial.STOPBITS_ONE,
+                 parity: str = serial.PARITY_ODD):
+        """Initialize serial port."""
+        super().__init__(timeout)
+        self.address = address
+        assert type(self.address) == str
+        self.serial_details = {'baudrate': baudrate,
+                               'bytesize': bytesize,
+                               'stopbits': stopbits,
+                               'parity': parity,
+                               'timeout': timeout}
+        self.ser = serial.Serial(self.address, **self.serial_details)  # type: ignore [arg-type]
+
+    def close(self) -> None:
+        """Close the serial connection."""
+        if self.ser and self.ser.is_open:
+            self.ser.close()
+
+    async def _handle_connection(self) -> None:
+        """Handle the serial connection status."""
+        self.open = True
+
+    async def _handle_communication(self, command: str) -> Optional[str]:
+        """Manage communication, including timeouts and logging."""
+        try:
+            self.ser.write(command.encode())
+            # don't strip() to keep the line length == 22
+            response = self.ser.readline().decode()
+            self.timeouts = 0
+        except (serial.SerialTimeoutException, serial.SerialException):
+            self.timeouts += 1
+            if self.timeouts == self.max_timeouts:
+                print(f'Reading from {self.address} timed out {self.timeouts} times.')
+                self.close()
+            response = None
+        return response
+
+
+class TcpClient(Client):
+    """A generic reconnecting asyncio TCP client.
+
+    This base functionality can be used by any industrial control device
+    communicating over TCP.
+    """
+
+    def __init__(self, address: str, timeout: float = 1.0):
+        """Set connection parameters.
+
+        Connection is handled asynchronously, either using `async with` or
+        behind the scenes on the first `await` call.
+        """
+        super().__init__(timeout)
+        try:
+            self.address, self.port = address.split(':')
+        except ValueError as e:
+            raise ValueError('address must be hostname:port') from e
+        self.reconnecting = False
+        self.timeouts = 0
+        self.connection: Dict[str, Any] = {}
+
+    def close(self) -> None:
+        """Close the TCP connection."""
+        if self.open:
+            self.connection['writer'].close()
+        self.open = False
+
+    async def _connect(self) -> None:
+        """Asynchronously open a TCP connection with the server."""
+        self.close()
+        reader, writer = await asyncio.open_connection(self.address, self.port)
+        self.connection = {'reader': reader, 'writer': writer}
+        self.open = True
+
     async def _handle_connection(self) -> None:
         """Automatically maintain TCP connection."""
         try:
             if not self.open:
                 await asyncio.wait_for(self._connect(), timeout=0.5)
             self.reconnecting = False
         except (asyncio.TimeoutError, OSError):
             if not self.reconnecting:
-                logger.error(f'Connecting to {self.ip} timed out.')
+                logger.error(f'Connecting to {self.address} timed out.')
             self.reconnecting = True
 
     async def _handle_communication(self, command: str) -> Optional[str]:
         """Manage communication, including timeouts and logging."""
         try:
             self.connection['writer'].write(command.encode() + self.eol)
             future = self.connection['reader'].readuntil(self.eol)
             line = await asyncio.wait_for(future, timeout=0.5)
             result = line.decode()
             self.timeouts = 0
         except (asyncio.TimeoutError, TypeError, OSError):
             self.timeouts += 1
             if self.timeouts == self.max_timeouts:
-                logger.error(f'Reading from {self.ip} timed out '
+                logger.error(f'Reading from {self.address} timed out '
                              f'{self.timeouts} times.')
                 self.close()
             result = None
         return result
```

### Comparing `sartorius-0.4.0/sartorius.egg-info/PKG-INFO` & `sartorius-0.5.0/sartorius.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sartorius
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python driver for Sartorius and Minebea Intec scales.
 Home-page: https://github.com/numat/sartorius/
 Author: Patrick Fuller
 Author-email: pat@numat-tech.com
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sartorius-0.4.0/setup.py` & `sartorius-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 from setuptools import setup
 
 with open('README.md') as in_file:
     long_description = in_file.read()
 
 setup(
     name="sartorius",
-    version="0.4.0",
+    version="0.5.0",
     description="Python driver for Sartorius and Minebea Intec scales.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/numat/sartorius/",
     author="Patrick Fuller",
     author_email="pat@numat-tech.com",
     packages=['sartorius'],
     package_data={'sartorius': ['py.typed']},
+    install_requires=['pyserial'],
     extras_require={
+
         'test': [
-            'mypy==1.2.0',
+            'mypy==1.3.0',
             'pytest>=6,<8',
             'pytest-cov>=4,<5',
             'pytest-asyncio==0.*',
-            'ruff==0.0.263'
+            'ruff==0.0.269',
+            'types-pyserial',
         ]
     },
     entry_points={
         'console_scripts': [('sartorius = sartorius:command_line')]
     },
     license='GPLv2',
     classifiers=[
```

