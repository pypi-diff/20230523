# Comparing `tmp/fmg-0.1.0.tar.gz` & `tmp/fmg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmg-0.1.0.tar", last modified: Tue May 23 02:08:31 2023, max compression
+gzip compressed data, was "fmg-0.2.0.tar", last modified: Tue May 23 02:53:33 2023, max compression
```

## Comparing `fmg-0.1.0.tar` & `fmg-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 02:08:31.287392 fmg-0.1.0/
--rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 fmg-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 fmg-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      770 2023-05-23 02:08:31.287392 fmg-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-05-23 02:07:31.000000 fmg-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 02:08:31.265809 fmg-0.1.0/fmg/
--rw-rw-rw-   0        0        0      180 2023-05-23 01:58:56.000000 fmg-0.1.0/fmg/__init__.py
--rw-rw-rw-   0        0        0       63 2023-05-23 02:04:42.000000 fmg-0.1.0/fmg/__version__.py
--rw-rw-rw-   0        0        0     8220 2023-05-23 01:58:56.000000 fmg-0.1.0/fmg/core.py
-drwxrwxrwx   0        0        0        0 2023-05-23 02:08:31.287392 fmg-0.1.0/fmg.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-23 02:08:31.000000 fmg-0.1.0/fmg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-23 02:08:31.000000 fmg-0.1.0/fmg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 02:08:31.000000 fmg-0.1.0/fmg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-23 02:08:31.000000 fmg-0.1.0/fmg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-23 02:08:31.000000 fmg-0.1.0/fmg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 02:08:31.287392 fmg-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3791 2023-05-23 02:04:42.000000 fmg-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.194414 fmg-0.2.0/
+-rw-rw-rw-   0        0        0     1060 2019-08-27 18:29:08.000000 fmg-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 fmg-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      770 2023-05-23 02:53:33.194414 fmg-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-05-23 02:07:31.000000 fmg-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.164577 fmg-0.2.0/fmg/
+-rw-rw-rw-   0        0        0      180 2023-05-23 01:58:56.000000 fmg-0.2.0/fmg/__init__.py
+-rw-rw-rw-   0        0        0       63 2023-05-23 02:53:21.000000 fmg-0.2.0/fmg/__version__.py
+-rw-rw-rw-   0        0        0     8864 2023-05-23 02:51:34.000000 fmg-0.2.0/fmg/core.py
+drwxrwxrwx   0        0        0        0 2023-05-23 02:53:33.194414 fmg-0.2.0/fmg.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-23 02:53:33.000000 fmg-0.2.0/fmg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 02:53:33.194414 fmg-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3791 2023-05-23 02:53:21.000000 fmg-0.2.0/setup.py
```

### Comparing `fmg-0.1.0/LICENSE` & `fmg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmg-0.1.0/PKG-INFO` & `fmg-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fast Memory Graphics for big image, use like OpenSlide
 Home-page: https://github.com/khtao/fmg
 Author: khtao
 Author-email: khtao@live.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fmg-0.1.0/fmg/core.py` & `fmg-0.2.0/fmg/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,18 +87,29 @@
         AbstractSlide.__init__(self)
         self._filename = filename
         self._mode = mode
         if mode == 'r':
             self._osr = json.load(open(filename))
             self._data = [lmdb.open(os.path.join(self._filename[:-4], 'level' + str(i)))
                           for i in range(self.level_count)]
+            self.check_data()
         elif mode == 'w':
 
             pass
 
+    def check_data(self):
+        for i in range(self.level_count):
+            txn = self._data[i].begin()
+            dimension = txn.get(key='dimension'.encode())
+            if dimension is not None:
+                dimension_w = dimension.decode()
+                dimension_r = str(self.level_dimensions[i])
+                if dimension_r != dimension_w:
+                    print('warning: read size %s does not match write size %s' % (dimension_w, dimension_r))
+
     def __repr__(self):
         return f'{self.__class__.__name__}({self._filename!r})'
 
     def close(self):
         """Close the OpenSlide object."""
         for dd in self._data:
             dd.close()
