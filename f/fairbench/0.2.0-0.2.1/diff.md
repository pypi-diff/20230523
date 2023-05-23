# Comparing `tmp/fairbench-0.2.0-py3-none-any.whl.zip` & `tmp/fairbench-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 22576 bytes, number of entries: 32
--rw-rw-rw-  2.0 fat      196 b- defN 23-May-14 10:32 fairbench/__init__.py
+Zip file size: 22677 bytes, number of entries: 32
+-rw-rw-rw-  2.0 fat      196 b- defN 23-May-23 12:15 fairbench/__init__.py
 -rw-rw-rw-  2.0 fat      512 b- defN 23-Jan-15 16:07 fairbench/accumulate.py
 -rw-rw-rw-  2.0 fat     1790 b- defN 23-Jan-15 16:07 fairbench/algorithms.py
 -rw-rw-rw-  2.0 fat     1885 b- defN 23-May-18 19:58 fairbench/export.py
 -rw-rw-rw-  2.0 fat     9339 b- defN 23-May-17 23:49 fairbench/fork.py
 -rw-rw-rw-  2.0 fat     1744 b- defN 23-Jan-15 16:07 fairbench/output.py
 -rw-rw-rw-  2.0 fat     2393 b- defN 23-Jan-15 16:07 fairbench/reduction.py
 -rw-rw-rw-  2.0 fat     1146 b- defN 23-Jan-15 16:07 fairbench/reporting.py
 -rw-rw-rw-  2.0 fat       38 b- defN 23-May-14 10:33 fairbench/bench/__init__.py
 -rw-rw-rw-  2.0 fat      583 b- defN 23-May-14 15:09 fairbench/bench/loader.py
 -rw-rw-rw-  2.0 fat      122 b- defN 23-May-13 22:58 fairbench/forks/__init__.py
--rw-rw-rw-  2.0 fat     1579 b- defN 23-May-18 19:42 fairbench/forks/categorical.py
+-rw-rw-rw-  2.0 fat     2041 b- defN 23-May-22 12:01 fairbench/forks/categorical.py
 -rw-rw-rw-  2.0 fat     1903 b- defN 23-May-17 23:49 fairbench/forks/explanation.py
--rw-rw-rw-  2.0 fat    22620 b- defN 23-May-18 21:03 fairbench/forks/fork.py
+-rw-rw-rw-  2.0 fat    22629 b- defN 23-May-23 09:59 fairbench/forks/fork.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Jan-14 23:08 fairbench/metrics/__init__.py
 -rw-rw-rw-  2.0 fat     1816 b- defN 23-May-15 14:34 fairbench/metrics/classification.py
 -rw-rw-rw-  2.0 fat     2007 b- defN 23-Jan-15 16:07 fairbench/metrics/disparate_impact.py
 -rw-rw-rw-  2.0 fat     1450 b- defN 23-Jan-15 16:07 fairbench/metrics/disparate_mistreatment.py
 -rw-rw-rw-  2.0 fat      207 b- defN 23-Jan-15 14:06 fairbench/reports/__init__.py
 -rw-rw-rw-  2.0 fat     1255 b- defN 23-May-18 22:06 fairbench/reports/accumulate.py
 -rw-rw-rw-  2.0 fat     1629 b- defN 23-May-18 18:48 fairbench/reports/adhoc.py
 -rw-rw-rw-  2.0 fat     2239 b- defN 23-May-18 21:23 fairbench/reports/base.py
 -rw-rw-rw-  2.0 fat     4980 b- defN 23-May-17 23:49 fairbench/reports/reduction.py
 -rw-rw-rw-  2.0 fat      883 b- defN 23-May-14 15:09 fairbench/reports/surrogate.py
 -rw-rw-rw-  2.0 fat      155 b- defN 23-Feb-20 08:42 fairbench/reports/reduction/__init__.py
 -rw-rw-rw-  2.0 fat      856 b- defN 23-May-14 19:29 fairbench/reports/reduction/expanders.py
 -rw-rw-rw-  2.0 fat     1819 b- defN 23-May-18 21:31 fairbench/reports/reduction/reduce.py
 -rw-rw-rw-  2.0 fat     2604 b- defN 23-Feb-20 08:40 fairbench/reports/reduction/reducers.py
