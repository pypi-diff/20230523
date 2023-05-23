# Comparing `tmp/cmrseq-0.19.tar.gz` & `tmp/cmrseq-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmrseq-0.19.tar", last modified: Sat May 20 15:03:23 2023, max compression
+gzip compressed data, was "cmrseq-0.20.tar", last modified: Tue May 23 16:36:47 2023, max compression
```

## Comparing `cmrseq-0.19.tar` & `cmrseq-0.20.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.528070 cmrseq-0.19/
--rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-12 07:05:08.000000 cmrseq-0.19/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3033 2023-05-20 15:03:23.528070 cmrseq-0.19/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2541 2023-04-12 07:05:08.000000 cmrseq-0.19/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.508062 cmrseq-0.19/cmrseq/
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq/contrib/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/contrib/sequences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-20 15:03:04.000000 cmrseq-0.19/cmrseq/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31132 2023-05-20 14:01:47.000000 cmrseq-0.19/cmrseq/core/_sequence.py
--rw-rw-rw-   0 root         (0) root         (0)     6328 2023-04-12 16:23:47.000000 cmrseq-0.19/cmrseq/core/_system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.516065 cmrseq-0.19/cmrseq/core/bausteine/
--rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-12 11:43:49.000000 cmrseq-0.19/cmrseq/core/bausteine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6728 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_adc.py
--rw-rw-rw-   0 root         (0) root         (0)    10380 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/core/bausteine/_delay.py
--rw-rw-rw-   0 root         (0) root         (0)    19958 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/core/bausteine/_gradients.py
--rw-rw-rw-   0 root         (0) root         (0)    14389 2023-04-13 09:15:52.000000 cmrseq-0.19/cmrseq/core/bausteine/_rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.520066 cmrseq-0.19/cmrseq/io/
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/io/_json.py
--rw-rw-rw-   0 root         (0) root         (0)    25750 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/io/_phillips_load.py
--rw-rw-rw-   0 root         (0) root         (0)    53656 2023-05-20 14:39:53.000000 cmrseq-0.19/cmrseq/io/_pulseq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.520066 cmrseq-0.19/cmrseq/parametric_definitions/
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13840 2023-04-15 09:54:10.000000 cmrseq-0.19/cmrseq/parametric_definitions/diffusion.py
--rw-rw-rw-   0 root         (0) root         (0)    14607 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/excitation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.524068 cmrseq-0.19/cmrseq/parametric_definitions/readout/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16753 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
--rw-rw-rw-   0 root         (0) root         (0)    23860 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_epi.py
--rw-rw-rw-   0 root         (0) root         (0)     8143 2023-04-12 07:06:42.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_radial.py
--rw-rw-rw-   0 root         (0) root         (0)    10626 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/readout/_spiral.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.524068 cmrseq-0.19/cmrseq/parametric_definitions/sequences/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13141 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_gradient_echo.py
--rw-rw-rw-   0 root         (0) root         (0)     8209 2023-05-20 14:45:45.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_spin_echo.py
--rw-rw-rw-   0 root         (0) root         (0)    18605 2023-04-13 15:56:56.000000 cmrseq-0.19/cmrseq/parametric_definitions/sequences/_ssfp.py
--rw-rw-rw-   0 root         (0) root         (0)    27016 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/parametric_definitions/velocity.py
--rw-rw-rw-   0 root         (0) root         (0)    16067 2023-04-12 16:23:47.000000 cmrseq-0.19/cmrseq/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)    11966 2023-04-12 07:05:08.000000 cmrseq-0.19/cmrseq/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-20 15:03:23.512063 cmrseq-0.19/cmrseq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3033 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1282 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-20 15:03:23.000000 cmrseq-0.19/cmrseq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-20 15:03:23.528070 cmrseq-0.19/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-12 07:05:08.000000 cmrseq-0.19/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.604550 cmrseq-0.20/
+-rw-rw-rw-   0 root         (0) root         (0)    35076 2023-04-12 07:04:17.000000 cmrseq-0.20/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-23 16:36:47.604550 cmrseq-0.20/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2023-04-12 07:04:17.000000 cmrseq-0.20/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.592545 cmrseq-0.20/cmrseq/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.592545 cmrseq-0.20/cmrseq/contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/contrib/sequences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.596547 cmrseq-0.20/cmrseq/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-23 16:36:35.000000 cmrseq-0.20/cmrseq/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34727 2023-05-23 16:08:46.000000 cmrseq-0.20/cmrseq/core/_sequence.py
+-rw-rw-rw-   0 root         (0) root         (0)     6328 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/_system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.596547 cmrseq-0.20/cmrseq/core/bausteine/
+-rw-rw-rw-   0 root         (0) root         (0)      678 2023-04-12 11:43:48.000000 cmrseq-0.20/cmrseq/core/bausteine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7561 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/bausteine/_adc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/bausteine/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/bausteine/_delay.py
+-rw-rw-rw-   0 root         (0) root         (0)    24837 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/bausteine/_gradients.py
+-rw-rw-rw-   0 root         (0) root         (0)    18181 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/core/bausteine/_rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.596547 cmrseq-0.20/cmrseq/io/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/io/_json.py
+-rw-rw-rw-   0 root         (0) root         (0)    25748 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/io/_phillips_load.py
+-rw-rw-rw-   0 root         (0) root         (0)    53656 2023-05-20 14:39:52.000000 cmrseq-0.20/cmrseq/io/_pulseq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.600548 cmrseq-0.20/cmrseq/parametric_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13840 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/parametric_definitions/diffusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    14602 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/parametric_definitions/excitation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.600548 cmrseq-0.20/cmrseq/parametric_definitions/readout/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/readout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16647 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)    23938 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/parametric_definitions/readout/_epi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2023-04-12 07:11:24.000000 cmrseq-0.20/cmrseq/parametric_definitions/readout/_radial.py
+-rw-rw-rw-   0 root         (0) root         (0)    10626 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/readout/_spiral.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.604550 cmrseq-0.20/cmrseq/parametric_definitions/sequences/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/sequences/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13141 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/sequences/_gradient_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)     8209 2023-05-20 14:45:47.000000 cmrseq-0.20/cmrseq/parametric_definitions/sequences/_spin_echo.py
+-rw-rw-rw-   0 root         (0) root         (0)    18600 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/parametric_definitions/sequences/_ssfp.py
+-rw-rw-rw-   0 root         (0) root         (0)    27016 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/parametric_definitions/velocity.py
+-rw-rw-rw-   0 root         (0) root         (0)    16097 2023-05-23 15:09:08.000000 cmrseq-0.20/cmrseq/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)    11966 2023-04-12 07:04:17.000000 cmrseq-0.20/cmrseq/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 16:36:47.592545 cmrseq-0.20/cmrseq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3033 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-23 16:36:47.000000 cmrseq-0.20/cmrseq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 16:36:47.604550 cmrseq-0.20/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-12 07:04:18.000000 cmrseq-0.20/setup.py
```

### Comparing `cmrseq-0.19/LICENSE` & `cmrseq-0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/PKG-INFO` & `cmrseq-0.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.19
+Version: 0.20
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.19/README.rst` & `cmrseq-0.20/README.rst`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/contrib/sequences.py` & `cmrseq-0.20/cmrseq/contrib/sequences.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/core/_sequence.py` & `cmrseq-0.20/cmrseq/core/_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,111 @@
 """ This Module contains the implementation of the core functionality Sequence"""
 __all__ = ["Sequence"]
 
 from copy import deepcopy
-from typing import List, Union, Iterable, Tuple
+from typing import List, Union, Iterable, Tuple, Dict
 from warnings import warn
 import re
 
 import numpy as np
 from pint import Quantity
 from tqdm import tqdm
 
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core.bausteine._adc import ADC
 from cmrseq.core.bausteine._rf import RFPulse
+from cmrseq.core.bausteine._gradients import Gradient
 from cmrseq.core._system import SystemSpec
 
 
 class Sequence:
-    """ This class groups the building blocks making up a MRI sequence"""
+    """ This class serves as a container for MRI-sequence building blocks.
+
+    All blocks contained in a sequence are kept as mutable objects of type SequenceBaseBlock or
+    rather its subclasses. This means if a contained block is changed/transformed outside
+    the sequence scope, these changes are also reflected in the sequence.
+
+    Below, the functionality provided by a cmrseq.Sequence object is explained according to the
+    groups:
+
+    - Instantiation and composition
+    - Get contained blocks
+    - Gridding, Moments and K-space
+
+
+    **Instantiation and composition**
+
+    To instantiate a Sequence you need a list containing building blocks and a sytem-specification
+    definition. On instantiation, all blocks are validated against the system limits. If any block
+    violates the limits, an exception is raised.
+
+    _Adding blocks_: Blocks or even entire sequences can be added to an existing sequence object
+    one the obe hand by using the 'add_block', 'append', 'extend' methods (see documentation).
+    And on the other hand, the Sequence class implements the addition operator, which combines
+    two sequence objects into either a new object containing copies of all blocks contained in the
+    other two or by in-place addition where no copies are made:
+
+    .. code::
+
+        new_sequence_object = sequence1 + sequence2   # Combination with copy
+        sequence1 += sequence2                        # inplace combination of seq2 into seq1
+
+
+    _Unique names_: a sequence objects keeps a mapping of automatically created unique names to the
+    actual blocks. Whenever blocks are added
+
+    **Get contained blocks**
+
+    There are multiple ways to query single or even multiple blocks at once from the sequence
+    object. To get a complete list of unique block-names use the property `seq.blocks`.
+
+    __Access by name__:
+    1. Indexing by unique name: `seq["trapezoidal_0"]`
+    2. Get all blocks by partial string match: `seq.get_block(partial_string_match=...)`
+    3. Get all blocks by matching regular expression on unique names: `seq.get_block(regular_expression=...)`
+
+    __Assuming temporal order of start__
+    1. Indexing by integer: `seq[0]`
+    2. Indexing by slice: `seq[0:5]`
+    3. Indexing by tuple of integers: `seq[(0, 2, 5)]`
+    4. Iterating over sequence: `[block for block in seq]`
+    5. Iterating over sequence with block-names `{name: block for (name, block) in seq.items()}`
+
+
+    **Gridding, Moments and K-space**
+
+    Gradients, RF and ADCs represented on a dense temporal grid defined by the system raster times
+    can be obtained by calling the methods: `gradients_to_grid`, `rf_to_grid`, and `adc_to_grid`.
+
+    Gradient moments of specified order can be integrated using the function `calculate_moment`.
+
+    To get a representation of the kspace-trajectory as well as timing and position of sampling
+    events defined by contained ADC blocks can be obtained by the `calculate_kspace` function.
+
+
+    :param building_blocks: List of building Blocks
+    :param system_specs: Instance of SystemSpec
+    """
+
+    #: System specification object
+    _system_specs: SystemSpec
+    #:
+    _blocks: List[SequenceBaseBlock]
+    #:
+    _block_lookup: Dict[str, SequenceBaseBlock]
 
     def __init__(self, building_blocks: List[SequenceBaseBlock], system_specs: SystemSpec):
         self._system_specs = system_specs
         self._blocks = building_blocks
+        self.validate()
+
         self._block_lookup = {}
         for block in self._blocks:
             self._add_unique_block_name(block)
 
-    def _add_unique_block_name(self, block: SequenceBaseBlock):
-        """Iterates over block names and adds a counter to the block name if it already is used to
-        create the dictionary (unique_block_name -> SequenceBaseBlock)
-        :param block:
-        """
-        i = 0
-        augmented_name = block.name + f"_{i}"
-        while self._block_lookup.get(augmented_name, None) is not None:
-            augmented_name = block.name + f"_{i}"
-            i += 1
-        self._block_lookup.update({augmented_name: block})
 
     def __add__(self, other: 'Sequence') -> 'Sequence':
         """ If both system specifications match, returns a new sequence containing deep copies
         of all blocks contained in self._blocks and other._blocks """
         self._check_sys_compatibility(other._system_specs)
         new_blocks = [deepcopy(b) for b in [*self._blocks, *other._blocks]]
         return Sequence(new_blocks, system_specs=deepcopy(self._system_specs))
@@ -87,26 +152,51 @@
                                       f" queries [str, int, slice, Tuple[int]]")
 
     def __iter__(self):
         """Returns an iterator yielding blocks sorted by theirs start time"""
         start_times = self._create_sorted_block_list(reversed=False)
         return (self._block_lookup[k] for (k, _) in start_times)
 
+    def items(self):
+        """Returns a generator yielding (unique_block_name, block) tuples"""
+        names_and_times = self._create_sorted_block_list(reversed=False)
+        return ((k, self._block_lookup[k]) for (k, _) in names_and_times)
+
+    def _add_unique_block_name(self, block: SequenceBaseBlock):
+        """Iterates over block names and adds a counter to the block name if it already is used to
+        create the dictionary (unique_block_name -> SequenceBaseBlock)
+        :param block:
+        """
+        i = 0
+        augmented_name = block.name + f"_{i}"
+        while self._block_lookup.get(augmented_name, None) is not None:
+            augmented_name = block.name + f"_{i}"
+            i += 1
+        self._block_lookup.update({augmented_name: block})
+
     def _check_sys_compatibility(self, system_specs: SystemSpec):
         equalities = [self._system_specs.__dict__[k] == system_specs.__dict__[k]
                       for k in self._system_specs.__dict__.keys()]
         if not all(equalities):
             raise ValueError("System specifications of added sequence do not match. Addition "
                              "for different system specifications is not implemented")
 
     def _create_sorted_block_list(self, reversed: bool = False):
         start_times = [(k, b.tmin) for k, b in self._block_lookup.items()]
         start_times.sort(key=lambda x: float(x[1].m_as("ms")), reverse=reversed)
         return start_times
 
+    def validate(self) -> None:
+        """ Calls the validation function of each block with self._system_specs
+
+        :raises ValueError: If any contained block fails to validate with own system specs
+        """
+        for block in self._blocks:
+            block.validate(system_specs=self._system_specs)
+
     def add_block(self, block: SequenceBaseBlock, copy: bool = True) -> None:
         """ Add the instance of block to the internal List of sequence blocks.
 
         **Note**: The internal definiton of blocks is mutuable, therefore if the new block is not
         copied, subsequent alterations can have unwanted side-effects inside the sequence.
 
         :raises ValueError: If block.validate() fails to validate using the system specs of self
@@ -144,58 +234,14 @@
         if block is None:
             raise ValueError(f"Tried to remove non-existing block; \n "
                              f"'{block_name}' not in {self.blocks}")
         block_index = [block is b for b in self._blocks].index(True)
         del self._blocks[block_index]
         del self._block_lookup[block_name]
 
-    def get_block(self, block_name: Union[str, Iterable[str]] = None,
-                  partial_string_match: Union[str, Iterable[str]] = None,
-                  regular_expression: Union[str, Iterable[str]] = None) \
-                  -> Union[SequenceBaseBlock, List[SequenceBaseBlock]]:
-        """ Returns reference to the block whose member `name` matches the specified argument.
-        If no block with given name is present in the sequence, it returns None
-
-        .. note::
-
-            Checks which keyword argument to use from left to right as specified in the signature.
-            If multiple are specified uses only the first one.
-
-        :raises: ValueError if no keyword-argument is specified
-
-        :param block_name: String or iterable of strings exactly matching a set of blocks contained
-                            in the sequence
-        :param partial_string_match: str or iterable of strings that specify partial string matches.
-                            All blocks partially matching at least one are returned.
-        :param regular_expression: str or iterable of strings containing regular expressions that
-                            are matched against the block-names. All blocks, matching at least one
-                            of the given expressions are returned.
-        :return: SequenceBaseBlock or List of SequenceBaseBlocks depending on the specified argument
-        """
-        if block_name is not None:
-            if isinstance(block_name, str):
-                return self._block_lookup.get(block_name, None)
-            else:
-                return [self._block_lookup[bn] for bn in block_name]
-        elif partial_string_match is not None:
-            if isinstance(partial_string_match, str):
-                partial_string_match = [partial_string_match, ]
-            partial_string_match = "|".join([f"(?:.*{p}.*)" for p in partial_string_match])
-            matched_block_names = [block for name, block in self._block_lookup.items()
-                                   if re.match(partial_string_match, name)]
-            return matched_block_names
-        elif regular_expression is not None:
-            if isinstance(regular_expression, str):
-                regular_expression = [regular_expression,]
-            regular_expression = "|".join([f"(?:{p})" for p in regular_expression])
-            matched_block_names = [block for name, block in self._block_lookup.items()
-                                   if re.match(regular_expression, name)]
-            return matched_block_names
-        else:
-            raise ValueError("At least one on the keyword arguments must be specified")
 
     def append(self, other: Union['Sequence', SequenceBaseBlock],
                copy: bool = True, end_time: Quantity = None) -> None:
         """If both system specifications match, copies all blocks from `other` shifts them by own
         tmax and adds the blocks to own collection
 
         :raises ValueError: If other fails to validate using the system specs of self
@@ -225,15 +271,15 @@
         if end_time is None:
             if not self._blocks:
                 end_time = Quantity(0., "ms")
             else:
                 end_time = np.max([block.tmax.m_as("ms") for block in self._blocks])
 
         for block in block_copies:
-            block.shift_time(Quantity(end_time, "ms"))
+            block.shift(Quantity(end_time, "ms"))
         self._blocks.extend(block_copies)
         for block in block_copies:
             self._add_unique_block_name(block)
 
     def extend(self, other: Iterable[Union['Sequence', SequenceBaseBlock]],
                copy: bool = True) -> None:
         """If both system specifications match, copies all blocks from `other` shifts them by own
@@ -247,37 +293,74 @@
 
         end_times = [b.end_time.m_as("ms") if isinstance(b, Sequence) else b.tmax.m_as("ms")
                      for b in other]
         end_times = np.cumsum([self.end_time.m_as("ms")] + end_times)
         for idx, other_it in enumerate(tqdm(other, desc="Extending Sequence")):
             self.append(other_it, copy, end_time=end_times[idx])
 
-    def validate(self) -> None:
-        """ Calls the validation function of each block with self._system_specs
+    def get_block(self, block_name: Union[str, Iterable[str]] = None,
+                  partial_string_match: Union[str, Iterable[str]] = None,
+                  regular_expression: Union[str, Iterable[str]] = None) \
+            -> Union[SequenceBaseBlock, List[SequenceBaseBlock]]:
+        """ Returns reference to the block whose member `name` matches the specified argument.
+        If no block with given name is present in the sequence, it returns None
 
-        :raises ValueError: If any contained block fails to validate with own system specs
+        .. note::
+
+            Checks which keyword argument to use from left to right as specified in the signature.
+            If multiple are specified uses only the first one.
+
+        :raises: ValueError if no keyword-argument is specified
+
+        :param block_name: String or iterable of strings exactly matching a set of blocks contained
+                            in the sequence
+        :param partial_string_match: str or iterable of strings that specify partial string matches.
+                            All blocks partially matching at least one are returned.
+        :param regular_expression: str or iterable of strings containing regular expressions that
+                            are matched against the block-names. All blocks, matching at least one
+                            of the given expressions are returned.
+        :return: SequenceBaseBlock or List of SequenceBaseBlocks depending on the specified argument
         """
-        for block in self._blocks:
-            block.validate(system_specs=self._system_specs)
+        if block_name is not None:
+            if isinstance(block_name, str):
+                return self._block_lookup.get(block_name, None)
+            else:
+                return [self._block_lookup[bn] for bn in block_name]
+        elif partial_string_match is not None:
+            if isinstance(partial_string_match, str):
+                partial_string_match = [partial_string_match, ]
+            partial_string_match = "|".join([f"(?:.*{p}.*)" for p in partial_string_match])
+            matched_block_names = [block for name, block in self._block_lookup.items()
+                                   if re.match(partial_string_match, name)]
+            return matched_block_names
+        elif regular_expression is not None:
+            if isinstance(regular_expression, str):
+                regular_expression = [regular_expression, ]
+            regular_expression = "|".join([f"(?:{p})" for p in regular_expression])
+            matched_block_names = [block for name, block in self._block_lookup.items()
+                                   if re.match(regular_expression, name)]
+            return matched_block_names
+        else:
+            raise ValueError("At least one on the keyword arguments must be specified")
 
     def shift_in_time(self, shift: Quantity) -> None:
         """ Shifts all blocks contained in the sequence object by the specified time
 
         :param shift: Quantity of dimesion time
         """
         for block in self._blocks:
-            block.shift_time(time_shift=shift)
+            block.shift(time_shift=shift)
 
     def time_reverse(self) -> None:
         """ Reverses the sequence in time
         """
         # flip about end of sequence
         time_flip_point = self.duration
         for block in self._blocks:
-            block.time_reverse(time_flip_point)
+            block.flip(time_flip_point)
 
     def invert_gradients(self) -> None:
         """Inverts all gradient amplitudes in sequence
         """
         for block in self._blocks:
             block.scale_gradients(-1.)
 
@@ -306,38 +389,41 @@
     def end_time(self):
         return Quantity(np.round(np.max([b.tmax.m_as("ms") for b in self._blocks]), 6), 'ms')
 
     @property
     def gradients(self) -> List[Tuple[Quantity, Quantity]]:
         """ Returns the gradient definitions (t, wf) of all blocks that are contained in the
         sequence. Blocks that do not contain a gradient definition are ignored"""
-        return [block.gradients for block in self._blocks if block.gradients is not None]
+        return [block.gradients for block in self._blocks if isinstance(block, Gradient)]
 
     @property
     # pylint: disable=C0103
     def rf(self) -> List[Tuple[Quantity, Quantity]]:
         """ Returns the rf definitions (t, amplitude) of all blocks that are contained in the
                 sequence. Blocks that do not contain a rf definition are ignored"""
         return [block.rf for block in self._blocks if isinstance(block, RFPulse)]
 
     @property
     def rf_events(self) -> List[Tuple[Quantity, Quantity]]:
         """ Returns the rf definitions (t, amplitude) of all blocks that are contained in the
                 sequence. Blocks that do not contain a rf definition are ignored"""
-        return [block.rf_events for block in self._blocks if block.rf_events is not None]
+        return [block.rf_events for block in self._blocks if isinstance(block, RFPulse)]
 
     @property
     def adc_centers(self) -> List[Quantity]:
         """ Returns the centers of all adc_blocks in the sequence."""
-        return [block.adc_center for block in self._blocks if block.adc_center is not None]
+        return [block.adc_center for block in self._blocks if isinstance(block, ADC)]
 
     @property
     def blocks(self) -> Tuple[str]:
-        """Returns a tuple containing the names of all blocks contained in the sequence object"""
-        return tuple(self._block_lookup.keys())
+        """Returns a tuple containing the names of all blocks contained in the sequence object,
+        where temporal ordering is assumed"""
+        names_and_times = self._create_sorted_block_list(reversed=False)
+        names = [n for n, t in names_and_times]
+        return names
 
     # pylint: disable=R0914, C0103
     def gradients_to_grid(self) -> Tuple[np.ndarray, np.ndarray]:
         """ Grids gradient definitions of all blocks contained in the sequence, on a joint time grid
         from the minimal to maximal value in single time-points definitions with a step-length
         defined in system_specs.grad_raster_time.
         If gradients occur at the same time on the same channel, they are added.
@@ -433,15 +519,15 @@
         :return: Tuple(np.array, np.array, np.array)
                       - (t, ) containing time-values
                       - (t, ) containing values of 0 or 1, indicating where the adc is active
                       - (t, ) containing the adc_phase in radians
                       - (#adc_blocks, 2) where (:, 0) contains the indices of the start time of the adc-block and (:, 1) the end time correspondingly.
         """
         # First grid all individual blocks on adc_raster times
-        adc_blocks = [block for block in self._blocks if block.adc_timing is not None]
+        adc_blocks = [block for block in self._blocks if isinstance(block, ADC)]
         gridded_adcs = []
         for block in adc_blocks:
             gridded_adcs.append(self._grid_single_adc_block(force_raster, block))
 
         # Secondly Insert the gridded adc-timings into the gradient raster
         gradient_raster = self.gradients_to_grid()[0]
 
@@ -534,15 +620,15 @@
         :return: Tuple of arrays containing:
 
                 - k-space trajectory on gradient rasters (-1, 3) in 1/m
                 - k-space points at adc events (-1, 3) in 1/m
                 - time at adc events (-1 ) in ms
         """
         # Subdivide gradient waveforms in periods between rf events for integration
-        rf_events = [block.rf_events for block in self._blocks if block.rf_events is not None]
+        rf_events = [block.rf_events for block in self._blocks if isinstance(block, RFPulse)]
 
         if rf_events:
             rf_factors = []
             for (t, fa) in rf_events:
                 factor = -1. if np.isclose(fa, np.pi, rtol=np.pi / 50) else 0.
                 rf_factors.append([t.m_as("ms"), factor])
             rf_factors = np.stack(rf_factors)
@@ -566,15 +652,15 @@
         else:
             k_of_t[:, 1:] = np.cumsum(np.diff(t_grid_global).reshape(1, -1) *
                                       (gradient_waveform[:, 1:] + gradient_waveform[:, :-1]) / 2,
                                       axis=1) * self._system_specs.gamma.m_as("MHz/T")
 
         # Evaluate k-space position at adc-events
         all_adc_timings = [block.adc_timing.m_as("ms") for block in self._blocks
-                           if block.adc_timing is not None]
+                           if isinstance(block, ADC)]
         if all_adc_timings:
             t_adc = np.around(np.concatenate(all_adc_timings, axis=0), decimals=6)
             k_adc = np.stack([np.interp(t_adc, t_grid_global, k) for k in k_of_t])
         else:
             k_adc = None
             t_adc = None
```

