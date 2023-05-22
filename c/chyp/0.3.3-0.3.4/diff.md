# Comparing `tmp/chyp-0.3.3.tar.gz` & `tmp/chyp-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.3.3.tar", last modified: Mon May 15 12:11:41 2023, max compression
+gzip compressed data, was "chyp-0.3.4.tar", last modified: Mon May 22 13:07:09 2023, max compression
```

## Comparing `chyp-0.3.3.tar` & `chyp-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3.3/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-15 12:11:41.629822 chyp-0.3.3/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9508 2023-05-13 17:50:25.000000 chyp-0.3.3/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3.3/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3.3/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3.3/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3.3/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3.3/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3.3/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5986 2023-05-11 09:13:14.000000 chyp-0.3.3/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15809 2023-05-15 12:09:38.000000 chyp-0.3.3/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3.3/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3.3/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3.3/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3.3/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3.3/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10454 2023-05-13 12:29:20.000000 chyp-0.3.3/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11316 2023-05-15 07:42:45.000000 chyp-0.3.3/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8791 2023-05-13 11:26:15.000000 chyp-0.3.3/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3.3/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3.3/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3.3/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4602 2023-05-11 09:04:26.000000 chyp-0.3.3/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4143 2023-05-11 20:25:03.000000 chyp-0.3.3/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3.3/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-15 12:11:41.629822 chyp-0.3.3/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-15 12:11:16.000000 chyp-0.3.3/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 13:07:09.527420 chyp-0.3.4/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3.4/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-22 13:07:09.527420 chyp-0.3.4/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9508 2023-05-13 17:50:25.000000 chyp-0.3.4/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 13:07:09.523420 chyp-0.3.4/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3.4/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3.4/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17136 2023-05-22 08:47:36.000000 chyp-0.3.4/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 13:07:09.527420 chyp-0.3.4/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3.4/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2521 2023-05-21 22:38:05.000000 chyp-0.3.4/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4260 2023-05-22 08:21:41.000000 chyp-0.3.4/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4174 2023-05-22 08:21:19.000000 chyp-0.3.4/chyp/gui/colors.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1409 2023-05-21 08:49:19.000000 chyp-0.3.4/chyp/gui/completion.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4758 2023-05-21 15:36:02.000000 chyp-0.3.4/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11629 2023-05-22 08:03:32.000000 chyp-0.3.4/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2634 2023-05-16 16:58:14.000000 chyp-0.3.4/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     7344 2023-05-22 08:48:47.000000 chyp-0.3.4/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3.4/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2656 2023-05-22 08:16:55.000000 chyp-0.3.4/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13408 2023-05-22 08:23:18.000000 chyp-0.3.4/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10454 2023-05-13 12:29:20.000000 chyp-0.3.4/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11334 2023-05-16 15:36:05.000000 chyp-0.3.4/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    14143 2023-05-22 08:59:15.000000 chyp-0.3.4/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3788 2023-05-22 08:48:25.000000 chyp-0.3.4/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3.4/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3.4/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4634 2023-05-16 16:15:03.000000 chyp-0.3.4/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4143 2023-05-11 20:25:03.000000 chyp-0.3.4/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 13:07:09.523420 chyp-0.3.4/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-22 13:07:09.000000 chyp-0.3.4/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3.4/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-22 13:07:09.527420 chyp-0.3.4/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-22 13:06:35.000000 chyp-0.3.4/setup.py
```

### Comparing `chyp-0.3.3/LICENSE` & `chyp-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/PKG-INFO` & `chyp-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3.3
+Version: 0.3.4
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.3.3/README.md` & `chyp-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/__init__.py` & `chyp-0.3.4/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/__main__.py` & `chyp-0.3.4/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/graph.py` & `chyp-0.3.4/chyp/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,25 @@
 class EData:
     def __init__(self,
             s: Optional[List[int]]=None,
             t: Optional[List[int]]=None,
             value: Any="",
             x: float=0,
             y: float=0,
+            fg: str='',
+            bg: str='',
             hyper: bool=True) -> None:
         self.value = value
         self.highlight = False
         self.x = x
         self.y = y
         self.s = [] if s is None else s
         self.t = [] if t is None else t
+        self.fg = fg
+        self.bg = bg
         self.hyper = hyper
 
     def __repr__(self) -> str:
         return "Edge: %s (%d, %d)" % (self.value, self.x, self.y)
 
     def box_size(self) -> int:
         """Returns the number of 'units' of width the box should have to display nicely.
@@ -126,15 +130,15 @@
             self.vindex += 1
         else:
             v = name
 
         self.vdata[v] = VData(x, y, value)
         return v
 
-    def add_edge(self, s:List[int], t:List[int], value:Any="", x:float=0, y:float=0, hyper:bool=True, name:int=-1) -> int:
+    def add_edge(self, s:List[int], t:List[int], value:Any="", x:float=0, y:float=0, fg:str='', bg:str='', hyper:bool=True, name:int=-1) -> int:
         """Add an edge to the graph
         
         :param s:     A list of source vertices
         :param t:     A list of target vertices
         :param value: The value carried by this edge (typically a string)
         :param x:     The X coordinate to draw the box representing this hyperedge
         :param y:     The Y coordinate
