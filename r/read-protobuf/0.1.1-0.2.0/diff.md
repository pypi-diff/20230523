# Comparing `tmp/read-protobuf-0.1.1.tar.gz` & `tmp/read-protobuf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/read-protobuf-0.1.1.tar", last modified: Fri Apr  6 02:25:34 2018, max compression
+gzip compressed data, was "read-protobuf-0.2.0.tar", last modified: Tue May 23 11:27:30 2023, max compression
```

## Comparing `read-protobuf-0.1.1.tar` & `read-protobuf-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/
--rw-r--r--   0 marcus     (501) staff       (20)     5629 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/PKG-INFO
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/tests/
--rw-r--r--   0 marcus     (501) staff       (20)      282 2018-04-05 17:45:03.000000 read-protobuf-0.1.1/tests/conftest.py
--rw-r--r--   0 marcus     (501) staff       (20)        0 2018-03-25 17:10:01.000000 read-protobuf-0.1.1/tests/__init__.py
--rw-r--r--   0 marcus     (501) staff       (20)     4547 2018-04-06 02:09:27.000000 read-protobuf-0.1.1/tests/test_read.py
--rw-r--r--   0 marcus     (501) staff       (20)     5707 2018-04-05 18:01:43.000000 read-protobuf-0.1.1/tests/demo_pb2.py
--rw-r--r--   0 marcus     (501) staff       (20)     4170 2018-04-06 01:39:01.000000 read-protobuf-0.1.1/README.md
--rw-r--r--   0 marcus     (501) staff       (20)     4361 2018-04-06 02:21:34.000000 read-protobuf-0.1.1/read_protobuf.py
--rw-r--r--   0 marcus     (501) staff       (20)      659 2018-04-06 02:24:51.000000 read-protobuf-0.1.1/setup.py
--rw-r--r--   0 marcus     (501) staff       (20)       78 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/setup.cfg
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     5629 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      302 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)       27 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)       14 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/top_level.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2018-04-06 02:25:34.000000 read-protobuf-0.1.1/read_protobuf.egg-info/dependency_links.txt
+drwxr-xr-x   0 marcshapiro   (501) staff       (20)        0 2023-05-23 11:27:30.617730 read-protobuf-0.2.0/
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     1070 2023-05-23 09:30:38.000000 read-protobuf-0.2.0/LICENSE
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     3037 2023-05-23 11:27:30.617359 read-protobuf-0.2.0/PKG-INFO
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     2586 2023-05-23 11:25:30.000000 read-protobuf-0.2.0/README.md
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     1437 2023-05-23 11:20:19.000000 read-protobuf-0.2.0/pyproject.toml
+drwxr-xr-x   0 marcshapiro   (501) staff       (20)        0 2023-05-23 11:27:30.613798 read-protobuf-0.2.0/read_protobuf.egg-info/
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     3037 2023-05-23 11:27:30.000000 read-protobuf-0.2.0/read_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 marcshapiro   (501) staff       (20)      252 2023-05-23 11:27:30.000000 read-protobuf-0.2.0/read_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 marcshapiro   (501) staff       (20)        1 2023-05-23 11:27:30.000000 read-protobuf-0.2.0/read_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 marcshapiro   (501) staff       (20)      156 2023-05-23 11:27:30.000000 read-protobuf-0.2.0/read_protobuf.egg-info/requires.txt
+-rw-r--r--   0 marcshapiro   (501) staff       (20)       14 2023-05-23 11:27:30.000000 read-protobuf-0.2.0/read_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     4548 2023-05-23 10:59:23.000000 read-protobuf-0.2.0/read_protobuf.py
+-rw-r--r--   0 marcshapiro   (501) staff       (20)       38 2023-05-23 11:27:30.617802 read-protobuf-0.2.0/setup.cfg
+drwxr-xr-x   0 marcshapiro   (501) staff       (20)        0 2023-05-23 11:27:30.616978 read-protobuf-0.2.0/tests/
+-rw-r--r--   0 marcshapiro   (501) staff       (20)     4205 2023-05-23 10:59:23.000000 read-protobuf-0.2.0/tests/test_read.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `read-protobuf-0.1.1/tests/test_read.py` & `read-protobuf-0.2.0/tests/test_read.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,187 @@
-"""
-Test util.py methods
-"""
-
 import os
-import pytest
+
 import pandas as pd
+import pytest
+
 from read_protobuf import read_protobuf
 
 from . import demo_pb2
 
 
 def write_demo(n=100):
     """Write demo pb string
 
     Args:
-      n (int, optional): number of entries in the demo pb record
+        n (int, optional): number of entries in the demo pb record
 
     Returns:
-      byte-string: serialized pb string
+        byte-string: serialized pb string
     """
 
     Collection = demo_pb2.Collection()
     Record = demo_pb2.Record()
 
     Record.int = 1234
     Record.float = 43.685
-    Record.nested.data = 1.2        #pylint: disable=E1101
-    Record.rep.extend([1])          #pylint: disable=E1101
-    Record.rep.extend([2])          #pylint: disable=E1101
+    Record.nested.data = 1.2  # pylint: disable=E1101
+    Record.rep.extend([1])  # pylint: disable=E1101
+    Record.rep.extend([2])  # pylint: disable=E1101
 
     RecordTwo = demo_pb2.Record()
     RecordTwo.int = 1253135
     RecordTwo.float = -73.2324
 
     # add both types of records at random
     for i in range(n):
         if i % 5 == 0:
-            Collection.records.extend([RecordTwo])  #pylint: disable=E1101
+            Collection.records.extend([RecordTwo])  # pylint: disable=E1101
         else:
-            Collection.records.extend([Record]) #pylint: disable=E1101
+            Collection.records.extend([Record])  # pylint: disable=E1101
 
     return Collection.SerializeToString()
 
-def write_demo_file(name='demo.pb'):
+
+def write_demo_file(name="demo.pb") -> str:
     """Write demo pb file
 
     Returns:
         str: path to demo file
     """
 
     Message = write_demo()
     pwd = os.path.dirname(os.path.realpath(__file__))
-    path = '{}/{}'.format(pwd, name)
+    path = "{}/{}".format(pwd, name)
 
-    with open(path, 'wb') as f:
+    with open(path, "wb") as f:
         f.write(Message)
 
     return path
 
 
-class TestRead(object):
-    """Test read-protobuf methods"""
+def test_read_bytes():
+    """test input serialized bytes"""
+
+    Message = write_demo()
+    Collection = demo_pb2.Collection()
+    df = read_protobuf(Message, Collection)
+
+    assert df is not None and isinstance(df, pd.DataFrame)
+
+
+def test_read_file() -> None:
+    """test input file path"""
+
+    path = write_demo_file()
+    Collection = demo_pb2.Collection()
+    df = read_protobuf(path, Collection)
+
+    assert df is not None and isinstance(df, pd.DataFrame)
+
 
-    def test_read_bytes(self):
-        """test input serialized bytes"""
+def test_defaults() -> None:
+    """test default inputs"""
 
-        Message = write_demo()
-        Collection = demo_pb2.Collection()
-        df = read_protobuf(Message, Collection)
+    Message = write_demo()
+    Collection = demo_pb2.Collection()
 
-        assert df is not None and isinstance(df, pd.DataFrame)
+    df = read_protobuf(Message, Collection)
 
+    assert "data" in df.columns
 
-    def test_read_file(self):
-        """test input file path"""
 
-        path = write_demo_file()
-        Collection = demo_pb2.Collection()
-        df = read_protobuf(path, Collection)
+def test_flatten() -> None:
+    """test flatten option"""
 
-        assert df is not None and isinstance(df, pd.DataFrame)
+    Message = write_demo()
+    Collection = demo_pb2.Collection()
 
-    def test_defaults(self):
-        """test default inputs"""
+    df = read_protobuf(Message, Collection, flatten=False)
 
-        Message = write_demo()
-        Collection = demo_pb2.Collection()
+    assert "records" in df.columns and len(df.columns) == 1
 
-        df = read_protobuf(Message, Collection)
 
-        assert 'data' in df.columns
+def test_prefix() -> None:
+    """test prefix option"""
 
-    def test_flatten(self):
-        """test flatten option"""
+    Message = write_demo()
+    Collection = demo_pb2.Collection()
 
-        Message = write_demo()
-        Collection = demo_pb2.Collection()
+    df = read_protobuf(Message, Collection, prefix_nested=True)
 
-        df = read_protobuf(Message, Collection, flatten=False)
+    assert "nested.data" in df.columns
 
-        assert 'records' in df.columns and len(df.columns) == 1
 
-    def test_prefix(self):
-        """test prefix option"""
+def test_multiple_input_bytes() -> None:
+    """test input multiple bytes"""
 
-        Message = write_demo()
-        Collection = demo_pb2.Collection()
+    Message = write_demo(n=29)
+    Message2 = write_demo(n=5)
 
-        df = read_protobuf(Message, Collection, prefix_nested=True)
+    Collection = demo_pb2.Collection()
 
-        assert 'nested.data' in df.columns
+    df = read_protobuf([Message, Message2], Collection)
 
-    def test_multiple_input_bytes(self):
-        """test input multiple bytes"""
+    assert df is not None and isinstance(df, pd.DataFrame)
 
-        Message = write_demo(n=29)
-        Message2 = write_demo(n=5)
 
-        Collection = demo_pb2.Collection()
+def test_multiple_input_files() -> None:
+    """test input multiple files"""
 
-        df = read_protobuf([Message, Message2], Collection)
+    path1 = write_demo_file()
+    path2 = write_demo_file("demo2.pb")
 
-        assert df is not None and isinstance(df, pd.DataFrame)
+    Collection = demo_pb2.Collection()
 
-    def test_multiple_input_files(self):
-        """test input multiple files"""
+    df = read_protobuf([path1, path2], Collection)
 
-        path1 = write_demo_file()
-        path2 = write_demo_file('demo2.pb')
+    assert df is not None and isinstance(df, pd.DataFrame)
 
-        Collection = demo_pb2.Collection()
 
-        df = read_protobuf([path1, path2], Collection)
+def test_multiple_input_types() -> None:
+    """test input multiple files and strings"""
 
-        assert df is not None and isinstance(df, pd.DataFrame)
+    Message = write_demo(n=29)
+    path2 = write_demo_file("demo2.pb")
 
+    Collection = demo_pb2.Collection()
 
-    def test_multiple_input_types(self):
-        """test input multiple files and strings"""
+    df = read_protobuf([Message, path2], Collection)
 
-        Message = write_demo(n=29)
-        path2 = write_demo_file('demo2.pb')
+    assert df is not None and isinstance(df, pd.DataFrame)
 
-        Collection = demo_pb2.Collection()
 
-        df = read_protobuf([Message, path2], Collection)
+def test_invalid_pb() -> None:
+    """test invalid pb class"""
 
-        assert df is not None and isinstance(df, pd.DataFrame)
+    Message = write_demo()
+    Collection = demo_pb2.Collection()
 
-    def test_invalid_pb(self):
-        """test invalid pb class"""
+    Record = demo_pb2.Record()
+    Record.int = 1234
+    Record.float = 43.685
+    Message2 = Record.SerializeToString()
 
-        Message = write_demo()
-        Collection = demo_pb2.Collection()
+    df = read_protobuf([Message, Message2], Collection)
 
-        Record = demo_pb2.Record()
-        Record.int = 1234
-        Record.float = 43.685
-        Message2 = Record.SerializeToString()
+    assert df is not None and isinstance(df, pd.DataFrame)
 
-        df = read_protobuf([Message, Message2], Collection)
+    with pytest.raises(ValueError):
+        df = read_protobuf([Message2], Collection)
 
-        assert df is not None and isinstance(df, pd.DataFrame)
 
-        with pytest.raises(ValueError):
-            df = read_protobuf([Message2], Collection)
+def test_invalid_input_path() -> None:
+    """test invalid input filepath"""
 
-    def test_invalid_input_path(self):
-        """test invalid input filepath"""
+    Collection = demo_pb2.Collection()
 
-        Collection = demo_pb2.Collection()
+    with pytest.raises(IOError):
+        read_protobuf("message", Collection)
 
-        with pytest.raises(IOError):
-            read_protobuf('message', Collection)
 
-    def test_invalid_input(self):
-        """test invalid input pb type"""
+def test_invalid_input() -> None:
+    """test invalid input pb type"""
 
-        Collection = demo_pb2.Collection()
+    Collection = demo_pb2.Collection()
 
-        with pytest.raises(TypeError):
-            read_protobuf(123, Collection)
+    with pytest.raises(TypeError):
+        read_protobuf(123, Collection)
```

