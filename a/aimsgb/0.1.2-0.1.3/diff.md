# Comparing `tmp/aimsgb-0.1.2.tar.gz` & `tmp/aimsgb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimsgb-0.1.2.tar", last modified: Fri May 12 05:17:06 2023, max compression
+gzip compressed data, was "aimsgb-0.1.3.tar", last modified: Tue May 23 21:21:36 2023, max compression
```

## Comparing `aimsgb-0.1.2.tar` & `aimsgb-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.261973 aimsgb-0.1.2/
--rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-0.1.2/LICENSE.txt
--rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-12 05:17:06.262088 aimsgb-0.1.2/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)     3697 2022-06-21 05:53:18.000000 aimsgb-0.1.2/README.rst
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.259312 aimsgb-0.1.2/aimsgb/
--rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-0.1.2/aimsgb/__init__.py
--rw-r--r--   0 jianli     (501) staff       (20)     7367 2023-05-09 23:32:55.000000 aimsgb-0.1.2/aimsgb/agb.py
--rw-r--r--   0 jianli     (501) staff       (20)     8833 2023-05-12 04:44:43.000000 aimsgb-0.1.2/aimsgb/grain.py
--rw-r--r--   0 jianli     (501) staff       (20)    22091 2023-05-12 04:44:56.000000 aimsgb-0.1.2/aimsgb/grain_bound.py
--rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-0.1.2/aimsgb/utils.py
-drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-12 05:17:06.261763 aimsgb-0.1.2/aimsgb.egg-info/
--rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/PKG-INFO
--rw-r--r--   0 jianli     (501) staff       (20)      310 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/SOURCES.txt
--rw-r--r--   0 jianli     (501) staff       (20)        1 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/dependency_links.txt
--rw-r--r--   0 jianli     (501) staff       (20)       43 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/entry_points.txt
--rw-r--r--   0 jianli     (501) staff       (20)       22 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/requires.txt
--rw-r--r--   0 jianli     (501) staff       (20)        7 2023-05-12 05:17:06.000000 aimsgb-0.1.2/aimsgb.egg-info/top_level.txt
--rw-r--r--   0 jianli     (501) staff       (20)       80 2023-05-12 05:17:06.262523 aimsgb-0.1.2/setup.cfg
--rw-r--r--   0 jianli     (501) staff       (20)     5238 2023-05-10 20:13:09.000000 aimsgb-0.1.2/setup.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.320016 aimsgb-0.1.3/
+-rw-r--r--   0 jianli     (501) staff       (20)     1788 2022-06-20 22:26:12.000000 aimsgb-0.1.3/LICENSE.txt
+-rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-23 21:21:36.320140 aimsgb-0.1.3/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)     3620 2023-05-21 04:14:14.000000 aimsgb-0.1.3/README.rst
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.317365 aimsgb-0.1.3/aimsgb/
+-rw-r--r--   0 jianli     (501) staff       (20)       47 2018-10-27 01:29:57.000000 aimsgb-0.1.3/aimsgb/__init__.py
+-rw-r--r--   0 jianli     (501) staff       (20)     7081 2023-05-23 20:48:44.000000 aimsgb-0.1.3/aimsgb/agb.py
+-rw-r--r--   0 jianli     (501) staff       (20)     9250 2023-05-23 20:48:44.000000 aimsgb-0.1.3/aimsgb/grain.py
+-rw-r--r--   0 jianli     (501) staff       (20)    22091 2023-05-15 17:32:21.000000 aimsgb-0.1.3/aimsgb/grain_bound.py
+-rw-r--r--   0 jianli     (501) staff       (20)     2256 2018-10-27 01:29:57.000000 aimsgb-0.1.3/aimsgb/utils.py
+drwxr-xr-x   0 jianli     (501) staff       (20)        0 2023-05-23 21:21:36.319633 aimsgb-0.1.3/aimsgb.egg-info/
+-rw-r--r--   0 jianli     (501) staff       (20)     4796 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/PKG-INFO
+-rw-r--r--   0 jianli     (501) staff       (20)      310 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/SOURCES.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        1 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/dependency_links.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       43 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/entry_points.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       22 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/requires.txt
+-rw-r--r--   0 jianli     (501) staff       (20)        7 2023-05-23 21:21:36.000000 aimsgb-0.1.3/aimsgb.egg-info/top_level.txt
+-rw-r--r--   0 jianli     (501) staff       (20)       80 2023-05-23 21:21:36.320695 aimsgb-0.1.3/setup.cfg
+-rw-r--r--   0 jianli     (501) staff       (20)     5238 2023-05-23 21:20:02.000000 aimsgb-0.1.3/setup.py
```

### Comparing `aimsgb-0.1.2/LICENSE.txt` & `aimsgb-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.2/PKG-INFO` & `aimsgb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.2
+Version: 0.1.3
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 2
```

### Comparing `aimsgb-0.1.2/README.rst` & `aimsgb-0.1.3/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Introduction
 ============
