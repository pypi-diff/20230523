# Comparing `tmp/python-canfix-0.2.0.tar.gz` & `tmp/python-canfix-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-canfix-0.2.0.tar", last modified: Tue Dec 22 19:06:50 2020, max compression
+gzip compressed data, was "python-canfix-0.3.0.tar", last modified: Tue May 23 16:12:43 2023, max compression
```

## Comparing `python-canfix-0.2.0.tar` & `python-canfix-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-12-22 19:06:50.000000 python-canfix-0.2.0/
--rw-rw-r--   0 phil      (1000) phil      (1000)    11359 2020-12-22 19:06:50.000000 python-canfix-0.2.0/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      544 2019-02-18 02:49:43.000000 python-canfix-0.2.0/setup.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-12-22 19:06:50.000000 python-canfix-0.2.0/canfix/
--rw-rw-r--   0 phil      (1000) phil      (1000)     5807 2020-12-19 21:05:04.000000 python-canfix-0.2.0/canfix/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4040 2018-12-03 15:15:14.000000 python-canfix-0.2.0/canfix/protocol.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3328 2020-12-22 18:40:37.000000 python-canfix-0.2.0/canfix/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    86606 2018-11-30 03:03:39.000000 python-canfix-0.2.0/canfix/canfix.json
--rw-rw-r--   0 phil      (1000) phil      (1000)     2206 2020-12-19 21:05:04.000000 python-canfix-0.2.0/canfix/globals.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-12-22 19:06:50.000000 python-canfix-0.2.0/canfix/messages/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3679 2019-01-17 19:36:00.000000 python-canfix-0.2.0/canfix/messages/bitrateset.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1516 2019-01-18 21:27:46.000000 python-canfix-0.2.0/canfix/messages/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     9430 2020-07-01 16:55:03.000000 python-canfix-0.2.0/canfix/messages/parameter.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3067 2019-01-17 19:34:35.000000 python-canfix-0.2.0/canfix/messages/nodeidset.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2762 2020-12-19 21:05:04.000000 python-canfix-0.2.0/canfix/messages/nodespecific.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4057 2019-01-17 20:40:51.000000 python-canfix-0.2.0/canfix/messages/nodestatus.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2140 2019-01-18 21:15:41.000000 python-canfix-0.2.0/canfix/messages/nodereport.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2586 2019-01-18 21:37:55.000000 python-canfix-0.2.0/canfix/messages/nodedescription.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4806 2019-01-25 15:45:36.000000 python-canfix-0.2.0/canfix/messages/parameterset.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4978 2019-01-17 19:35:47.000000 python-canfix-0.2.0/canfix/messages/edparameter.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4301 2019-04-20 21:25:27.000000 python-canfix-0.2.0/canfix/messages/nodeidentification.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2017 2020-12-19 21:05:04.000000 python-canfix-0.2.0/canfix/messages/nodealarm.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1844 2020-12-19 21:05:04.000000 python-canfix-0.2.0/canfix/messages/twoway.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4504 2019-04-24 16:48:44.000000 python-canfix-0.2.0/canfix/messages/updatefirmware.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4530 2019-01-17 19:33:11.000000 python-canfix-0.2.0/canfix/messages/twowayconnection.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     6884 2019-07-12 14:45:51.000000 python-canfix-0.2.0/canfix/messages/nodeconfiguration.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     9296 2018-10-16 02:22:29.000000 python-canfix-0.2.0/README.rst
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-12-22 19:06:50.000000 python-canfix-0.2.0/tests/
--rw-rw-r--   0 phil      (1000) phil      (1000)     2198 2019-05-08 22:10:57.000000 python-canfix-0.2.0/tests/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2016-06-19 19:43:52.000000 python-canfix-0.2.0/tests/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3125 2016-06-19 19:50:43.000000 python-canfix-0.2.0/tests/node_alarm.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    14337 2018-11-30 16:14:08.000000 python-canfix-0.2.0/tests/parameter.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4943 2020-12-19 21:05:04.000000 python-canfix-0.2.0/tests/msgtypes.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     5573 2020-12-19 21:05:04.000000 python-canfix-0.2.0/tests/two_way_msg.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    36416 2020-12-19 21:05:04.000000 python-canfix-0.2.0/tests/node_specific.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     4708 2019-05-09 12:37:36.000000 python-canfix-0.2.0/tests/dataconversion.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2020-12-22 19:06:50.000000 python-canfix-0.2.0/python_canfix.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)    11359 2020-12-22 19:06:49.000000 python-canfix-0.2.0/python_canfix.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2020-12-22 19:06:49.000000 python-canfix-0.2.0/python_canfix.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       11 2020-12-22 19:06:49.000000 python-canfix-0.2.0/python_canfix.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       13 2020-12-22 19:06:49.000000 python-canfix-0.2.0/python_canfix.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      958 2020-12-22 19:06:49.000000 python-canfix-0.2.0/python_canfix.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2020-12-22 19:06:50.000000 python-canfix-0.2.0/setup.cfg
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 16:12:43.335379 python-canfix-0.3.0/
+-rw-r--r--   0 phil      (1000) phil      (1000)    17986 2019-06-17 15:29:55.000000 python-canfix-0.3.0/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     9595 2023-05-23 16:12:43.335379 python-canfix-0.3.0/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)     9305 2022-10-01 21:20:46.000000 python-canfix-0.3.0/README.rst
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 16:12:43.335379 python-canfix-0.3.0/canfix/
+-rw-r--r--   0 phil      (1000) phil      (1000)     3328 2020-12-22 18:40:37.000000 python-canfix-0.3.0/canfix/__init__.py
+-rw-r--r--   0 phil      (1000) phil      (1000)    86606 2018-11-30 03:03:39.000000 python-canfix-0.3.0/canfix/canfix.json
+-rw-r--r--   0 phil      (1000) phil      (1000)     2243 2023-05-09 21:18:07.000000 python-canfix-0.3.0/canfix/globals.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 16:12:43.335379 python-canfix-0.3.0/canfix/messages/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1516 2019-01-18 21:27:46.000000 python-canfix-0.3.0/canfix/messages/__init__.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     3682 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/bitrateset.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4981 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/edparameter.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     2020 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodealarm.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     6890 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodeconfiguration.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     2589 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodedescription.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4304 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodeidentification.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     3070 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodeidset.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     2143 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/nodereport.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     2768 2023-03-17 01:22:58.000000 python-canfix-0.3.0/canfix/messages/nodespecific.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     5165 2023-05-18 22:38:05.000000 python-canfix-0.3.0/canfix/messages/nodestatus.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     9950 2023-05-20 14:28:11.000000 python-canfix-0.3.0/canfix/messages/parameter.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4809 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/parameterset.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     1847 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/twoway.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4533 2022-10-01 21:20:46.000000 python-canfix-0.3.0/canfix/messages/twowayconnection.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4586 2023-01-30 15:29:37.000000 python-canfix-0.3.0/canfix/messages/updatefirmware.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4040 2018-12-03 15:15:14.000000 python-canfix-0.3.0/canfix/protocol.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     6163 2023-05-19 00:37:15.000000 python-canfix-0.3.0/canfix/utils.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 16:12:43.335379 python-canfix-0.3.0/python_canfix.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     9595 2023-05-23 16:12:43.000000 python-canfix-0.3.0/python_canfix.egg-info/PKG-INFO
+-rw-r--r--   0 phil      (1000) phil      (1000)      966 2023-05-23 16:12:43.000000 python-canfix-0.3.0/python_canfix.egg-info/SOURCES.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)        1 2023-05-23 16:12:43.000000 python-canfix-0.3.0/python_canfix.egg-info/dependency_links.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       11 2023-05-23 16:12:43.000000 python-canfix-0.3.0/python_canfix.egg-info/requires.txt
+-rw-r--r--   0 phil      (1000) phil      (1000)       13 2023-05-23 16:12:43.000000 python-canfix-0.3.0/python_canfix.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2023-05-23 16:12:43.335379 python-canfix-0.3.0/setup.cfg
+-rw-r--r--   0 phil      (1000) phil      (1000)      544 2023-03-16 22:47:23.000000 python-canfix-0.3.0/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2023-05-23 16:12:43.335379 python-canfix-0.3.0/tests/
+-rw-r--r--   0 phil      (1000) phil      (1000)        0 2016-06-19 19:43:52.000000 python-canfix-0.3.0/tests/__init__.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4708 2019-05-09 12:37:36.000000 python-canfix-0.3.0/tests/dataconversion.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     4982 2022-10-01 21:20:46.000000 python-canfix-0.3.0/tests/msgtypes.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     3140 2022-10-01 21:20:46.000000 python-canfix-0.3.0/tests/node_alarm.py
+-rw-r--r--   0 phil      (1000) phil      (1000)    36595 2023-03-17 01:17:49.000000 python-canfix-0.3.0/tests/node_specific.py
+-rw-r--r--   0 phil      (1000) phil      (1000)    14400 2022-10-01 21:20:46.000000 python-canfix-0.3.0/tests/parameter.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     5597 2022-10-01 21:20:46.000000 python-canfix-0.3.0/tests/two_way_msg.py
+-rw-r--r--   0 phil      (1000) phil      (1000)     2198 2019-05-08 22:10:57.000000 python-canfix-0.3.0/tests/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-canfix-0.2.0/PKG-INFO` & `python-canfix-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,233 +1,236 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: python-canfix
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python CAN-FIX Library
 Home-page: https://github.com/birkelbach/python-canfix
 Author: Phil Birkelbach
 Author-email: phil@petrasoft.net
 License: GNU General Public License Version 2
