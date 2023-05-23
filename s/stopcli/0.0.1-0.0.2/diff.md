# Comparing `tmp/stopcli-0.0.1.tar.gz` & `tmp/stopcli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopcli-0.0.1.tar", last modified: Tue May 23 07:19:56 2023, max compression
+gzip compressed data, was "stopcli-0.0.2.tar", last modified: Tue May 23 07:32:13 2023, max compression
```

## Comparing `stopcli-0.0.1.tar` & `stopcli-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:19:56.244581 stopcli-0.0.1/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      141 2023-05-23 07:19:56.244417 stopcli-0.0.1/PKG-INFO
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:19:56.242386 stopcli-0.0.1/app/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 06:50:44.000000 stopcli-0.0.1/app/__init__.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:19:56.242701 stopcli-0.0.1/app/classes/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 06:46:16.000000 stopcli-0.0.1/app/classes/__init__.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3873 2023-05-23 06:51:27.000000 stopcli-0.0.1/app/classes/stop_sheet.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      281 2023-04-10 01:56:30.000000 stopcli-0.0.1/app/constants.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      534 2023-05-23 06:57:58.000000 stopcli-0.0.1/app/generator.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      435 2023-05-23 06:58:43.000000 stopcli-0.0.1/app/main.py
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-23 07:19:56.244663 stopcli-0.0.1/setup.cfg
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      487 2023-05-23 07:19:55.000000 stopcli-0.0.1/setup.py
-drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:19:56.244035 stopcli-0.0.1/stopcli.egg-info/
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      141 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/PKG-INFO
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)      308 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/SOURCES.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/dependency_links.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/entry_points.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)       89 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/requires.txt
--rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-23 07:19:56.000000 stopcli-0.0.1/stopcli.egg-info/top_level.txt
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:32:13.771184 stopcli-0.0.2/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      141 2023-05-23 07:32:13.771001 stopcli-0.0.2/PKG-INFO
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:32:13.768301 stopcli-0.0.2/app/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 06:50:44.000000 stopcli-0.0.2/app/__init__.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:32:13.768820 stopcli-0.0.2/app/classes/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 06:46:16.000000 stopcli-0.0.2/app/classes/__init__.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)     3873 2023-05-23 06:51:27.000000 stopcli-0.0.2/app/classes/stop_sheet.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      281 2023-04-10 01:56:30.000000 stopcli-0.0.2/app/constants.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      571 2023-05-23 07:31:20.000000 stopcli-0.0.2/app/generator.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      435 2023-05-23 06:58:43.000000 stopcli-0.0.2/app/main.py
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       38 2023-05-23 07:32:13.771241 stopcli-0.0.2/setup.cfg
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      487 2023-05-23 07:32:04.000000 stopcli-0.0.2/setup.py
+drwxr-xr-x   0 wilsonmendoza   (501) staff       (20)        0 2023-05-23 07:32:13.770687 stopcli-0.0.2/stopcli.egg-info/
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      141 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/PKG-INFO
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)      308 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/SOURCES.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        1 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/dependency_links.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       41 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/entry_points.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)       89 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/requires.txt
+-rw-r--r--   0 wilsonmendoza   (501) staff       (20)        4 2023-05-23 07:32:13.000000 stopcli-0.0.2/stopcli.egg-info/top_level.txt
```

### Comparing `stopcli-0.0.1/app/classes/stop_sheet.py` & `stopcli-0.0.2/app/classes/stop_sheet.py`

 * *Files identical despite different names*

### Comparing `stopcli-0.0.1/app/generator.py` & `stopcli-0.0.2/app/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     for player in players:
         template = StopSheet(player.upper())
         pdf = template.generate_pdf()
         bytes = pdf.output()
         reader = PdfReader(BytesIO(bytes))
         merger.append(reader)
 
-    merger.write("sheets.pdf")
-    merger.close()
-    os.system("open sheets.pdf")
+    if len(players) > 0:
+        merger.write("sheets.pdf")
+        merger.close()
+        os.system("open sheets.pdf")
```

