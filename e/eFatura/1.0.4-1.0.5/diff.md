# Comparing `tmp/eFatura-1.0.4.tar.gz` & `tmp/eFatura-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.4.tar", last modified: Tue May 23 12:48:35 2023, max compression
+gzip compressed data, was "eFatura-1.0.5.tar", last modified: Tue May 23 14:14:52 2023, max compression
```

## Comparing `eFatura-1.0.4.tar` & `eFatura-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.330132 eFatura-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 12:47:58.000000 eFatura-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 12:48:35.326132 eFatura-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-23 12:47:58.000000 eFatura-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 12:47:58.000000 eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 12:47:58.000000 eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-23 12:47:58.000000 eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 12:47:58.000000 eFatura-1.0.4/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:48:35.326132 eFatura-1.0.4/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 12:48:35.000000 eFatura-1.0.4/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:48:35.330132 eFatura-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-23 12:47:58.000000 eFatura-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 14:14:26.000000 eFatura-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 14:14:52.895744 eFatura-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-23 14:14:26.000000 eFatura-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-23 14:14:26.000000 eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.895744 eFatura-1.0.5/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 14:14:26.000000 eFatura-1.0.5/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:14:52.891744 eFatura-1.0.5/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 14:14:52.000000 eFatura-1.0.5/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 14:14:52.895744 eFatura-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-23 14:14:26.000000 eFatura-1.0.5/setup.py
```

### Comparing `eFatura-1.0.4/PKG-INFO` & `eFatura-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.4
+Version: 1.0.5
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.4 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.5 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð eFatura
```

### Comparing `eFatura-1.0.4/README.md` & `eFatura-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml`

 * *Files 4% similar despite different names*

#### Comparing `eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.appdata.xml`

```diff
@@ -28,12 +28,12 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.4" date="2023-5-23"/>
+    <release version="1.0.5" date="2023-5-23"/>
     <release version="0.0.1" date="2022-8-13"/>
   </releases>
   <content_rating type="oars-1.1"/>
 </component>
