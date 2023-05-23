# Comparing `tmp/ersciyt-1.89.tar.gz` & `tmp/ersciyt-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.89.tar", last modified: Sun May 21 07:56:34 2023, max compression
+gzip compressed data, was "ersciyt-1.9.tar", last modified: Tue May 23 15:17:48 2023, max compression
```

## Comparing `ersciyt-1.89.tar` & `ersciyt-1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 07:56:34.698267 ersciyt-1.89/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-21 07:56:01.000000 ersciyt-1.89/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-21 07:56:01.000000 ersciyt-1.89/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-21 07:56:34.699267 ersciyt-1.89/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-21 07:56:01.000000 ersciyt-1.89/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 07:56:34.697267 ersciyt-1.89/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 07:56:34.698267 ersciyt-1.89/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 07:56:34.698267 ersciyt-1.89/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     8338 2023-05-21 07:56:01.000000 ersciyt-1.89/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 07:56:34.698267 ersciyt-1.89/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-21 07:56:34.000000 ersciyt-1.89/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-21 07:56:34.000000 ersciyt-1.89/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 07:56:34.000000 ersciyt-1.89/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-21 07:56:34.000000 ersciyt-1.89/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-21 07:56:34.000000 ersciyt-1.89/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-21 07:56:34.699267 ersciyt-1.89/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-21 07:56:01.000000 ersciyt-1.89/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.640834 ersciyt-1.9/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-23 15:17:40.000000 ersciyt-1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-23 15:17:40.000000 ersciyt-1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-23 15:17:48.640834 ersciyt-1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2023-05-23 15:17:40.000000 ersciyt-1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.638834 ersciyt-1.9/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)        2 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/static/ytvid.mp4
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     8711 2023-05-23 15:17:40.000000 ersciyt-1.9/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:17:48.639834 ersciyt-1.9/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      417 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-23 15:17:48.000000 ersciyt-1.9/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-23 15:17:48.640834 ersciyt-1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-23 15:17:40.000000 ersciyt-1.9/setup.py
```

### Comparing `ersciyt-1.89/LICENSE` & `ersciyt-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.89/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.9/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.89/ersciyt/urls.py` & `ersciyt-1.9/ersciyt/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,11 +8,13 @@
     path('vid/', views.vid ),
     path('youtube/', views.vid ),
     #path('mp3/<str:link>/', views.ytmp3 ),
     #path('ab/<str:time>/<str:link>/', views.abcut ),
     #path('<str:lang>/<str:link>/', views.sub ),
     path('shqr/', views.shqr ),
     path('mp4/<str:link>/', views.ytmp4 ),
+    path('yt/<str:link>/', views.yt2mp4 ),
     path('nginx/', views.ngin ),
     path('<str:link>/', views.ytdwn ),
     
+    
 ]
```

### Comparing `ersciyt-1.89/ersciyt/views.py` & `ersciyt-1.9/ersciyt/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,24 @@
             os.remove("/tmp/a.mp4")
         os.system('yt-dlp  -f 18 -o /tmp/a.mp4 https://www.youtube.com/watch?v={}'.format(link)) 
         urllink = settings.ERSCIYT_LINK if hasattr(settings, 'ERSCIYT_LINK') and settings.ERSCIYT_LINK else ""
         return redirect(urllink)
     except:
         return HttpResponse ('Youtube Url Is Mistake!')
 
+def yt2mp4(request,link):
+    try:        
+        vidpath = finders.find('ytvid.mp4')        
+        if os.path.isfile(vidpath):
+            os.remove(vipath)
+        os.system('yt-dlp  -f 18 -o {} https://www.youtube.com/watch?v={}'.format(vidpath,link)) 
+        return redirect("/static/ytvid.mp4")
+    except:
+        return HttpResponse ('Youtube Url Is Mistake!')
+
 def shqr(request):
     try:
         pic=request.GET['idx']
         qr_code = pyqrcode.create(pic)#request.headers['HTTP_REFERER'])
         qr_code.svg('a.svg', scale=6)
         img=open('a.svg', "r")
         #image_data = base64.b64encode(img.read()).decode('utf-8')
```

### Comparing `ersciyt-1.89/setup.cfg` & `ersciyt-1.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.89
+version = 1.9
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