### Comparing `cmrseq-0.19/cmrseq/core/_system.py` & `cmrseq-0.20/cmrseq/core/_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # if False
 
     def __init__(self,
                  gamma: Quantity = Quantity(42.576, "MHz/T"),
                  grad_raster_time: Quantity = Quantity(1e-2, "ms"),
                  max_grad: Quantity = Quantity(40, "mT/m"),
                  max_slew: Quantity = Quantity(120, "mT/m/ms"),
-                 rf_peak_power: Quantity = Quantity(20, "uT"),
+                 rf_peak_power: Quantity = Quantity(30, "uT"),
                  rf_raster_time: Quantity = Quantity(1e-2, "ms"),
                  rf_dead_time: Quantity = Quantity(0., "ms"),
                  rf_ringdown_time: Quantity = Quantity(1e-3, "ms"),
                  adc_raster_time: Quantity = Quantity(1e-2, "ms"),
                  adc_dead_time: Quantity = Quantity(0., "ms"),
                  b0: Quantity = Quantity(1.5, "T")):
```

### Comparing `cmrseq-0.19/cmrseq/core/bausteine/__init__.py` & `cmrseq-0.20/cmrseq/core/bausteine/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/core/bausteine/_adc.py` & `cmrseq-0.20/cmrseq/core/bausteine/_adc.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,16 +10,23 @@
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core._system import SystemSpec
 
 
 class ADC(SequenceBaseBlock):
     """ ADC-specific extension to the SequenceBaseBlock, serves as base class for all
     ADC implementations"""
