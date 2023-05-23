# Comparing `tmp/olympipe-1.1.7.tar.gz` & `tmp/olympipe-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympipe-1.1.7.tar", max compression
+gzip compressed data, was "olympipe-1.1.8.tar", max compression
```

## Comparing `olympipe-1.1.7.tar` & `olympipe-1.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-05-11 20:44:35.079416 olympipe-1.1.7/LICENSE
--rw-r--r--   0        0        0     3887 2023-05-11 20:44:35.083416 olympipe-1.1.7/README.md
--rw-r--r--   0        0        0    10410 2023-05-11 20:44:35.083416 olympipe-1.1.7/olympipe/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-11 20:44:35.083416 olympipe-1.1.7/olympipe/dispatcher.py
--rw-r--r--   0        0        0        0 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/__init__.py
--rw-r--r--   0        0        0     1718 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/batch.py
--rw-r--r--   0        0        0      530 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/explode.py
--rw-r--r--   0        0        0      524 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/filter.py
--rw-r--r--   0        0        0     2185 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/generic.py
--rw-r--r--   0        0        0     1649 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/instance.py
--rw-r--r--   0        0        0     1180 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/reduce.py
--rw-r--r--   0        0        0      408 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/task.py
--rw-r--r--   0        0        0     1899 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/pipes/timebatch.py
--rw-r--r--   0        0        0        0 2023-05-11 20:44:35.084416 olympipe-1.1.7/olympipe/py.typed
--rw-r--r--   0        0        0      646 2023-05-11 20:44:35.084416 olympipe-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 07:04:07.327230 olympipe-1.1.8/LICENSE
+-rw-r--r--   0        0        0     3887 2023-05-23 07:04:07.330230 olympipe-1.1.8/README.md
+-rw-r--r--   0        0        0    10513 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/dispatcher.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/__init__.py
+-rw-r--r--   0        0        0     1718 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/batch.py
+-rw-r--r--   0        0        0      530 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/explode.py
+-rw-r--r--   0        0        0      524 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/filter.py
+-rw-r--r--   0        0        0     2428 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/generic.py
+-rw-r--r--   0        0        0     1649 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/instance.py
+-rw-r--r--   0        0        0     1180 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/reduce.py
+-rw-r--r--   0        0        0      408 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/task.py
+-rw-r--r--   0        0        0     1899 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/pipes/timebatch.py
+-rw-r--r--   0        0        0        0 2023-05-23 07:04:07.330230 olympipe-1.1.8/olympipe/py.typed
+-rw-r--r--   0        0        0      646 2023-05-23 07:04:07.330230 olympipe-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 olympipe-1.1.8/PKG-INFO
```

### Comparing `olympipe-1.1.7/LICENSE` & `olympipe-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/README.md` & `olympipe-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/__init__.py` & `olympipe-1.1.8/olympipe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __version__ = "1.1.1"
 
-from multiprocessing import Process, Queue
+from multiprocessing import Process, Queue, TimeoutError
 from threading import Timer
 from typing import (
     Any,
     Callable,
     Dict,
     Generic,
     Iterable,
@@ -246,16 +246,18 @@
                     continue
                 try:
                     packet = output_queue.get(timeout=0.1)
                     if GenericPipe.is_death_packet(packet):
                         output_queues[i] = None
                     else:
                         outputs[i].append(packet)
-                except Exception:
+                except TimeoutError:
                     pass
+                except Exception as e:
+                    print("Error waiting:", e)
 
         return outputs
 
     def wait_for_completion(
         self, other_pipes: List["Pipeline[Any]"] = [], debug_graph: Optional[str] = None
     ) -> None:
         """_summary_
```

### Comparing `olympipe-1.1.7/olympipe/dispatcher.py` & `olympipe-1.1.8/olympipe/dispatcher.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/batch.py` & `olympipe-1.1.8/olympipe/pipes/batch.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/explode.py` & `olympipe-1.1.8/olympipe/pipes/explode.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/filter.py` & `olympipe-1.1.8/olympipe/pipes/filter.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/generic.py` & `olympipe-1.1.8/olympipe/pipes/generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+import multiprocessing
 import queue
 import time
 from multiprocessing import Process, Queue
 from queue import Empty
 from threading import Timer
 from typing import Any, Generic, Optional, Tuple, TypeVar, cast
 
 R = TypeVar("R")
 S = TypeVar("S")
 
 
 class GenericPipe(Process, Generic[R, S]):
-    __kill_word: Any = Empty
+    __kill_word: Any = Exception("Pipeline kill")
 
     def __init__(self, source: "Queue[R]", target: "Queue[S]"):
         super().__init__(daemon=True)
         self._source = source
         self._target = target
         self._timeout: Optional[float] = 0.1
         Timer(0.01, self.start).start()
 
     @staticmethod
     def is_death_packet(p: Any) -> bool:
         try:
-            return p[0] is GenericPipe.__kill_word
+            return (
+                type(p[0]) is type(GenericPipe.__kill_word)
+                and p[0].args == GenericPipe.__kill_word.args
+            )
+
         except Exception:
             return False
 
     @staticmethod
     def get_kill_word(count: int = 1) -> Any:
         return (GenericPipe.__kill_word, count)
 
@@ -51,16 +56,18 @@
         return cast(S, data)
 
     def _send_to_next(self, processed: S):
         while True:
             try:
                 self._target.put(processed, timeout=self._timeout)
                 break
-            except Exception as e:
+            except multiprocessing.TimeoutError:
                 pass
+            except Exception as e:
+                print("Error sending:", e)
 
     def run(self):
         while True:
             try:
                 data = self._source.get(timeout=self._timeout)
                 if GenericPipe.is_death_packet(data):
                     self._kill(data)
```

### Comparing `olympipe-1.1.7/olympipe/pipes/instance.py` & `olympipe-1.1.8/olympipe/pipes/instance.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/reduce.py` & `olympipe-1.1.8/olympipe/pipes/reduce.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/olympipe/pipes/timebatch.py` & `olympipe-1.1.8/olympipe/pipes/timebatch.py`

 * *Files identical despite different names*

### Comparing `olympipe-1.1.7/pyproject.toml` & `olympipe-1.1.8/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olympipe"
-version = "1.1.7"
+version = "1.1.8"
 description = "A powerful parallel pipelining tool"
 readme = "README.md"
 license = "MIT"
 homepage = "https://gitlab.com/gabraken/olympipe"
 repository = "https://gitlab.com/gabraken/olympipe"
 authors = ["Gabriel Kasser <gabriel.kasser@gmail.com>"]
 keywords = ["pipeline", "multiprocessing"]
```

### Comparing `olympipe-1.1.7/PKG-INFO` & `olympipe-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympipe
-Version: 1.1.7
+Version: 1.1.8
 Summary: A powerful parallel pipelining tool
 Home-page: https://gitlab.com/gabraken/olympipe
 License: MIT
 Keywords: pipeline,multiprocessing
 Author: Gabriel Kasser
 Author-email: gabriel.kasser@gmail.com
 Requires-Python: >=3.7.2,<4.0
```