### Comparing `read-protobuf-0.1.1/read_protobuf.py` & `read-protobuf-0.2.0/read_protobuf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,145 +1,160 @@
 """
 read-protobuf
 
-Attributes:
-    DEFAULTS (dict): Default inputs
+Small library to read serialized protobuf(s) directly into Pandas DataFrame
 """
 
-import pandas as pd
-
-DEFAULTS = {
-    'flatten': True,
-    'prefix_nested': False
-}
-
-
-class ProtobufReader(object):
-    """ ProtobufReader class to handle interpretation"""
+from __future__ import annotations
 
-    def __init__(self, flatten=DEFAULTS['flatten'],
-                       prefix_nested=DEFAULTS['prefix_nested']):
+from typing import Any
 
-        self.flatten = flatten
-        self.prefix_nested = prefix_nested
-
-    def to_array(self, Message, field=None):
-        """Convert an arbitrary message to an array
+import google
+import pandas as pd
 
-        Args:
-            Message (TYPE): Description
-            field (string, optional): field within message to convert to array
+DEFAULT_FLATTEN = True
+DEFAULT_PREFIX_NESTED = False
 
-        Returns:
-            TYPE: Description
-        """
-        if field:
-            array = [self.interpret_message(m) for m in getattr(Message, field)]
-        else:
-            array = [self.interpret_message(Message)]
 
