# Comparing `tmp/lackadaisical-1.0.0a2-py3-none-any.whl.zip` & `tmp/lackadaisical-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4276 bytes, number of entries: 11
--rw-r--r--  2.0 unx        8 b- defN 23-May-18 08:08 lackadaisical/VERSION
--rw-r--r--  2.0 unx     1167 b- defN 23-May-18 08:08 lackadaisical/__init__.py
--rw-r--r--  2.0 unx      359 b- defN 23-May-18 08:08 lackadaisical/faster_than.py
--rw-r--r--  2.0 unx       67 b- defN 23-May-18 08:08 lackadaisical/logging.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-18 08:08 lackadaisical/py.typed
--rw-r--r--  2.0 unx      368 b- defN 23-May-18 08:08 lackadaisical/too_slow.py
--rw-r--r--  2.0 unx     1073 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/LICENSE
--rw-r--r--  2.0 unx      880 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      902 b- defN 23-May-18 08:08 lackadaisical-1.0.0a2.dist-info/RECORD
-11 files, 4930 bytes uncompressed, 2730 bytes compressed:  44.6%
+Zip file size: 5079 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        6 b- defN 23-May-23 10:20 lackadaisical/VERSION
+-rw-r--r--  2.0 unx      284 b- defN 23-May-23 10:20 lackadaisical/__init__.py
+-rw-r--r--  2.0 unx      789 b- defN 23-May-23 10:20 lackadaisical/faster_than.py
+-rw-r--r--  2.0 unx       67 b- defN 23-May-23 10:20 lackadaisical/logging.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 10:20 lackadaisical/py.typed
+-rw-r--r--  2.0 unx      701 b- defN 23-May-23 10:20 lackadaisical/too_slow.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-23 10:20 lackadaisical-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3214 b- defN 23-May-23 10:20 lackadaisical-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 10:20 lackadaisical-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-23 10:20 lackadaisical-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      892 b- defN 23-May-23 10:20 lackadaisical-1.0.1.dist-info/RECORD
+11 files, 7132 bytes uncompressed, 3553 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: lackadaisical/py.typed
 Comment: 
 
 Filename: lackadaisical/too_slow.py
 Comment: 
 
-Filename: lackadaisical-1.0.0a2.dist-info/LICENSE
+Filename: lackadaisical-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: lackadaisical-1.0.0a2.dist-info/METADATA
+Filename: lackadaisical-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: lackadaisical-1.0.0a2.dist-info/WHEEL
+Filename: lackadaisical-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: lackadaisical-1.0.0a2.dist-info/top_level.txt
+Filename: lackadaisical-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: lackadaisical-1.0.0a2.dist-info/RECORD
+Filename: lackadaisical-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lackadaisical/VERSION

```diff
@@ -1 +1 @@
-1.0.0a2
+1.0.1
```

## lackadaisical/__init__.py

```diff
@@ -1,34 +1,7 @@
-"""
-# Support
-
-Please submit all your questions, feature requests and bug reports at
-[github.com/cariad/lackadaisical/issues](https://github.com/cariad/lackadaisical/issues).
-Thank you!
-
-# Licence
-
-Lackadaisical is [open-source](https://github.com/cariad/lackadaisical) and
-released under the
-[MIT License](https://github.com/cariad/lackadaisical/blob/main/LICENSE).
-
-You don't have to give attribution in your project, but -- as a freelance
-developer with rent to pay -- I appreciate it!
-
-# Author
-
-Hello! 👋 I'm **Cariad Eccleston**, and I'm a freelance Amazon Web Services
-architect, DevOps evangelist, CI/CD pipeline engineer and backend developer.
-
-You can find me at [cariad.earth](https://www.cariad.earth),
-[github/cariad](https://github.com/cariad),
-[linkedin/cariad](https://linkedin.com/in/cariad) and on Mastodon at
-[@cariad@tech.lgbt](https://tech.lgbt/@cariad).
-"""
-
 from importlib.resources import open_text
 
 from lackadaisical.faster_than import assert_faster_than
 from lackadaisical.too_slow import TooSlow
 
 with open_text(__package__, "VERSION") as t:
     __version__ = t.readline().strip()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## lackadaisical/faster_than.py

```diff
@@ -3,12 +3,31 @@
 from typing import Iterator
 
 from lackadaisical.too_slow import TooSlow
 
 
 @contextmanager
 def assert_faster_than(seconds: float) -> Iterator[None]:
