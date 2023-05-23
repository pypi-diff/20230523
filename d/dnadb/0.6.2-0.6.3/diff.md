# Comparing `tmp/dnadb-0.6.2.tar.gz` & `tmp/dnadb-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.6.2.tar", last modified: Tue May 23 05:25:33 2023, max compression
+gzip compressed data, was "dnadb-0.6.3.tar", last modified: Tue May 23 07:19:48 2023, max compression
```

## Comparing `dnadb-0.6.2.tar` & `dnadb-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.2/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 05:25:33.525107 dnadb-0.6.2/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.2/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 05:23:54.000000 dnadb-0.6.2/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 05:25:33.525107 dnadb-0.6.2/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.521106 dnadb-0.6.2/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 05:24:04.000000 dnadb-0.6.2/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.2/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.2/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.2/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.2/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.2/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.2/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5115 2023-05-23 05:23:05.000000 dnadb-0.6.2/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7840 2023-05-23 05:23:22.000000 dnadb-0.6.2/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6057 2023-05-23 05:23:27.000000 dnadb-0.6.2/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    11231 2023-05-23 05:23:36.000000 dnadb-0.6.2/src/dnadb/sample.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.2/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.2/src/dnadb/types.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.2/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.3/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 07:19:48.883777 dnadb-0.6.3/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.3/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 07:17:21.000000 dnadb-0.6.3/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 07:19:48.883777 dnadb-0.6.3/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 07:17:33.000000 dnadb-0.6.3/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.3/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.3/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.3/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.3/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.3/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.3/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4958 2023-05-23 07:14:31.000000 dnadb-0.6.3/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     8047 2023-05-23 07:16:22.000000 dnadb-0.6.3/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6278 2023-05-23 07:17:08.000000 dnadb-0.6.3/src/dnadb/fastq.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/integration/
+-rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-23 06:13:30.000000 dnadb-0.6.3/src/dnadb/integration/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.883777 dnadb-0.6.3/src/dnadb/integration/tf/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       18 2023-05-23 06:20:23.000000 dnadb-0.6.3/src/dnadb/integration/tf/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     3200 2023-05-23 06:56:03.000000 dnadb-0.6.3/src/dnadb/integration/tf/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11231 2023-05-23 05:23:36.000000 dnadb-0.6.3/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.3/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.3/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.3/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 07:19:48.879777 dnadb-0.6.3/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      644 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 07:19:48.000000 dnadb-0.6.3/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.6.2/LICENSE` & `dnadb-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/PKG-INFO` & `dnadb-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.2/pyproject.toml` & `dnadb-0.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.6.2"
+version = "0.6.3"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.6.2/src/dnadb/datasets/dataset.py` & `dnadb-0.6.3/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/datasets/greengenes.py` & `dnadb-0.6.3/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.6.3/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.6.3/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/db.py` & `dnadb-0.6.3/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/dna.py` & `dnadb-0.6.3/src/dnadb/dna.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,17 +29,14 @@
 __iupac_lcm = np.lcm.reduce([len(v) for v in IUPAC_MAP.values()])
 IUPAC_AUGMENT_LOOKUP_TABLE = np.full((len(IUPAC_MAP), __iupac_lcm), 255, dtype=np.uint8)
 for __base, __bases in IUPAC_MAP.items():
     __repeat = __iupac_lcm // len(__bases)
     __repeated_bases = BASE_LOOKUP_TABLE[np.array(list(map(ord, __bases*__repeat)), np.uint8) - ord('A')]
     IUPAC_AUGMENT_LOOKUP_TABLE[BASE_LOOKUP_TABLE[ord(__base) - ord('A')]] = __repeated_bases
 
-ENC_AMBIGUOUS_BASE_MAP = {BASE_LOOKUP_TABLE[ord(b) - 65]: tuple(BASE_LOOKUP_TABLE[ord(c) - 65] for c in cs)
-    for b, cs in IUPAC_MAP.items()}
-
 # DNA Sequence Encoding/Decoding -------------------------------------------------------------------
 
 def encode(ascii_bases: npt.NDArray[np.uint8]) ->  npt.NDArray[np.uint8]:
     """
     Encode the given DNA bases in ASCII form into an integer vector representation.
     """
     return BASE_LOOKUP_TABLE[ascii_bases - 65]