@@ -139,33 +150,33 @@
 
         Unlike in the C interface, the image data returned by this
         function is not premultiplied."""
         x_start, y_start = location
         x_end, y_end = x_start + size[0], y_start + size[1]
         dimension = self.level_dimensions[level]
         step = self._osr['patch_size']
-        x_min = math.floor(x_start / self._osr['patch_size']) * self._osr['patch_size']
-        y_min = math.floor(y_start / self._osr['patch_size']) * self._osr['patch_size']
-        x_max = math.ceil(x_end / self._osr['patch_size']) * self._osr['patch_size']
-        y_max = math.ceil(y_end / self._osr['patch_size']) * self._osr['patch_size']
+        x_min = math.floor(x_start / step) * step
+        y_min = math.floor(y_start / step) * step
+        x_max = math.ceil(x_end / step) * step
+        y_max = math.ceil(y_end / step) * step
         image = np.zeros((y_max - y_min, x_max - x_min, 3), dtype=np.uint8)
         txn = self._data[level].begin()
         for w in range(x_min, min(x_max, dimension[0]), step):
             for h in range(y_min, min(y_max, dimension[1]), step):
                 w_max = min(w + step, dimension[0])
                 h_max = min(h + step, dimension[1])
                 buff = txn.get(key=str((w, h, w_max, h_max)).encode())
                 buff = np.frombuffer(buff, dtype=np.uint8)
                 buff = cv2.imdecode(buff, cv2.IMREAD_COLOR)
                 image[h - y_min:h_max - y_min, w - x_min:w_max - x_min, :] = buff
         image = image[y_start - y_min:y_end - y_min, x_start - x_min:x_end - x_min, :]
         return Image.fromarray(image)
 
     def save_from_numpy(self, data, ext='.jpg',
-                        params=[cv2.IMWRITE_JPEG_QUALITY, 85],
+                        params=[cv2.IMWRITE_JPEG_QUALITY, 90],
                         pyramid=False, mpp=None, patch_size=256):
         assert self._mode == 'w'
         w, h, c = data.shape
         level_count = 1
         level_dimensions = [(h, w)]
         level_downsamples = [(1.0, 1.0)]
         level_data = [data]
@@ -195,14 +206,19 @@
         if os.path.exists(self._filename[:-4]):
             shutil.rmtree(self._filename[:-4])
         os.makedirs(self._filename[:-4])
         self._data = []
         for i in range(level_count):
             self._data.append(lmdb.open(os.path.join(self._filename[:-4], 'level' + str(i)), map_size=1099511627776))
         for i, dimension in enumerate(level_dimensions):
+            txn = self._data[i].begin(write=True)
+            txn.put(key='patch_size'.encode(), value=str(patch_size).encode())
+            txn.put(key='mpp'.encode(), value=str(mpp).encode())
+            txn.put(key='dimension'.encode(), value=str(dimension).encode())
+            txn.commit()
             for x in range(0, dimension[0], patch_size):
                 patches = []
                 locations = []
                 for y in range(0, dimension[1], patch_size):
                     x_max = min(x + patch_size, dimension[0])
                     y_max = min(y + patch_size, dimension[1])
                     patches.append(level_data[i][y:y_max, x:x_max, :])
```

### Comparing `fmg-0.1.0/fmg.egg-info/PKG-INFO` & `fmg-0.2.0/fmg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fast Memory Graphics for big image, use like OpenSlide
 Home-page: https://github.com/khtao/fmg
 Author: khtao
 Author-email: khtao@live.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fmg-0.1.0/setup.py` & `fmg-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'fmg'
 DESCRIPTION = 'Fast Memory Graphics for big image, use like OpenSlide'
 URL = 'https://github.com/khtao/fmg'
 EMAIL = 'khtao@live.cn'
 AUTHOR = 'khtao'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'lmdb', 'opencv-python', 'numpy', 'pillow'
 ]
 
 # What packages are optional?
```