```

### Comparing `eFatura-1.0.4/Shared/org.KekikAkademi.eFatura.svg` & `eFatura-1.0.5/Shared/org.KekikAkademi.eFatura.svg`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/eFatura/Assets/logo.png` & `eFatura-1.0.5/eFatura/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/eFatura/Core/__init__.py` & `eFatura-1.0.5/eFatura/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/eFatura/GUI/__init__.py` & `eFatura-1.0.5/eFatura/GUI/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,74 +23,80 @@
 
         ayarlar = Gtk.Settings.get_default()
         ayarlar.set_property("gtk-application-prefer-dark-theme", True)
 
         self.pencere = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10, margin=20)
         self.add(self.pencere)
 
-        self.giris_alanlarini_olustur()
+        # !
+        Program(self)
+        # !
 
-    def giris_alanlarini_olustur(self):
-        girislar_cerceve = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10)
-        self.pencere.pack_start(girislar_cerceve, False, False, 0)
+    def pencereyi_kapat(self, widget, event):
+        dialog = Gtk.MessageDialog(
+            parent              = self,
+            modal               = True,
+            destroy_with_parent = True,
+            message_type        = Gtk.MessageType.QUESTION,
+            buttons             = Gtk.ButtonsType.OK_CANCEL,
+            text                = "Program Kapanıyor",
+        )
+        dialog.format_secondary_text("Bunu yapmak istediğinize emin misiniz?")
+        response = dialog.run()
+        dialog.destroy()
+
+        if response == Gtk.ResponseType.OK:
+            Gtk.main_quit()
+        else:
+            return True
+
+    def goster(self):
+        self.show_all()
+        Gtk.main()
+
+
+class Program():
+    def __init__(self, parent:Gtk.Window):
+        self.parent = parent
+
+        sorgu_alani = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10)
+        parent.pencere.pack_start(sorgu_alani, False, False, 0)
 
         self.arama_metni = Gtk.Entry()
         self.arama_metni.set_placeholder_text("Vergi / TC Kimlik Numarası")
         self.arama_metni.connect("activate", self.ara_butonuna_tiklandiginda)
-        girislar_cerceve.pack_start(self.arama_metni, False, False, 0)
+        sorgu_alani.pack_start(self.arama_metni, False, False, 0)
 
         self.ara_butonu = Gtk.Button.new_with_label("Ara")
         self.ara_butonu.connect("clicked", self.ara_butonuna_tiklandiginda)
-        girislar_cerceve.pack_start(self.ara_butonu, False, False, 0)
+        sorgu_alani.pack_start(self.ara_butonu, False, False, 0)
         self.ara_butonu.grab_focus()
 
-        self.cikti_cercevesi = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10)
-        self.pencere.pack_start(self.cikti_cercevesi, True, True, 0)
+        self.cikti_alani = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10)
+        parent.pencere.pack_start(self.cikti_alani, True, True, 0)
 
     def ara_butonuna_tiklandiginda(self, widget):
         self.ara_butonu.grab_focus()
         arama_sorgusu = self.arama_metni.get_text()
         self.arama_metni.set_text("")
 
-        self.cikti_cercevesi.foreach(Gtk.Widget.destroy)
+        self.cikti_alani.foreach(Gtk.Widget.destroy)
 
         bekleme_etiketi = Gtk.Label()
         bekleme_etiketi.set_markup("<span foreground='#EF7F1A' font_desc='12'>Lütfen Bekleyiniz...</span>")
         bekleme_etiketi.set_margin_top(10)
         bekleme_etiketi.set_halign(Gtk.Align.CENTER)
         bekleme_etiketi.set_justify(Gtk.Justification.CENTER)
         bekleme_etiketi.set_line_wrap(True)
         bekleme_etiketi.set_max_width_chars(30)
-        self.cikti_cercevesi.pack_start(bekleme_etiketi, False, False, 0)
-        self.show_all()
+        self.cikti_alani.pack_start(bekleme_etiketi, False, False, 0)
+        self.parent.show_all()
 
         def arama_tamamlandi():
             sonuc = e_fatura(arama_sorgusu)
             if sonuc:
                 bekleme_etiketi.set_markup(f"<span foreground='#17a2b8' font_desc='12'>{arama_sorgusu} Numarası\nE-Fatura Mükellefidir..</span>")
             else:
                 bekleme_etiketi.set_markup(f"<span foreground='#dc3545' font_desc='12'>{arama_sorgusu} Numarası\nE-Fatura Mükellefi Değildir..</span>")
-            self.show_all()
-
-        GLib.timeout_add(100, arama_tamamlandi)
-
-    def pencereyi_kapat(self, widget, event):
-        dialog = Gtk.MessageDialog(
-            parent              = self,
-            modal               = True,
-            destroy_with_parent = True,
-            message_type        = Gtk.MessageType.QUESTION,
-            buttons             = Gtk.ButtonsType.OK_CANCEL,
-            text                = "Program Kapanıyor",
-        )
-        dialog.format_secondary_text("Bunu yapmak istediğinize emin misiniz?")
-        response = dialog.run()
-        dialog.destroy()
+            self.parent.show_all()
 
-        if response == Gtk.ResponseType.OK:
-            Gtk.main_quit()
-        else:
-            return True
-
-    def goster(self):
-        self.show_all()
-        Gtk.main()
+        GLib.timeout_add(100, arama_tamamlandi)
```

### Comparing `eFatura-1.0.4/eFatura/Libs/Oturum.py` & `eFatura-1.0.5/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/eFatura/konsol.py` & `eFatura-1.0.5/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/eFatura.egg-info/PKG-INFO` & `eFatura-1.0.5/eFatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.4
+Version: 1.0.5
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.4 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.0.5 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð eFatura
```

### Comparing `eFatura-1.0.4/eFatura.egg-info/SOURCES.txt` & `eFatura-1.0.5/eFatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.4/setup.py` & `eFatura-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.4",
+    version      = "1.0.5",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