--rw-rw-rw-  2.0 fat      786 b- defN 23-May-18 23:43 fairbench-0.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 23:43 fairbench-0.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-18 23:43 fairbench-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2689 b- defN 23-May-18 23:43 fairbench-0.2.0.dist-info/RECORD
-32 files, 71481 bytes uncompressed, 18254 bytes compressed:  74.5%
+-rw-rw-rw-  2.0 fat      786 b- defN 23-May-23 13:05 fairbench-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 13:05 fairbench-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-23 13:05 fairbench-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2689 b- defN 23-May-23 13:05 fairbench-0.2.1.dist-info/RECORD
+32 files, 71952 bytes uncompressed, 18355 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -78,20 +78,20 @@
 
 Filename: fairbench/reports/reduction/reduce.py
 Comment: 
 
 Filename: fairbench/reports/reduction/reducers.py
 Comment: 
 
-Filename: fairbench-0.2.0.dist-info/METADATA
+Filename: fairbench-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: fairbench-0.2.0.dist-info/WHEEL
+Filename: fairbench-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: fairbench-0.2.0.dist-info/top_level.txt
+Filename: fairbench-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: fairbench-0.2.0.dist-info/RECORD
+Filename: fairbench-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fairbench/forks/categorical.py

```diff
@@ -1,8 +1,8 @@
-from fairbench.forks.fork import tobackend, istensor
+from fairbench.forks.fork import tobackend, istensor, Fork
 from typing import Iterable, Mapping
 
 
 class Categorical(dict):
     def __and__(self, other):
         ret = Categorical()
         for k, v in self.items():
@@ -42,14 +42,27 @@
 
 @Transform
 def binary(x):
     x = tobackend(x)
     return {"1": x, "0": 1 - x}
 
 
+class Categories:
+    def __init__(self, values: Iterable, generator=lambda data, category: data == category):
+        self.categories = list(values)
+        self.generator = generator
+
+    def __call__(self, other):
+        return self.__matmul__(other)
+
+    def __matmul__(self, other):
+        assert not isinstance(other, Fork)
+        return Categorical({str(category): self.generator(other, category) for category in self.categories})
+
+
 @Transform
 def categories(x):
     assert isinstance(x, Iterable)
     if isinstance(x, Mapping):
         return Categorical(x)
     vals = list(set(x))
     return {
```

## fairbench/forks/fork.py

```diff
@@ -92,29 +92,29 @@
     if isinstance(value, ep.Tensor):
         return value.raw
 
     return value
 
 
 class Fork(Mapping):
-    def __init__(self, *args, _prefix="", **branches):
+    def __init__(self, *args, _separator="", **branches):
         for arg in args:
             if not isinstance(arg, dict):
                 raise TypeError(
                     "Forks can only support dicts (holding branch values) as positional arguments"
                 )
             for k, v in arg.items():
                 if k in branches:
                     raise TypeError(f"Branch {k} provided multiple times")
                 branches[k] = v
         self._branches = dict()
         for k, v in branches.items():
             if isinstance(v, dict) and v.__class__.__name__ == "Categorical":
                 for k2, v2 in v.items():
-                    self._branches[str(k2) if _prefix is None else k + _prefix + str(k2)] = v2
+                    self._branches[str(k2) if _separator is None else k + _separator + str(k2)] = v2
             else:
                 self._branches[k] = v
 
     def __getattribute__(self, name):
         if name in ["_branches", "_repr_html_"] or name in dir(Fork):
             return object.__getattribute__(self, name)
         if name.startswith("_"):
```

