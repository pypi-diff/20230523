# Comparing `tmp/dnadb-0.6.1.tar.gz` & `tmp/dnadb-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.6.1.tar", last modified: Tue May 23 04:50:58 2023, max compression
+gzip compressed data, was "dnadb-0.6.2.tar", last modified: Tue May 23 05:25:33 2023, max compression
```

## Comparing `dnadb-0.6.1.tar` & `dnadb-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.1/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 04:50:58.193070 dnadb-0.6.1/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.1/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 04:50:32.000000 dnadb-0.6.1/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 04:50:58.193070 dnadb-0.6.1/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 04:50:25.000000 dnadb-0.6.1/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.1/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.1/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.1/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.1/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.1/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.1/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.6.1/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7774 2023-05-21 15:17:15.000000 dnadb-0.6.1/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5991 2023-05-21 14:19:54.000000 dnadb-0.6.1/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    11003 2023-05-23 04:49:42.000000 dnadb-0.6.1/src/dnadb/sample.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.1/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.1/src/dnadb/types.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.1/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 04:50:58.193070 dnadb-0.6.1/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 04:50:58.000000 dnadb-0.6.1/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.2/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 05:25:33.525107 dnadb-0.6.2/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.2/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-23 05:23:54.000000 dnadb-0.6.2/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-23 05:25:33.525107 dnadb-0.6.2/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.521106 dnadb-0.6.2/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-23 05:24:04.000000 dnadb-0.6.2/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.2/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.2/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.2/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.2/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.2/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.2/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5115 2023-05-23 05:23:05.000000 dnadb-0.6.2/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7840 2023-05-23 05:23:22.000000 dnadb-0.6.2/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6057 2023-05-23 05:23:27.000000 dnadb-0.6.2/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11231 2023-05-23 05:23:36.000000 dnadb-0.6.2/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.2/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.2/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.2/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-23 05:25:33.525107 dnadb-0.6.2/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-23 05:25:33.000000 dnadb-0.6.2/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.6.1/LICENSE` & `dnadb-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/PKG-INFO` & `dnadb-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.1/pyproject.toml` & `dnadb-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.6.1/src/dnadb/datasets/dataset.py` & `dnadb-0.6.2/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/datasets/greengenes.py` & `dnadb-0.6.2/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.6.2/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.6.2/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/db.py` & `dnadb-0.6.2/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/dna.py` & `dnadb-0.6.2/src/dnadb/dna.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import abc
+from dataclasses import dataclass
 import itertools
 import numpy as np
 import numpy.typing as npt
 import scipy as sp
 
 BASES = "ACGT"
 AMBIGUOUS_BASES = "MRWSYKVHDBN"
@@ -128,7 +128,18 @@
 
 
 def to_dna(rna_sequence: str) -> str:
     """
     Convert a DNA sequence to RNA.
     """
     return rna_sequence.replace('U', 'T')
+
+# Data Classes -------------------------------------------------------------------------------------
+
+@dataclass(init=False, frozen=True)
+class AbstractSequenceWrapper:
+    __slots__ = ("sequence",)
+
+    sequence: str
+
+    def __len__(self):
+        return len(self.sequence)
```

### Comparing `dnadb-0.6.1/src/dnadb/fasta.py` & `dnadb-0.6.2/src/dnadb/fasta.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 from functools import singledispatchmethod
 import io
 import numpy as np
 from pathlib import Path
 from typing import Generator, Iterable, Optional, Tuple, Union
 
 from .db import DbFactory, DbWrapper
+from .dna import AbstractSequenceWrapper
 from .taxonomy import TaxonomyEntry
 from .types import int_t
 from .utils import open_file
 
 @dataclass(frozen=True, order=True)
-class FastaEntry:
+class FastaEntry(AbstractSequenceWrapper):
     """
     A container class to represent a FASTA entry
     """
     __slots__ = ("identifier", "sequence", "extra")
 
     identifier: str
     sequence: str
```

### Comparing `dnadb-0.6.1/src/dnadb/fastq.py` & `dnadb-0.6.2/src/dnadb/fastq.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 from typing import Generator, Iterable, Tuple, Union
 
 from .db import DbFactory, DbWrapper
+from .dna import AbstractSequenceWrapper
 from .types import int_t
 from .utils import open_file
 
 def phred_encode(probabilities: npt.ArrayLike, encoding: int_t = 33) -> str:
     scores = (-10 * np.log10(np.array(probabilities))).astype(int)
     return ''.join((chr(score + encoding)) for score in scores)
 
@@ -92,15 +93,15 @@
             self.control_number,
             self.sequence_index
         ]))
         return sequence_id
 
 
 @dataclass(frozen=True, order=True)
-class FastqEntry:
+class FastqEntry(AbstractSequenceWrapper):
     """
     A class representation of a FASTQ entry containing the sequnce identifier, sequence, and quality
     scores.
     """
     __slots__ = ("header_str", "sequence", "quality_scores")
 
     header_str: str
```

### Comparing `dnadb-0.6.1/src/dnadb/sample.py` & `dnadb-0.6.2/src/dnadb/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import abc
 from dataclasses import dataclass, field
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 from typing import Generator, Iterable, Optional, Tuple, Union
 
-from dnadb.fasta import FastaEntry
-
 from .db import DbFactory, DbWrapper
+from .dna import AbstractSequenceWrapper
 from .fasta import FastaDb, FastaEntry, FastaIndexDb
 from .fastq import FastqDb, FastqEntry
 from .types import int_t
 
 @dataclass(frozen=True, order=True)
 class SampleMappingEntry:
     name: str
@@ -131,14 +130,22 @@
 
 
 class SampleInterface(abc.ABC):
     def __init__(self, name: str):
         self.name = name
 
     @abc.abstractmethod
+    def sample(
+        self,
+        n: int,
+        rng: np.random.Generator = np.random.default_rng()
+    ) -> Generator[AbstractSequenceWrapper, None, None]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
     def __contains__(self, key) -> bool:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def __len__(self) -> bool:
         raise NotImplementedError()
```

### Comparing `dnadb-0.6.1/src/dnadb/taxonomy.py` & `dnadb-0.6.2/src/dnadb/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb/utils.py` & `dnadb-0.6.2/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.6.1/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.6.2/src/dnadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.6.1/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.6.2/src/dnadb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