+    """
+    Tracks the execution time of a block of code and raises `TooSlow` if the
+    actual duration is not less than `seconds`.
+
+    Can be used as either a function decorator or a context manager.
+
+    ```python
+    @assert_faster_than(30)
+    def test() -> None:
+        my_slow_function()
+    ```
+
+    ```python
+    def test() -> None:
+        with assert_faster_than(30):
+            my_slow_function()
+    ```
+    """
+
     start = perf_counter()
     yield
     duration = perf_counter() - start
-    if duration > seconds:
+    if duration >= seconds:
         raise TooSlow(seconds, duration)
```

## lackadaisical/too_slow.py

```diff
@@ -1,11 +1,31 @@
 class TooSlow(Exception):
+    """
+    Raised if a block of code takes too long to execute.
+    """
+
     def __init__(self, expected: float, actual: float) -> None:
-        self.expected_seconds = expected
-        self.actual_seconds = actual
+        self._expected = expected
+        self._actual = actual
 
-        actual_plural = "" if actual == 1 else "s"
+        plural = "" if actual == 1 else "s"
 
         super().__init__(
-            f"Operation took {actual:.1f} second{actual_plural} (expected "
-            f"{expected} at most)"
+            f"Operation took {actual:.1f} second{plural} (expected {expected} "
+            "at most)"
         )
+
+    @property
+    def actual(self) -> float:
+        """
+        Actual execution time in seconds.
+        """
+
+        return self._actual
+
+    @property
+    def expected(self) -> float:
+        """
+        Expected execution time in seconds.
+        """
+
+        return self._expected
```

## Comparing `lackadaisical-1.0.0a2.dist-info/LICENSE` & `lackadaisical-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lackadaisical-1.0.0a2.dist-info/RECORD` & `lackadaisical-1.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-lackadaisical/VERSION,sha256=LXUCGsKHGGt0wefNXJd79GwVqjrn4sseR1ce6an5XIY,8
-lackadaisical/__init__.py,sha256=97kd_ckRTm4dZrW1btjjsIpsMxugkEtWzc8kgR6Qc7s,1167
-lackadaisical/faster_than.py,sha256=MiX8eXyel7D_jM7P7vlRwhX2ucOrBGiYbCbUSSM3m8I,359
+lackadaisical/VERSION,sha256=ROFh5ElcrCz3hYBD6eZBjpV58N3ProJvmjcmIpaM4GY,6
+lackadaisical/__init__.py,sha256=hUgjVTKUVAwmNi70l_l8JIaAr-NgNlQhIMmNFOGM5z8,284
+lackadaisical/faster_than.py,sha256=pOwbbJiniI10y59iNrmYfQt3BVxLancekg3QzU2rAPU,789
 lackadaisical/logging.py,sha256=sNW5CzWbjJq_QFfvS8UjrjNZrYwpa5O6VoNJ3CWmYEo,67
 lackadaisical/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lackadaisical/too_slow.py,sha256=KYqSJjSi91L8Yh4G8zJd3691-h5gl6bAk2diUbhhEew,368
-lackadaisical-1.0.0a2.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
-lackadaisical-1.0.0a2.dist-info/METADATA,sha256=Cu1JgNkWBDaLlIFocscibKfsUXLNY4oq42KvgwjrJUI,880
-lackadaisical-1.0.0a2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-lackadaisical-1.0.0a2.dist-info/top_level.txt,sha256=Rf4_1coYZpMJ35dacwQtLPJLW16DM98lWHwuEQ5nmRw,14
-lackadaisical-1.0.0a2.dist-info/RECORD,,
+lackadaisical/too_slow.py,sha256=iWRHwpjOiFj3iqzAVPFbt-oAJeAz8bf-8wu4MNoH1HI,701
+lackadaisical-1.0.1.dist-info/LICENSE,sha256=jXz8xZq3cMjXXQ2Hb9sj6RNKFigwHmut-OnbWc-uHOU,1073
+lackadaisical-1.0.1.dist-info/METADATA,sha256=FQ4POWcL0SL94ShfxEfp7BuLx01l_nzM4jgW17zYNck,3214
+lackadaisical-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+lackadaisical-1.0.1.dist-info/top_level.txt,sha256=Rf4_1coYZpMJ35dacwQtLPJLW16DM98lWHwuEQ5nmRw,14
+lackadaisical-1.0.1.dist-info/RECORD,,
```

