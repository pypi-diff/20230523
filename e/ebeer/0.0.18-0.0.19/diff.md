# Comparing `tmp/ebeer-0.0.18.tar.gz` & `tmp/ebeer-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebeer-0.0.18.tar", last modified: Mon May 22 22:27:59 2023, max compression
+gzip compressed data, was "ebeer-0.0.19.tar", last modified: Tue May 23 13:08:24 2023, max compression
```

## Comparing `ebeer-0.0.18.tar` & `ebeer-0.0.19.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 22:26:45.000000 ebeer-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 22:26:45.000000 ebeer-0.0.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 22:27:59.690166 ebeer-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-22 22:26:45.000000 ebeer-0.0.18/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-22 22:26:45.000000 ebeer-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 22:27:59.690166 ebeer-0.0.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.682165 ebeer-0.0.18/src/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.682165 ebeer-0.0.18/src/ebeer/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/beer_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12718 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/label_index.py
--rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-22 22:26:45.000000 ebeer-0.0.18/src/ebeer/trained_model.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/src/ebeer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 22:27:59.000000 ebeer-0.0.18/src/ebeer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 22:27:59.690166 ebeer-0.0.18/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-22 22:26:45.000000 ebeer-0.0.18/tests/test_classify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:07:14.000000 ebeer-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 13:07:14.000000 ebeer-0.0.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 13:08:24.554558 ebeer-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 13:07:14.000000 ebeer-0.0.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-23 13:07:14.000000 ebeer-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:08:24.554558 ebeer-0.0.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.546558 ebeer-0.0.19/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.546558 ebeer-0.0.19/src/ebeer/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/beer_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/data_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6684424 2023-05-23 13:07:14.000000 ebeer-0.0.19/src/ebeer/trained_model.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/src/ebeer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 13:08:24.000000 ebeer-0.0.19/src/ebeer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:08:24.554558 ebeer-0.0.19/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-23 13:07:14.000000 ebeer-0.0.19/tests/test_classify.py
```

### Comparing `ebeer-0.0.18/LICENSE` & `ebeer-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.18/pyproject.toml` & `ebeer-0.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0", "wheel", "build"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ebeer"
-version = "0.0.18"
+version = "0.0.19"
 authors = [
     { name="diego vasque maldonado", email="diegoomal13@gmail.com" }
 ]
 description = "CNN Trained to predict brazilian beers"
 readme = "src/README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ebeer-0.0.18/src/ebeer/beer_classifier.py` & `ebeer-0.0.19/src/ebeer/beer_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 
 class BeerClassifier:
 
     def __init__(self) -> None:
         pass
 
-    def predict(self, path_img):
+    @staticmethod
+    def predict(path_img):
 
         width = 128
         height = 128
         size = (width, height)
         channels = 3
         n_neuronios_saida = 20
         learning_rate = 1e-4
@@ -52,15 +53,15 @@
             metrics=[
                 'accuracy',
                 tf.keras.metrics.Precision(),
                 tf.keras.metrics.Recall()
             ]
         )
 
-        cnn_weights_path = self.get_cnn_weights_path()
+        cnn_weights_path = BeerClassifier.get_cnn_weights_path()
         model = keras.models.load_model(cnn_weights_path)
 
         image_original = tf.keras.utils.load_img(
             path_img,
             grayscale=False,
             color_mode="rgb",
             target_size=None,
@@ -73,11 +74,17 @@
 
         predicted = model.predict(image_prepared)
 
         n_pos = predicted.argmax(axis=-1)[0]
 
         return n_pos
 
-    def get_cnn_weights_path(self):
+    @staticmethod
+    def get_cnn_weights_path():
         resource_path = importlib_resources.files('ebeer').joinpath(
             'trained_model.h5')
-        return resource_path
+        return resource_path
+
+    @staticmethod
+    def predict_simple(path_img):
+        import ebeer.data_label
+        return ebeer.DataLabel[BeerClassifier.predict(path_img)]
```

### Comparing `ebeer-0.0.18/src/ebeer/label_index.py` & `ebeer-0.0.19/src/ebeer/data_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-labels_index = {
+DataLabel = {
     
        0 : { 
         "name": "amstel"
         , "description": "amstel description"
         , "ibu": "0"
         , "abv" : "5%"
         , "brewery": "heiniken"
```

### Comparing `ebeer-0.0.18/src/ebeer/trained_model.h5` & `ebeer-0.0.19/src/ebeer/trained_model.h5`

 * *Files identical despite different names*

### Comparing `ebeer-0.0.18/tests/test_classify.py` & `ebeer-0.0.19/tests/test_classify.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 class Test_Classify:
 
     def test_has_weights_file(self):
 
         import importlib_resources
 
-        resource_path = importlib_resources.files('ebeer').joinpath('trained_model.h5')
+        resource_path = importlib_resources.files(
+            'ebeer').joinpath('trained_model.h5')
 
         flg = False if resource_path is None else True
 
         print('flg:', flg)
 
         assert True
 
     def test_predict(self):
 
         import ebeer
 
-        bc = ebeer.BeerClassifier()
+        n_pos = ebeer.BeerClassifier.predict("assets/beer_imgs/0.jpg")
 
-        n_pos = bc.predict("./assets/beer_imgs/0.jpg")
+        print("Label:", ebeer.DataLabel[n_pos]["name"])
 
-        print("Label:", ebeer.labels_index[n_pos]["name"])
+        assert True
+
+    def test_predict_simple(self):
+
+        import ebeer
+
+        beerData = ebeer.BeerClassifier.predict_simple(
+            "assets/beer_imgs/0.jpg")
+
+        print('beerData:', beerData)
 
         assert True
```