-        return array
+def _to_array(
+    message, flatten: bool, prefix_nested: bool, field: str = None
+) -> list[dict[str, Any]]:
+    """Convert an arbitrary message to an array
+
+    Parameters
+    ----------
+    message : TYPE
+        Description
+    flatten : bool
+        See `read_protobuf`
+    prefix_nested : bool
+        See `read_protobuf`
+    field : str, optional
+        Field within message to convert to array
+
+    Returns
+    -------
+    list[dict[str, Any]]
+        List of interpreted messages
+    """
+    if field:
+        arr = [_interpret_message(m, flatten, prefix_nested) for m in getattr(message, field)]
+    else:
+        arr = [_interpret_message(message, flatten, prefix_nested)]
+
+    return arr
+
+
+def _interpret_message(message, flatten: bool, prefix_nested: bool) -> dict[str, Any]:
+    """Interpret a message into a dict or array.
+
+    Parameters
+    ----------
+    message : TYPE
+        Description
+    flatten : bool
+        See `read_protobuf`
+    prefix_nested : bool
+        See `read_protobuf`
+
+    Returns
+    -------
+    dict[str, Any]
+    """
 
-    def interpret_message(self, Message):
-        """Interpret a message into a dict or array
+    data = {}  # default to dict
+    for field in message.ListFields():
+        # repeated nested message
+        if field[0].type == field[0].TYPE_MESSAGE and field[0].label == field[0].LABEL_REPEATED:
+            # is this the only field in the pb? if so, look at flatten
+            if len(message.ListFields()) == 1 and flatten:
+                data = _to_array(message, flatten, prefix_nested, field[0].name)
 
-        Args:
-            Message (TYPE): Description
-
-        Returns:
-            dict | list: protobuf message interpreted into a list or dict
-        """
-
-        data = {}  # default to dict
-        for field in Message.ListFields():
-
-            # repeated nested message
-            if field[0].type == field[0].TYPE_MESSAGE and field[0].label == field[0].LABEL_REPEATED:
-
-                # is this the only field in the pb? if so, look at flatten
-                if len(Message.ListFields()) == 1 and self.flatten:
-                    data = self.to_array(Message, field[0].name)
-
-                # if there are multiple repeated messages in object, set as keys
-                else:
-                    data[field[0].name] = self.to_array(Message, field[0].name)
-
-            # nested message
-            elif field[0].type == field[0].TYPE_MESSAGE:
-                if self.flatten:
-                    nested_dict = self.interpret_message(field[1])
-                    for key in nested_dict:
-                        if key in data or self.prefix_nested:
-                            data['{}.{}'.format(field[0].name, key)] = nested_dict[key]
-                        else:
-                            data[key] = nested_dict[key]
-                else:
-                    data[field[0].name] = self.interpret_message(field[1])
-
-            # repeated scalar
-            elif field[0].label == field[0].LABEL_REPEATED:
-                data[field[0].name] = list(field[1])
+            # if there are multiple repeated messages in object, set as keys
+            else:
+                data[field[0].name] = _to_array(message, flatten, prefix_nested, field[0].name)
 
