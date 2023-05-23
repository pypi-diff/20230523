# Comparing `tmp/streamlit-deckgl-0.3.0.tar.gz` & `tmp/streamlit-deckgl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.3.0.tar", last modified: Tue May 16 00:07:39 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.4.0.tar", last modified: Tue May 23 21:10:03 2023, max compression
```

## Comparing `streamlit-deckgl-0.3.0.tar` & `streamlit-deckgl-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.3.0/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-16 00:03:31.000000 streamlit-deckgl-0.3.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.338717 streamlit-deckgl-0.3.0/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.338717 streamlit-deckgl-0.3.0/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-05-15 20:40:20.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      816 2023-05-15 23:58:43.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     3348 2023-05-16 00:01:14.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-16 00:07:39.342717 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-16 00:07:39.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-16 00:07:38.000000 streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 21:10:03.964684 streamlit-deckgl-0.4.0/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.0/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.0/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-23 21:10:03.964684 streamlit-deckgl-0.4.0/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.4.0/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-23 21:10:03.964684 streamlit-deckgl-0.4.0/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-23 21:06:07.000000 streamlit-deckgl-0.4.0/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 21:10:03.960684 streamlit-deckgl-0.4.0/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 21:10:03.960684 streamlit-deckgl-0.4.0/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2672 2023-05-15 20:40:20.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 21:10:03.964684 streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      816 2023-05-15 23:58:43.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3353 2023-05-23 21:08:27.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-23 21:10:03.960684 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-23 21:10:03.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-23 21:10:03.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-23 21:10:03.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-23 21:10:03.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-23 21:10:03.000000 streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.3.0/LICENSE` & `streamlit-deckgl-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.3.0/PKG-INFO` & `streamlit-deckgl-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.3.0
+Version: 0.4.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `streamlit-deckgl-0.3.0/README.md` & `streamlit-deckgl-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.3.0/setup.py` & `streamlit-deckgl-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.3.0",
+    version="0.4.0",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
```

### Comparing `streamlit-deckgl-0.3.0/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.4.0/src/streamlit_deckgl/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/main.js` & `streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/main.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -15,15 +15,14 @@
     if (!window.rendered) {
         const {
             spec,
             tooltip,
             height,
             customLibraries,
             configuration,
-            decription,
             events,
             description,
             overlay,
             mapbox_key,
             google_maps_key,
         } = event.detail.args;
 
@@ -43,25 +42,27 @@
 
         let deckInstance = null;
         let overlayInstance = null;
 
         const mapEventHandler = (eventType, info) => {
             if (eventType === "deck-view-state-change-event") {
                 currentViewState = info;
-                console.log(info);
 
                 if (overlayInstance) {
                     overlayInstance.setProps({
                         viewState: currentViewState
                     });
                 }
             }
 
-            if (events && eventlist.includes(eventType) && info.object) {
-                Streamlit.setComponentValue(info.object);
+            if (events && eventlist.includes(eventType)) {
+                Streamlit.setComponentValue({
+                    ...info.object,
+                    coordinate: info.coordinate,
+                });
             }
         };
 
         deckInstance = createDeck({
             mapboxApiKey: mapbox_key,
             googleMapsApiKey: google_maps_key,
             container,
```

### Comparing `streamlit-deckgl-0.3.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.4.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.3.0/src/streamlit_deckgl.egg-info/PKG-INFO` & `streamlit-deckgl-0.4.0/src/streamlit_deckgl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-deckgl
-Version: 0.3.0
+Version: 0.4.0
 Summary: Streamlit component for deck.gl visualisation
 Author: Oceanum
 Author-email: developers@oceanum.science
 Keywords: streamlit,pydeck,deck.gl,visualisation
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

