# Comparing `tmp/tlogg-0.5.0a8.tar.gz` & `tmp/tlogg-0.5.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlogg-0.5.0a8.tar", last modified: Thu Jan 19 13:43:00 2023, max compression
+gzip compressed data, was "tlogg-0.5.0a9.tar", last modified: Tue May 23 16:59:41 2023, max compression
```

## Comparing `tlogg-0.5.0a8.tar` & `tlogg-0.5.0a9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/
--rw-rw-r--   0 one       (1000) one       (1000)     2422 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1715 2023-01-19 13:42:55.000000 tlogg-0.5.0a8/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1252 2023-01-19 13:42:55.000000 tlogg-0.5.0a8/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/tlogg/
--rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/tlogg/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1241 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     2858 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     3251 2023-01-19 13:42:55.000000 tlogg-0.5.0a8/tlogg/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     4788 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/filetree.py
--rw-rw-r--   0 one       (1000) one       (1000)     9882 2023-01-06 11:04:42.000000 tlogg-0.5.0a8/tlogg/app/fileviewer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1412 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/glbl.py
--rw-rw-r--   0 one       (1000) one       (1000)     6428 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/highlighters.py
--rw-rw-r--   0 one       (1000) one       (1000)    10367 2023-01-19 13:41:55.000000 tlogg-0.5.0a8/tlogg/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)     3178 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/options.py
--rw-rw-r--   0 one       (1000) one       (1000)     7483 2022-09-28 12:16:27.000000 tlogg-0.5.0a8/tlogg/app/predefinedfilters.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-01-19 13:43:00.882301 tlogg-0.5.0a8/tlogg.egg-info/
--rw-rw-r--   0 one       (1000) one       (1000)     2422 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      448 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       37 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       34 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)        6 2023-01-19 13:43:00.000000 tlogg-0.5.0a8/tlogg.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/
+-rw-rw-r--   0 one       (1000) one       (1000)     2422 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1715 2023-05-23 16:59:37.000000 tlogg-0.5.0a9/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     1253 2023-05-23 16:59:37.000000 tlogg-0.5.0a9/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/tlogg/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1239 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1242 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/tlogg/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1241 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2844 2023-05-23 16:27:45.000000 tlogg-0.5.0a9/tlogg/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3251 2023-05-23 16:59:37.000000 tlogg-0.5.0a9/tlogg/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4788 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/app/filetree.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9870 2023-05-23 16:28:09.000000 tlogg-0.5.0a9/tlogg/app/fileviewer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1412 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/app/glbl.py
+-rw-rw-r--   0 one       (1000) one       (1000)     6428 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/app/highlighters.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10367 2023-01-19 13:41:55.000000 tlogg-0.5.0a9/tlogg/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3178 2022-09-28 12:16:27.000000 tlogg-0.5.0a9/tlogg/app/options.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7513 2023-05-23 16:55:55.000000 tlogg-0.5.0a9/tlogg/app/predefinedfilters.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2023-05-23 16:59:41.307569 tlogg-0.5.0a9/tlogg.egg-info/
+-rw-rw-r--   0 one       (1000) one       (1000)     2422 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)      448 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       37 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       35 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        6 2023-05-23 16:59:41.000000 tlogg-0.5.0a9/tlogg.egg-info/top_level.txt
```

### Comparing `tlogg-0.5.0a8/PKG-INFO` & `tlogg-0.5.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlogg
-Version: 0.5.0a8
+Version: 0.5.0a9
 Summary: A fast, advanced log explorer
 Home-page: https://github.com/ceccopierangiolieugenio/tlogg
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tlogg-0.5.0a8/README.md` & `tlogg-0.5.0a9/README.md`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/setup.py` & `tlogg-0.5.0a9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.5.0a8"
+version = "0.5.0a9"
 name = "tlogg"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -28,15 +28,15 @@
         "Intended Audience :: Information Technology",
         "Topic :: Terminals",
         "Topic :: Software Development :: User Interfaces"],
     include_package_data=False,
     packages=['tlogg','tlogg.app'],
     python_requires=">=3.8",
     install_requires=[
-        'pyTermTk>=0.9.0a37',
+        'pyTermTk>=0.30.0a69',
         'appdirs',
         'pyyaml'],
     entry_points={
         'console_scripts': [
             'tlogg = tlogg:main',
         ],
     },
```

### Comparing `tlogg-0.5.0a8/tlogg/__init__.py` & `tlogg-0.5.0a9/tlogg/__init__.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/__main__.py` & `tlogg-0.5.0a9/tlogg/__main__.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/__init__.py` & `tlogg-0.5.0a9/tlogg/app/__init__.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/about.py` & `tlogg-0.5.0a9/tlogg/app/about.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,19 +44,19 @@
         TTkAbout.__init__(self, *args, **kwargs)
         self._name = kwargs.get('name' , 'About' )
         self.setTitle('[PierCecco Cecco] Eugenio Parodi proudly presents...')
         self.resize(56,16)
 
 
 
-    def paintEvent(self):
+    def paintEvent(self, canvas):
         c = [0xFF,0xFF,0xFF]
         for y, line in enumerate(About.tlogg):
-            self._canvas.drawText(pos=(13,3+y),text=line, color=TTkColor.fg(f'#{c[0]:02X}{c[1]:02X}{c[2]:02X}'))
+            canvas.drawText(pos=(13,3+y),text=line, color=TTkColor.fg(f'#{c[0]:02X}{c[1]:02X}{c[2]:02X}'))
             c[2]-=0x18
             c[0]-=0x08
