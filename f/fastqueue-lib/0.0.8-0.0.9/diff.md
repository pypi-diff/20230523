# Comparing `tmp/fastqueue-lib-0.0.8.tar.gz` & `tmp/fastqueue-lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastqueue-lib-0.0.8.tar", last modified: Tue May 16 05:13:11 2023, max compression
+gzip compressed data, was "fastqueue-lib-0.0.9.tar", last modified: Wed May 17 02:48:48 2023, max compression
```

## Comparing `fastqueue-lib-0.0.8.tar` & `fastqueue-lib-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/fastqueue/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/fastqueue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/fastqueue/prototypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-16 05:13:11.000000 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-16 05:13:11.000000 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:13:11.000000 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 05:13:11.000000 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 05:13:11.000000 fastqueue-lib-0.0.8/fastqueue_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/src/ccqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/src/cllqueue.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    29961 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/src/fastqueue.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:13:11.592950 fastqueue-lib-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-05-16 05:12:59.000000 fastqueue-lib-0.0.8/tests/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:48:48.030657 fastqueue-lib-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 02:48:48.030657 fastqueue-lib-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:48:48.026656 fastqueue-lib-0.0.9/fastqueue/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/fastqueue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/fastqueue/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:48:48.026656 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 02:48:48.000000 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-17 02:48:48.000000 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:48:48.000000 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 02:48:48.000000 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 02:48:48.000000 fastqueue-lib-0.0.9/fastqueue_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 02:48:48.030657 fastqueue-lib-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:48:48.030657 fastqueue-lib-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/src/ccqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/src/cllqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30364 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/src/fastqueue.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:48:48.030657 fastqueue-lib-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-05-17 02:48:29.000000 fastqueue-lib-0.0.9/tests/test_queue.py
```

### Comparing `fastqueue-lib-0.0.8/LICENSE` & `fastqueue-lib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/PKG-INFO` & `fastqueue-lib-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastqueue-lib-0.0.8/README.md` & `fastqueue-lib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/fastqueue/prototypes.py` & `fastqueue-lib-0.0.9/fastqueue/prototypes.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/fastqueue_lib.egg-info/PKG-INFO` & `fastqueue-lib-0.0.9/fastqueue_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastqueue-lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Fast single ended queue library for python
 Author-email: Matthew Taylor <matthew.taylor.andre@gmail.com>
 Project-URL: Homepage, https://github.com/MatthewAndreTaylor/fastqueue
 Keywords: Queue
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastqueue-lib-0.0.8/pyproject.toml` & `fastqueue-lib-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastqueue-lib"
-version = "0.0.8"
+version = "0.0.9"
 description="Fast single ended queue library for python"
 authors = [
     {name = "Matthew Taylor", email = "matthew.taylor.andre@gmail.com"},
 ]
 urls = {Homepage = "https://github.com/MatthewAndreTaylor/fastqueue"}
 requires-python = ">=3.9"
 keywords = [ "Queue" ]