+    #: Quantity[ms] defining sampling event times
+    adc_timing: Quantity = None
+
+    #: Quantity[ms] Time defining the center of the adc-events
+    adc_center: Quantity = None
+
     #: Quantity[rad]
     phase_offset: Quantity
+
     #: Quantity[Hz]
     frequency_offset: Quantity
 
     def __init__(self, system_specs: SystemSpec, name: str,
                  frequency_offset: Quantity, phase_offset: Quantity):
         super().__init__(system_specs, name)
         self.frequency_offset = frequency_offset.to("Hz")
@@ -35,17 +42,34 @@
         return phase_per_time
 
     @property
     def tmin(self):
         return self.adc_timing[0]
 
     @property
-    def duration(self):
-        return self.tmax - self.tmin
+    def tmax(self):
+        return self.adc_timing[-1]
+
+    def validate(self, system_specs: SystemSpec):
+        return
+
+    def shift(self, time_shift: Quantity) -> None:
+        """Adds the time-shift to all adc definition points and the adc-center"""
+        time_shift = time_shift.to("ms")
+        self.adc_timing += time_shift
+        self.adc_center += time_shift
+
+    def flip(self, time_flip: Quantity = None):
+        if time_flip is None:
+            time_flip = self.tmax
+        self.adc_timing = np.flip(time_flip.to("ms") - self.adc_timing, axis=0)
+        self.adc_center = np.flip(time_flip.to("ms") - self.adc_center, axis=0)
 
