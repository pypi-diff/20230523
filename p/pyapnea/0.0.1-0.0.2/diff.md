# Comparing `tmp/pyapnea-0.0.1.tar.gz` & `tmp/pyapnea-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapnea-0.0.1.tar", last modified: Tue Apr 18 13:19:04 2023, max compression
+gzip compressed data, was "pyapnea-0.0.2.tar", last modified: Tue May 23 15:49:00 2023, max compression
```

## Comparing `pyapnea-0.0.1.tar` & `pyapnea-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 13:19:04.666492 pyapnea-0.0.1/
--rw-rw-r--   0 julien    (1000) julien    (1000)    35149 2023-03-23 12:56:37.000000 pyapnea-0.0.1/LICENSE
--rw-rw-r--   0 julien    (1000) julien    (1000)      742 2023-04-18 13:19:04.666492 pyapnea-0.0.1/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)      181 2023-04-17 18:05:47.000000 pyapnea-0.0.1/README.md
--rw-rw-r--   0 julien    (1000) julien    (1000)      651 2023-04-18 13:15:13.000000 pyapnea-0.0.1/pyproject.toml
--rw-rw-r--   0 julien    (1000) julien    (1000)       38 2023-04-18 13:19:04.666492 pyapnea-0.0.1/setup.cfg
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 13:19:04.654492 pyapnea-0.0.1/src/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-03-24 12:46:53.000000 pyapnea-0.0.1/src/__init__.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 13:19:04.654492 pyapnea-0.0.1/src/pyapnea/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-03-23 12:56:37.000000 pyapnea-0.0.1/src/pyapnea/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1532 2023-04-17 18:27:14.000000 pyapnea-0.0.1/src/pyapnea/base_functions.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 13:19:04.662492 pyapnea-0.0.1/src/pyapnea/oscar/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-03-23 12:56:37.000000 pyapnea-0.0.1/src/pyapnea/oscar/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1442 2023-04-17 18:08:33.000000 pyapnea-0.0.1/src/pyapnea/oscar/data_structure.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    16682 2023-04-17 18:23:16.000000 pyapnea-0.0.1/src/pyapnea/oscar/oscar_constants.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2308 2023-04-17 18:12:08.000000 pyapnea-0.0.1/src/pyapnea/oscar/oscar_getter.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     6823 2023-04-17 18:27:14.000000 pyapnea-0.0.1/src/pyapnea/oscar/oscar_loader.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2023-04-18 13:19:04.654492 pyapnea-0.0.1/src/pyapnea.egg-info/
--rw-rw-r--   0 julien    (1000) julien    (1000)      742 2023-04-18 13:19:04.000000 pyapnea-0.0.1/src/pyapnea.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)      413 2023-04-18 13:19:04.000000 pyapnea-0.0.1/src/pyapnea.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)        1 2023-04-18 13:19:04.000000 pyapnea-0.0.1/src/pyapnea.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       17 2023-04-18 13:19:04.000000 pyapnea-0.0.1/src/pyapnea.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-23 15:48:40.000000 pyapnea-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 15:49:00.854722 pyapnea-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 15:48:40.000000 pyapnea-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 15:48:40.000000 pyapnea-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 15:49:00.854722 pyapnea-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/base_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea/oscar/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-05-23 15:48:40.000000 pyapnea-0.0.2/src/pyapnea/oscar/oscar_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:49:00.854722 pyapnea-0.0.2/src/pyapnea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 15:49:00.000000 pyapnea-0.0.2/src/pyapnea.egg-info/top_level.txt
```

### Comparing `pyapnea-0.0.1/LICENSE` & `pyapnea-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapnea-0.0.1/PKG-INFO` & `pyapnea-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyapnea
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package related to Apnea data analysis
 Author-email: Julien Laumonier <julien.laumonier@iid.ulaval.ca>
 Project-URL: Homepage, https://github.com/iid-ulaval/pyapnea
 Project-URL: Bug Tracker, https://github.com/iid-ulaval/pyapnea/issues
+Project-URL: Documentation, https://pyapnea.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyApnea v0.0.1
+# PyApnea v0.1.1
 
 Python package related to apnea data analysis.
 
 This version contains functions to read session files from OSCAR software (https://www.sleepfiles.com/OSCAR/)
 
-
+Documentation can be found on [ReadTheDocs](https://pyapnea.readthedocs.io/en/latest/)
```

### Comparing `pyapnea-0.0.1/pyproject.toml` & `pyapnea-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=67.0", "pandas>=2.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyapnea"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Julien Laumonier", email="julien.laumonier@iid.ulaval.ca" },
 ]
 description = "Python package related to Apnea data analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/iid-ulaval/pyapnea"