-aimsgb, an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
+aimsgb is an efficient and open-source Python library for generating atomic coordinates in periodic grain boundary models. It is designed to
 construct various grain boundary structures from cubic and non-cubic initial
 configurations. A convenient command line tool has also been provided to enable
 easy and fast construction of tilt and twist boundaries by assigining the degree
 of fit (Σ), rotation axis, grain boundary plane and initial crystal structure.
-aimsgb is expected to greatly accelerate the theoretical investigation of
-grain boundary properties and facilitate the experimental analysis of grain
-boundary structures as well.
 
 We also provide a web-based GUI to access aimsgb framework: `aimsgb.org
-<http://aimsgb.org/>`_
+<https://aimsgb.org/>`_
 
 Install aimsgb
 ==============
 Method 1: Use Pip
 -----------------
 The easiest way to install aimsgb is to simply run a one-liner in pip::
 
@@ -35,14 +32,19 @@
     pip install .
 
 4. or to install the package in development mode::
 
     pip install -e .
 
 
+Usage
+==================
+Refer to the `documentation
+<https://aimsgb-docs.readthedocs.io/en/latest/>`_ for more details.
+
 How to cite aimsgb
 ==================
 
 If you use aimsgb in your research, please consider citing the following work:
 
     Jianli Cheng, Jian Luo, Kesong Yang. *Aimsgb: An algorithm and open-source python
     library to generate periodic grain boundary structures.* Computational Materials
@@ -66,15 +68,14 @@
 This software program and documentation are copyrighted by The Regents of the University of California. The software program and documentation are supplied “as is”, without any accompanying services from The Regents. The Regents does not warrant that the operation of the program will be uninterrupted or error-free. The end-user understands that the program was developed for research purposes and is advised not to rely exclusively on the program for any reason.
 
 IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE SOFTWARE PROVIDED HEREUNDER IS ON AN “AS IS” BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
 
 
 Authors
 =======
-Dr. Jianli Cheng (jic198@ucsd.edu)
-New Email: jianlicheng@lbl.gov
+Dr. Jianli Cheng (chengjianli90@gmail.com)
 
 Prof. Kesong Yang  (kesong@ucsd.edu)
 
 About the aimsgb Development Team
 =================================
 http://materials.ucsd.edu/
```

### Comparing `aimsgb-0.1.2/aimsgb/agb.py` & `aimsgb-0.1.3/aimsgb/agb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 from __future__ import division
 
 import sys
 import argparse
 import numpy as np
-from mp_api.client import MPRester, MPRestError
 
 from aimsgb import Grain, GBInformation, GrainBoundary
 
 __author__ = "Jianli Cheng and Kesong YANG"
 __copyright__ = "Copyright (C) 2018 The Regents of the University of California"
 __maintainer__ = "Jianli Cheng"
 __email__ = "jic198@ucsd.edu"
@@ -36,20 +35,15 @@
 def gb(args):
     axis = list(map(int, args.axis))
     plane = args.plane
     initial_struct = None
     if args.filename:
         initial_struct = Grain.from_file(args.filename)
     elif args.mpid:
-        mpr = MPRester()
-        try:
-            s = mpr.get_structure_by_material_id(args.mpid)
-            initial_struct = Grain.from_dict(s.as_dict())
-        except MPRestError:
-            raise MPRestError("Please run 'export MP_API_KEY=YOUR_MAPI_KEY' to setup your api_key first.")
+        initial_struct = Grain.from_mp_id(args.mpid)
     if initial_struct is None:
         raise ValueError("Please provide either filename or mpid.")
     
     gb = GrainBoundary(axis, args.sigma, plane, initial_struct, args.uc_a, args.uc_b)
     to_primitive = False if args.conventional else True
     gb.build_gb(args.vacuum, args.add_if_dist, to_primitive, args.delete_layer,
                 args.tol).to(filename=args.out, fmt=args.fmt)
```

### Comparing `aimsgb-0.1.2/aimsgb/grain.py` & `aimsgb-0.1.3/aimsgb/grain.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,30 @@
             axis = (0, 1, 0)
         anchor = grain_b.lattice.get_cartesian_coords(np.array([.0, .0, .0]))
         # print(axis, anchor)
         # exit()
         grain_b.rotate_sites(theta=np.radians(180), axis=axis, anchor=anchor)
         return grain_b
 
+    @classmethod
+    def from_mp_id(cls, mp_id):
+        """
+        Get a structure from Materials Project database.
+        Args:
+            mp_id (str): Materials Project ID.
+
+        Returns:
+            A structure object.
+        """
+        from mp_api.client import MPRester
+
+        mpr = MPRester()
+        s = mpr.get_structure_by_material_id(mp_id, conventional_unit_cell=True)
+        return cls.from_dict(s.as_dict())
+
     def make_supercell(self, scaling_matrix):
         """
         Create a supercell. Very similar to pymatgen's Structure.make_supercell
         However, we need to make sure that all fractional coordinates that equal
         to 1 will become 0 and the lattice are redefined so that x_c = [0, 0, c]
     
         Args:
@@ -167,15 +183,15 @@
         csl_t = csl.transpose()
         # rotate along a longer axis between a and b
         grain_a = self.copy()
         grain_a.make_supercell(csl_t)
         # grain_a.to(filename='POSCAR')
         # exit()
 
-        if not all([i == 90 for i in grain_a.lattice.angles]):
+        if not grain_a.lattice.is_orthogonal:
             warnings.warn("The lattice system of the grain is not orthogonal. "
                           "aimsgb will find a supercell of the grain structure "
                           "that is orthogonalized. This may take a while. ")
             cst = CubicSupercellTransformation(force_90_degrees=True,
                                                min_length=min(grain_a.lattice.abc))
             _s = grain_a.copy()
             _s = cst.apply_transformation(_s)
```

### Comparing `aimsgb-0.1.2/aimsgb/grain_bound.py` & `aimsgb-0.1.3/aimsgb/grain_bound.py`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.2/aimsgb/utils.py` & `aimsgb-0.1.3/aimsgb/utils.py`

 * *Files identical despite different names*

### Comparing `aimsgb-0.1.2/aimsgb.egg-info/PKG-INFO` & `aimsgb-0.1.3/aimsgb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimsgb
-Version: 0.1.2
+Version: 0.1.3
 Summary: aimsgb is a python library for generatng the atomic coordinates of periodic grain boundaries.Copyright © 2018 The Regents of the University of California.All Rights Reserved. See more in Copyright.
 Home-page: http://aimsgb.org
 Author: Jianli Cheng and Kesong YANG
 Maintainer: Jianli Cheng, Sicong JIANG, and Kesong YANG
 Maintainer-email: chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu
 Keywords: material science,grain boundary,molecular simulation
 Classifier: Programming Language :: Python :: 2
```

### Comparing `aimsgb-0.1.2/setup.py` & `aimsgb-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 =================================
 http://materials.ucsd.edu/
 """
 
 setup(
     name="aimsgb",
     packages=find_packages(),
-    version="0.1.2",
+    version="0.1.3",
     setup_requires=["setuptools>=18.0"],
     install_requires=["pymatgen", "mp_api", "numpy"],
     include_package_data=True,
     author="Jianli Cheng and Kesong YANG",
     maintainer="Jianli Cheng, Sicong JIANG, and Kesong YANG",
     maintainer_email="chengjianli90@gmail.com, sij014@ucsd.edu, kesong@ucsd.edu",
     url="http://aimsgb.org",
```