+    def snap_to_raster(self, system_specs: SystemSpec):
+        pass
 
 class SymmetricADC(ADC):
     """ ADC object with instantaneous encoding events at k-space positions """
 
     def __init__(self, system_specs: SystemSpec,
                  num_samples: int,
                  dwell: Quantity = None,
```

### Comparing `cmrseq-0.19/cmrseq/core/bausteine/_delay.py` & `cmrseq-0.20/cmrseq/core/bausteine/_delay.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 __all__ = ["Delay"]
 
 import numpy as np
 from pint import Quantity
 
 from cmrseq.core._system import SystemSpec
 
-from cmrseq.core.bausteine._base import SequenceBaseBlock
+from cmrseq.core.bausteine._gradients import Gradient
 
 
-class Delay(SequenceBaseBlock):
+class Delay(Gradient):
     """ Defines a gradient with zero magnitude and given duration"""
 
     def __init__(self, system_specs: SystemSpec,
                  duration: Quantity,
                  delay: Quantity = Quantity(0., "ms"),
                  name: str = "delay"):
         """ Defines a gradient with zero magnitude and given duration. This block only makes sense
```

### Comparing `cmrseq-0.19/cmrseq/core/bausteine/_gradients.py` & `cmrseq-0.20/cmrseq/core/bausteine/_gradients.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 """This module contains implementation for gradient blocks"""
 __all__ = ["Gradient", "TrapezoidalGradient", "ArbitraryGradient"]
 
+from typing import Tuple
 from warnings import warn
 import numpy as np
 from pint import Quantity
 
 from cmrseq.core.bausteine._base import SequenceBaseBlock
 from cmrseq.core._system import SystemSpec
 
 
 class Gradient(SequenceBaseBlock):
+    """
+
+    """
+    #: Tuple containing defining points of gradient waveforms as np.array (wrapped as Quantity)
+    #: with shape (time: (t, ), waveform: (3, t)). Between points, linear interpolation is assumed
+    gradients: Tuple[Quantity, Quantity] = None
+
     def __add__(self, other) -> (Quantity, Quantity):
         """ Add to gradient definition and always returns a Tuple (time_points[n], waveforms[3, n])
 
         :param other:
         :return:
         """
 
@@ -83,14 +91,95 @@
     def tmin(self) -> Quantity:
         return self.gradients[0][0]
 
     @property
     def tmax(self) -> Quantity:
         return self.gradients[0][-1]
 
+    def scale_gradients(self, factor: float) -> None:
+        """ Scales gradients by given factor if gradients are defined.
+
+        :param factor: factor to globally scale the amplitude of gradient defintion.
+        """
+        t, grads = self.gradients
+        self.gradients = (t, factor * grads)
+
+    def rotate_gradients(self, rotation_matrix: np.ndarray) -> None:
+        """ Rotates gradients to according to the gradient axes transformation:
+
+        [[1 0 0][0 1 0][0 0 0]].T -> rotation matrix
+
+        :raises: ValueError - if rotation_matrix is not valid : must be an orthogonal matrix
+
+        :param rotation_matrix: (3, 3) rotation matrix containing the new column basis vectors
+                                (meaning in [:, i], i indexes the new orientation of MPS).
+                                Vectors are normalized along axis=0 to ensure same magnitude
+        """
+        valid_rotation = np.all(np.isclose((np.matmul(rotation_matrix, rotation_matrix.T)),
+                                           np.identity(3), rtol=1e-10))
+        if not valid_rotation:
+            raise ValueError(f"Rotation matrix is not valid\n {np.matmul(rotation_matrix, rotation_matrix.T)} \n"
+                             f"should be identity")
+
+        t, wf = self.gradients
+        vector_norms = np.linalg.norm(rotation_matrix, axis=0, keepdims=True)
+        rotation_matrix = rotation_matrix / vector_norms
+        wf_rot = np.einsum("it, ij -> jt", wf.m_as("mT/m"), rotation_matrix)
+        self.gradients = (t, Quantity(wf_rot, "mT/m"))
+
+    def _clean(self):
+        """ If gradient definition contains duplicate consecutive points, the second one is
+        removed"""
+        deltat = np.diff(np.around(self.gradients[0].to("ms").m, decimals=6), axis=0)
+        deltag = np.diff(np.around(self.gradients[1].to("mT/m").m, decimals=6), axis=1)
+        duplicate_idx = np.where(np.logical_and(deltat == 0., np.all(deltag == 0., axis=0)))
+        t, g = self.gradients
+        cleaned_t = Quantity(np.delete(t.m_as("ms"), duplicate_idx), "ms")
+        cleaned_g = Quantity(np.delete(g.m_as("mT/m"), duplicate_idx, axis=1), "mT/m")
+        self.gradients = (cleaned_t, cleaned_g)
+
+    def validate(self, system_specs: SystemSpec) -> None:
+        """ Validates if the contained gradient_definition is valid for the given system-
+        specifications.
+        """
+        max_grad_in_specs = np.all(np.abs(self.gradients[1].m_as("mT/m"))
+                                   <= system_specs.max_grad.m_as("mT/m"))
+        grad_slew = (np.diff(self.gradients[1].m_as("mT/m"), axis=1) /
+                     np.diff(self.gradients[0].m_as("ms"), axis=0)[np.newaxis])
+        grad_slew_in_specs = np.all(np.around(grad_slew, decimals=6)
+                                    <= system_specs.max_slew.m_as("mT/m/ms"))
+        tgridded = self.gradients[0].m_as("ms") / system_specs.grad_raster_time.m_as("ms")
+        grad_on_grid = np.allclose(tgridded, np.around(tgridded), rtol=1e-6)
+        if not all([max_grad_in_specs, grad_slew_in_specs, grad_on_grid]):
+            raise ValueError(f"Gradient definition of {self.name} invalid:\n"
+                             f"\t- max grad: {max_grad_in_specs}\n"
+                             f"\t- max slew: {grad_slew_in_specs}\n"
+                             f"\t- definition on grid: {grad_on_grid}")
+
+    def snap_to_raster(self, system_specs: SystemSpec):
+        warn("When calling snap_to_raster the waveform points are simply rounded to their nearest"
+             f"neighbour if the difference is below the relative tolerance. Therefore this in"
+             f" not guaranteed to be precise anymore")
+        time_ndt = np.around(self.gradients[0].m_as("ms") /
+                             system_specs.grad_raster_time.m_as("ms"), decimals=0)
+        time_ndt = time_ndt * system_specs.grad_raster_time.to("ms")
+        self.gradients = (time_ndt.to("ms"), self.gradients[1].to("mT/m"))
+
+    def shift(self, time_shift: Quantity) -> None:
+        """Adds the time-shift to all gradient definition points"""
+        self.gradients = (self.gradients[0] + time_shift.to("ms"), self.gradients[1])
+
+    def flip(self, time_flip: Quantity = None):
+        """Time reverses block by flipping about a given time point. If no
+        time is specified, the center of this gradient block is choosen."""
+        if time_flip is None:
+            time_flip = self.tmin + (self.tmax - self.tmin) / 2
+        self.gradients = (np.flip(time_flip.to("ms") - self.gradients[0], axis=0),
+                          np.flip(self.gradients[1], axis=1))
+
 
 class TrapezoidalGradient(Gradient):
     """ Module implementing a trapezoidal gradient pulse, from specified parameters"""
 
     # pylint: disable=R0913
     def __init__(self,
                  system_specs: SystemSpec,
```

### Comparing `cmrseq-0.19/cmrseq/io/_json.py` & `cmrseq-0.20/cmrseq/io/_json.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/io/_phillips_load.py` & `cmrseq-0.20/cmrseq/io/_phillips_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,29 +511,29 @@
 
         time_to_ref = gradient_block["bp"].get("time_resolved", time)
         delay = Quantity(time_to_ref[0], "ms")
         seq_block = cmrseq.bausteine.ArbitraryGradient(system_specs=self.system_specs,
                                                        time_points=time + delay,
                                                        waveform=amplitude * direction[:, np.newaxis],
                                                        name=gradient_block["name"].strip(),
-                                                       snap_to_raster=False)
+                                                       snap_to_raster=True)
         o_matrix = gradient_block.get("o_matrix", None)
         if o_matrix is not None and rotate_to_xyz:
             seq_block.rotate_gradients(o_matrix["matrix_rotated"])
         return seq_block
 
     def _make_rf_block(self, rf_dict: dict):
         delay = Quantity(rf_dict["start"] - rf_dict["ref"], "ms")
         wf = Quantity(rf_dict["am_waveform"]["samples"] * rf_dict["am_scale"], "uT")
         t = Quantity(np.linspace(0, rf_dict["dur"], rf_dict["am_waveform"]["size"]), "ms") + delay
         rf_block = cmrseq.bausteine.ArbitraryRFPulse(system_specs=self.system_specs,
                                                      time_points=t,
                                                      waveform=wf,
                                                      name=rf_dict["name"].strip(),
-                                                     snap_to_raster=False)
+                                                     snap_to_raster=True)
         return rf_block
 
     def _make_aq_block(self, aq_dict: dict) -> List[cmrseq.bausteine.SymmetricADC]:
         number_of_composite_aqs = aq_dict["rep"]
         delay_first = self.system_specs.time_to_raster(Quantity(aq_dict["start"] - aq_dict["ref"], "ms"))
         delay_add = Quantity(aq_dict["dur"], "ms") + Quantity(aq_dict["interval"], "ms")
```

### Comparing `cmrseq-0.19/cmrseq/io/_pulseq.py` & `cmrseq-0.20/cmrseq/io/_pulseq.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/diffusion.py` & `cmrseq-0.20/cmrseq/parametric_definitions/diffusion.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
              - gmax: actually used max-gradient
              - slew: actually used slew-rate
              - b_actual: actual resulting b-value
     """
     # Strip units consistently for scipy optimize call
     gamma = system_specs.gamma_rad.m_as("1/ms/mT")
     max_slew = system_specs.max_slew.m_as("mT/m/ms") * 0.98
-    gmax = system_specs.max_grad.m_as("mT/m") * 0.99
+    gmax = system_specs.max_grad.m_as("mT/m") * 0.98
     zeta = system_specs.time_to_raster(Quantity(gmax / max_slew, "ms"))
     zeta = zeta.m
 
     def _optim(x): # Minimize total duration
         return 12 * zeta + 7 * x[0]
 
     def _constraint(x): # Match the target b-value
```

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/excitation.py` & `cmrseq-0.20/cmrseq/parametric_definitions/excitation.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                                             center=0.5, name="rf_excitation")
     ssgrad = cmrseq.bausteine.TrapezoidalGradient.from_fdur_amp(system_specs=system_specs,
                                                                 orientation=slice_normal,
                                                                 amplitude=gradient_amplitude,
                                                                 flat_duration=pulse_duration,
                                                                 name="slice_select")
 
-    rf_block.shift_time(ssgrad.gradients[0][1])
+    rf_block.shift(ssgrad.gradients[0][1])
 
     ssrefocus = cmrseq.bausteine.TrapezoidalGradient.from_area(
         system_specs=system_specs,
         orientation=-slice_normal,
         area=Quantity(np.abs(np.linalg.norm(ssgrad.area.m_as("mT/m*ms"), axis=-1) / 2), "mT/m*ms"),
         delay=ssgrad.gradients[0][-1],
         name="slice_select_rewind")
```

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/readout/__init__.py` & `cmrseq-0.20/cmrseq/parametric_definitions/readout/__init__.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py` & `cmrseq-0.20/cmrseq/parametric_definitions/readout/_cartesian_single_lines.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     if prephaser_duration is None:
         prephaser_duration = fastest_prep_flatdur + 2 * fastest_prep_ramp
     else:
         # Check if duration is sufficient for _combined_ prephaser gradients
         if prephaser_duration < np.round(fastest_prep_flatdur + 2 * fastest_prep_ramp, 7):
             raise ValueError("Prephaser duration is to short for combined PE+RO k-space traverse.")
 
-    readout_pulse.shift_time(prephaser_duration + delay)
+    readout_pulse.shift(prephaser_duration + delay)
     ro_prep_pulse = cmrseq.bausteine.TrapezoidalGradient.from_dur_area(
         system_specs=system_specs,
         orientation=np.array([-1., 0., 0.]),
         duration=prephaser_duration,
         area=prephaser_ro_area,
         delay=delay, name="ro_prephaser")
 
@@ -204,17 +204,17 @@
                              adc_duration=adc_duration, delay=delay,
                              prephaser_duration=prephaser_duration)
     # Copy prephasers
     prep_ro_block = deepcopy(seq.get_block("ro_prephaser_0"))
     prep_pe_block = deepcopy(seq.get_block("pe_prephaser_0"))
 
     # Shift to end of readout