-Description: =========================
-        Python CAN-FIX Library
-        =========================
-        
-        python-canfix is a Python package that abstracts the details of the
-        CAN-FIX communication protocol.
-        
-        CAN-FIX is the CAN bus implementation of a set of protocols and specifications
-        known as FIX. FIX stands for Flight Information eXchange and is an attempt to
-        standardize communication among aircraft systems in small aircraft.
-        
-        The project is hosted on GitHub at...
-        
-        https://github.com/birkelbach/python-canfix
-        
-        Installation
-        ============
-        
-        Install ``canfix`` with ``pip``:
-        ::
-        
-            $ pip install python-canfix
-        
-        
-        You can also install directly from the source directory by running:
-        ::
-        
-            $ python setup.py install
-        
-        The only dependency is python-can, which should be automatically installed
-        by the above commands.
-        
-        API
-        ===
-        
-        You should be familiar with the CANFIX protocol specification before using
-        this library.  CANFIX has several different message types.  Each of these
-        types is representd by a class in this library.
-        
-        
-        NodeAlarm Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``NoneAlarm.node`` - Sets or returns the node address of the node that sent (or will send) the Alarm Message.  Should be an
-        integer between 1 and 254
-        
-        ``NodeAlarm.alarm`` - Sets or returns the alarm type.  The meaning of this data is dependent on the individual node type.
-        Should be an integer between 0 and 65,535.
-        
-        ``NodeAlarm.data`` - Sets or returns a list that represents the data for this alarm.  What the data represents is dependent
-        on the specific type of node and the alarm type.  It should be a list of bytes of up to 6 bytes in length.
-        
-        ``NodeAlarm.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
-        is set with a message received from the can bus then the message will be parsed and the node, alarm and data properties
-        will be set accordingly.  If it is read then the message will be constructed with the node, alarm and data properties
-        that should have been previously set.
-        
-        Example Usage::
-        
-            >>> na = canfix.NodeAlarm()
-            >>> na.node = 12
-            >>> na.alarm = 45321
-            >>> na.data = [4,5,6,7]
-            >>> na.msg
-            >>> na.msg
-            can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
-            data=[0x9, 0xb1, 0x4, 0x5, 0x6, 0x7])
-        
-            >>> msg = bus.recv() # Assume we read the same message that we created above
-            >>> na = canfix.NodeAlarm(msg)
-            >>> print(na)
-            [12] Node Alarm 45321 Data 04050607
-        
-        
-        Parameter Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``Parameter.node`` - Sets or returns the node address of the node that sent (or will send) the Parameter.
-        Should be an integer between 1 and 254
-        
-        ``Parameter.identifier`` - Sets or returns the CAN bus identifier for this parameter.  If the identifier is out of
-        of range for Parameter messages a ValueError exception will be raised.  Setting this will also cause protocol specific
-        information to be set in the object.  This includes the data type, the engineering units, name etc.
-        
-        ``Parameter.name`` - Sets or returns the name of the parameter.  i.e. "Indicated Airspeed"  If the name is not found
-        in the protocol ValueError exception will be raised.  Setting this will also cause protocol specific
-        information to be set in the object.  This includes the data type, the engineering units, identifier etc.
-        
-        ``Parameter.index`` - Sets or returns the index of the parameter.  Should be an integer between 0 and 255.
-        
-        ``Parameter.failure`` - Sets or returns the flag that indicates data failure.  Should be ``True`` or ``False``
-        
-        ``Parameter.quality`` - Sets or returns the flag that indicates data quality.  Should be ``True`` or ``False``
-        
-        ``Parameter.annunciate`` - Sets or returns the flag that indicates the paramter should be annunciated.
-        Should be ``True`` or ``False``
-        
-        ``Parameter.meta`` - Sets or returns the meta data index for the Parameter.  Should be an integer between 0 and 15
-        
-        ``Parameter.value`` - Sets or returns the value for the parameter.  It can be a list of multiple values if the
-        particular parameter is expecting multiple values.  It can also be a string
-        
-        ``Parameter.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
-        is set with a message received from the can bus then the message will be parsed and the properties
-        will be set accordingly.  If it is read then the message will be constructed with properties
-        that should have been previously set.
-        
-        ``Parameter.fullName`` - Returns a string that represents the parameter that includes the index and the index name.
-        This property is read only.
-        
-        ``Parameter.units`` - Read only property that returns a string indicating the engineering units for this Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.type`` - Read only property that returns a string indicating the datatype for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.min`` - Read only property that returns a value that indicates the minimum value for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.max`` - Read only property that returns a value that indicates the maximum value for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.format`` - Read only property that returns the format of the data in the Parameter value.  This is typically
-        used to indicated what WORD and BYTE type data means.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.remarks`` - Read only property that returns a list of remarks that are associated with this Parameter
-        in the protocol specification.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.indexName`` - Read only property that retuns he name of what the index represents.  i.e. Cylinder
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.multiplier`` - Read only property that returns the multiplier for the Parameter.  Some paramters use
-        an integer with a multiplier as the value in the message.  For example if we had a Parameter value of 123.4 and
-        the multiplier is 0.1 then the data that would be communicated on the bus would be 1234.  The receiver would then
-        multiply by 0.1 to get the original value of 123.4.  The ``python-canfix`` library handles these details for you
-        so you don't need to concern yourself with this detail.  It is a part of the protocol and is included here for
-        applications that want to display protocol specific information to the user.
-        This is a protocol specific piece of information and should not change.
-        
-        Example Usage::
-        
-            >>> pa = canfix.Parameter()
-            >>> pa.node = 2
-            >>> pa.value = 123.4
-            >>> print(pa)
-            [2] Indicated Airspeed: 123.4 knots
-            >>> pa.msg
-            can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0x183,
-            dlc=0, data=[0x2, 0x0, 0x0, 0xd2, 0x4])
-        
-        
-        TwoWayMsg Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``TwoWayMsg.channel`` - Sets the channel that this message will be sent on.  There are
-        16 channels numbered 0-15
-        
-        ``TwoWayMsg.type`` - Set to either 'Request' or 'Response'  This determines which
-        side of the channel to use.
-        
-        ``TwoWayMsg.data`` - Up to eight bytes
-        
-        NodeSpecific Class
-        ------------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``NodeSpecific.destNode`` - Represents the node address of the node that this
-        message is addressed to.  Should be an integer between 1 and 254.
-        
-        ``NodeSpecific.controlCode`` - The control code for the messge.  Currently, valid
-        values are 0-10.  Future versions of the CAN-FIX specification may use 11-127 and
-        values from 128 to 255 are reserved for user defined functions.  The control
-        code is basically the function of the message.  See the CAN-FIX specification
-        for details.
-        
-        ``NodeSpecific.data`` - Up to 8 bytes of data that is dependent on which type
-        of message that is being sent.
-        
-        Functions
-        ---------
-        
-        ``parseMessage(msg)`` - When passed a ``Message`` this function figures
-        out what the message type is, instantiates the correct object type and
-        returns that object.  This function would be used for most all received
-        messages.
-        
-        Example Usage::
-        
-          >>> msg = bus.recv()
-          >>> msg
-          can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False,
-          is_error_frame=False, arbitration_id=0x183, dlc=5,
-          data=[0xc, 0x0, 0x0, 0xd2, 0x4])
-          >>> p = canfix.parseMessage(msg)
-          >>> p
-          <canfix.Parameter object at 0x7f6984fe9c10>
-          >>> print(p)
-          [12] Indicated Airspeed: 123.4 knots
-        
 Platform: UNKNOWN