-"Bug Tracker" = "https://github.com/iid-ulaval/pyapnea/issues"
+"Bug Tracker" = "https://github.com/iid-ulaval/pyapnea/issues"
+"Documentation" = "https://pyapnea.readthedocs.io/en/latest/"
```

### Comparing `pyapnea-0.0.1/src/pyapnea/base_functions.py` & `pyapnea-0.0.2/src/pyapnea/base_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import struct
+from typing import Any
 
 
-def binary(num):
-    """ transform a number to a binary format as string (3 => '00000011')"""
+def binary(num: float) -> str:
+    """
+    Transform a number to a binary format as string (3 => '00000011')
+
+    Args:
+        num: number to transform
+
+    Returns:
+        String representing `num`
+    """
     return ''.join('{:0>8b}'.format(c) for c in struct.pack('!f', num))
 
 
 def _debug_individual_unpack(buffer, formt, position):
     """ display individual unpacked values."""
     print('from', position,
           'to', position + struct.calcsize(formt),
@@ -24,16 +33,20 @@
                       'to', p + struct.calcsize(e),
                       'size', struct.calcsize(e),
                       'raw bytes ', buffer[p:p + struct.calcsize(e)].hex(),
                       'value', struct.unpack_from(e, buffer, offset=p))
                 p = p + struct.calcsize(e)
 
 
-def unpack(buffer, formt, position):
+def unpack(buffer: bytes, formt: str, position: int) -> tuple[int, tuple[Any, ...]]:
     """
     Unpack a number of values from buffer beginning at position.
-    :param buffer: Buffer to extract values.
-    :param formt: values format from struct package.
-    :param position: position to begin.
-    :return: new unread position after extract the fields and tuple of fields.
+
+    Args:
+        buffer: Buffer to extract values.
+        formt: values format from struct package.
+        position: position to begin.
+
+    Returns:
+        New unread position after extract the fields and tuple of fields.
     """
     return position + struct.calcsize(formt), struct.unpack_from(formt, buffer, offset=position)
```

### Comparing `pyapnea-0.0.1/src/pyapnea/oscar/data_structure.py` & `pyapnea-0.0.2/src/pyapnea/oscar/data_structure.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Data structure for an Oscar session. Follow the structure of the file described in the following image:
+
+![image](images/oscar_format.drawio.png)
+"""
 from dataclasses import dataclass, field
 
 
 @dataclass
 class OSCARSessionHeader:
     """ Header data for OSCAR session """
     magicnumber: int = 0
```

### Comparing `pyapnea-0.0.1/src/pyapnea/oscar/oscar_constants.py` & `pyapnea-0.0.2/src/pyapnea/oscar/oscar_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from enum import Enum, auto
 
-
 # Groups
 GRP_CPAP = "CPAP"
 GRP_POS = "POS"
 GRP_OXI = "OXI"
 GRP_JOURNAL = "JOURNAL"
 GRP_SLEEP = "SLEEP"
 
@@ -49,15 +48,14 @@
 STR_GRAPH_ObstructLevel = "ObstructLevel"
 STR_GRAPH_PressureMeasured = "PressureMeasured"
 STR_GRAPH_rRMV = "rRMV"
 STR_GRAPH_rMVFluctuation = "rMVFluctuation"
 STR_GRAPH_FlowFull = "FlowFull"
 STR_GRAPH_SPRStatus = "SPRStatus"
 
-
 # Units
 STR_UNIT_M = " m"
 STR_UNIT_CM = " cm"
 STR_UNIT_INCH = "in"
 STR_UNIT_FOOT = "ft"
 STR_UNIT_POUND = "lb"
 STR_UNIT_OUNCE = "oz"
@@ -68,19 +66,19 @@
 STR_UNIT_Seconds = "Seconds"
 STR_UNIT_h = "h"  # hours shortform
 STR_UNIT_m = "m"  # minutes shortform
 STR_UNIT_s = "s"  # seconds shortform
 STR_UNIT_ms = "ms"  # milliseconds
 STR_UNIT_EventsPerHour = "Events/hr"  # Events per hour
 STR_UNIT_Percentage = "%"
-STR_UNIT_Hz = "Hz"          # Hertz
-STR_UNIT_BPM = "bpm"        # Beats per Minute
-STR_UNIT_LPM = "l/min"      # Litres per Minute
+STR_UNIT_Hz = "Hz"  # Hertz
+STR_UNIT_BPM = "bpm"  # Beats per Minute
+STR_UNIT_LPM = "l/min"  # Litres per Minute
 STR_UNIT_Litres = "Litres"
-STR_UNIT_ml = "ml"        # millilitres
+STR_UNIT_ml = "ml"  # millilitres
 STR_UNIT_BreathsPerMinute = "Breaths/min"  # Breaths per minute
 STR_UNIT_Unknown = "?"
 STR_UNIT_Ratio = "ratio"
 STR_UNIT_Severity = "Severity (0-1)"
 STR_UNIT_Degrees = "Degrees"
```

### Comparing `pyapnea-0.0.1/src/pyapnea/oscar/oscar_getter.py` & `pyapnea-0.0.2/src/pyapnea/oscar/oscar_getter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,46 @@
+from typing import Union
+
 import pandas as pd
 
 from .oscar_constants import CHANNELS
+from .data_structure import OSCARSession, OSCARSessionChannel
 
 
-def get_channel_from_code(oscar_session_data, channel_id):
+def get_channel_from_code(oscar_session_data: OSCARSession, channel_id: int) -> Union[OSCARSessionChannel, None]:
     """
     Get channel data inside OSCARSession data structure from a channel_id