-        self._canvas.drawText(pos=(26,4),text=f"  Version: {TloggCfg.version}", color=TTkColor.fg('#AAAAFF'))
-        self._canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
-        self._canvas.drawText(pos=(2,13),text=f"https://github.com/ceccopierangiolieugenio/tlogg", color=TTkColor.fg('#44FFFF'))
-        self._canvas.drawText(pos=(2,14),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
+        canvas.drawText(pos=(26,4),text=f"  Version: {TloggCfg.version}", color=TTkColor.fg('#AAAAFF'))
+        canvas.drawText(pos=(14,11),text=f"Powered By, pyTermTk")
+        canvas.drawText(pos=(2,13),text=f"https://github.com/ceccopierangiolieugenio/tlogg", color=TTkColor.fg('#44FFFF'))
+        canvas.drawText(pos=(2,14),text=f"https://github.com/ceccopierangiolieugenio/pyTermTk", color=TTkColor.fg('#44FFFF'))
 
-        TTkWindow.paintEvent(self)
+        TTkWindow.paintEvent(self, canvas)
```

### Comparing `tlogg-0.5.0a8/tlogg/app/cfg.py` & `tlogg-0.5.0a9/tlogg/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import yaml
 
 class TloggCfg:
-    version="0.5.0a8"
+    version="0.5.0a9"
     name="tlogg"
     cfgVersion = '1.0'
     pathCfg="."
     colors=[]
     filters=[]
     options={}
     searches=[]
```

### Comparing `tlogg-0.5.0a8/tlogg/app/filetree.py` & `tlogg-0.5.0a9/tlogg/app/filetree.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/fileviewer.py` & `tlogg-0.5.0a9/tlogg/app/fileviewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     def getLine(self, num) -> str:
         return self._fileBuffer.getLine(num)
 
     def getLineNum(self, num) -> int:
         return num
 
-    def paintEvent(self):
+    def paintEvent(self, canvas):
         ox,oy = self.getViewOffsets()
         bufferLen = self.getLen()
         for i in range(min(self.height(),bufferLen-oy)):
             line = TTkString(self.getLine(i+oy).replace('\n','')).tab2spaces()
             lineNum = self.getLineNum(i+oy)
             if lineNum in self._indexesMark:
                 symbolcolor = TTkColor.fg("#00ffff")
@@ -166,19 +166,19 @@
                         line = line.setColor(searchedColor, match=match)
 
             # Add Line Number
             lenLineNumber = len(str(self.getLineNum(bufferLen-1)))
             lineNumber = TTkString() + numberColor + str(lineNum).rjust(lenLineNumber) + TTkColor.RST + ' '
             # Compose print line
             printLine = TTkString() + symbolcolor + symbol + TTkColor.RST + ' ' + lineNumber + line.substring(ox)
-            self.getCanvas().drawText(pos=(0,i), text=printLine, color=selectedColor, width=self.width(), )
+            canvas.drawText(pos=(0,i), text=printLine, color=selectedColor, width=self.width(), )
 
         # Draw the loading banner
         if self._indexing is not None:
-            self.getCanvas().drawText(pos=(0,0), text=f" [ Indexed: {int(100*self._indexing)}% ] ")
+            canvas.drawText(pos=(0,0), text=f" [ Indexed: {int(100*self._indexing)}% ] ")
 
 class FileViewerSearch(FileViewer):
     __slots__ = ('_indexes')
     def __init__(self, *args, **kwargs):
         self._indexes = []
         FileViewer.__init__(self, *args, **kwargs)
         self._name = kwargs.get('name' , 'FileViewerSearch' )
```

### Comparing `tlogg-0.5.0a8/tlogg/app/glbl.py` & `tlogg-0.5.0a9/tlogg/app/glbl.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/highlighters.py` & `tlogg-0.5.0a9/tlogg/app/highlighters.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/main.py` & `tlogg-0.5.0a9/tlogg/app/main.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/options.py` & `tlogg-0.5.0a9/tlogg/app/options.py`

 * *Files identical despite different names*

### Comparing `tlogg-0.5.0a8/tlogg/app/predefinedfilters.py` & `tlogg-0.5.0a9/tlogg/app/predefinedfilters.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,26 +153,26 @@
         for filter in filters:
             def _cb(p, sb):
                 def _ret(state):
                     txt = sb.currentText()
                     if state == TTkK.Checked:
                         if not txt:
                             txt = p
-                        elif p not in txt:
+                        elif txt.find(p) == -1:
                             txt += '|'+p
                     else:
                         p1 = f"|{p}"
                         p2 = f"{p}|"
-                        if p1 in txt:
+                        if txt.find(p1) != -1:
                             txt = txt.replace(p1,'')
-                        elif p2 in txt:
+                        elif txt.find(p2) != -1:
                             txt = txt.replace(p2,'')
                         else:
                             txt = txt.replace(p,'')
                     sb.setCurrentText(txt)
                 return _ret
 
-            layout.addWidget(cb := TTkCheckbox(text=filter['name'],checked=filter['pattern'] in searchbox.currentText()))
+            layout.addWidget(cb := TTkCheckbox(text=filter['name'],checked=searchbox.currentText().find(filter['pattern'])!=-1))
             cb.stateChanged.connect(_cb(filter['pattern'], searchbox))
         w,h = self.minimumSize()
         self.resize(w,h)
```

### Comparing `tlogg-0.5.0a8/tlogg.egg-info/PKG-INFO` & `tlogg-0.5.0a9/tlogg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlogg
-Version: 0.5.0a8
+Version: 0.5.0a9
 Summary: A fast, advanced log explorer
 Home-page: https://github.com/ceccopierangiolieugenio/tlogg
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