+License-File: LICENSE
+
+=========================
+Python CAN-FIX Library
+=========================
+
+python-canfix is a Python package that abstracts the details of the
+CAN-FIX communication protocol.
+
+CAN-FIX is the CAN bus implementation of a set of protocols and specifications
+known as FIX. FIX stands for Flight Information eXchange and is an attempt to
+standardize communication among aircraft systems in small aircraft.
+
+The project is hosted on GitHub at...
+
+https://github.com/birkelbach/python-canfix
+
+Installation
+============
+
+Install ``canfix`` with ``pip``:
+::
+
+    $ pip install python-canfix
+
+
+You can also install directly from the source directory by running:
+::
+
+    $ python setup.py install
+
+The only dependency is python-can, which should be automatically installed
+by the above commands.
+
+API
+===
+
+You should be familiar with the CANFIX protocol specification before using
+this library.  CANFIX has several different message types.  Each of these
+types is representd by a class in this library.
+
+
+NodeAlarm Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``NoneAlarm.node`` - Sets or returns the node address of the node that sent (or will send) the Alarm Message.  Should be an
+integer between 1 and 254
+
+``NodeAlarm.alarm`` - Sets or returns the alarm type.  The meaning of this data is dependent on the individual node type.
+Should be an integer between 0 and 65,535.
+
+``NodeAlarm.data`` - Sets or returns a list that represents the data for this alarm.  What the data represents is dependent
+on the specific type of node and the alarm type.  It should be a list of bytes of up to 6 bytes in length.
+
+``NodeAlarm.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
+is set with a message received from the can bus then the message will be parsed and the node, alarm and data properties
+will be set accordingly.  If it is read then the message will be constructed with the node, alarm and data properties
+that should have been previously set.
+
+Example Usage::
+
+    >>> na = canfix.NodeAlarm()
+    >>> na.node = 12
+    >>> na.alarm = 45321
+    >>> na.data = [4,5,6,7]
+    >>> na.msg
+    >>> na.msg
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
+    data=[0x9, 0xb1, 0x4, 0x5, 0x6, 0x7])
+
+    >>> msg = bus.recv() # Assume we read the same message that we created above
+    >>> na = canfix.NodeAlarm(msg)
+    >>> print(na)
+    [12] Node Alarm 45321 Data 04050607
+
+
+Parameter Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``Parameter.node`` - Sets or returns the node address of the node that sent (or will send) the Parameter.
+Should be an integer between 1 and 254
+
+``Parameter.identifier`` - Sets or returns the CAN bus identifier for this parameter.  If the identifier is out of
+of range for Parameter messages a ValueError exception will be raised.  Setting this will also cause protocol specific
+information to be set in the object.  This includes the data type, the engineering units, name etc.
+
+``Parameter.name`` - Sets or returns the name of the parameter.  i.e. "Indicated Airspeed"  If the name is not found
+in the protocol ValueError exception will be raised.  Setting this will also cause protocol specific
+information to be set in the object.  This includes the data type, the engineering units, identifier etc.
+
+``Parameter.index`` - Sets or returns the index of the parameter.  Should be an integer between 0 and 255.
+
+``Parameter.failure`` - Sets or returns the flag that indicates data failure.  Should be ``True`` or ``False``
+
+``Parameter.quality`` - Sets or returns the flag that indicates data quality.  Should be ``True`` or ``False``
+
+``Parameter.annunciate`` - Sets or returns the flag that indicates the paramter should be annunciated.
+Should be ``True`` or ``False``
+
+``Parameter.meta`` - Sets or returns the meta data index for the Parameter.  Should be an integer between 0 and 15
+
+``Parameter.value`` - Sets or returns the value for the parameter.  It can be a list of multiple values if the
+particular parameter is expecting multiple values.  It can also be a string
+
+``Parameter.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
+is set with a message received from the can bus then the message will be parsed and the properties
+will be set accordingly.  If it is read then the message will be constructed with properties
+that should have been previously set.
+
+``Parameter.fullName`` - Returns a string that represents the parameter that includes the index and the index name.
+This property is read only.
+
+``Parameter.units`` - Read only property that returns a string indicating the engineering units for this Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.type`` - Read only property that returns a string indicating the datatype for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.min`` - Read only property that returns a value that indicates the minimum value for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.max`` - Read only property that returns a value that indicates the maximum value for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.format`` - Read only property that returns the format of the data in the Parameter value.  This is typically
+used to indicated what WORD and BYTE type data means.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.remarks`` - Read only property that returns a list of remarks that are associated with this Parameter
+in the protocol specification.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.indexName`` - Read only property that retuns he name of what the index represents.  i.e. Cylinder
+This is a protocol specific piece of information and should not change.
+
+``Parameter.multiplier`` - Read only property that returns the multiplier for the Parameter.  Some paramters use
+an integer with a multiplier as the value in the message.  For example if we had a Parameter value of 123.4 and
+the multiplier is 0.1 then the data that would be communicated on the bus would be 1234.  The receiver would then
+multiply by 0.1 to get the original value of 123.4.  The ``python-canfix`` library handles these details for you
+so you don't need to concern yourself with this detail.  It is a part of the protocol and is included here for
+applications that want to display protocol specific information to the user.
+This is a protocol specific piece of information and should not change.
+
+Example Usage::
+
+    >>> pa = canfix.Parameter()
+    >>> pa.node = 2
+    >>> pa.value = 123.4
+    >>> print(pa)
+    [2] Indicated Airspeed: 123.4 knots
+    >>> pa.msg
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0x183,
+    dlc=0, data=[0x2, 0x0, 0x0, 0xd2, 0x4])
+
+
+TwoWayMsg Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``TwoWayMsg.channel`` - Sets the channel that this message will be sent on.  There are
+16 channels numbered 0-15
+
+``TwoWayMsg.type`` - Set to either 'Request' or 'Response'  This determines which
+side of the channel to use.
+
+``TwoWayMsg.data`` - Up to eight bytes
+
+NodeSpecific Class
+------------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``NodeSpecific.destNode`` - Represents the node address of the node that this
+message is addressed to.  Should be an integer between 1 and 254.
+
+``NodeSpecific.controlCode`` - The control code for the messge.  Currently, valid
+values are 0-10.  Future versions of the CAN-FIX specification may use 11-127 and
+values from 128 to 255 are reserved for user defined functions.  The control
+code is basically the function of the message.  See the CAN-FIX specification
+for details.
+
+``NodeSpecific.data`` - Up to 8 bytes of data that is dependent on which type
+of message that is being sent.
+
+Functions
+---------
+
+``parseMessage(msg)`` - When passed a ``Message`` this function figures
+out what the message type is, instantiates the correct object type and
+returns that object.  This function would be used for most all received
+messages.
+
+Example Usage::
+
+  >>> msg = bus.recv()
+  >>> msg
+  can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False,
+  is_error_frame=False, arbitration_id=0x183, dlc=5,
+  data=[0xc, 0x0, 0x0, 0xd2, 0x4])
+  >>> p = canfix.parseMessage(msg)
+  >>> p
+  <canfix.Parameter object at 0x7f6984fe9c10>
+  >>> print(p)
+  [12] Indicated Airspeed: 123.4 knots
+
+
```

### Comparing `python-canfix-0.2.0/setup.py` & `python-canfix-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #from distutils.core import setup
 from setuptools import setup, find_packages
 
 setup(
     name='python-canfix',
-    version='0.2.0',
+    version='0.3.0',
     long_description=open('README.rst').read(),
     description="Python CAN-FIX Library",
     author="Phil Birkelbach",
     author_email="phil@petrasoft.net",
     license='GNU General Public License Version 2',
     url='https://github.com/birkelbach/python-canfix',
     packages=find_packages(),
```

### Comparing `python-canfix-0.2.0/canfix/utils.py` & `python-canfix-0.3.0/canfix/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,52 +66,58 @@
                 x.append(True)
             else:
                 x.append(False)
         return x
     # If we get here then the data type is a numeric type or a CHAR
     try:
         x = struct.unpack(table[datatype], data)[0]
+        if multiplier != 1:
+            return x * multiplier
+        else:
+            return x
         return x * multiplier
     except KeyError:
         # If we get a KeyError on the dict then it's a CHAR
         if "CHAR" in datatype:
             return data.decode("utf-8")
         return None
     except struct.error:
         return None
 
 # This function takes a datatype, value and multiplier and converts the single
 # value into a bytearray and returns that bytearray
 def pack(datatype, value, multiplier):
-    table = {"SHORT":"<b", "USHORT":"<B", "UINT":"<H",
+    table = {"BYTE":"<b", "WORD":"<H", "SHORT":"<b", "USHORT":"<B", "UINT":"<H",
              "INT":"<h", "DINT":"<l", "UDINT":"<L", "FLOAT":"<f"}
 
-    if datatype == "BYTE":
-        x = bytearray([0x00])
-        for bit in range(8):
-            if value[bit]:
-                x[0] |= 0x01<<bit
-    elif datatype == "WORD":
-        x = bytearray([0x00, 0x00])
-        for bit in range(8):
-            if value[bit]:
-                x[0] |= 0x01<<bit
-            if value[bit+8]:
-                x[1] |= 0x01<<bit
+    # We represent the BYTE and WORD types as a list of bools but the caller
+    # may just send us an int.  If it's the list we'll deal with it here
+    # otherwise we'll deal with it as an int.
+    if isinstance(value, list): 
+        if datatype == "BYTE":
+            x = bytearray([0x00])
+            for bit in range(8):
+                if value[bit]:
+                    x[0] |= 0x01<<bit
+        elif datatype == "WORD":
+            x = bytearray([0x00, 0x00])
+            for bit in range(8):
+                if value[bit]:
+                    x[0] |= 0x01<<bit
+                if value[bit+8]:
+                    x[1] |= 0x01<<bit
     else:
         try:
             if datatype != "FLOAT":
                 x = struct.pack(table[datatype], int(round(value / multiplier)))
             else:
                 x = struct.pack(table[datatype], value / multiplier)
         except KeyError:
             if "CHAR" in datatype:
                 return [ord(value)]
-            # else:
-            #     raise
             return None
     return x
 
 
 
 def getValue(datatype, data, multiplier = 1.0):
     """Takes the data type, a byte array of data and the multiplier
```

### Comparing `python-canfix-0.2.0/canfix/protocol.py` & `python-canfix-0.3.0/canfix/protocol.py`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/canfix/__init__.py` & `python-canfix-0.3.0/canfix/__init__.py`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/canfix/canfix.json` & `python-canfix-0.3.0/canfix/canfix.json`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/canfix/globals.py` & `python-canfix-0.3.0/canfix/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,7 +49,10 @@
 TWOWAY_CONN_CHANS = 0x7e0
 
 class MsgSizeError(Exception):
     pass
 
 class TypeMissingError(Exception):
     pass
+
+class NotFound(Exception):
+    pass
```

### Comparing `python-canfix-0.2.0/canfix/messages/bitrateset.py` & `python-canfix-0.3.0/canfix/messages/bitrateset.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             else:
                 self.msgType = MSG_REQUEST
                 self.bitrate = msg.data[2]
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/__init__.py` & `python-canfix-0.3.0/canfix/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/canfix/messages/parameter.py` & `python-canfix-0.3.0/canfix/messages/parameter.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.multiplier = p.multiplier
         if self.multiplier == None:
             self.multiplier = 1
 
     def setIdentifier(self, identifier):
         if identifier in parameters:
             log.debug("Setting parameter id {}".format(identifier))
-            self.__msg = can.Message(arbitration_id=identifier, extended_id=False)
+            self.__msg = can.Message(arbitration_id=identifier, is_extended_id=False)
         else:
             raise ValueError("Bad Parameter Identifier Given")
 
         self.__identifier = self.__msg.arbitration_id
         self.__parameterData(self.__msg.arbitration_id)
 
     def getIdentifier(self):
@@ -78,15 +78,15 @@
 
     identifier = property(getIdentifier, setIdentifier)
 
     def setName(self, name):
         x = getParameterByName(name)
         if x:
             log.debug("Setting parameter id to {}, based on name {}".format(x.id, name))
-            self.__msg = can.Message(arbitration_id=x.id, extended_id=False)
+            self.__msg = can.Message(arbitration_id=x.id, is_extended_id=False)
             self.__identifier = x.id
             self.__parameterData(self.__msg.arbitration_id)
             return
         raise ValueError("Unknown Parameter Name - {}".format(name))
 
     def getName(self):
         return self.__name
@@ -210,23 +210,54 @@
             return "%s %s %i" % (self.__name, self.indexName, self.index + 1)
         else:
             return self.__name
 
     fullName = property(getFullName)
 
     def valueStr(self, units=False):
-        if self.__identifier == 0x580: #Time
-            return "%02i:%02i:%02i" % (self.value[0], self.value[1], self.value[2])
-        elif self.__identifier == 0x581: #Date
-            return "%i-%i-%i" % (self.value[0], self.value[1], self.value[2])
-        else:
-            if self.units:
-                return "{:g} {}".format(self.value, self.units)
+        try:
+            if self.__identifier == 0x580: #Time
+                return "%02i:%02i:%02i" % (self.value[0], self.value[1], self.value[2])
+            elif self.__identifier == 0x581: #Date
+                return "%i-%i-%i" % (self.value[0], self.value[1], self.value[2])
+            elif self.__identifier in [0x11A, 0x11B, 0x300, 0x301, 0x302, 0x303, 0x304, 0x305, 0x306, 0x307]:
+                s = f"{self.value[0]}, {self.value[1]}, "
+                for bit in self.value[2]:
+                    if bit:
+                        s += '1'
+                    else:
+                        s += '0'
+                return s
+            elif self.type[:5] == 'BYTE[': # Handle byte arrays
+                s = ''
+                for b in self.value:
+                    for bit in b:
+                        if bit:
+                            s += '1'
+                        else:
+                            s += '0'
+                    s += ' '
+                return s
+            elif self.type =='BYTE' or self.type == 'WORD':
+                s=''
+                for i, bit in enumerate(self.value):
+                    if bit:
+                            s += '1'
+                    else:
+                        s += '0'
+                    if i == 8:
+                        s += ' '
+                return s
             else:
-                return str(self.value)
+                if self.units:
+                    return "{:g} {}".format(self.value, self.units)
+                else:
+                    return str(self.value)
+        except:
+            return "ERR"
 
 
     def __eq__(self, other):
         return (self.__identifier*16 + self.index) == (other.__identifier*16 + other.index)
 
     def __ne__(self, other):
         return not (self == other)
@@ -247,33 +278,19 @@
     def __str__(self):
         s = '[' + str(self.node) + '] ' + self.name
         if self.meta: s = s + ' ' + self.meta
         if self.indexName:
             s = s + ' ' + self.indexName + ' ' + str(self.index+1)
         s = s + ': '
         if self.value != None:
-            if isinstance(self.value, list):
-                if self.type == "BYTE" or self.type == "WORD":
-                    n = 0 #loop counter
-                    for each in reversed(self.value):
-                        if each == True:
-                            s = s+'1'
-                        else:
-                            s = s+'0'
-                        n += 1
-                        if n % 4 == 0: #add a space every four bits
-                            s = s+' '
-                else:
-                    for each in self.value:
-                        s = s + str(each) + ','
-                s = s.strip(', ')
-            else:
-               s = s + str(self.value)
-            if self.units != None:
-                s = s + ' ' + self.units
-            if self.failure:
-                s = s + ' [FAIL]'
-            if self.quality:
-                s = s + ' [QUAL]'
-            if self.annunciate:
-                s = s + ' [ANNUNC]'
+            s += self.valueStr(units=True)
+        else:
+            s = s + str(self.value)
+        # if self.units != None:
+        #     s = s + ' ' + self.units
+        if self.failure:
+            s = s + ' [FAIL]'
+        if self.quality:
+            s = s + ' [QUAL]'
+        if self.annunciate:
+            s = s + ' [ANNUNC]'
         return s
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodeidset.py` & `python-canfix-0.3.0/canfix/messages/nodeidset.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             else:
                 self.msgType = MSG_REQUEST
                 self.newNode = msg.data[2]
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodespecific.py` & `python-canfix-0.3.0/canfix/messages/nodespecific.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,26 @@
              "Parameter Set 224"]
     start_id = NODE_SPECIFIC_MSGS
 
     def __init__(self, msg=None):
         if msg != None:
             self.setMessage(msg)
         else:
-            self.controlCode = 0
+            self.controlCode = None
             self.data = bytearray([])
 
     def setMessage(self, msg):
         log.debug(str(msg))
         self.sendNode = msg.arbitration_id - self.start_id
         self.controlCode = msg.data[0]
         #self.destNode = msg.data[1]
         self.data = msg.data[1:]
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data.append(self.controlCode)
         #msg.data.append(self.destNode)
         for each in self.data:
             msg.data.append(each)
         msg.dlc = len(msg.data)
         return msg
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodestatus.py` & `python-canfix-0.3.0/canfix/messages/nodestatus.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,23 @@
 from .nodespecific import NodeSpecific
 
 
 class NodeStatus(NodeSpecific):
     # These are the defined types in the protocol.  The parameter would be
     # used to index this list.  For others the type would have to be set before
     # the value accessed.
-    knownTypes = (("WORD",1), ("INT",0.1), ("UDINT",1), ("UDINT",1), ("INT",0.1), ("UDINT",1))
+    knownTypes = (("Status","WORD",1),
+                  ("Unit Temperature", "INT",0.1),
+                  ("Supply Voltage","INT",0.1),
+                  ("CAN Transmit Frame Count", "UDINT",1),
+                  ("CAN Receive Frame Count", "UDINT",1),
+                  ("CAN Transmit Error Count", "UDINT",1),
+                  ("CAN Transmit Error Count", "UDINT",1),
+                  ("CAN Receive Overrun Count", "UDINT",1),
+                  ("Serial Number", "UDINT",1))
     def __init__(self, msg=None, parameter=None, value=None, datatype=None, multiplier=1.0):
         if msg != None:
             self.setMessage(msg)
         else:
             self.controlCode = 0x06
             self.sendNode = None
             self.parameter = parameter
@@ -53,36 +61,36 @@
         self.valueData = msg.data[3:]
         try:
             ts = utils.getTypeSize(self.type)
         except KeyError:
             ts = None
         if ts:
             if msg.dlc != (3 + ts):
-                raise MsgSizeError("Message size is incorrect")
+                raise MsgSizeError("Message size is incorrect - {}".format(msg))
         if msg.dlc < 3:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def setParameter(self, parameter):
         if parameter == None:
             self.__parameter = None
             return
         if parameter < 0 or parameter > 65535:
             raise ValueError("Paremeter Type must be between 0 and 65535")
         self.__parameter = parameter
         if self.__parameter < len(self.knownTypes):
-            self.type = self.knownTypes[self.__parameter][0]
-            self.multiplier = self.knownTypes[self.__parameter][1]
+            self.type = self.knownTypes[self.__parameter][1]
+            self.multiplier = self.knownTypes[self.__parameter][2]
         else:
             self.type = None # This'll cause an error somewhere.
             self.multiplier = 1
 
     def getParameter(self):
         return self.__parameter
 
@@ -104,13 +112,27 @@
         self.valueData = utils.setValue(self.type, value, self.multiplier)
 
     def getValue(self):
         return utils.getValue(self.type, self.valueData, self.multiplier)
 
     value = property(getValue, setValue)
 
-
     def __str__(self):
-        s = "[" + str(self.sendNode) + "]"
-        s += "->[" + str(self.destNode) + "] "
+        s = "[" + str(self.sendNode) + "] "
         s += self.codes[self.controlCode]
+        if self.__parameter < len(self.knownTypes):
+            if self.__parameter == 0 :
+                if self.value == [False]*16:
+                    s += ": {} GOOD".format(self.knownTypes[self.__parameter][0])
+                else:
+                    errors = ""
+                    for each in self.value:
+                        if each:
+                            errors += '1'
+                        else:
+                            errors += '0'
+                    s += ": {} ERROR {}".format(self.knownTypes[self.__parameter][0], errors)
+            else:
+                s += ": {} {}".format(self.knownTypes[self.__parameter][0], self.value)
+        else:
+            s+= ": Parameter {} {}".format(self.__parameter, self.data)
         return s
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodereport.py` & `python-canfix-0.3.0/canfix/messages/nodereport.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         assert self.controlCode == 0x05
         self.destNode = msg.data[1]
 
         if msg.dlc != 2:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodedescription.py` & `python-canfix-0.3.0/canfix/messages/nodedescription.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.packetnumber = msg.data[3] * 256 + msg.data[2]
         self.chars = msg.data[4:]
 
         if msg.dlc < 8:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/parameterset.py` & `python-canfix-0.3.0/canfix/messages/parameterset.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         if ts:
             if msg.dlc != (3 + ts):
                 raise MsgSizeError("Message size is incorrect")
         if msg.dlc < 3:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def setParameter(self, parameter):
```

### Comparing `python-canfix-0.2.0/canfix/messages/edparameter.py` & `python-canfix-0.3.0/canfix/messages/edparameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 raise ValueError("Unknown Error Code {}".format(msg.data[2]))
         elif msg.dlc == 4:
             self.identifier = msg.data[2] + (msg.data[3]<<8)
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodeidentification.py` & `python-canfix-0.3.0/canfix/messages/nodeidentification.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             self.device = msg.data[3]
             self.fwrev = msg.data[4]
             self.model = msg.data[5] + (msg.data[6]<<8) + (msg.data[7]<<16)
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodealarm.py` & `python-canfix-0.3.0/canfix/messages/nodealarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             raise ValueError("Node Alarm message missing alarm code")
         self.timestamp = msg.timestamp
         self.alarm = msg.data[0] + msg.data[1]*256
         self.data = msg.data[2:]
         self.data.extend(bytearray(max(0, 5-len(self.data)))) # Pad data with zeros
 
     def getMessage(self):
-        msg = can.Message(extended_id=False)
+        msg = can.Message(is_extended_id=False)
         msg.arbitration_id = self.node
         msg.data.append(int(self.alarm % 256))
         msg.data.append(int(self.alarm / 256))
         for each in self.data:
             msg.data.append(each)
         return msg
```

### Comparing `python-canfix-0.2.0/canfix/messages/twoway.py` & `python-canfix-0.3.0/canfix/messages/twoway.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.data = msg.data
         if msg.arbitration_id % 2 == 0:
             self.type = "Request"
         else:
             self.type = "Response"
 
     def getMessage(self):
-        msg = can.Message(extended_id=False)
+        msg = can.Message(is_extended_id=False)
         msg.arbitration_id = self.channel*2 + TWOWAY_CONN_CHANS
         if self.type == "Response":
             msg.arbitration_id += 1
         msg.data = self.data
         return msg
 
     msg = property(getMessage, setMessage)
```

### Comparing `python-canfix-0.2.0/canfix/messages/updatefirmware.py` & `python-canfix-0.3.0/canfix/messages/updatefirmware.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,18 @@
             self.setMessage(msg)
         else:
             self.controlCode = 0x07
             self.msgType = MSG_RESPONSE
             self.sendNode = None
             self.destNode = node
             self.errorCode = 0x00
-            if verification is not None: self.verification = verification
+            if verification is not None:
+                self.__verification = verification
+            else:
+                self.__verification = None
             if channel is not None: self.channel = channel
 
     def setMessage(self, msg):
         log.debug(str(msg))
         self.sendNode = msg.arbitration_id - self.start_id
         self.controlCode = msg.data[0]
         assert self.controlCode == 0x07
@@ -53,15 +56,15 @@
             self.msgType = MSG_REQUEST
             self.verification = msg.data[2] + (msg.data[3]<<8)
             self.channel = msg.data[4]
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/twowayconnection.py` & `python-canfix-0.3.0/canfix/messages/twowayconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             self.msgType = MSG_REQUEST
             self.channel = msg.data[2]
             self.connectionType = msg.data[3] + (msg.data[4]<<8)
         else:
             raise MsgSizeError("Message size is incorrect")
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def getData(self):
```

### Comparing `python-canfix-0.2.0/canfix/messages/nodeconfiguration.py` & `python-canfix-0.3.0/canfix/messages/nodeconfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             self.valueData = msg.data[4:]
 
         self.controlCode = msg.data[0]
         assert self.controlCode == 0x09
         self.destNode = msg.data[1]
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def setKey(self, key):
@@ -147,15 +147,15 @@
 
         self.controlCode = msg.data[0]
         assert self.controlCode == 0x0A
         self.destNode = msg.data[1]
         self.rawdata = msg.data[2:]
 
     def getMessage(self):
-        msg = can.Message(arbitration_id=self.sendNode + self.start_id, extended_id=False)
+        msg = can.Message(arbitration_id=self.sendNode + self.start_id, is_extended_id=False)
         msg.data = self.data
         msg.dlc = len(msg.data)
         return msg
 
     msg = property(getMessage, setMessage)
 
     def setKey(self, key):
```

### Comparing `python-canfix-0.2.0/README.rst` & `python-canfix-0.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     >>> na = canfix.NodeAlarm()
     >>> na.node = 12
     >>> na.alarm = 45321
     >>> na.data = [4,5,6,7]
     >>> na.msg
     >>> na.msg
-    can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
     data=[0x9, 0xb1, 0x4, 0x5, 0x6, 0x7])
 
     >>> msg = bus.recv() # Assume we read the same message that we created above
     >>> na = canfix.NodeAlarm(msg)
     >>> print(na)
     [12] Node Alarm 45321 Data 04050607
 
@@ -155,15 +155,15 @@
 
     >>> pa = canfix.Parameter()
     >>> pa.node = 2
     >>> pa.value = 123.4
     >>> print(pa)
     [2] Indicated Airspeed: 123.4 knots
     >>> pa.msg
-    can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0x183,
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0x183,
     dlc=0, data=[0x2, 0x0, 0x0, 0xd2, 0x4])
 
 
 TwoWayMsg Class
 ---------------
 
 The constructor can take one named parameter.  ``msg`` can be assigned a
@@ -209,15 +209,15 @@
 returns that object.  This function would be used for most all received
 messages.
 
 Example Usage::
 
   >>> msg = bus.recv()
   >>> msg
-  can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False,
+  can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False,
   is_error_frame=False, arbitration_id=0x183, dlc=5,
   data=[0xc, 0x0, 0x0, 0xd2, 0x4])
   >>> p = canfix.parseMessage(msg)
   >>> p
   <canfix.Parameter object at 0x7f6984fe9c10>
   >>> print(p)
   [12] Indicated Airspeed: 123.4 knots
```

### Comparing `python-canfix-0.2.0/tests/utils.py` & `python-canfix-0.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/tests/node_alarm.py` & `python-canfix-0.3.0/tests/node_alarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,45 +20,45 @@
 
 class TestNodeAlarm(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_FirstNodeNoDataFromMessage(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x01, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x01, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.NodeAlarm)
         self.assertEqual(p.alarm, 1)
         self.assertEqual(p.data, b'\x00\x00\x00\x00\x00')
         self.assertEqual(p.node, 0x01)
 
     def test_LastNodeNoDataFromMessage(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0xFF, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0xFF, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.NodeAlarm)
         self.assertEqual(p.alarm, 1)
         self.assertEqual(p.data, b'\x00\x00\x00\x00\x00')
         self.assertEqual(p.node,255)
 
     def test_NodeMissingAlarmFromMessage(self):
-        msg = can.Message(extended_id=False, arbitration_id=0x01)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x01)
 
         with self.assertRaises(ValueError):
             p = canfix.parseMessage(msg)
 
     def test_ZeroNodeNotNodeAlarm(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x00, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x00, data=d)
         p = canfix.parseMessage(msg)
         self.assertNotIsInstance(p,canfix.NodeAlarm)
 
     def test_0x100NodeNotNodeAlarm(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x100, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x100, data=d)
         p = canfix.parseMessage(msg)
         self.assertNotIsInstance(p,canfix.NodeAlarm)
 
     def test_CANMessageFromNodeAlarm(self):
         p = canfix.NodeAlarm()
         p.node = 0x01
         p.alarm = 7
```

### Comparing `python-canfix-0.2.0/tests/parameter.py` & `python-canfix-0.3.0/tests/parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,21 +22,21 @@
     """In these tests we just try to spot check some parameters that represent
        different data types"""
     def setUp(self):
         pass
 
     def test_ParameterFlaps(self):
         d = bytearray([0x00, 0x00, 0x00, 0x01])
-        msg = can.Message(arbitration_id=0x100, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x100, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Flap Control Switches #1")
 
     def test_ParameterEncoder(self):
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x11B, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x11B, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Encoder Input (High Priority) #2")
         self.assertEqual(p.value, [0, 0, [False]*8])
 
         d = bytearray([0x00, 0x00, 0x00, 0xFB, 0xFF, 0x00, 0x00, 0x00])
         msg.data = d
         p = canfix.parseMessage(msg)
@@ -45,15 +45,15 @@
         d = bytearray([0x00, 0x00, 0x00, 0x05, 0x00, 0x00, 0x00, 0x00])
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertEqual(p.value, [5, 0, [False]*8])
 
     def test_ParameterPitchControlPosition(self):
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x124, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x124, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Pitch Control Position")
         self.assertEqual(p.value, 0)
 
         d = bytearray([0x00, 0x00, 0x00, 0xF0, 0xD8]) # -10,000
         msg.data = d
         p = canfix.parseMessage(msg)
@@ -67,15 +67,15 @@
         d = bytearray([0x00, 0x00, 0x00, 0x04, 0xd9]) # -9,980
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertEqual(p.value, -99.8)
 
     def test_ParameterIndicatedAirspeed(self):
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x183, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x183, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Airspeed")
         self.assertEqual(p.value, 0.0)
 
         d = bytearray([0x00, 0x00, 0x00, 0x0F, 0x27]) # 9999
         msg.data = d
         p = canfix.parseMessage(msg)
@@ -84,15 +84,15 @@
         d = bytearray([0x00, 0x00, 0x00, 0x87, 0x13]) # 4999
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertLess(abs(p.value - 499.9), 0.005)
 
     def test_ParameterIndicatedAltitude(self):
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x184, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x184, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Altitude")
         self.assertEqual(p.value, 0.0)
 
         d = bytearray([0x00, 0x00, 0x00, 0x18, 0xFC, 0xFF, 0xFF]) # -1,000
         msg.data = d
         p = canfix.parseMessage(msg)
@@ -102,15 +102,15 @@
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertEqual(p.value, 60000)
 
     def test_ParameterLatitude(self):
 
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x1C3, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x1C3, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Aircraft Position Latitude")
         self.assertEqual(p.value, 0.0)
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00, 0xB4, 0x42]) # 90.0
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertLess(abs(p.value - 90.0), 0.00005)
@@ -118,130 +118,130 @@
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00, 0xB4, 0xc2]) # 4999
         msg.data = d
         p = canfix.parseMessage(msg)
         self.assertLess(abs(p.value - -90.0), 0.00005)
 
     def test_ParameterAircraftIdentifier(self):
         d = bytearray([0x00, 0x00, 0x00, 0x37, 0x32, 0x37, 0x57, 0x42])
-        msg = can.Message(arbitration_id=0x587, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x587, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Aircraft Identifier")
         self.assertEqual(p.value, "727WB")
 
     def test_ParameterTime(self):
         d = bytearray([0x02, 0x00, 0x00, 13, 23, 59, 0x2C, 0x02])
-        msg = can.Message(arbitration_id=0x580, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x580, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Time")
         self.assertEqual(p.value, [13, 23, 59, 556])
 
     def test_ParameterDate(self):
         d = bytearray([0x02, 0x00, 0x00, 0xE0, 0x07, 7, 27])
-        msg = can.Message(arbitration_id=0x581, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x581, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Date")
         self.assertEqual(p.value, [2016, 7, 27])
 
 
     # TODO Right now parameters that don't have enough bytes will return None
     # for the value.  Is this really what we want?  Might should raise an
     # exception.
     def test_ParameterShortData(self):
         d = bytearray([0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(arbitration_id=0x184, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x184, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Altitude")
         self.assertEqual(p.value, None)
 
 
     def test_ParameterIndex(self):
         d = bytearray([0x00, 0x00, 0x00, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.index, 0)
 
         d = bytearray([0x00, 0x01, 0x00, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.index, 1)
 
         d = bytearray([0x00, 0xFF, 0x00, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.index, 255)
 
     def test_ParameterQuality(self):
         d = bytearray([0x00, 0x00, 0x00, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.annunciate, False)
         self.assertEqual(p.quality, False)
         self.assertEqual(p.failure, False)
 
         d = bytearray([0x00, 0x00, 0x01, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.annunciate, True)
         self.assertEqual(p.quality, False)
         self.assertEqual(p.failure, False)
 
         d = bytearray([0x00, 0x00, 0x02, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.annunciate, False)
         self.assertEqual(p.quality, True)
         self.assertEqual(p.failure, False)
 
         d = bytearray([0x00, 0x00, 0x04, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.annunciate, False)
         self.assertEqual(p.quality, False)
         self.assertEqual(p.failure, True)
 
         d = bytearray([0x00, 0x00, 0x07, 0xd2, 0x04])
-        msg = can.Message(arbitration_id=0x501, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x501, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Cylinder Head Temperature #2")
         self.assertEqual(p.value, 123.4)
         self.assertEqual(p.annunciate, True)
         self.assertEqual(p.quality, True)
         self.assertEqual(p.failure, True)
 
     def test_ParameterMeta(self):
         d = bytearray([0x00, 0x00, 0x00, 0x1c, 0x04]) # 1052
-        msg = can.Message(arbitration_id=0x183, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x183, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Airspeed")
         self.assertEqual(p.value, 105.2)
         self.assertEqual(p.meta, None)
 
         d = bytearray([0x00, 0x00, 0x10, 0x1c, 0x04]) # 1052
-        msg = can.Message(arbitration_id=0x183, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x183, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Airspeed")
         self.assertEqual(p.value, 105.2)
         self.assertEqual(p.meta, 'Min')
 
         d = bytearray([0x00, 0x00, 0xF0, 0x1c, 0x04]) # 1052
-        msg = can.Message(arbitration_id=0x183, extended_id=False, data=d)
+        msg = can.Message(arbitration_id=0x183, is_extended_id=False, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p.name, "Indicated Airspeed")
         self.assertEqual(p.value, 105.2)
         self.assertEqual(p.meta, 'Vy')
 
 
 class TestParameterSimpleSender(unittest.TestCase):
```

### Comparing `python-canfix-0.2.0/tests/msgtypes.py` & `python-canfix-0.3.0/tests/msgtypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,103 +20,103 @@
 
 class TestParameter(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_None(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x00, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x00, data=d)
         p = canfix.parseMessage(msg)
         self.assertEqual(p, None)
 
     def test_malformed(self):
         """
         The following should NOT assert
         """
         d = bytearray([0,0,4,0,0,0,0,0])
-        msg = can.Message(extended_id=False, arbitration_id=0xc, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0xc, data=d)
         p = canfix.parseMessage(msg)
 
         d = bytearray([1,2,3,4])
-        msg = can.Message(extended_id=False, arbitration_id=0x123, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x123, data=d)
         p = canfix.parseMessage(msg)
 
-        msg = can.Message(extended_id=False, arbitration_id=0x123, data=[0], is_error_frame=True)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x123, data=[0], is_error_frame=True)
         p = canfix.parseMessage(msg)
         self.assertTrue(p is None)
 
     def test_FirstNodeAlarm(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x01, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x01, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeAlarm)
         self.assertEqual(p.node, 0x01)
 
     def test_LastNodeAlarm(self):
         d = bytearray([0x01, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0xFF, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0xFF, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeAlarm)
         self.assertEqual(p.node, 0xFF)
 
     def test_FirstParameter(self):
         d = bytearray([0x01, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x100, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x100, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.Parameter)
         self.assertEqual(p.node, 0x01)
         self.assertEqual(p.index, 2)
         self.assertEqual(p.function, 3)
 
     def test_LastDefinedParameter(self):
         d = bytearray([0x01, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x587, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x587, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.Parameter)
         self.assertEqual(p.node, 0x01)
         self.assertEqual(p.index, 2)
         self.assertEqual(p.function, 3)
 
     # TODO Right now undefined parameters raise an excpetion.
     # def test_LastParameter(self):
     #     d = bytearray([0x01, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-    #     msg = can.Message(extended_id=False, arbitration_id=0x6DF, data=d)
+    #     msg = can.Message(is_extended_id=False, arbitration_id=0x6DF, data=d)
     #     p = canfix.parseMessage(msg)
     #     self.assertIsInstance(p, canfix.Parameter)
     #     self.assertEqual(p.node, 0x01)
     #     self.assertEqual(p.index, 2)
     #     self.assertEqual(p.function, 3)
 
     def test_FirstTwoWayMessage(self):
         d = bytearray([0x01, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x7E0, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7E0, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.TwoWayMsg)
         self.assertEqual(p.channel, 0x00)
         self.assertEqual(p.type, "Request")
 
     def test_LastTwoWayMessage(self):
         d = bytearray([0x01, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x7FF, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7FF, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.TwoWayMsg)
         self.assertEqual(p.channel, 0x0F)
         self.assertEqual(p.type, "Response")
 
     def test_FirstNodeSpecificMessage(self):
         d = bytearray([0x61, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E0, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E0, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeSpecific)
         self.assertEqual(p.sendNode, 0x00)
         self.assertEqual(p.controlCode, 0x61)
 
     def test_LastNodeSpecificMessage(self):
         d = bytearray([0x61, 0x02, 0x03, 0x00, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x7DF, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7DF, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeSpecific)
         self.assertEqual(p.sendNode, 0xFF)
         self.assertEqual(p.controlCode, 0x61)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `python-canfix-0.2.0/tests/two_way_msg.py` & `python-canfix-0.3.0/tests/two_way_msg.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,76 +21,76 @@
 
 class TestTwoWayMessage(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_RequestMessageCh0(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=TWOWAY_CONN_CHANS, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=TWOWAY_CONN_CHANS, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 0x00)
         self.assertEqual(p.type,"Request")
 
     def test_RequestMessageCh1(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 0x01)
         self.assertEqual(p.type,"Request")
 
     def test_RequestMessageCh15(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 14, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 14, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 7)
         self.assertEqual(p.type,"Request")
 
     def test_RequestMessageCh0NoData(self):
-        msg = can.Message(extended_id=False, arbitration_id=TWOWAY_CONN_CHANS)
+        msg = can.Message(is_extended_id=False, arbitration_id=TWOWAY_CONN_CHANS)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data,b'')
         self.assertEqual(p.channel, 0x00)
         self.assertEqual(p.type,"Request")
 
     def test_ResponseMessageCh0(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=0x7E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 0x00)
         self.assertEqual(p.type,"Response")
 
     def test_ResponseMessageCh1(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=0x7E3, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7E3, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 0x01)
         self.assertEqual(p.type,"Response")
 
     def test_ResponseMessageCh15(self):
         d = bytearray([0x01, 0x00, 0xAB, 0xCD, 0xEF, 0xFF, 0xEE, 0x11])
-        msg = can.Message(extended_id=False, arbitration_id=0x7FF, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x7FF, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data, b'\x01\x00\xAB\xCD\xEF\xFF\xEE\x11')
         self.assertEqual(p.channel, 0x0F)
         self.assertEqual(p.type,"Response")
 
     def test_ResponseMessageCh0NoData(self):
-        msg = can.Message(extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 1)
+        msg = can.Message(is_extended_id=False, arbitration_id=TWOWAY_CONN_CHANS + 1)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p,canfix.TwoWayMsg)
         self.assertEqual(p.data,b'')
         self.assertEqual(p.channel, 0x00)
         self.assertEqual(p.type,"Response")
 
     def test_CANMessageRequestCh0(self):
```

### Comparing `python-canfix-0.2.0/tests/node_specific.py` & `python-canfix-0.3.0/tests/node_specific.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,32 +22,32 @@
 
 class TestNodeSpecific(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeSpecificMessage(self):
         d = bytearray([0x61, 0x02, 0x03, 0x40, 0x50, 0x60, 0x70, 0x80])
-        msg = can.Message(extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeSpecific)
         self.assertEqual(p.sendNode, 0x00)
         self.assertEqual(p.controlCode, 0x61)
         self.assertEqual(p.data, bytearray([0x02, 0x03, 0x40, 0x50, 0x60, 0x70, 0x80]))
 
         d = bytearray([0x61, 0x02, 0x03, 0x40, 0x50, 0x60, 0x70, 0x80])
-        msg = can.Message(extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS + 255, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS + 255, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeSpecific)
         self.assertEqual(p.sendNode, 0xFF)
         self.assertEqual(p.controlCode, 0x61)
         self.assertEqual(p.data, bytearray([0x02, 0x03, 0x40, 0x50, 0x60, 0x70, 0x80]))
 
     def test_NodeSpecificMessageNoData(self):
         d = bytearray([0x61])
-        msg = can.Message(extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=NODE_SPECIFIC_MSGS, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeSpecific)
         self.assertEqual(p.sendNode, 0x00)
         self.assertEqual(p.controlCode, 0x61)
 
     def test_NodeSpecificCANMessage(self):
         p = canfix.NodeSpecific()
@@ -82,15 +82,16 @@
 
     # TODO is this the behaviour that we want?  Should it pass?
     def test_NodeSpecificCANMessageCCNotSet(self):
         p = canfix.NodeSpecific()
         p.sendNode = 23
         p.destNode = 1
         #p.controlCode = 0xFF
-        m = p.msg
+        with self.assertRaises(TypeError):
+            m = p.msg
 
     # def test_NodeSpecific_setNodeIdentification(self):
     #     # Test the setNodeIdentification() Function
     #     p = canfix.NodeSpecific()
     #     p.sendNode = 21
     #     p.destNode = 22
     #     p.setNodeIdentification(0x23, 0x01, 0x010203)
@@ -111,42 +112,42 @@
 
 class TestNodeIdentification(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeIdentificationMessageRequest(self):
         d = bytearray([0x00, 0x02])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeIdentification)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x00)
         self.assertEqual(p.destNode, 0x02)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
 
     def test_NodeIdentificationMessageResponse(self):
         d = bytearray([0x00, 0x02, 0x01, 0x40, 0x50, 0x60, 0x70, 0x80])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeIdentification)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x00)
         self.assertEqual(p.destNode, 0x02)
         self.assertEqual(p.device, 0x40)
         self.assertEqual(p.fwrev, 0x50)
         self.assertEqual(p.model, 8417376)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
 
     def test_NodeIdentificationMessageSizeError(self):
         d = bytearray([0x00, 0x02, 0x01, 0x40, 0x50, 0x60, 0x70])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
         d = bytearray([0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
 
 
     def test_NodeIdentificationBuildResponse(self):
         n = canfix.NodeIdentification(device=12, fwrev=22, model=76543)
         n.sendNode = 0x01
@@ -180,36 +181,36 @@
 
 class TestBitRateSet(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_BitRateSetMessageRequest(self):
         d = bytearray([0x01, 0x02, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.BitRateSet)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x01)
         self.assertEqual(p.destNode, 0x02)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.bitrate, 1)
 
     def test_BitRateSetMessageResponse(self):
         d = bytearray([0x01, 0x02])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.BitRateSet)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x01)
         self.assertEqual(p.destNode, 0x02)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
 
         d = bytearray([0x01, 0x02, 0xFF])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.BitRateSet)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x01)
         self.assertEqual(p.destNode, 0x02)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_FAIL)
@@ -263,15 +264,15 @@
 
 class TestNodeIDSet(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeIDSetMessageRequest(self):
         d = bytearray([0x02, 0x03, 0x04])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeIDSet)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x02)
         self.assertEqual(p.destNode, 0x03)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.newNode, 4)
@@ -290,19 +291,19 @@
         n.destNode = 0x01
         n.msgType = canfix.MSG_RESPONSE
         self.assertEqual(n.msg.arbitration_id, NODE_SPECIFIC_MSGS+0x03)
         self.assertEqual(n.msg.data, bytearray([0x02, 0x01, 0x00]))
 
     def test_NodeIDSetMsgSizeError(self):
         d = bytearray([0x02, 0x03, 0x04, 0x05])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
         d = bytearray([0x02, 0x03])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
 
     def test_NodeIDSetNodeIDError(self):
         n = canfix.NodeIDSet()
         n.sendNode = 0x05
         n.destNode = 0x01
@@ -314,36 +315,36 @@
 
 class TestDisableParameter(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_DisableParameterMessageRequest(self):
         d = bytearray([0x03, 0x04, 0x05, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.DisableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x03)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.identifier, 261)
 
     def test_DisableParameterMessageResponse(self):
         d = bytearray([0x03, 0x04, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.DisableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x03)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
 
         d = bytearray([0x03, 0x04, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.DisableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x03)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_FAIL)
@@ -376,19 +377,19 @@
         self.assertEqual(n.msg.data, bytearray([0x03, 0x01, 0x00]))
 
         n.status = canfix.MSG_FAIL
         self.assertEqual(n.msg.data, bytearray([0x03, 0x01, 0x01]))
 
     def test_DisableParameterMsgSizeError(self):
         d = bytearray([0x03, 0x03, 0x04, 0x05, 0x06])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
         d = bytearray([0x03, 0x03])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
 
     def test_DisableParameterNodeIDError(self):
         n = canfix.DisableParameter()
         n.sendNode = 0x05
         n.destNode = 0x01
@@ -404,36 +405,36 @@
 
 class TestEnableParameter(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_EnableParameterMessageRequest(self):
         d = bytearray([0x04, 0x04, 0x05, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.EnableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x04)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.identifier, 261)
 
     def test_EnableParameterMessageResponse(self):
         d = bytearray([0x04, 0x04, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.EnableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x04)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
 
         d = bytearray([0x04, 0x04, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.EnableParameter)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x04)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.status, canfix.MSG_FAIL)
@@ -466,19 +467,19 @@
         self.assertEqual(n.msg.data, bytearray([0x04, 0x01, 0x00]))
 
         n.status = canfix.MSG_FAIL
         self.assertEqual(n.msg.data, bytearray([0x04, 0x01, 0x01]))
 
     def test_EnableParameterMsgSizeError(self):
         d = bytearray([0x04, 0x03, 0x04, 0x05, 0x06])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
         d = bytearray([0x04, 0x03])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         with self.assertRaises(canfix.MsgSizeError):
             p = canfix.parseMessage(msg)
 
     def test_EnableParameterNodeIDError(self):
         n = canfix.EnableParameter()
         n.sendNode = 0x05
         n.destNode = 0x01
@@ -494,15 +495,15 @@
 
 class TestNodeReport(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeReportMessageRequest(self):
         d = bytearray([0x05, 0x04])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E1, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E1, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeReport)
         self.assertEqual(p.sendNode, 0x01)
         self.assertEqual(p.controlCode, 0x05)
         self.assertEqual(p.destNode, 0x04)
 
     def test_NodeReportBuildRequest(self):
@@ -515,15 +516,15 @@
 
 class TestNodeStatus(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeStatusMessage(self):
         d = bytearray([0x06, 0x00, 0x00, 0x00, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         p.type = "WORD"
         self.assertIsInstance(p, canfix.NodeStatus)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.controlCode, 0x06)
         self.assertEqual(p.parameter, 0x00)
         self.assertEqual(p.value, [False]*16)
@@ -541,17 +542,17 @@
     def test_NodeStatusAllParametersBuild(self):
         wordval = [False]*16
         wordval[2] = True
         wordval[15] = True
         # Parameter, Value, Result
         tests = ((0x00, wordval, [0x04, 0x80]),
                  (0x01, 73.2, [0xDC, 0x02]),
-                 (0x02, 234567, [0x47, 0x94, 0x03, 0x00]),
+                 (0x02, 14.2, [0x8E, 0x00]),
                  (0x03, 876543, [0xFF, 0x5F, 0x0D, 0x00]),
-                 (0x04, 14.2, [0x8E, 0x00]),
+                 (0x04, 234567, [0x47, 0x94, 0x03, 0x00]),
                  (0x05, 123456789, [0x15, 0xCD, 0x5B, 0x07])
                 )
         n = canfix.NodeStatus()
         n.sendNode = 0x04
         for each in tests:
             n.parameter = each[0]
             n.value = each[1]
@@ -562,39 +563,39 @@
 
 class TestUpdateFirmware(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_UpdateFirmwareMessageRequest(self):
         d = bytearray([0x07, 0x04, 0x39, 0x30, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.UpdateFirmware)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x07)
         self.assertEqual(p.verification, 12345)
         self.assertEqual(p.channel, 0)
 
     def test_UpdateFirmwareMessageResponseFail(self):
         d = bytearray([0x07, 0x04, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.UpdateFirmware)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x07)
         self.assertEqual(p.status, canfix.MSG_FAIL)
         self.assertEqual(p.errorCode, 0x01)
 
     def test_UpdateFirmwareMessageResponseSucceed(self):
         d = bytearray([0x07, 0x04, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.UpdateFirmware)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x07)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
@@ -628,39 +629,39 @@
 
 class TestTwoWayConnection(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_TwoWayConnectionMessageRequest(self):
         d = bytearray([0x08, 0x04, 0x02, 0x39, 0x30])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.TwoWayConnection)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x08)
         self.assertEqual(p.connectionType, 12345)
         self.assertEqual(p.channel, 0x02)
 
     def test_TwoWayConnectionMessageResponseFail(self):
         d = bytearray([0x08, 0x04, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.TwoWayConnection)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x08)
         self.assertEqual(p.status, canfix.MSG_FAIL)
         self.assertEqual(p.errorCode, 0x01)
 
     def test_TwoWayConnectionMessageResponseSucceed(self):
         d = bytearray([0x08, 0x04, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.TwoWayConnection)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.controlCode, 0x08)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
@@ -694,38 +695,38 @@
 
 class TestConfigurationSet(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_ConfigurationSetMessageRequest(self):
         d = bytearray([0x09, 0x04, 0x0F, 0x00, 0x55])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         p.datatype = "BYTE"
         self.assertIsInstance(p, canfix.NodeConfigurationSet)
         self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.key, 15)
         self.assertEqual(p.value, [True,False,True,False,True,False,True,False])
 
     def test_ConfigurationSetMessageResponseFail(self):
         d = bytearray([0x09, 0x05, 0x0F])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeConfigurationSet)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x05)
         self.assertEqual(p.status, canfix.MSG_FAIL)
         self.assertEqual(p.errorCode, 15)
 
     def test_ConfigurationSetMessageResponseSuccess(self):
         d = bytearray([0x09, 0x05, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeConfigurationSet)
         self.assertEqual(p.msgType, canfix.MSG_RESPONSE)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x05)
         self.assertEqual(p.status, canfix.MSG_SUCCESS)
         self.assertEqual(p.errorCode, 0)
@@ -761,36 +762,36 @@
 
 class TestConfigurationQuery(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_ConfigurationQueryMessageRequest(self):
         d = bytearray([0x0A, 0x04, 0x0F, 0x00])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeConfigurationQuery)
         #self.assertEqual(p.msgType, canfix.MSG_REQUEST)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.key, 15)
 
     def test_ConfigurationQueryMessageResponseSuccess(self):
         d = bytearray([0x0A, 0x04, 0x00, 0x55])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         p.datatype = "BYTE"
         self.assertIsInstance(p, canfix.NodeConfigurationQuery)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.error, 0x00)
         self.assertEqual(p.value, [True,False,True,False,True,False,True,False])
 
     def test_ConfigurationQueryMessageResponseFail(self):
         d = bytearray([0x0A, 0x04, 0x01])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeConfigurationQuery)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.error, 0x01)
 
     def test_ConfigurationQueryBuildRequest(self):
@@ -827,29 +828,29 @@
 
 class TestParameterSet(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_ParameterSetMessage(self):
         d = bytearray([0x0C, 0x83, 0x19, 0x0F, 0x27])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.ParameterSet)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.index, 3)
         self.assertEqual(p.type, "UINT")
         self.assertEqual(p.multiplier, 0.1)
         self.assertTrue(abs(p.value - 999.9) < 0.1)
 
     def test_ParameterSetIndexCalc(self):
         for i in range(256):
             cc = (i // 32) + 0x0C
             x = (i % 32) << 11 | 0x183
             d = bytearray([cc, x % 256, x >> 8, 0x0F, 0x27])
-            msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+            msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
             p = canfix.parseMessage(msg)
             self.assertIsInstance(p, canfix.ParameterSet)
             self.assertEqual(p.sendNode, 0x02)
             self.assertEqual(p.index, i)
 
     def test_ParameterSetBuild(self):
         n = canfix.ParameterSet(parameter="Indicated Airspeed")
@@ -869,15 +870,15 @@
 
 class TestNodeDescription(unittest.TestCase):
     def setUp(self):
         pass
 
     def test_NodeDescriptionMessage(self):
         d = bytearray([0x0B, 0x04, 0x01, 0x00, ord('A'), ord('B'), ord('C'), ord('D')])
-        msg = can.Message(extended_id=False, arbitration_id=0x6E2, data=d)
+        msg = can.Message(is_extended_id=False, arbitration_id=0x6E2, data=d)
         p = canfix.parseMessage(msg)
         self.assertIsInstance(p, canfix.NodeDescription)
         self.assertEqual(p.sendNode, 0x02)
         self.assertEqual(p.destNode, 0x04)
         self.assertEqual(p.packetnumber, 1)
         self.assertEqual(p.chars, bytearray([ord('A'), ord('B'), ord('C'), ord('D')]))
 
@@ -886,14 +887,16 @@
         n.sendNode = 0x03
         n.destNode = 0x04
         n.packetnumber = 0x13
         n.chars = "ABCD"
         self.assertEqual(n.msg.arbitration_id, NODE_SPECIFIC_MSGS+0x03)
         self.assertEqual(n.msg.data, bytearray([0x0B, 0x04, 0x13, 0x00, ord('A'), ord('B'), ord('C'), ord('D')]))
 
+          
+
 # TODO Test default destination node
 # TODO Test __str__ outputs for requests and responses
 # TODO Test error code strings
 # TODO Test Node Description Message
 
 
 if __name__ == '__main__':
```

### Comparing `python-canfix-0.2.0/tests/dataconversion.py` & `python-canfix-0.3.0/tests/dataconversion.py`

 * *Files identical despite different names*

### Comparing `python-canfix-0.2.0/python_canfix.egg-info/PKG-INFO` & `python-canfix-0.3.0/python_canfix.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,233 +1,236 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: python-canfix
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python CAN-FIX Library
 Home-page: https://github.com/birkelbach/python-canfix
 Author: Phil Birkelbach
 Author-email: phil@petrasoft.net
 License: GNU General Public License Version 2
-Description: =========================
-        Python CAN-FIX Library
-        =========================
-        
-        python-canfix is a Python package that abstracts the details of the
-        CAN-FIX communication protocol.
-        
-        CAN-FIX is the CAN bus implementation of a set of protocols and specifications
-        known as FIX. FIX stands for Flight Information eXchange and is an attempt to
-        standardize communication among aircraft systems in small aircraft.
-        
-        The project is hosted on GitHub at...
-        
-        https://github.com/birkelbach/python-canfix
-        
-        Installation
-        ============
-        
-        Install ``canfix`` with ``pip``:
-        ::
-        
-            $ pip install python-canfix
-        
-        
-        You can also install directly from the source directory by running:
-        ::
-        
-            $ python setup.py install
-        
-        The only dependency is python-can, which should be automatically installed
-        by the above commands.
-        
-        API
-        ===
-        
-        You should be familiar with the CANFIX protocol specification before using
-        this library.  CANFIX has several different message types.  Each of these
-        types is representd by a class in this library.
-        
-        
-        NodeAlarm Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``NoneAlarm.node`` - Sets or returns the node address of the node that sent (or will send) the Alarm Message.  Should be an
-        integer between 1 and 254
-        
-        ``NodeAlarm.alarm`` - Sets or returns the alarm type.  The meaning of this data is dependent on the individual node type.
-        Should be an integer between 0 and 65,535.
-        
-        ``NodeAlarm.data`` - Sets or returns a list that represents the data for this alarm.  What the data represents is dependent
-        on the specific type of node and the alarm type.  It should be a list of bytes of up to 6 bytes in length.
-        
-        ``NodeAlarm.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
-        is set with a message received from the can bus then the message will be parsed and the node, alarm and data properties
-        will be set accordingly.  If it is read then the message will be constructed with the node, alarm and data properties
-        that should have been previously set.
-        
-        Example Usage::
-        
-            >>> na = canfix.NodeAlarm()
-            >>> na.node = 12
-            >>> na.alarm = 45321
-            >>> na.data = [4,5,6,7]
-            >>> na.msg
-            >>> na.msg
-            can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
-            data=[0x9, 0xb1, 0x4, 0x5, 0x6, 0x7])
-        
-            >>> msg = bus.recv() # Assume we read the same message that we created above
-            >>> na = canfix.NodeAlarm(msg)
-            >>> print(na)
-            [12] Node Alarm 45321 Data 04050607
-        
-        
-        Parameter Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``Parameter.node`` - Sets or returns the node address of the node that sent (or will send) the Parameter.
-        Should be an integer between 1 and 254
-        
-        ``Parameter.identifier`` - Sets or returns the CAN bus identifier for this parameter.  If the identifier is out of
-        of range for Parameter messages a ValueError exception will be raised.  Setting this will also cause protocol specific
-        information to be set in the object.  This includes the data type, the engineering units, name etc.
-        
-        ``Parameter.name`` - Sets or returns the name of the parameter.  i.e. "Indicated Airspeed"  If the name is not found
-        in the protocol ValueError exception will be raised.  Setting this will also cause protocol specific
-        information to be set in the object.  This includes the data type, the engineering units, identifier etc.
-        
-        ``Parameter.index`` - Sets or returns the index of the parameter.  Should be an integer between 0 and 255.
-        
-        ``Parameter.failure`` - Sets or returns the flag that indicates data failure.  Should be ``True`` or ``False``
-        
-        ``Parameter.quality`` - Sets or returns the flag that indicates data quality.  Should be ``True`` or ``False``
-        
-        ``Parameter.annunciate`` - Sets or returns the flag that indicates the paramter should be annunciated.
-        Should be ``True`` or ``False``
-        
-        ``Parameter.meta`` - Sets or returns the meta data index for the Parameter.  Should be an integer between 0 and 15
-        
-        ``Parameter.value`` - Sets or returns the value for the parameter.  It can be a list of multiple values if the
-        particular parameter is expecting multiple values.  It can also be a string
-        
-        ``Parameter.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
-        is set with a message received from the can bus then the message will be parsed and the properties
-        will be set accordingly.  If it is read then the message will be constructed with properties
-        that should have been previously set.
-        
-        ``Parameter.fullName`` - Returns a string that represents the parameter that includes the index and the index name.
-        This property is read only.
-        
-        ``Parameter.units`` - Read only property that returns a string indicating the engineering units for this Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.type`` - Read only property that returns a string indicating the datatype for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.min`` - Read only property that returns a value that indicates the minimum value for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.max`` - Read only property that returns a value that indicates the maximum value for the Parameter.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.format`` - Read only property that returns the format of the data in the Parameter value.  This is typically
-        used to indicated what WORD and BYTE type data means.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.remarks`` - Read only property that returns a list of remarks that are associated with this Parameter
-        in the protocol specification.
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.indexName`` - Read only property that retuns he name of what the index represents.  i.e. Cylinder
-        This is a protocol specific piece of information and should not change.
-        
-        ``Parameter.multiplier`` - Read only property that returns the multiplier for the Parameter.  Some paramters use
-        an integer with a multiplier as the value in the message.  For example if we had a Parameter value of 123.4 and
-        the multiplier is 0.1 then the data that would be communicated on the bus would be 1234.  The receiver would then
-        multiply by 0.1 to get the original value of 123.4.  The ``python-canfix`` library handles these details for you
-        so you don't need to concern yourself with this detail.  It is a part of the protocol and is included here for
-        applications that want to display protocol specific information to the user.
-        This is a protocol specific piece of information and should not change.
-        
-        Example Usage::
-        
-            >>> pa = canfix.Parameter()
-            >>> pa.node = 2
-            >>> pa.value = 123.4
-            >>> print(pa)
-            [2] Indicated Airspeed: 123.4 knots
-            >>> pa.msg
-            can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False, is_error_frame=False, arbitration_id=0x183,
-            dlc=0, data=[0x2, 0x0, 0x0, 0xd2, 0x4])
-        
-        
-        TwoWayMsg Class
-        ---------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``TwoWayMsg.channel`` - Sets the channel that this message will be sent on.  There are
-        16 channels numbered 0-15
-        
-        ``TwoWayMsg.type`` - Set to either 'Request' or 'Response'  This determines which
-        side of the channel to use.
-        
-        ``TwoWayMsg.data`` - Up to eight bytes
-        
-        NodeSpecific Class
-        ------------------
-        
-        The constructor can take one named parameter.  ``msg`` can be assigned a
-        python-can ``Message`` and the instantiated object will be initialized
-        with the correct information.
-        
-        **Properties**
-        
-        ``NodeSpecific.destNode`` - Represents the node address of the node that this
-        message is addressed to.  Should be an integer between 1 and 254.
-        
-        ``NodeSpecific.controlCode`` - The control code for the messge.  Currently, valid
-        values are 0-10.  Future versions of the CAN-FIX specification may use 11-127 and
-        values from 128 to 255 are reserved for user defined functions.  The control
-        code is basically the function of the message.  See the CAN-FIX specification
-        for details.
-        
-        ``NodeSpecific.data`` - Up to 8 bytes of data that is dependent on which type
-        of message that is being sent.
-        
-        Functions
-        ---------
-        
-        ``parseMessage(msg)`` - When passed a ``Message`` this function figures
-        out what the message type is, instantiates the correct object type and
-        returns that object.  This function would be used for most all received
-        messages.
-        
-        Example Usage::
-        
-          >>> msg = bus.recv()
-          >>> msg
-          can.Message(timestamp=0.0, is_remote_frame=False, extended_id=False,
-          is_error_frame=False, arbitration_id=0x183, dlc=5,
-          data=[0xc, 0x0, 0x0, 0xd2, 0x4])
-          >>> p = canfix.parseMessage(msg)
-          >>> p
-          <canfix.Parameter object at 0x7f6984fe9c10>
-          >>> print(p)
-          [12] Indicated Airspeed: 123.4 knots
-        
 Platform: UNKNOWN
+License-File: LICENSE
+
+=========================
+Python CAN-FIX Library
+=========================
+
+python-canfix is a Python package that abstracts the details of the
+CAN-FIX communication protocol.
+
+CAN-FIX is the CAN bus implementation of a set of protocols and specifications
+known as FIX. FIX stands for Flight Information eXchange and is an attempt to
+standardize communication among aircraft systems in small aircraft.
+
+The project is hosted on GitHub at...
+
+https://github.com/birkelbach/python-canfix
+
+Installation
+============
+
+Install ``canfix`` with ``pip``:
+::
+
+    $ pip install python-canfix
+
+
+You can also install directly from the source directory by running:
+::
+
+    $ python setup.py install
+
+The only dependency is python-can, which should be automatically installed
+by the above commands.
+
+API
+===
+
+You should be familiar with the CANFIX protocol specification before using
+this library.  CANFIX has several different message types.  Each of these
+types is representd by a class in this library.
+
+
+NodeAlarm Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``NoneAlarm.node`` - Sets or returns the node address of the node that sent (or will send) the Alarm Message.  Should be an
+integer between 1 and 254
+
+``NodeAlarm.alarm`` - Sets or returns the alarm type.  The meaning of this data is dependent on the individual node type.
+Should be an integer between 0 and 65,535.
+
+``NodeAlarm.data`` - Sets or returns a list that represents the data for this alarm.  What the data represents is dependent
+on the specific type of node and the alarm type.  It should be a list of bytes of up to 6 bytes in length.
+
+``NodeAlarm.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
+is set with a message received from the can bus then the message will be parsed and the node, alarm and data properties
+will be set accordingly.  If it is read then the message will be constructed with the node, alarm and data properties
+that should have been previously set.
+
+Example Usage::
+
+    >>> na = canfix.NodeAlarm()
+    >>> na.node = 12
+    >>> na.alarm = 45321
+    >>> na.data = [4,5,6,7]
+    >>> na.msg
+    >>> na.msg
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0xc, dlc=0,
+    data=[0x9, 0xb1, 0x4, 0x5, 0x6, 0x7])
+
+    >>> msg = bus.recv() # Assume we read the same message that we created above
+    >>> na = canfix.NodeAlarm(msg)
+    >>> print(na)
+    [12] Node Alarm 45321 Data 04050607
+
+
+Parameter Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``Parameter.node`` - Sets or returns the node address of the node that sent (or will send) the Parameter.
+Should be an integer between 1 and 254
+
+``Parameter.identifier`` - Sets or returns the CAN bus identifier for this parameter.  If the identifier is out of
+of range for Parameter messages a ValueError exception will be raised.  Setting this will also cause protocol specific
+information to be set in the object.  This includes the data type, the engineering units, name etc.
+
+``Parameter.name`` - Sets or returns the name of the parameter.  i.e. "Indicated Airspeed"  If the name is not found
+in the protocol ValueError exception will be raised.  Setting this will also cause protocol specific
+information to be set in the object.  This includes the data type, the engineering units, identifier etc.
+
+``Parameter.index`` - Sets or returns the index of the parameter.  Should be an integer between 0 and 255.
+
+``Parameter.failure`` - Sets or returns the flag that indicates data failure.  Should be ``True`` or ``False``
+
+``Parameter.quality`` - Sets or returns the flag that indicates data quality.  Should be ``True`` or ``False``
+
+``Parameter.annunciate`` - Sets or returns the flag that indicates the paramter should be annunciated.
+Should be ``True`` or ``False``
+
+``Parameter.meta`` - Sets or returns the meta data index for the Parameter.  Should be an integer between 0 and 15
+
+``Parameter.value`` - Sets or returns the value for the parameter.  It can be a list of multiple values if the
+particular parameter is expecting multiple values.  It can also be a string
+
+``Parameter.msg`` - Sets or returns a can.Message class that is suitable for use with a python-can bus.  If this property
+is set with a message received from the can bus then the message will be parsed and the properties
+will be set accordingly.  If it is read then the message will be constructed with properties
+that should have been previously set.
+
+``Parameter.fullName`` - Returns a string that represents the parameter that includes the index and the index name.
+This property is read only.
+
+``Parameter.units`` - Read only property that returns a string indicating the engineering units for this Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.type`` - Read only property that returns a string indicating the datatype for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.min`` - Read only property that returns a value that indicates the minimum value for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.max`` - Read only property that returns a value that indicates the maximum value for the Parameter.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.format`` - Read only property that returns the format of the data in the Parameter value.  This is typically
+used to indicated what WORD and BYTE type data means.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.remarks`` - Read only property that returns a list of remarks that are associated with this Parameter
+in the protocol specification.
+This is a protocol specific piece of information and should not change.
+
+``Parameter.indexName`` - Read only property that retuns he name of what the index represents.  i.e. Cylinder
+This is a protocol specific piece of information and should not change.
+
+``Parameter.multiplier`` - Read only property that returns the multiplier for the Parameter.  Some paramters use
+an integer with a multiplier as the value in the message.  For example if we had a Parameter value of 123.4 and
+the multiplier is 0.1 then the data that would be communicated on the bus would be 1234.  The receiver would then
+multiply by 0.1 to get the original value of 123.4.  The ``python-canfix`` library handles these details for you
+so you don't need to concern yourself with this detail.  It is a part of the protocol and is included here for
+applications that want to display protocol specific information to the user.
+This is a protocol specific piece of information and should not change.
+
+Example Usage::
+
+    >>> pa = canfix.Parameter()
+    >>> pa.node = 2
+    >>> pa.value = 123.4
+    >>> print(pa)
+    [2] Indicated Airspeed: 123.4 knots
+    >>> pa.msg
+    can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False, is_error_frame=False, arbitration_id=0x183,
+    dlc=0, data=[0x2, 0x0, 0x0, 0xd2, 0x4])
+
+
+TwoWayMsg Class
+---------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``TwoWayMsg.channel`` - Sets the channel that this message will be sent on.  There are
+16 channels numbered 0-15
+
+``TwoWayMsg.type`` - Set to either 'Request' or 'Response'  This determines which
+side of the channel to use.
+
+``TwoWayMsg.data`` - Up to eight bytes
+
+NodeSpecific Class
+------------------
+
+The constructor can take one named parameter.  ``msg`` can be assigned a
+python-can ``Message`` and the instantiated object will be initialized
+with the correct information.
+
+**Properties**
+
+``NodeSpecific.destNode`` - Represents the node address of the node that this
+message is addressed to.  Should be an integer between 1 and 254.
+
+``NodeSpecific.controlCode`` - The control code for the messge.  Currently, valid
+values are 0-10.  Future versions of the CAN-FIX specification may use 11-127 and
+values from 128 to 255 are reserved for user defined functions.  The control
+code is basically the function of the message.  See the CAN-FIX specification
+for details.
+
+``NodeSpecific.data`` - Up to 8 bytes of data that is dependent on which type
+of message that is being sent.
+
+Functions
+---------
+
+``parseMessage(msg)`` - When passed a ``Message`` this function figures
+out what the message type is, instantiates the correct object type and
+returns that object.  This function would be used for most all received
+messages.
+
+Example Usage::
+
+  >>> msg = bus.recv()
+  >>> msg
+  can.Message(timestamp=0.0, is_remote_frame=False, is_extended_id=False,
+  is_error_frame=False, arbitration_id=0x183, dlc=5,
+  data=[0xc, 0x0, 0x0, 0xd2, 0x4])
+  >>> p = canfix.parseMessage(msg)
+  >>> p
+  <canfix.Parameter object at 0x7f6984fe9c10>
+  >>> print(p)
+  [12] Indicated Airspeed: 123.4 knots
+
+
```

### Comparing `python-canfix-0.2.0/python_canfix.egg-info/SOURCES.txt` & `python-canfix-0.3.0/python_canfix.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 canfix/__init__.py
 canfix/canfix.json
 canfix/globals.py
 canfix/protocol.py
 canfix/utils.py
```