-    :param oscar_session_data: OSCARSession filled from file
-    :param channel_id: one channel id (see channelID in oscar_constants.py)
-    :return: channel data or None if the channelID is not found
+
+    Args:
+        oscar_session_data: OSCARSession filled from file
+        channel_id: one channel id (.value, see channelID in oscar_constants.py)
+
+    Returns:
+        Channel data (`OSCARSessionChannel`) or None if the channelID is not found in the session
     """
     list_result = [item for item in oscar_session_data.data.channels if item.code == channel_id]
     if len(list_result) > 0:
         return list_result[0]
     else:
         return None
 
 
-def event_data_to_dataframe(oscar_session_data, channel_id):
+def event_data_to_dataframe(oscar_session_data: OSCARSession, channel_id: int) -> pd.DataFrame:
     """
-    get the event data as dataframe of an OSCARSession from a channelID
-    :param oscar_session_data: OSCARSession filled from file
-    :param channel_id: one channel id (see channelID in oscar_constants.py)
-    :return: a dataframe with the following columns :
-             "time",  "time_absolute".
-             "data", "data2" (if exists),
-             ChannelID text, ChannelID text +"2" (see oscar_constants.py)
-             if the channelID is not found, return an empty dataframe containing
-             2 columns "time_absolute" and  ChannelID text
+    Get the event data as dataframe of an OSCARSession from a channelID.
+
+    Args:
+        oscar_session_data: OSCARSession filled from file
+        channel_id: One channel id (see channelID in oscar_constants.py)
+
+    Returns:
+        A dataframe with the following columns : ["time",  "time_utc", "data", "data2" (if exists), \
+        ChannelID text, ChannelID text +"2" (see oscar_constants.py) ]. \
+        if the `channel_id` is not found, return an empty dataframe containing \
+        2 columns "time_utc" and ChannelID text
     """
     channel = get_channel_from_code(oscar_session_data, channel_id)
     y_col_name = [c[5] for c in CHANNELS if c[1].value == channel_id][0]
     if channel is not None:
         gain = channel.events[0].gain
         if channel.events[0].t8 == 0:
             channel.events[0].time = range(0, channel.events[0].evcount * int(channel.events[0].rate),
@@ -41,14 +50,15 @@
         df[y_col_name] = df['data'] * gain
 
         if channel.events[0].second_field:
             # not tested because do not have 2nd field in files
             df['data2'] = channel.events[0].data2
             df[y_col_name + '2'] = df['data2'] * gain
 
-        df['time_absolute'] = df['time'] + channel.events[0].ts1
-        df['time_absolute'] = pd.to_datetime(df['time_absolute'], unit='ms')
+        df['time_utc'] = df['time'] + channel.events[0].ts1
+        df['time_utc'] = pd.to_datetime(df['time_utc'], unit='ms')
+        df['time_utc'] = df['time_utc'].dt.tz_localize('UTC')
 
     else:
-        df = pd.DataFrame(data={'time_absolute': [],
+        df = pd.DataFrame(data={'time_utc': [],
                                 y_col_name: []})
     return df
```

### Comparing `pyapnea-0.0.1/src/pyapnea/oscar/oscar_loader.py` & `pyapnea-0.0.2/src/pyapnea/oscar/oscar_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from .data_structure import OSCARSessionHeader, OSCARSession, OSCARSessionData, OSCARSessionChannel, OSCARSessionEvent
 from ..base_functions import unpack
 
 
-def read_session_header(buffer, position):
+def read_session_header(buffer: bytes, position: int) -> tuple[int, OSCARSessionHeader]:
     """
     Read the header of an OSCAR session file. Only support version >= 10 at the moment.