@@ -147,15 +151,15 @@
         """
         if name == -1:
             e = self.eindex
             self.eindex += 1
         else:
             e = name
 
-        self.edata[e] = EData(s, t, value, x, y, hyper)
+        self.edata[e] = EData(s, t, value, x, y, fg, bg, hyper)
         for v in s: self.vdata[v].out_edges.add(e)
         for v in t: self.vdata[v].in_edges.add(e)
         return e
 
     def remove_vertex(self, v: int, strict: bool=False) -> None:
         if strict:
             if (len(self.vertex_data(v).in_edges)  > 0 or
@@ -339,15 +343,15 @@
             vd = other.vertex_data(v)
             vmap[v] = self.add_vertex(vd.x, vd.y - min_other + 1, vd.value)
 
         for e in other.edges():
             ed = other.edge_data(e)
             self.add_edge([vmap[v] for v in ed.s],
                           [vmap[v] for v in ed.t],
-                          ed.value, ed.x, ed.y - min_other + 1)
+                          ed.value, ed.x, ed.y - min_other + 1, ed.fg, ed.bg, ed.hyper)
         
         self.set_inputs(self.inputs() + [vmap[v] for v in other.inputs()])
         self.set_outputs(self.outputs() + [vmap[v] for v in other.outputs()])
 
     def __mul__(self, other: Graph) -> Graph:
         g = self.copy()
         g.tensor(other)
@@ -370,15 +374,15 @@
             vd = other.vertex_data(v)
             vmap[v] = self.add_vertex(vd.x - min_other, vd.y, vd.value)
 
         for e in other.edges():
             ed = other.edge_data(e)
             self.add_edge([vmap[v] for v in ed.s],
                           [vmap[v] for v in ed.t],
-                          ed.value, ed.x - min_other, ed.y)
+                          ed.value, ed.x - min_other, ed.y, ed.fg, ed.bg, ed.hyper)
         
         plug1 = self.outputs()
         plug2 = [vmap[v] for v in other.inputs()]
         quotient: Dict[int,int] = dict()
         if len(plug1) != len(plug2):
             raise GraphError("Attempting to plug a graph with %d outputs into one with %d inputs" % (len(plug1), len(plug2)))
 
@@ -394,19 +398,19 @@
                 quotient[p2] = p1
 
     def __rshift__(self, other: Graph) -> Graph:
         g = self.copy()
         g.compose(other)
         return g
 
-def gen(value: str, arity: int, coarity: int) -> Graph:
+def gen(value: str, arity: int, coarity: int, fg: str='', bg: str='') -> Graph:
     g = Graph()
     inputs = [g.add_vertex(-1.5, i - (arity-1)/2) for i in range(arity)]
     outputs = [g.add_vertex(1.5, i - (coarity-1)/2) for i in range(coarity)]
-    g.add_edge(inputs, outputs, value)
+    g.add_edge(inputs, outputs, value, fg=fg, bg=bg)
     g.set_inputs(inputs)
     g.set_outputs(outputs)
     return g
         
 def perm(p: List[int]) -> Graph:
     g = Graph()
     size = len(p)
```

### Comparing `chyp-0.3.3/chyp/gui/__init__.py` & `chyp-0.3.4/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/gui/document.py` & `chyp-0.3.4/chyp/gui/document.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,41 +18,25 @@
 from PySide6.QtCore import QDir, QFileInfo, QSettings, Signal
 from PySide6.QtGui import QFont, QTextDocument
 from PySide6.QtWidgets import QFileDialog, QMessageBox, QPlainTextDocumentLayout, QWidget
 
 from .highlighter import ChypHighlighter
 
 class ChypDocument(QTextDocument):
-    recentFilesChanged = Signal()
     fileNameChanged = Signal()
-    documentReplaced = Signal()
+    # documentReplaced = Signal()
 
     def __init__(self, parent: QWidget) -> None:
         super().__init__(parent)
         self.parent_widget = parent
         self.setDefaultFont(QFont("monospace", 14))
         self.setDocumentLayout(QPlainTextDocumentLayout(self))
         self.highlighter = ChypHighlighter(self)
         self.file_name = ''
         
-    def recent_files(self) -> List[str]:
-        conf = QSettings('chyp', 'chyp')
-        o = conf.value('recent_files', [])
-        return o if isinstance(o, list) else []
-
-    def add_to_recent_files(self, file_name: str) -> None:
-        conf = QSettings('chyp', 'chyp')
-        o = conf.value('recent_files', [])
-        recent_files: List[str] = o if isinstance(o, list) else [] 
-        recent_files = [f for f in recent_files if f != file_name]
-        recent_files.insert(0, file_name)
-        recent_files = recent_files[:10]
-        conf.setValue('recent_files', recent_files)
-        self.recentFilesChanged.emit()
-
     def confirm_close(self) -> bool:
         if self.isModified():
             text = "Do you wish to save changes to {}?".format(
                     self.file_name if self.file_name != '' else 'Untitled')
             res = QMessageBox.question(self.parent_widget,
                                        "Save changes",
                                        text,
@@ -66,41 +50,30 @@
             elif res == QMessageBox.StandardButton.No:
                 return True
             else:
                 return False
         else:
             return True
 
-    def new(self) -> None:
-        if self.confirm_close():
-            self.file_name = ''
-            self.setPlainText('')
-            self.setModified(False)
-            self.fileNameChanged.emit()
-            self.documentReplaced.emit()
+    def add_to_recent_files(self, file_name: str) -> None:
+        conf = QSettings('chyp', 'chyp')
+        o = conf.value('recent_files', [])
+        recent_files: List[str] = o if isinstance(o, list) else [] 
+        recent_files = [f for f in recent_files if f != file_name]
+        recent_files.insert(0, file_name)
+        recent_files = recent_files[:10]
+        conf.setValue('recent_files', recent_files)
 
-    def open(self, file_name: str='') -> None:
-        if self.confirm_close():
-            conf = QSettings('chyp', 'chyp')
-            if file_name == '':
-                o = conf.value('last_dir')
-                last_dir = o if isinstance(o, str) else QDir.home().absolutePath()
-                file_name, _ = QFileDialog.getOpenFileName(self.parent_widget,
-                                                           "Open File",
-                                                           last_dir,
-                                                           'chyp files (*.chyp)')
-            if file_name:
-                conf.setValue('last_dir', QFileInfo(file_name).absolutePath())
-                self.file_name = file_name
-                with open(file_name) as f:
-                    self.setPlainText(f.read())
-                self.add_to_recent_files(self.file_name)
-                self.setModified(False)
-                self.fileNameChanged.emit()
-                self.documentReplaced.emit()
+    def open(self, file_name: str) -> None:
+        self.file_name = file_name
+        with open(file_name) as f:
+            self.setPlainText(f.read())
+        self.add_to_recent_files(self.file_name)
+        self.setModified(False)
+        self.fileNameChanged.emit()
 
     def save(self) -> bool:
         if self.file_name:
             with open(self.file_name, 'w') as f:
                 f.write(self.toPlainText())
             self.add_to_recent_files(self.file_name)
             self.setModified(False)
```

### Comparing `chyp-0.3.3/chyp/gui/editor.py` & `chyp-0.3.4/chyp/gui/mainwindow.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,405 +10,349 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-from typing import Callable, Dict, Optional, Tuple
-from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, QTimer, Qt, QSettings
-from PySide6.QtGui import QCloseEvent, QKeySequence, QTextCursor
-from PySide6.QtWidgets import QApplication, QHBoxLayout, QMainWindow, QMenuBar, QSplitter, QTreeView, QVBoxLayout, QWidget
-
-from ..layout import convex_layout
-from ..graph import Graph
-from ..state import RewriteState, State
-from ..term import graph_to_term
-from ..matcher import match_rule
-from ..rewrite import rewrite
-
-from .errorlist import ErrorListModel
-from .graphview import GraphView
-from .codeview import CodeView
-from .document import ChypDocument
-from .highlighter import STATUS_GOOD, STATUS_BAD
+from typing import Callable, List, Optional
+from PySide6.QtCore import QByteArray, QDir, QFileInfo, QSettings, Qt
+from PySide6.QtGui import QActionGroup, QCloseEvent, QKeySequence
+from PySide6.QtWidgets import QApplication, QFileDialog, QMainWindow, QMenuBar, QMessageBox, QTabWidget, QVBoxLayout, QWidget
 
-class Editor(QMainWindow):
+from .editor import Editor
+
+
+class MainWindow(QMainWindow):
     def __init__(self) -> None:
         super().__init__()
         conf = QSettings('chyp', 'chyp')
 
         self.setWindowTitle("chyp")
 
+        self.tabs = QTabWidget()
+        self.tabs.setFocusPolicy(Qt.FocusPolicy.NoFocus)
+        self.tabs.currentChanged.connect(self.tab_changed)
+
         w = QWidget(self)
         w.setLayout(QVBoxLayout())
         self.setCentralWidget(w)
         w.layout().setContentsMargins(0,0,0,0)
         w.layout().setSpacing(0)
+        w.layout().addWidget(self.tabs)
         self.resize(1600, 800)
         
         geom = conf.value("editor_window_geometry")
         if geom and isinstance(geom, QByteArray): self.restoreGeometry(geom)
         self.show()
 
-        # save splitter position
-        self.splitter = QSplitter(Qt.Orientation.Vertical)
-        w.layout().addWidget(self.splitter)
-
-        self.state = State()
-
-        self.lhs_view = GraphView()
-        self.rhs_view = GraphView()
-        self.rhs_view.setVisible(False)
-
-        self.graph_panel = QWidget(self)
-        self.graph_panel.setLayout(QHBoxLayout())
-        self.graph_panel.layout().addWidget(self.lhs_view)
-        self.graph_panel.layout().addWidget(self.rhs_view)
-        self.splitter.addWidget(self.graph_panel)
-
-        self.code_view = CodeView()
-        self.doc = ChypDocument(self)
-        self.code_view.setDocument(self.doc)
-        self.doc.fileNameChanged.connect(self.update_file_name)
-        self.doc.modificationChanged.connect(self.update_file_name)
-        self.doc.recentFilesChanged.connect(self.update_recent_files)
-        self.doc.documentReplaced.connect(self.reset_state)
+        self.active_editor: Optional[Editor] = None
+        self.add_tab(Editor(), "Untitled")
         self.update_file_name()
+        self.build_menu()
 
-        self.splitter.addWidget(self.code_view)
-        self.code_view.setFocus()
 
-        self.error_view = QTreeView()
-        self.error_view.setModel(ErrorListModel())
-        self.splitter.addWidget(self.error_view)
+    def remove_empty_editor(self) -> None:
+        if self.active_editor:
+            if self.active_editor.title() == 'Untitled' and self.active_editor.doc.toPlainText() == '':
+                self.tabs.removeTab(self.tabs.indexOf(self.active_editor))
+                self.active_editor = None
 
-        self.build_menu()
+    def update_file_name(self) -> None:
+        for i in range(self.tabs.count()):
+            w = self.tabs.widget(i)
+            if isinstance(w, Editor):
+                self.tabs.setTabText(i, w.title())
+        if self.active_editor:
+            self.setWindowTitle('chyp - ' + self.active_editor.title())
+
+    def tab_changed(self, i: int) -> None:
+        w = self.tabs.widget(i)
+        if isinstance(w, Editor):
+            self.active_editor = w
+            self.active_editor.code_view.setFocus()
+            self.update_file_name()
+
+    def update_themes(self) -> None:
+        conf = QSettings('chyp', 'chyp')
+        theme_name = conf.value('theme')
+        if not theme_name or not isinstance(theme_name, str):
+            theme_name = 'catppuccin_macchiato'
+
+        def set_th(t: str) -> Callable:
+            def f() -> None:
+                conf.setValue('theme', t)
+                QMessageBox.information(self, 'Theme set',
+                                        'You must restart Chyp for the new theme to take effect.')
+            return f
+
+        themes_group = QActionGroup(self)
+
+        view_themes_dark = self.view_themes.addAction("Dark")
+        view_themes_dark.setCheckable(True)
+        view_themes_dark.setChecked(theme_name == 'catppuccin_macchiato')
+        view_themes_dark.triggered.connect(set_th('catppuccin_macchiato'))
+
+        view_themes_light = self.view_themes.addAction("Light")
+        view_themes_light.setCheckable(True)
+        view_themes_light.setChecked(theme_name == 'catppuccin_latte')
+        view_themes_light.triggered.connect(set_th('catppuccin_latte'))
+
+        themes_group.addAction(view_themes_dark)
+        themes_group.addAction(view_themes_light)
 
-        splitter_state = conf.value("editor_splitter_state")
-        if splitter_state and isinstance(splitter_state, QByteArray): self.splitter.restoreState(splitter_state)
+    def recent_files(self) -> List[str]:
+        conf = QSettings('chyp', 'chyp')
+        o = conf.value('recent_files', [])
+        return o if isinstance(o, list) else []
+
+    def update_recent_files(self) -> None:
+        def open_recent(f: str) -> Callable:
+            return lambda: self.open(f)
 
-        self.code_view.cursorPositionChanged.connect(self.show_at_cursor)
-        self.code_view.textChanged.connect(self.invalidate_text)
-        self.parsed = True
+        self.file_open_recent.clear()
+        for f in self.recent_files():
+            fi = QFileInfo(f)
+            action = self.file_open_recent.addAction(fi.fileName())
+            action.triggered.connect(open_recent(f))
+
+    def add_tab(self, editor: Editor, title: str) -> None:
+        self.tabs.addTab(editor, title)
+        editor.doc.fileNameChanged.connect(self.update_file_name)
+        editor.doc.modificationChanged.connect(self.update_file_name)
+        self.tabs.setCurrentWidget(editor)
+        editor.reset_state()
+
+    def close_tab(self, editor: Optional[Editor]=None) -> bool:
+        if editor is None:
+            editor = self.active_editor
+
+        if editor:
+            i = self.tabs.indexOf(editor)
+            if i != -1 and editor.doc.confirm_close():
+                editor.doc.fileNameChanged.disconnect(self.update_file_name)
+                editor.doc.modificationChanged.disconnect(self.update_file_name)
+                self.tabs.removeTab(i)
+
+                if self.tabs.count() == 0:
+                    app = QApplication.instance()
+                    if app:
+                        app.quit()
+
+                return True
+
+        return False
+
+    def new(self) -> None:
+        self.remove_empty_editor()
+        editor = Editor()
+        self.add_tab(editor, "Untitled")
+
+    def open(self, file_name: str='') -> None:
+        conf = QSettings('chyp', 'chyp')
+
+        # if no file name provided, show open dialog
+        if file_name == '':
+            o = conf.value('last_dir')
+            last_dir = o if isinstance(o, str) else QDir.home().absolutePath()
+            file_name, _ = QFileDialog.getOpenFileName(self,
+                                                       "Open File",
+                                                       last_dir,
+                                                       'chyp files (*.chyp)')
+
+        # if file is already open, just focus the tab
+        for i in range(self.tabs.count()):
+            w = self.tabs.widget(i)
+            if isinstance(w, Editor) and w.doc.file_name == file_name:
+                self.tabs.setCurrentWidget(w)
+                return
+
+        try:
+            editor = Editor()
+            editor.doc.open(file_name)
+            conf.setValue('last_dir', QFileInfo(file_name).absolutePath())
+            self.remove_empty_editor()
+            self.update_recent_files()
+            editor.doc.fileNameChanged.connect(self.update_file_name)
+            self.add_tab(editor, editor.title())
+        except FileNotFoundError:
+            QMessageBox.warning(self, "File not found", "File not found: " + file_name)
+
+
+    def save(self) -> None:
+        if self.active_editor:
+            self.active_editor.doc.save()
+            self.update_recent_files()
+
+    def save_as(self) -> None:
+        if self.active_editor:
+            self.active_editor.doc.save_as()
+            self.update_recent_files()
+    
+    def undo(self) -> None:
+        if self.active_editor:
+            self.active_editor.code_view.undo()
+
+    def redo(self) -> None:
+        if self.active_editor:
+            self.active_editor.code_view.redo()
+
+    def show_errors(self) -> None:
+        if self.active_editor:
+            self.active_editor.show_errors()
+
+    def add_rewrite_step(self) -> None:
+        if self.active_editor:
+            self.active_editor.code_view.add_line_below("  = ? by ")
+
+    def repeat_rewrite_step(self) -> None:
+        if self.active_editor:
+            self.active_editor.repeat_step_at_cursor()
+
+    def next_rewrite(self) -> None:
+        if self.active_editor:
+            self.active_editor.next_rewrite_at_cursor()
+
+    def next_part(self) -> None:
+        if self.active_editor:
+            self.active_editor.next_part(step=1)
+
+    def previous_part(self) -> None:
+        if self.active_editor:
+            self.active_editor.next_part(step=-1)
+
+    def next_tab(self) -> None:
+        c = self.tabs.count()
+        if c != 0:
+            i = (self.tabs.currentIndex() + 1) % c
+            self.tabs.setCurrentIndex(i)
+
+    def previous_tab(self) -> None:
+        c = self.tabs.count()
+        if c != 0:
+            i = (self.tabs.currentIndex() - 1) % c
+            self.tabs.setCurrentIndex(i)
+
+    def goto_import(self) -> None:
+        if self.active_editor:
+            f = self.active_editor.import_at_cursor()
+            if f:
+                self.open(f)
+
+
+    def closeEvent(self, e: QCloseEvent) -> None:
+        conf = QSettings('chyp', 'chyp')
+        conf.setValue("editor_window_geometry", self.saveGeometry())
+
+        if self.active_editor:
+            conf.setValue("editor_splitter_state", self.active_editor.splitter.saveState())
+            sizes = self.active_editor.splitter.sizes()
+            if sizes[2] != 0:
+                conf.setValue('error_panel_size', sizes[2])
 
-        # keep a cache of graphs that have already been laid out
-        self.graph_cache : Dict[int, Tuple[Graph, Optional[Graph]]] = dict()
+        while self.tabs.count() > 0:
+            w = self.tabs.widget(0)
+            if isinstance(w, Editor):
+                if not self.close_tab(w):
+                    e.ignore()
+                    return
+            else:
+                raise RuntimeError("Unexpected widget in tab list")
 
-        # keep a revision count, so we don't trigger parsing until the user stops typing for a bit
-        self.revision = 0
+        e.accept()
 
     def build_menu(self) -> None:
         menu = QMenuBar()
         file_menu = menu.addMenu("&File")
         edit_menu = menu.addMenu("&Edit")
         code_menu = menu.addMenu("&Code")
+        view_menu = menu.addMenu("&View")
 
         file_new = file_menu.addAction("&New")
-        file_new.triggered.connect(self.doc.new)
+        file_new.triggered.connect(lambda: self.new())
 
         file_open = file_menu.addAction("&Open")
         file_open.setShortcut(QKeySequence(QKeySequence.StandardKey.Open))
-        file_open.triggered.connect(lambda: self.doc.open())
+        file_open.triggered.connect(lambda: self.open())
 
         self.file_open_recent = file_menu.addMenu("Open &Recent")
         self.update_recent_files()
 
         file_menu.addSeparator()
 
+        file_close = file_menu.addAction("&Close")
+        file_close.setShortcut(QKeySequence(QKeySequence.StandardKey.Close))
+        file_close.triggered.connect(lambda: self.close_tab())
+
         file_save = file_menu.addAction("&Save")
         file_save.setShortcut(QKeySequence(QKeySequence.StandardKey.Save))
-        file_save.triggered.connect(self.doc.save)
+        file_save.triggered.connect(lambda: self.save())
 
         file_save_as = file_menu.addAction("Save &As")
         file_save_as.setShortcut(QKeySequence(QKeySequence.StandardKey.SaveAs))
-        file_save_as.triggered.connect(self.doc.save_as)
+        file_save_as.triggered.connect(lambda: self.save_as())
 
         file_menu.addSeparator()
 
         file_exit = file_menu.addAction("E&xit")
         file_exit.setShortcut(QKeySequence(QKeySequence.StandardKey.Quit))
 
         app = QApplication.instance()
         if app:
             file_exit.triggered.connect(app.quit)
 
         edit_undo = edit_menu.addAction("&Undo")
         edit_undo.setShortcut(QKeySequence(QKeySequence.StandardKey.Undo))
-        edit_undo.triggered.connect(self.code_view.undo)
+        edit_undo.triggered.connect(lambda: self.undo())
 
         edit_redo = edit_menu.addAction("&Redo")
         edit_redo.setShortcut(QKeySequence(QKeySequence.StandardKey.Redo))
-        edit_redo.triggered.connect(self.code_view.redo)
+        edit_redo.triggered.connect(lambda: self.redo())
 
         # code_run = code_menu.addAction("&Run")
         # code_run.setShortcut(QKeySequence("Ctrl+R"))
         # code_run.triggered.connect(self.update_state)
 
         code_show_errors = code_menu.addAction("Show &Errors")
         code_show_errors.setShortcut(QKeySequence("F4"))
-        code_show_errors.triggered.connect(self.show_errors)
+        code_show_errors.triggered.connect(lambda: self.show_errors())
 
         code_add_rewrite_step = code_menu.addAction("&Add Rewrite Step")
         code_add_rewrite_step.setShortcut(QKeySequence("Ctrl+Return"))
-        code_add_rewrite_step.triggered.connect(lambda: self.code_view.add_line_below("  = ? by "))
+        code_add_rewrite_step.triggered.connect(lambda: self.add_rewrite_step())
 
         code_add_rewrite_step = code_menu.addAction("&Repeat Rewrite Step")
         code_add_rewrite_step.setShortcut(QKeySequence("Ctrl+Shift+Return"))
-        code_add_rewrite_step.triggered.connect(self.repeat_step_at_cursor)
+        code_add_rewrite_step.triggered.connect(lambda: self.repeat_rewrite_step())
 
         code_next_rewrite = code_menu.addAction("&Next Rewrite")
         code_next_rewrite.setShortcut(QKeySequence("Ctrl+N"))
-        code_next_rewrite.triggered.connect(self.next_rewrite_at_cursor)
+        code_next_rewrite.triggered.connect(lambda: self.next_rewrite())
 
         code_menu.addSeparator()
 
         code_next_part = code_menu.addAction("Next &Part")
         code_next_part.setShortcut(QKeySequence("Ctrl+J"))
-        code_next_part.triggered.connect(lambda: self.next_part(step=1))
+        code_next_part.triggered.connect(lambda: self.next_part())
 
         code_previous_part = code_menu.addAction("Previous &Part")
         code_previous_part.setShortcut(QKeySequence("Ctrl+K"))
-        code_previous_part.triggered.connect(lambda: self.next_part(step=-1))
-
-        self.setMenuBar(menu)
-
-    def update_file_name(self) -> None:
-        title = 'chyp - '
-        if self.doc.file_name:
-            fi = QFileInfo(self.doc.file_name)
-            title += fi.fileName()
-        else:
-            title += 'Untitled'
-
-        if self.doc.isModified():
-            title += '*'
-
-        self.setWindowTitle(title)
+        code_previous_part.triggered.connect(lambda: self.previous_part())
 
-    def update_recent_files(self) -> None:
-        def open_recent(f: str) -> Callable:
-            return lambda: self.doc.open(f)
-
-        self.file_open_recent.clear()
-        for f in self.doc.recent_files():
-            fi = QFileInfo(f)
-            action = self.file_open_recent.addAction(fi.fileName())
-            action.triggered.connect(open_recent(f))
+        view_next_tab = view_menu.addAction("&Next Tab")
+        view_next_tab.setShortcut(QKeySequence("Ctrl+]"))
+        view_next_tab.triggered.connect(lambda: self.next_tab())
+
+        view_previous_tab = view_menu.addAction("&Previous Tab")
+        view_previous_tab.setShortcut(QKeySequence("Ctrl+["))
+        view_previous_tab.triggered.connect(lambda: self.previous_tab())
+
+        view_menu.addSeparator()
+        view_goto_import = view_menu.addAction("&Go To Import")
+        view_goto_import.setShortcut(QKeySequence("Ctrl+G"))
+        view_goto_import.triggered.connect(lambda: self.goto_import())
+
+        view_menu.addSeparator()
+        self.view_themes = view_menu.addMenu("&Themes")
+        self.update_themes()
 
-    def reset_state(self) -> None:
-        cursor = self.code_view.textCursor()
-        cursor.setPosition(0)
-        self.code_view.setTextCursor(cursor)
-
-    def invalidate_text(self) -> None:
-        self.parsed = False
-        self.graph_cache = dict()
-        self.code_view.set_current_region(None)
-        self.revision += 1
-
-        def update(r: int) -> Callable:
-            def f():
-                if r == self.revision:
-                    self.update_state()
-            return f
-
-        QTimer.singleShot(100, update(self.revision))
-        # self.update_state(sync=False)
-
-    def next_part(self, step:int=1) -> None:
-        if not self.parsed: return
-
-        cursor = self.code_view.textCursor()
-        pos = cursor.position()
-        p = self.state.part_with_index_at(pos)
-        i = p[0] if p else 0
-        i += step
-
-        if i >= 0 and i < len(self.state.parts):
-            p1 = self.state.parts[i]
-            cursor.setPosition(p1[1])
-            self.code_view.setTextCursor(cursor)
-            
-
-    def show_errors(self):
-        conf = QSettings('chyp', 'chyp')
-        error_panel_size = conf.value('error_panel_size', 100)
-        if isinstance(error_panel_size, str):
-            error_panel_size = int(error_panel_size)
-        if not isinstance(error_panel_size, int) or error_panel_size == 0:
-            error_panel_size = 100
-        
-        sizes = self.splitter.sizes()
-        if sizes[2] == 0:
-            sizes[2] = error_panel_size
-            if sizes[1] >= error_panel_size + 50:
-                sizes[1] -= error_panel_size
-            else:
-                sizes[0] -= error_panel_size
-        else:
-            conf.setValue('error_panel_size', sizes[2])
-            sizes[1] += sizes[2]
-            sizes[2] = 0
-        self.splitter.setSizes(sizes)
-
-    def show_at_cursor(self) -> None:
-        if not self.parsed: return
-
-        pos = self.code_view.textCursor().position()
-        p = self.state.part_with_index_at(pos)
-        if p:
-            i, part = p
-            self.code_view.set_current_region((part[0], part[1]))
-            if part[2] in ('let','gen') and part[3] in self.state.graphs:
-                if i not in self.graph_cache:
-                    g = self.state.graphs[part[3]].copy()
-                    convex_layout(g)
-                    self.graph_cache[i] = (g, None)
-                else:
-                    g, _ = self.graph_cache[i]
-                self.rhs_view.setVisible(False)
-                self.lhs_view.set_graph(g)
-            elif part[2] == 'rule' and part[3] in self.state.rules:
-                if i not in self.graph_cache:
-                    lhs = self.state.rules[part[3]].lhs.copy()
-                    rhs = self.state.rules[part[3]].rhs.copy()
-                    convex_layout(lhs)
-                    convex_layout(rhs)
-                    self.graph_cache[i] = (lhs, rhs)
-                else:
-                    lhs, rhs0 = self.graph_cache[i]
-                    if not rhs0: raise ValueError("Rule in graph_cache should have RHS")
-                    rhs = rhs0
-                self.rhs_view.setVisible(True)
-                self.lhs_view.set_graph(lhs)
-                self.rhs_view.set_graph(rhs)
-            elif part[2] == 'rewrite' and part[3] in self.state.rewrites:
-                rw = self.state.rewrites[part[3]]
-                if i not in self.graph_cache:
-                    if not rw.stub:
-                        if rw.status == RewriteState.UNCHECKED:
-                            rw.status = RewriteState.CHECKING
-                            def check_finished(i: int) -> Callable:
-                                def f() -> None:
-                                    self.graph_cache.pop(i, None)
-                                    self.show_at_cursor()
-                                return f
-
-                            check_thread = CheckThread(rw, self)
-                            check_thread.finished.connect(check_finished(i))
-                            check_thread.start()
-
-                    lhs = rw.lhs.copy() if rw.lhs else Graph()
-                    rhs = rw.rhs.copy() if rw.rhs else Graph()
-                    convex_layout(lhs)
-                    convex_layout(rhs)
-                    self.graph_cache[i] = (lhs, rhs)
-                else:
-                    lhs, rhs0 = self.graph_cache[i]
-                    if not rhs0: raise ValueError("Rewrite step in graph_cache should have RHS")
-                    rhs = rhs0
-
-                if rw.status == RewriteState.VALID:
-                    self.code_view.set_current_region((part[0], part[1]), status=STATUS_GOOD)
-                elif rw.status == RewriteState.INVALID:
-                    self.code_view.set_current_region((part[0], part[1]), status=STATUS_BAD)
-
-                self.rhs_view.setVisible(True)
-                self.lhs_view.set_graph(lhs)
-                if rhs: self.rhs_view.set_graph(rhs)
-
-
-    def next_rewrite_at_cursor(self) -> None:
-        self.update_state()
-        if not self.parsed: return
-
-        pos = self.code_view.textCursor().position()
-        part = self.state.part_at(pos)
-        if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
-            rw = self.state.rewrites[part[3]]
-            if rw.rule and rw.lhs:
-                start, end = rw.term_pos
-                text = self.code_view.toPlainText()
-                term = text[start:end]
-                seen = set([term])
-
-                found_prev = (term == '?')
-                rw_term = None
-                for m in match_rule(rw.rule, rw.lhs):
-                    t = graph_to_term(rewrite(rw.rule, m))
-                    if found_prev and not t in seen:
-                        rw_term = t
-                        break
-                    elif not rw_term:
-                        rw_term = t
-
-                    seen.add(t)
-                    found_prev = (term == t)
-
-                if rw_term:
-                    cursor = self.code_view.textCursor()
-                    cursor.clearSelection()
-                    cursor.setPosition(start)
-                    cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
-                    cursor.insertText(rw_term)
-                    self.code_view.setTextCursor(cursor)
-                    self.update_state()
-
-    def repeat_step_at_cursor(self) -> None:
-        self.update_state()
-        pos = self.code_view.textCursor().position()
-        part = self.state.part_at(pos)
-        if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
-            rule = self.state.rewrites[part[3]].rule
-
-            if rule:
-                self.code_view.add_line_below('  = ? by ' + rule.name)
-                self.update_state()
-                self.next_rewrite_at_cursor()
-
-    def update_state(self) -> None:
-        self.state = State()
-        self.code_view.set_current_region(None)
-        
-        self.state.update(self.code_view.toPlainText())
-        model = self.error_view.model()
-        if isinstance(model, ErrorListModel):
-            model.set_errors(self.state.errors)
-
-        if len(self.state.errors) == 0:
-            self.lhs_view.set_graph(Graph())
-            self.rhs_view.setVisible(False)
-            self.parsed = True
-            self.show_at_cursor()
-
-
-
-    def closeEvent(self, e: QCloseEvent) -> None:
-        if self.doc.confirm_close():
-            conf = QSettings('chyp', 'chyp')
-            conf.setValue("editor_window_geometry", self.saveGeometry())
-            conf.setValue("editor_splitter_state", self.splitter.saveState())
-            sizes = self.splitter.sizes()
-            if sizes[2] != 0:
-                conf.setValue('error_panel_size', sizes[2])
-            e.accept()
-        else:
-            e.ignore()
-
-class CheckThread(QThread):
-    def __init__(self, rw: RewriteState, parent: Optional[QObject] = None) -> None:
-        super().__init__(parent)
-        self.rw = rw
-
-    def run(self) -> None:
-        self.rw.check()
-
-# class UpdateStateThread(QThread):
-#     def __init__(self, state: State, code: str, parent: Optional[QObject] = None) -> None:
-#         super().__init__(parent)
-#         self.state = state
-#         self.code = code
-
-#     def run(self) -> None:
-#         self.msleep(300)
-#         self.state.update(self.code)
+        self.setMenuBar(menu)
```

### Comparing `chyp-0.3.3/chyp/gui/graphscene.py` & `chyp-0.3.4/chyp/gui/graphscene.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,50 +22,60 @@
                                QGraphicsPathItem, QGraphicsRectItem, QGraphicsScene,
                                QGraphicsSceneMouseEvent, QStyleOptionGraphicsItem, QWidget)
 
 from ..graph import Graph
 
 SCALE = 50.0
 
+BOX_WIDTH = 1.1
+
 class EItem(QGraphicsRectItem):
     def __init__(self, g: Graph, e: int) -> None:
-        super().__init__(-0.4 * SCALE, -0.8 * SCALE, 0.8 * SCALE, 1.6 * SCALE)
+        super().__init__(-0.5 * BOX_WIDTH * SCALE, -0.8 * SCALE, BOX_WIDTH * SCALE, 1.6 * SCALE)
         self.g = g
         self.e = e
         ed = g.edge_data(e)
+        self.bg = ed.bg
+        self.fg = ed.fg
+        self.value = ed.value
         self.num_s = len(ed.s)
         self.num_t = len(ed.t)
         self.is_id = isinstance(ed.value, str) and str(ed.value) == 'id'
 
         self.setPos(ed.x * SCALE, ed.y * SCALE)
 
         if self.is_id:
             self.setRect(-0.2 * SCALE, -0.2 * SCALE, 0.4 * SCALE, 0.4 * SCALE)
             self.setPen(QPen(QColor(200,200,200)))
             self.setBrush(QBrush(QColor(200,200,200)))
             self.setVisible(False)
         else:
             if self.num_s <= 1 and self.num_t <= 1:
-                self.setRect(-0.4 * SCALE, -0.4 * SCALE, 0.8 * SCALE, 0.8 * SCALE)
+                self.setRect(-0.5 * BOX_WIDTH * SCALE, -0.4 * SCALE, BOX_WIDTH * SCALE, 0.8 * SCALE)
+
+            if self.bg != '':
+                self.setBrush(QBrush(QColor(self.bg)))
+            else:
+                self.setBrush(QBrush(QColor(200,200,255)))
 
-            self.setBrush(QBrush(QColor(200,200,255)))
             if ed.highlight:
                 # pen = QPen(QColor(0,150,0))
                 pen = self.pen()
                 pen.setWidth(3)
                 self.setPen(pen)
             else:
                 self.setPen(QPen(QColor(0,0,0)))
 
     def paint(self, painter: QPainter, option: QStyleOptionGraphicsItem, widget: Optional[QWidget]=None) -> None:
         super().paint(painter, option, widget)
-        ed = self.g.edge_data(self.e)
 
-        painter.setFont(QFont("sans", 14))
-        painter.drawText(self.boundingRect(), Qt.AlignmentFlag.AlignCenter, str(ed.value)) # type:ignore
+        if self.fg != '':
+            self.setPen(QPen(QColor(self.fg)))
+        painter.setFont(QFont("sans", 11))
+        painter.drawText(self.boundingRect(), Qt.AlignmentFlag.AlignCenter, str(self.value)) # type:ignore
 
 class VItem(QGraphicsEllipseItem):
     def __init__(self, g: Graph, v: int) -> None:
         super().__init__(-0.0625 * SCALE, -0.0625 * SCALE, 0.125 * SCALE, 0.125 * SCALE)
         self.setVisible(False)
         self.g = g
         self.v = v
@@ -87,15 +97,15 @@
         self.i = i
         self.src = src
         self.refresh()
 
     def refresh(self) -> None:
         path = QPainterPath()
 
-        x_shift = (0 if self.eitem.is_id else 0.4) * SCALE
+        x_shift = (0 if self.eitem.is_id else 0.5 * BOX_WIDTH) * SCALE
 
         if self.src:
             if self.eitem.num_s == 1:
                 y_shift = 0.0
             else:
                 y_shift = ((self.i / (self.eitem.num_s - 1)) - 0.5) * SCALE
```

### Comparing `chyp-0.3.3/chyp/gui/graphview.py` & `chyp-0.3.4/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/layout.py` & `chyp-0.3.4/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/matcher.py` & `chyp-0.3.4/chyp/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
             if v in self.vmap and self.vmap[v] in future:
                 return False
         return True
 
 
 
 class Matches(Iterable):
-    def __init__(self, dom: Graph, cod: Graph, initial_match: Optional[Match] = None, convex=True) -> None:
+    def __init__(self, dom: Graph, cod: Graph, initial_match: Optional[Match] = None, convex: bool=True) -> None:
         if initial_match is None: initial_match = Match(dom=dom, cod=cod) 
         self.convex = convex
 
         if initial_match.map_scalars():
             self.match_stack = [initial_match]
         else:
             self.match_stack = []
@@ -278,18 +278,18 @@
                         match_log("match is not convex, dropping")
                 else:
                     return m
             else:
                 self.match_stack += m.more()
         raise StopIteration
 
-def match_graph(dom: Graph, cod: Graph, convex=True) -> Iterable[Match]:
+def match_graph(dom: Graph, cod: Graph, convex: bool=True) -> Iterable[Match]:
     return Matches(dom, cod, convex=convex)
 
-def match_rule(r: Rule, g: Graph, convex=True) -> Iterable[Match]:
+def match_rule(r: Rule, g: Graph, convex: bool=True) -> Iterable[Match]:
     return Matches(r.lhs, g, convex=convex)
 
 def find_iso(g: Graph, h: Graph) -> Optional[Match]:
     g_in = g.inputs()
     g_out = g.outputs()
     h_in = h.inputs()
     h_out = h.outputs()
```

### Comparing `chyp-0.3.3/chyp/rewrite.py` & `chyp-0.3.4/chyp/rewrite.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             m1.vimg.add(v1)
 
     # now add the edges from rhs to h and connect them using vmap1
     for e in r.rhs.edges():
         ed = r.rhs.edge_data(e)
         e1 = h.add_edge([m1.vmap[v] for v in ed.s],
                         [m1.vmap[v] for v in ed.t],
-                        ed.value, ed.x, ed.y, ed.hyper)
+                        ed.value, ed.x, ed.y, ed.fg, ed.bg, ed.hyper)
         m1.emap[e] = e1
         m1.eimg.add(e1)
 
     return [m1]
 
 def rewrite(r: Rule, m: Match) -> Graph:
     """Apply the given rewrite r to at match m and return the first result