@@ -131,15 +128,15 @@
     """
     Convert a DNA sequence to RNA.
     """
     return rna_sequence.replace('U', 'T')
 
 # Data Classes -------------------------------------------------------------------------------------
 
-@dataclass(init=False, frozen=True)
+@dataclass(frozen=True)
 class AbstractSequenceWrapper:
     __slots__ = ("sequence",)
 
     sequence: str
 
     def __len__(self):
         return len(self.sequence)
```

### Comparing `dnadb-0.6.2/src/dnadb/fasta.py` & `dnadb-0.6.3/src/dnadb/fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 from .utils import open_file
 
 @dataclass(frozen=True, order=True)
 class FastaEntry(AbstractSequenceWrapper):
     """
     A container class to represent a FASTA entry
     """
-    __slots__ = ("identifier", "sequence", "extra")
+    __slots__ = ("identifier", "extra")
 
     identifier: str
-    sequence: str
     extra: str
 
     @classmethod
     def deserialize(cls, entry: bytes) -> "FastaEntry":
         """
         Deserialize a FASTA entry from a byte string
         """
@@ -37,14 +36,19 @@
         header, *sequence_parts = entry.split('\n')
         header_line = header[1:].rstrip().split(maxsplit=1)
         identifier = header_line[0]
         extra = header_line[1] if len(header_line) > 1 else ""
         sequence = "".join(sequence_parts)
         return cls(identifier, sequence, extra)
 
+    def __init__(self, identifier: str, sequence: str, extra: str = ""):
+        object.__setattr__(self, "identifier", identifier)
+        object.__setattr__(self, "sequence", sequence)
+        object.__setattr__(self, "extra", extra)
+
     def serialize(self) -> bytes:
         return "\x00".join((self.identifier, self.sequence, self.extra)).encode()
 
     def __str__(self):
         header_line = f"{self.identifier} {self.extra}".rstrip()
         return f">{header_line}\n{self.sequence}"
```

### Comparing `dnadb-0.6.2/src/dnadb/fastq.py` & `dnadb-0.6.3/src/dnadb/fastq.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,29 +98,33 @@
 
 @dataclass(frozen=True, order=True)
 class FastqEntry(AbstractSequenceWrapper):
     """
     A class representation of a FASTQ entry containing the sequnce identifier, sequence, and quality
     scores.
     """
-    __slots__ = ("header_str", "sequence", "quality_scores")
+    __slots__ = ("header_str", "quality_scores")
 
     header_str: str
-    sequence: str
     quality_scores: str
 
     @classmethod
     def deserialize(cls, entry: bytes) -> "FastqEntry":
         return cls(*entry.decode().split('\x00'))
 
     @classmethod
     def from_str(cls, entry: str) -> "FastqEntry":
         header, sequence, _, quality_scores= entry.rstrip().split('\n')
         return cls(header, sequence, quality_scores)
 
+    def __init__(self, header: str, sequence: str, quality_scores: str):
+        object.__setattr__(self, "header_str", header)
+        object.__setattr__(self, "sequence", sequence)
+        object.__setattr__(self, "quality_scores", quality_scores)
+
     def serialize(self) -> bytes:
         return '\x00'.join((self.header_str, self.sequence, self.quality_scores)).encode()
 
     @property
     def header(self):
         return FastqHeader.from_str(self.header_str)
```

### Comparing `dnadb-0.6.2/src/dnadb/sample.py` & `dnadb-0.6.3/src/dnadb/sample.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/taxonomy.py` & `dnadb-0.6.3/src/dnadb/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb/utils.py` & `dnadb-0.6.3/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.2/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.6.3/src/dnadb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.2
+Version: 0.6.3
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.2/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.6.3/src/dnadb.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 src/dnadb.egg-info/dependency_links.txt
 src/dnadb.egg-info/requires.txt
 src/dnadb.egg-info/top_level.txt
 src/dnadb/datasets/__init__.py
 src/dnadb/datasets/dataset.py
 src/dnadb/datasets/greengenes.py
 src/dnadb/datasets/silva/__init__.py
-src/dnadb/datasets/silva/taxonomy_map.py
+src/dnadb/datasets/silva/taxonomy_map.py
+src/dnadb/integration/__init__.py
+src/dnadb/integration/tf/__init__.py
+src/dnadb/integration/tf/dna.py
```