-    :param buffer: buffer containing the header data
-    :param position: position of the header in the buffer
-    :return: new position after header data in buffer and an OSCARSessionHeader data structure
+
+    Args:
+        buffer: Buffer containing the header data
+        position: Position of the header in the buffer
+
+    Returns:
+        New position after header data in buffer and an `OSCARSessionHeader` data structure
     """
     header_data = OSCARSessionHeader()
     position, (magicnum, version, typ, machid, sessid, s_first, s_last) = unpack(buffer, 'IHHIIqq', position)
     header_data.magicnumber = magicnum
     header_data.version = version
     header_data.filetype = typ
     header_data.deviceid = machid
@@ -27,20 +31,24 @@
         header_data.crc16 = crc16
     else:
         print('VERSION NOT SUPPORTED')
 
     return position, header_data
 
 
-def read_event_metadata(buffer, position):
+def read_event_metadata(buffer: bytes, position: int) -> tuple[int, OSCARSessionEvent]:
     """
     Read one event metadata of an OSCAR session file.
-    :param buffer: buffer containing the session data
-    :param position: position of the current event metadata
-    :return: new position after current event metadata in buffer and an OSCARSessionEvent data structure
+
+    Args:
+        buffer: buffer containing the session data
+        position: position of the current event metadata
+
+    Returns:
+        New position after current event metadata in buffer and an OSCARSessionEvent data structure
     """
     position, (ts1, ts2, evcount, t8, rate, gain, offset, mn, mx, len_dim) = unpack(buffer,
                                                                                     '<qqiBdddddi',
                                                                                     position)
     event_data = OSCARSessionEvent()
     event_data.ts1 = ts1
     event_data.ts2 = ts2
@@ -51,96 +59,115 @@
     event_data.offset = offset
     event_data.mn = mn
     event_data.mx = mx
     event_data.len_dim = len_dim
     # See QT QDataStream.cpp QDataStream &QDataStream::readBytes(char *&s, uint &l)
     # not totally sure about this but seems to work with signed int length
     if len_dim != -1:
-        position, (dim,) = unpack(buffer, str(len_dim)+'s', position)
+        position, (dim,) = unpack(buffer, str(len_dim) + 's', position)
         event_data.dim = dim.decode('UTF-16-LE')
     else:
         event_data.dim = ''
     position, (second_field,) = unpack(buffer, '?', position)
     event_data.second_field = second_field
 
     if second_field:
         position, (mn2, mx2) = unpack(buffer, 'ff', position)
         event_data.mn2 = mn2
         event_data.mx2 = mx2
 
     return position, event_data
 
 
-def read_channel_metadata(buffer, position):
+def read_channel_metadata(buffer: bytes, position: int) -> tuple[int, OSCARSessionChannel]:
     """
     Read metadata of a channel in an OSCAR session file.
-    :param buffer: buffer containing the session data
-    :param position: position of the current channel metadata
-    :return: new position after current channel metadata in buffer and an OSCARSessionChannel data structure
+
+    Args:
+        buffer: buffer containing the session data
+        position: position of the current channel metadata
+
+    Returns:
+        New position after current channel metadata in buffer and an OSCARSessionChannel data structure
     """
     position, (code,) = unpack(buffer, 'I', position)
     position, (size2,) = unpack(buffer, 'h', position)
     channel_data = OSCARSessionChannel()
     # Codes are described in oscar_constants.cpp
     channel_data.code = code
     channel_data.size2 = size2
     for evt in range(size2):
         position, event_data = read_event_metadata(buffer, position)
         channel_data.events.append(event_data)
     return position, channel_data
 
 
-def read_channel_data(buffer, position, data_data, channel_num):
+def read_channel_data(buffer: bytes,
+                      position: int,
+                      data_data: OSCARSessionData,
+                      channel_num: int) -> tuple[int, OSCARSessionChannel]:
     """
     Read data of one channel of an OSCAR session file.