```

### Comparing `fastqueue-lib-0.0.8/setup.py` & `fastqueue-lib-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/src/ccqueue.cpp` & `fastqueue-lib-0.0.9/src/ccqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/src/cllqueue.cpp` & `fastqueue-lib-0.0.9/src/cllqueue.cpp`

 * *Files identical despite different names*

### Comparing `fastqueue-lib-0.0.8/src/fastqueue.c` & `fastqueue-lib-0.0.9/src/fastqueue.c`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 #include "pythread.h"
 
 /**
  * Single ended Contiguous Python Queue
  * --- fastqueue.QueueC ---
  */
 typedef struct {
-    PyObject_HEAD PyObject** objects;
+    PyObject_HEAD
+    PyObject** objects;
     int length;
     int capacity;
     int front;
     int back;
 } QueueC;
 
 static PyObject* QueueC_is_empty(QueueC* self, PyObject* args) {
@@ -64,14 +65,17 @@
     copy->capacity = self->capacity;
     copy->front = self->front;
     copy->back = self->back;
     return (PyObject*)copy;
 }
 
 static void QueueC_dealloc(QueueC* self) {
+    if (self == NULL) {
+        return;
+    }
     PyObject_GC_UnTrack(self);
     free(self->objects);
     Py_TYPE(self)->tp_free(self);
 }
 
 static int QueueC_clear(QueueC* self) {
     if (self->length == 0) {
@@ -320,30 +324,31 @@
     int numEntries; // Number of entries into this node
     int front;
     int back;
     struct QueueNode* next;
 } QueueNode_t;
 
 typedef struct Queue {
-    PyObject_HEAD QueueNode_t* head;
+    PyObject_HEAD
+    QueueNode_t* head;
     QueueNode_t* tail;
     int length; // Total number of py_objects stored in the queue
 } Queue_t;
 
 PyDoc_STRVAR(is_empty_doc, "Returns whether the queue is empty.");
 static PyObject* Queue_is_empty(Queue_t* self, PyObject* args) {
     if (self->length == 0) {
         Py_RETURN_TRUE;
     } else {
         Py_RETURN_FALSE;
     }
 }
 
 // Initialize a new QueueNode
-static QueueNode_t* QueueNode_new() {
+static inline QueueNode_t* QueueNode_new() {
     QueueNode_t* node = (QueueNode_t*)malloc(sizeof(QueueNode_t));
     node->numEntries = 0;
     node->front = 255;
     node->back = 0;
     node->next = NULL;
     return node;
 }
@@ -439,23 +444,23 @@
              "Remove and return an item from the end of the Queue.");
 static PyObject* Queue_dequeue(Queue_t* self) {
     if (self->length == 0) {
         PyErr_SetString(PyExc_IndexError, "dequeue from an empty Queue");
         return NULL;
     }
 
-    PyObject* py_object = self->head->py_objects[self->head->back];
-    self->head->back = (self->head->back + 1) & 255;
-    self->head->numEntries--;
+    QueueNode_t* head = self->head;
+    PyObject* py_object = head->py_objects[head->back];
+    head->back = (head->back + 1) & 255;
+    head->numEntries--;
     self->length--;
 
-    if (self->head->numEntries <= 0) {
-        QueueNode_t* oldHead = self->head;
-        self->head = self->head->next;
-        free(oldHead);
+    if (head->numEntries <= 0) {
+        self->head = head->next;
+        free(head);
     }
 
     if (self->head == NULL) {
         self->tail = NULL;
     }
 
     return py_object;
@@ -485,14 +490,17 @@
     self->head = NULL;
     self->tail = NULL;
     return 0;
 }
 
 // Deallocate the Queue
 static void Queue_dealloc(Queue_t* self) {
+    if (self == NULL) {
+        return;
+    }
     PyObject_GC_UnTrack(self);
     if (self->head != NULL) {
         Queue_clear(self);
     }
     Py_TYPE(self)->tp_free((PyObject*)self);
 }
 
@@ -666,15 +674,16 @@
     (initproc)Queue_init,                    /* tp_init */
     PyType_GenericAlloc,                     /* tp_alloc */
     (newfunc)Queue_new,                      /* tp_new */
     PyObject_GC_Del,                         /* tp_free */
 };
 
 typedef struct LockQueue {
-    PyObject_HEAD Queue_t* queue;
+    PyObject_HEAD
+    Queue_t* queue;
     PyThread_type_lock lock;
 } LockQueue_t;
 
 static PyObject* LockQueue_new(PyTypeObject* type, PyObject* args,
                                PyObject* kwargs) {
     LockQueue_t* self = (LockQueue_t*)type->tp_alloc(type, 0);
     if (self == NULL) {
@@ -768,21 +777,31 @@
 static int LockQueue_contains(LockQueue_t* self, PyObject* args) {
     PyThread_acquire_lock(self->lock, 1);
     int res = Queue_contains(self->queue, args);
     PyThread_release_lock(self->lock);
     return res;
 }
 
+PyDoc_STRVAR(get_doc,
+             "Return the first element of the LockQueue, None if no element exists.");
+static PyObject* LockQueue_get(LockQueue_t* self, PyObject* args) {
+    if (LockQueue_len(self) > 0) {
+        return LockQueue_dequeue(self);
+    }
+    Py_RETURN_NONE;
+}
+
 static PyMethodDef LockQueue_methods[] = {
     {"is_empty", (PyCFunction)LockQueue_is_empty, METH_NOARGS, is_empty_doc},
     {"enqueue", (PyCFunction)LockQueue_enqueue, METH_O, enqueue_doc},
     {"dequeue", (PyCFunction)LockQueue_dequeue, METH_NOARGS, dequeue_doc},
     {"extend", (PyCFunction)LockQueue_extend, METH_O, extend_doc},
     {"__copy__", (PyCFunction)LockQueue_copy, METH_NOARGS, copy_doc},
     {"copy", (PyCFunction)LockQueue_copy, METH_NOARGS, copy_doc},
+    {"get", (PyCFunction)LockQueue_get, METH_NOARGS, get_doc},
     {NULL, NULL, 0, NULL}};
 
 static PySequenceMethods LockQueue_sequence_methods = {
     (lenfunc)LockQueue_len,             /* sq_length */
     0,                                  /* sq_concat */
     NULL,                               /* sq_repeat */
     (ssizeargfunc)LockQueue_item,       /* sq_item */
```

### Comparing `fastqueue-lib-0.0.8/tests/test_queue.py` & `fastqueue-lib-0.0.9/tests/test_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     # Tests for mutation
     lst = [1, 2, 3]
     queue.extend(lst)
     assert len(queue) == 3
     assert lst == [1, 2, 3]
     assert lst[2] == 3
     assert queue[2] == 3
-
     queue.extend([])
     assert len(queue) == 3
     assert lst == [1, 2, 3]
     assert lst[2] == 3
     assert queue[2] == 3
 
     with pytest.raises(TypeError):
@@ -174,14 +173,17 @@
     assert q.is_empty()
     q = queue([i for i in range(10)])
     assert len(q) == 10
     assert not q.is_empty()
     assert [q.dequeue() for _ in range(len(q))] == list(range(10))
     q = queue(range(10))
     assert len(q) == 10
+    q.enqueue(10)
+    assert list(q) == [i for i in range(11)]
+    assert [q.dequeue() for _ in range(len(q))] == list(range(11))
 
     with pytest.raises(TypeError):
         q = queue(0)
 
     with pytest.raises(TypeError):
         q = queue([1, 2], [])
```