```

### Comparing `chyp-0.3.3/chyp/rule.py` & `chyp-0.3.4/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/scraps.py` & `chyp-0.3.4/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp/state.py` & `chyp-0.3.4/chyp/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,18 +86,18 @@
 
 class State:
     def __init__(self) -> None:
         self.graphs: Dict[str, Graph] = dict()
         self.rules: Dict[str, Rule] = dict()
         self.rewrites: Dict[str, RewriteState] = dict()
         self.parts: List[Tuple[int, int, str, str]] = list()
-        self.errors: List[Tuple[int, str]] = list()
+        self.errors: List[Tuple[str, int, str]] = list()
 
-    def update(self, code: str) -> None:
-        parse_data = parse(code)
+    def update(self, code: str, file_name: str) -> None:
+        parse_data = parse(code, file_name)
         self.graphs = parse_data.graphs
         self.rules = parse_data.rules
         self.parts = parse_data.parts
         self.errors = parse_data.errors
 
         for name, (t_start, t_end, equiv, rule, lhs, rhs, lhs_match, rhs_match) in parse_data.rewrites.items():
             stub = not (':' in name)
```

### Comparing `chyp-0.3.3/chyp/term.py` & `chyp-0.3.4/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.3/chyp.egg-info/PKG-INFO` & `chyp-0.3.4/chyp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3.3
+Version: 0.3.4
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chyp-0.3.3/chyp.egg-info/SOURCES.txt` & `chyp-0.3.4/chyp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 chyp.egg-info/dependency_links.txt
 chyp.egg-info/entry_points.txt
 chyp.egg-info/requires.txt
 chyp.egg-info/top_level.txt
 chyp/gui/__init__.py
 chyp/gui/app.py
 chyp/gui/codeview.py
+chyp/gui/colors.py
+chyp/gui/completion.py
 chyp/gui/document.py
 chyp/gui/editor.py
 chyp/gui/errorlist.py
 chyp/gui/graphscene.py
 chyp/gui/graphview.py
 chyp/gui/highlighter.py
 chyp/gui/mainwindow.py
```

### Comparing `chyp-0.3.3/setup.py` & `chyp-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.3.3",
+    version="0.3.4",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for monoidal categories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