## Comparing `fairbench-0.2.0.dist-info/METADATA` & `fairbench-0.2.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairbench
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fairness model assessment framework
 Home-page: https://github.com/mever-team/FairBench
 Author: Emmanouil (Manios) Krasanakis
 Author-email: maniospas@hotmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `fairbench-0.2.0.dist-info/RECORD` & `fairbench-0.2.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 fairbench/fork.py,sha256=VAgJ6MeD5a6mK_BMrIJdXPxLpp7wz0wjTSy59IJOSJU,9339
 fairbench/output.py,sha256=wvusKkx72F9i0EZoWpM8vR3NYTkpJTc8rtj5oLTKkRA,1744
 fairbench/reduction.py,sha256=PkHMY4B8SuwwV7-dq_dQXW2bhx2tr8jQ7iAXy9kilVE,2393
 fairbench/reporting.py,sha256=jcZtJXjTQAstzTPMjcnQei053k_LUkVrA1oLVsfOIog,1146
 fairbench/bench/__init__.py,sha256=piA_S0SAZ96_-MxdcGO_V7pCKngOFBeAv8KGj9rkGRA,38
 fairbench/bench/loader.py,sha256=BXmttN9Ee-TA6FAb1gXMhlJutDN2B6XIea6TU0Cre14,583
 fairbench/forks/__init__.py,sha256=eBRDSxc31Pc1yKCc1VjFBvPMsBVaOzVOfXHpkYQodG0,122
-fairbench/forks/categorical.py,sha256=3dZqvs_BQNN4E3DpfRd2ZzZv5FUrNbP4mPAfa1x2rGI,1579
+fairbench/forks/categorical.py,sha256=sOECZ2-WrbZomqLcZz7bTXJR4vKRPoXsR6OrpjlIMdw,2041
 fairbench/forks/explanation.py,sha256=rQjkNuemRDvjSp4R2Gw8Mv2o8-Fd_mrbrIM_v7opEY0,1903
-fairbench/forks/fork.py,sha256=oWqLWouxxSb3qRi7hpDBga0XoPUCm2t4n4q6y-nokf4,22620
+fairbench/forks/fork.py,sha256=IMtBv-d9iuAi_9A4NpQVycCcwp6cN4Hvx9ZHJm04Rdg,22629
 fairbench/metrics/__init__.py,sha256=i2kNaDKTfTSEh1aGZ83ByaVXwv0gYE-guFNjj9XlF6I,154
 fairbench/metrics/classification.py,sha256=263Wz5ILnq3OxyzPopLAM-tWszcsC2v1F6SSKqqDuVo,1816
 fairbench/metrics/disparate_impact.py,sha256=rLO82wWOSDI4s5aK9WjehIbuUrCLuog7pOV8SSBVEZI,2007
 fairbench/metrics/disparate_mistreatment.py,sha256=4xtayr0k5Z7ZAtlrFevDiUjQloJ6uhqPucgxPFrwES8,1450
 fairbench/reports/__init__.py,sha256=YQm7A6K3PUB4uNOw3iDu2RUaoWa07Rsn3GJr4wZkn2M,207
 fairbench/reports/accumulate.py,sha256=xRY708vEy7B3DcyC2Tec8XLdFAv9Q_Ru7Hw1np_l64Y,1255
 fairbench/reports/adhoc.py,sha256=7FhOawdzoK3MtY6o8wLaxKDrJ1QZmG5XTTSxra4-D-w,1629
 fairbench/reports/base.py,sha256=tCpaurqYfuV3MGkwNIAr7QFlPeFHDenC2rgPUVKm79A,2239
 fairbench/reports/reduction.py,sha256=zSo8Whi-tW8trPmN946e2gyLp6xR7b8WMZzYyPmWgIc,4980
 fairbench/reports/surrogate.py,sha256=LnV6kkNPMGL2SYEBSSIFWjkXQ8N5m2k4y5as2zUyDt8,883
 fairbench/reports/reduction/__init__.py,sha256=a3c0w4bKV3f6NXnGMPPGFRxdfg_YIrcccy_mEBSr8zk,155
 fairbench/reports/reduction/expanders.py,sha256=BR6R9VwcFjbPC8WROrrE823oGwcbjuTgXyKBWjwvs3o,856
 fairbench/reports/reduction/reduce.py,sha256=fXNdsdSQnXS9ah_E9v9DicbZcZZE23bgAWr-Jee8i-E,1819
 fairbench/reports/reduction/reducers.py,sha256=5NA8FbXLieB9iV22aqPyOrpy7MZLtFviHiedxrMGMv0,2604
-fairbench-0.2.0.dist-info/METADATA,sha256=IF4bKFyOfbbnbwoUu_OhsMsl-iCgzZAeQRSZItCmMUc,786
-fairbench-0.2.0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fairbench-0.2.0.dist-info/top_level.txt,sha256=V_xpM0npsVDF1PcMECNA-pE1JrkHNp3p62aiR-7iqDk,10
-fairbench-0.2.0.dist-info/RECORD,,
+fairbench-0.2.1.dist-info/METADATA,sha256=-klzTrYG8Rfg6mi9zK5uygw675W6tZ02T0A0ZleIJQ4,786
+fairbench-0.2.1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fairbench-0.2.1.dist-info/top_level.txt,sha256=V_xpM0npsVDF1PcMECNA-pE1JrkHNp3p62aiR-7iqDk,10
+fairbench-0.2.1.dist-info/RECORD,,
```

