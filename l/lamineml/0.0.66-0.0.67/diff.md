# Comparing `tmp/lamineml-0.0.66.tar.gz` & `tmp/lamineml-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamineml-0.0.66.tar", last modified: Sat May 20 17:25:30 2023, max compression
+gzip compressed data, was "lamineml-0.0.67.tar", last modified: Mon May 22 15:49:36 2023, max compression
```

## Comparing `lamineml-0.0.66.tar` & `lamineml-0.0.67.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 17:25:30.315310 lamineml-0.0.66/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.66/LICENSE
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 17:25:30.315310 lamineml-0.0.66/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.66/README.md
--rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.66/pyproject.toml
--rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-20 17:25:30.315310 lamineml-0.0.66/setup.cfg
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 17:25:30.311310 lamineml-0.0.66/src/
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 17:25:30.315310 lamineml-0.0.66/src/lamine/
--rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.66/src/lamine/__init__.py
--rw-rw-r--   0 hello     (1000) hello     (1000)     4288 2023-05-20 17:24:44.000000 lamineml-0.0.66/src/lamine/tools.py
-drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-20 17:25:30.315310 lamineml-0.0.66/src/lamineml.egg-info/
--rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-20 17:25:30.000000 lamineml-0.0.66/src/lamineml.egg-info/PKG-INFO
--rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-20 17:25:30.000000 lamineml-0.0.66/src/lamineml.egg-info/SOURCES.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-20 17:25:30.000000 lamineml-0.0.66/src/lamineml.egg-info/dependency_links.txt
--rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-20 17:25:30.000000 lamineml-0.0.66/src/lamineml.egg-info/top_level.txt
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-22 15:49:36.656447 lamineml-0.0.67/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2021-07-31 02:25:56.000000 lamineml-0.0.67/LICENSE
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-22 15:49:36.656447 lamineml-0.0.67/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2304 2021-07-31 02:25:56.000000 lamineml-0.0.67/README.md
+-rw-rw-r--   0 hello     (1000) hello     (1000)      126 2023-05-18 14:20:16.000000 lamineml-0.0.67/pyproject.toml
+-rw-rw-r--   0 hello     (1000) hello     (1000)      626 2023-05-22 15:49:36.656447 lamineml-0.0.67/setup.cfg
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-22 15:49:36.652447 lamineml-0.0.67/src/
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-22 15:49:36.656447 lamineml-0.0.67/src/lamine/
+-rw-rw-r--   0 hello     (1000) hello     (1000)        0 2023-04-29 17:24:39.000000 lamineml-0.0.67/src/lamine/__init__.py
+-rw-rw-r--   0 hello     (1000) hello     (1000)     4868 2023-05-22 15:49:04.000000 lamineml-0.0.67/src/lamine/tools.py
+drwxrwxr-x   0 hello     (1000) hello     (1000)        0 2023-05-22 15:49:36.656447 lamineml-0.0.67/src/lamineml.egg-info/
+-rw-rw-r--   0 hello     (1000) hello     (1000)     2806 2023-05-22 15:49:36.000000 lamineml-0.0.67/src/lamineml.egg-info/PKG-INFO
+-rw-rw-r--   0 hello     (1000) hello     (1000)      229 2023-05-22 15:49:36.000000 lamineml-0.0.67/src/lamineml.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        1 2023-05-22 15:49:36.000000 lamineml-0.0.67/src/lamineml.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello     (1000) hello     (1000)        7 2023-05-22 15:49:36.000000 lamineml-0.0.67/src/lamineml.egg-info/top_level.txt
```

### Comparing `lamineml-0.0.66/PKG-INFO` & `lamineml-0.0.67/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.66
+Version: 0.0.67
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lamineml-0.0.66/README.md` & `lamineml-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `lamineml-0.0.66/setup.cfg` & `lamineml-0.0.67/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lamineml
-version = 0.0.66
+version = 0.0.67
 author = Lamine ML
 author_email = lamineml128@gmail.com
 description = use this library in kivy android
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `lamineml-0.0.66/src/lamine/tools.py` & `lamineml-0.0.67/src/lamine/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 g =autoclass("android.view.Gravity")
 t= autoclass("android.widget.Toast")
 window=autoclass ("android.view.WindowManager$LayoutParams")
 window2 =autoclass("android.view.WindowManager")
 ac=autoclass("android.app.ActivityManager")
 com =autoclass("android.content.ComponentName")
 pak =autoclass("android.content.pm.PackageManager")
+WebView = autoclass('android.webkit.WebView')
+WebViewClient = autoclass('android.webkit.WebViewClient')
+view =autoclass("android.view.View")
 
 
 from android.runnable import run_on_ui_thread
 def remove_apps(pk):
     s=Intent()
     s.setAction(Intent.ACTION_DELETE)
     s.setData(uri.parse("package:"+pk+""))
@@ -85,15 +88,14 @@
     else:
         return "None"
     return f
 def getLanguage():
     return  getL.getDefault().getDisplayLanguage()
 def unhide(package_name,package_name_activity):
     p= activity.getPackageManager()
-    pak = autoclass("android.content.pm.PackageManager")
 
     c=com(package_name,package_name_activity)
     p.setComponentEnabledSetting(c,pak.COMPONENT_ENABLED_STATE_ENABLED,pak.DONT_KILL_APP)
 def hide(package_name,package_name_activity):
     com = autoclass("android.content.ComponentName")
 
     p= activity.getPackageManager()
@@ -102,14 +104,30 @@
 def isSecure():
     x=cast ("android.app.KeyguardManager",activity.getSystemService(Context.KEYGUARD_SERVICE)  )
     h=x.isKeyguardSecure()
     if(h):
         return True
     else:
         return False
+
+@run_on_ui_thread
+def create_webview(html,*args):
+    webview = WebView(activity)
+    webview.getSettings().setJavaScriptEnabled(True)
+    wvc = WebViewClient();
+    webview.setWebViewClient(wvc);
+    activity.setContentView(webview)
+    webview.loadDataWithBaseURL(None, html, None, "UTF-8", None)
+    if webview.canGoBack():
+        webview.goBack()
+@run_on_ui_thread
+def hide_Navigation():
+    activity.getWindow().getDecorView().setSystemUiVisibility(view.SYSTEM_UI_FLAG_HIDE_NAVIGATION);
+
+
 def isMusicActive():
     x = cast("android.media.AudioManager", activity.getSystemService(Context.AUDIO_SERVICE))
     h = x.isMusicActive()
     if (h):
         return True
     else:
         return False
```

### Comparing `lamineml-0.0.66/src/lamineml.egg-info/PKG-INFO` & `lamineml-0.0.67/src/lamineml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamineml
-Version: 0.0.66
+Version: 0.0.67
 Summary: use this library in kivy android
 Home-page: https://github.com/pypa/sampleproject
 Author: Lamine ML
 Author-email: lamineml128@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