-    :param buffer: buffer containing the session data
-    :param position: position of the channel to read
-    :param data_data: OSCARSessionData structure already filled with other metadata
-    :param channel_num: id of channel to read
-    :return: new position after the channel data and the OSCARSessionChannel data structure
+
+    Args:
+        buffer: buffer containing the session data
+        position: position of the channel to read
+        data_data: OSCARSessionData structure already filled with other metadata
+        channel_num: id of channel to read
+
+    Returns:
+        New position after the channel data and the OSCARSessionChannel data structure
     """
     channel_data = data_data.channels[channel_num]
     for evt_id in range(channel_data.size2):
         event_data = channel_data.events[evt_id]
         # 's' is not correct since it interprets as char
-        position, data = unpack(buffer, 'h'*event_data.evcount, position)
+        position, data = unpack(buffer, 'h' * event_data.evcount, position)
         event_data.data = list(data)
         if event_data.second_field:
-            position, data2 = unpack(buffer, 'h'*event_data.evcount, position)
+            position, data2 = unpack(buffer, 'h' * event_data.evcount, position)
             event_data.data2 = list(data2)
         if event_data.t8 != 0:
             position, time_data = unpack(buffer, 'I' * event_data.evcount, position)
             event_data.time = list(time_data)
     return position, channel_data
 
 
-def read_session_data(buffer, position):
+def read_session_data(buffer: bytes, position: int) -> tuple[int, OSCARSessionData]:
     """
     Read the session data of an OSCAR session file.
-    :param buffer: buffer containing the session data
-    :param position: position of the session data in the buffer
-    :return: new position after session data in buffer and an OSCARSessionData data structure
+
+    Args:
+        buffer: buffer containing the session data
+        position: position of the session data in the buffer
+
+    Returns:
+        New position after session data in buffer and an OSCARSessionData data structure
     """
     data_data = OSCARSessionData()
     position, (mcsize,) = unpack(buffer, 'h', position)
     data_data.mcsize = mcsize
     for c in range(mcsize):
         position, channel_data = read_channel_metadata(buffer, position)
         data_data.channels.append(channel_data)
     for c in range(mcsize):
         position, channel_data = read_channel_data(buffer, position, data_data, c)
     return position, data_data
 
 
-def read_session(buffer, position):
+def read_session(buffer: bytes, position: int) -> tuple[int, OSCARSession]:
     """
     Read a session of an OSCAR session file. Only support version >= 10 at the moment.
-    :param buffer: buffer containing the session
-    :param position: position of the session in the buffer
-    :return: new position after session in buffer and an OSCARSession data structure
+
+    Args:
+        buffer: buffer containing the session
+        position: position of the session in the buffer
+
+    Returns:
+        New position after session in buffer and an OSCARSession data structure
     """
     databytes = None
     compmethod = 0
     # Header
     position, oscar_session_header = read_session_header(buffer, position)
 
     temp = buffer[position:]
@@ -159,18 +186,22 @@
     oscar_session = OSCARSession()
     oscar_session.header = oscar_session_header
     oscar_session.data = oscar_session_data
 
     return position, oscar_session
 
 
-def load_session(filename):
+def load_session(filename: str) -> OSCARSession:
     """
     Load an OSCAR session file (.001)
-    :param filename: full path of the file including filename
-    :return: An OSCARSession instance containing data from file
+
+    Args:
+        filename: full path of the file including filename
+
+    Returns:
+        An OSCARSession instance containing data from file
     """
     with open(filename, mode='rb') as file:
         data = file.read()
         position = 0
         position, oscar_session_data = read_session(data, position)
     return oscar_session_data
```

### Comparing `pyapnea-0.0.1/src/pyapnea.egg-info/PKG-INFO` & `pyapnea-0.0.2/src/pyapnea.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyapnea
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package related to Apnea data analysis
 Author-email: Julien Laumonier <julien.laumonier@iid.ulaval.ca>
 Project-URL: Homepage, https://github.com/iid-ulaval/pyapnea
 Project-URL: Bug Tracker, https://github.com/iid-ulaval/pyapnea/issues
+Project-URL: Documentation, https://pyapnea.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyApnea v0.0.1
+# PyApnea v0.1.1
 
 Python package related to apnea data analysis.
 
 This version contains functions to read session files from OSCAR software (https://www.sleepfiles.com/OSCAR/)
 
-
+Documentation can be found on [ReadTheDocs](https://pyapnea.readthedocs.io/en/latest/)
```