-            # scalar
+        # nested message
+        elif field[0].type == field[0].TYPE_MESSAGE:
+            if flatten:
+                nested_dict = _interpret_message(field[1], flatten, prefix_nested)
+                for key in nested_dict:
+                    if key in data or prefix_nested:
+                        data["{}.{}".format(field[0].name, key)] = nested_dict[key]
+                    else:
+                        data[key] = nested_dict[key]
             else:
-                data[field[0].name] = field[1]
+                data[field[0].name] = _interpret_message(field[1], flatten, prefix_nested)
 
-        return data
+        # repeated scalar
+        elif field[0].label == field[0].LABEL_REPEATED:
+            data[field[0].name] = list(field[1])
 
+        # scalar
+        else:
+            data[field[0].name] = field[1]
 
-def read_protobuf(pb, MessageType, flatten=DEFAULTS['flatten'],
-                               prefix_nested=DEFAULTS['prefix_nested']):
-    """Summary
+    return data
 
-    Args:
-        pb (string | bytes |list): file path to pb file(s) or bytes from pb file(s). Multiple entries allowed in list.
-        MessageType (google.protobuf.message.Message): Message class of pb message
-        flatten (bool, optional): flatten all nested objects into a 2-d dataframe. This will also collapse  repeated message containers
-        prefix_nested (bool, optional): prefix all flattened objects with parent keys
 
-    Returns:
-        DataFrame: pandas dataframe with interpreted pb data
+def read_protobuf(
+    pb: str | bytes | list,
+    MessageType: google.protobuf.message.Message,
+    flatten: bool = DEFAULT_FLATTEN,
+    prefix_nested: bool = DEFAULT_PREFIX_NESTED,
+) -> pd.DataFrame:
+    """Read protobuf file(s) or bytes into a Pandas DataFrame.
+
+    Parameters
+    ----------
+    pb : string | bytes | list
+        File path to pb file(s) or bytes from pb file(s).
+        Multiple entries allowed in list.
+    MessageType : google.protobuf.message.Message
+        Message class of pb message
+    flatten : bool, optional
+        Flatten all nested objects into a 2-d dataframe.
+        This will also collapse repeated message containers
+    prefix_nested : bool, optional
+        Prefix all flattened objects with parent keys
+
+    Returns
+    -------
+    DataFrame
+        Pandas DataFrame with interpreted pb data
     """
 
     # message parsing
     if not isinstance(pb, list):
         pb = [pb]
 
     raw = bytes()
     for entry in pb:
-
         if isinstance(entry, bytes):
-
             # python 2 interprets "bytes" as "str"
             # if the entry can be decoded as ascii, treat as a path
             try:
-                entry.decode('ascii')
-                with open(entry, 'rb') as f:
+                entry.decode("ascii")
+                with open(entry, "rb") as f:
                     raw += f.read()
             except (UnicodeDecodeError, AttributeError):
                 raw += entry
 
         elif isinstance(entry, str):
-
-            with open(entry, 'rb') as f:
+            with open(entry, "rb") as f:
                 raw += f.read()
 
         else:
-            raise TypeError('unknown input source for protobuf')
+            raise TypeError("unknown input source for protobuf")
 
     # parse concatenated message
-    Message = MessageType.FromString(raw)
+    message = MessageType.FromString(raw)
 
     # check message
-    if not Message.ListFields():
-        raise ValueError('Parsed message is empty')
-
-    # instantiate reader
-    reader = ProtobufReader(flatten, prefix_nested)
+    if not message.ListFields():
+        raise ValueError("Parsed message is empty")
 
     # intepret message
-    data = reader.interpret_message(Message)
+    data = _interpret_message(message, flatten, prefix_nested)
 
     # put data into frame
-    df = pd.DataFrame(data)
-
-    return df
+    return pd.DataFrame(data)
```