-    ro_duration = seq.get_block("trapezoidal_readout_0").duration
-    prep_pe_block.shift_time(ro_duration + prep_pe_block.duration)
-    prep_ro_block.shift_time(ro_duration + prep_ro_block.duration)
+    ro_duration = seq["trapezoidal_readout_0"].duration
+    prep_pe_block.shift(ro_duration + prep_pe_block.duration)
+    prep_ro_block.shift(ro_duration + prep_ro_block.duration)
 
     # Invert amplidute
     prep_pe_block.scale_gradients(-1)
 
     prep_pe_block.name = "pe_prephaser_balance"
     prep_ro_block.name = "ro_prephaser_balance"
 
@@ -278,29 +278,28 @@
     ro_delay = delay + excitation_center_time + echo_time - adc_duration / 2
     readout_pulse = cmrseq.bausteine.TrapezoidalGradient.from_fdur_amp(
         system_specs=system_specs,
         orientation=np.array([1., 0., 0.]),
         flat_duration=adc_duration,
         amplitude=ro_amp, delay=ro_delay,
         name="readout_grad")
-    readout_pulse.shift_time(-readout_pulse.rise_time)
+    readout_pulse.shift(-readout_pulse.rise_time)
     prephaser_ro_area = readout_pulse.area[0] / 2.
     prephaser_pe_area = np.abs(k_phase / system_specs.gamma)
 
     # Total gradient traverse is a combination of ro and pe directions.
     # Need to solve as single gradient to ensure slew and strength restrictions are met
     combined_kspace_traverse = np.sqrt((prephaser_ro_area * system_specs.gamma) ** 2 + k_phase ** 2)
     [_, fastest_prep_ramp, fastest_prep_flatdur] = system_specs.get_shortest_gradient(
         combined_kspace_traverse / system_specs.gamma)
 
-    # If prephaser duration was not specified use the fastest posible prephaser
+    # If prephaser duration was not specified use the fastest possible prephaser
     if prephaser_duration is None:
         prephaser_duration = fastest_prep_flatdur + 2 * fastest_prep_ramp
     else:
-        # Check if duration is sufficient for _combined_ prephaser gradients
         if prephaser_duration < fastest_prep_flatdur + 2 * fastest_prep_ramp:
             raise ValueError("Prephaser duration is to short to for combined PE+RO "
                              "k-space traverse.")
 
     prephaser_delay = delay + echo_time / 2 - pulse_duration / 2 \
                       - prephaser_duration + excitation_center_time
     ro_prep_pulse = cmrseq.bausteine.TrapezoidalGradient.from_dur_area(
```

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/readout/_epi.py` & `cmrseq-0.20/cmrseq/parametric_definitions/readout/_epi.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,20 +60,21 @@
     :param blip_direction: (str) from ['up', 'down'] specifies the direction of phase encoding steps
     :param partial_fourier_lines: (int) number of lines to be skipped before k-space center
     :param slope_sampling: if True the unbound method (epi_ramp_sampling) is used, otherwise the 
                             unbound method (epi_flat_sampling) is used. 
     :param max_total_duration: Quantity needs to be specified if water-fat-shift is set to maximum.
     :param water-fat-shift: one of ['minimum', 'maximum', #pixels(float)]. Determines the echo-spacing therefore the 
                             duration of all
-                            according to the formula :math:`P/(C * (N+1)) = T` with (P)ixels, (C)hemicalf shift 
+                            according to the formula :math:`P/(C * (N+1)) = T` with (P)ixels, (C)hemical shift
                             frequency, (N)umber of k-space lines and (T) Echo spacing
     :param delay: Time gap added before the sequence
     """
     # Calculate k-space definitions
-    k_space_kwargs = _epi_fov_definition(field_of_view, matrix_size, blip_direction, partial_fourier_lines)
+    k_space_kwargs = _epi_fov_definition(field_of_view, matrix_size,
+                                         blip_direction, partial_fourier_lines)
     
     # Create building blocks to assemble epi train
     if slope_sampling:
         _ = _epi_ramp_sampling(system_specs=system_specs, water_fat_shift=water_fat_shift, 
                                max_total_duration=max_total_duration, **k_space_kwargs)
         ro_prephaser, pe_prephaser, readout_gradient, blip_gradient, adc_block = _
     else:
@@ -81,22 +82,22 @@
                                max_total_duration=max_total_duration, **k_space_kwargs)
         ro_prephaser, pe_prephaser, readout_gradient, blip_gradient, adc_block = _
 
     # Assemble single shot epi
     block_list = [ro_prephaser, pe_prephaser]
     for line_idx in range(matrix_size[1]):
         ro_block = deepcopy(readout_gradient)
-        ro_block.shift_time(ro_prephaser.duration + line_idx * readout_gradient.duration)
+        ro_block.shift(ro_prephaser.duration + line_idx * readout_gradient.duration)
         ro_block.scale_gradients((-1) ** line_idx)
         
         adc = deepcopy(adc_block)
-        adc.shift_time(ro_prephaser.duration + line_idx * readout_gradient.duration)
+        adc.shift(ro_prephaser.duration + line_idx * readout_gradient.duration)
         
         blip_block = deepcopy(blip_gradient)
-        blip_block.shift_time(ro_prephaser.duration + (line_idx + 1) * readout_gradient.duration)
+        blip_block.shift(ro_prephaser.duration + (line_idx + 1) * readout_gradient.duration)
         block_list.extend([ro_block, adc, blip_block])
        
     seq = cmrseq.Sequence(block_list[:-1], system_specs)
     if delay is not None:
         seq.shift_in_time(delay)
     return seq         
 
@@ -133,15 +134,15 @@
     """
    
     # Calculate Phase encoding Blip
     blip_amp, blip_rise, blip_flat = system_specs.get_shortest_gradient(np.abs(k_phase_step) / system_specs.gamma)
     blip_amp = np.sign(k_phase_step) * blip_amp
     blip_gradient = cmrseq.bausteine.TrapezoidalGradient(system_specs, orientation=np.array([0., 1., 0.]), amplitude=blip_amp,
                                                          flat_duration=blip_flat, rise_time=blip_rise, name="blip")
-    blip_gradient.shift_time(-blip_rise)
+    blip_gradient.shift(-blip_rise)
 
     # Calculate readout block
     kro_overshoot = (blip_gradient.duration / 2) ** 2 * system_specs.max_slew * system_specs.gamma
 
      # Calculate prephaser gradients
     combined_kspace_traverse = np.sqrt((k_readout / 2 + kro_overshoot / 2) ** 2 + k_phase_start ** 2)    
     [_, prephaser_rise, prephaser_flat] = system_specs.get_shortest_gradient(combined_kspace_traverse / system_specs.gamma)
@@ -225,15 +226,15 @@
     shortest_echo_spacing = min_adc_duration + 2 * ro_rise
     longest_echo_spacing = _calculate_longest_echo_spacing(system_specs, max_total_duration, 
                                                           (ro_rise*2 + min_adc_duration) * 1.5, k_phase_lines)
     echo_spacing = _set_echo_spacing_from_water_fat_shift(system_specs, water_fat_shift=water_fat_shift, 
                                                           n_epi_lines=k_phase_lines,
                                                           shortest_echo_spacing=shortest_echo_spacing,
                                                           longest_echo_spacing=longest_echo_spacing)
-    
+    echo_spacing = system_specs.time_to_raster(echo_spacing, "grad")
     ## This optimization requires following assumptions:
     # - Triangular blips
     # - Rise time delta of readout and blip are the same
     # (1) $\Delta k_{PE} = \gamma G_{PE} \delta $ 
     # (2) $k_{RO_max} = \gamma G_{RO} (T_{Echo_spacing} + 2\delta)$ => replace delta using (1)
     # (3) $s_{max} = \sqrt{G_{RO}^2 + G_{PE}^2} / \delta  => solve for G_{RO}
     # => Replace G_RO in (2) using (3) hand to wolfram alpha for simplification
@@ -263,26 +264,26 @@
         raise ValueError("No solution for triangular blips found. Decrease resolution in PE-direction or"
                          "try increasing the water-fat-shift.")
     
     shortes_root_idx = np.argmin(acceptable_roots[grads_in_bounds])
     ro_rise = acceptable_roots[grads_in_bounds][shortes_root_idx]
     ro_amp = ro_grad_amps[grads_in_bounds][shortes_root_idx]
     pe_amp = pe_grad_amps[grads_in_bounds][shortes_root_idx]
-    ## End of Triangular blip opitmization
 
+    ## End of Triangular blip opitmization
     readout_gradient = cmrseq.bausteine.TrapezoidalGradient(system_specs=system_specs, 
                                                             orientation=np.array([1., 0., 0.]),
                                                             flat_duration=echo_spacing-2*ro_rise, rise_time=ro_rise,
                                                             amplitude=ro_amp, name='readout')
     adc_block = cmrseq.bausteine.SymmetricADC(system_specs, num_samples, duration=echo_spacing-2*ro_rise, delay=ro_rise)
     blip_gradient = cmrseq.bausteine.TrapezoidalGradient(system_specs=system_specs, 
                                                          orientation=np.array([0., 1., 0.]) * np.sign(k_phase_step), 
                                                          flat_duration=Quantity(0, "ms"), rise_time=ro_rise, 
                                                          amplitude=pe_amp, name="blip")
-    blip_gradient.shift_time(-ro_rise)
+    blip_gradient.shift(-ro_rise)
 
     # Calculate prephaser gradients
     prephaser_ro_area = np.abs(readout_gradient.area[0]) / 2 
     prephaser_pe_area = np.abs(k_phase_start) / system_specs.gamma
     combined_kspace_traverse = np.sqrt((prephaser_ro_area * system_specs.gamma ) ** 2 + k_phase_start ** 2)    
     [_, prephaser_rise, prephaser_flat] = system_specs.get_shortest_gradient(combined_kspace_traverse / system_specs.gamma)
```

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/readout/_radial.py` & `cmrseq-0.20/cmrseq/parametric_definitions/readout/_radial.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/readout/_spiral.py` & `cmrseq-0.20/cmrseq/parametric_definitions/readout/_spiral.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_gradient_echo.py` & `cmrseq-0.20/cmrseq/parametric_definitions/sequences/_gradient_echo.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_spin_echo.py` & `cmrseq-0.20/cmrseq/parametric_definitions/sequences/_spin_echo.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/sequences/_ssfp.py` & `cmrseq-0.20/cmrseq/parametric_definitions/sequences/_ssfp.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     repetition_time = system_specs.time_to_raster(repetition_time)
     if repetition_time < minimal_tr:
         warn(f"Repetition time too short to be feasible, set TR to {minimal_tr}")
         repetition_time = minimal_tr
 
     tr_delay_half = system_specs.time_to_raster((repetition_time - minimal_tr)/2)
 
-    ss_compensate.shift_time(-ss_compensate.tmin + repetition_time - ss_compensate.duration)
+    ss_compensate.shift(-ss_compensate.tmin + repetition_time - ss_compensate.duration)
 
     # Add delay to match TR/2 after the first exication
     rf_seq.append(cmrseq.bausteine.Delay(system_specs, repetition_time/2 - rf_seq.duration))
 
     # Assemble blocks to list of sequences each representing one TR
     seq_list = [rf_seq]
     for tr_idx, ro_b in enumerate(ro_blocks):
```

### Comparing `cmrseq-0.19/cmrseq/parametric_definitions/velocity.py` & `cmrseq-0.20/cmrseq/parametric_definitions/velocity.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq/plotting.py` & `cmrseq-0.20/cmrseq/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import matplotlib.pyplot as plt
 from matplotlib import lines
 import matplotlib.patches as patches
 from mpl_toolkits.mplot3d.axes3d import Axes
 from matplotlib.ticker import FormatStrFormatter
 
 from cmrseq.core._sequence import Sequence
+from cmrseq.core.bausteine import ADC
 import cmrseq
 
 
 # pylint: disable=R0914, W0212, C0103, W0106
 def plot_moment(seq: Sequence, moment_order: int = 0,
                 axes: Tuple[plt.Axes] = None) -> plt.Figure:
     """ Creates a figure with a 3x1 subplot grid and plots the gradient moment
@@ -136,17 +137,17 @@
     t, gradients = seq.gradients_to_grid()
     if gradients is not None:
         labels = ["Gx", "Gy", "Gz"]
         for idx, ax, gc in zip(range(3), axes[1:], gradients):
             ax.plot(t, gc, color=f"C{idx}", label=labels[idx])
 
     # Plot ADC
-    for block in seq._blocks:
-        sampling_times = block.adc_timing
-        if sampling_times is not None:
+    for block in seq:
+        if isinstance(block, ADC):
+            sampling_times = block.adc_timing
             rect = patches.Rectangle((block.tmin.m_as("ms"), adc_yoffset-1),
                                      (block.tmax - block.tmin).m_as("ms"),
                                      2, linewidth=1.5, facecolor=(0, 0, 0, 0.1),
                                      edgecolor=(0., 0., 0., 0.2))
             if plot_center_lines:
                 axes[0].axvline(block.adc_center.m_as("ms"), linestyle="--",
                                 color=(234 / 256, 211 / 256, 168 / 256, 1.))
```

### Comparing `cmrseq-0.19/cmrseq/utils.py` & `cmrseq-0.20/cmrseq/utils.py`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/cmrseq.egg-info/PKG-INFO` & `cmrseq-0.20/cmrseq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmrseq
-Version: 0.19
+Version: 0.20
 Summary: UNKNOWN
 Home-page: https://gitlab.ethz.ch/jweine/cmrseq
 Author: Jonathan Weine, Charles McGrath
 Author-email: weine@biomed.ee.ethz.ch, mcgrath@biomed.ee.ethz.ch
 License: UNKNOWN
 Project-URL: Documentation, https://people.ee.ethz.ch/~jweine/cmrseq/latest/index.html
 Project-URL: Source, https://gitlab.ethz.ch/jweine/cmrseq
```

### Comparing `cmrseq-0.19/cmrseq.egg-info/SOURCES.txt` & `cmrseq-0.20/cmrseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmrseq-0.19/setup.py` & `cmrseq-0.20/setup.py`

 * *Files identical despite different names*

