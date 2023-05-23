# Comparing `tmp/eFatura-1.0.2.tar.gz` & `tmp/eFatura-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.2.tar", last modified: Thu May 18 12:17:29 2023, max compression
+gzip compressed data, was "eFatura-1.0.3.tar", last modified: Tue May 23 12:08:51 2023, max compression
```

## Comparing `eFatura-1.0.2.tar` & `eFatura-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-18 12:17:07.000000 eFatura-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-18 12:17:29.575943 eFatura-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-18 12:17:07.000000 eFatura-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/eFatura/
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/KekikGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/konsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-18 12:17:07.000000 eFatura-1.0.2/eFatura/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 12:17:29.575943 eFatura-1.0.2/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 12:17:29.000000 eFatura-1.0.2/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 12:17:29.575943 eFatura-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-18 12:17:07.000000 eFatura-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 12:08:19.000000 eFatura-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 12:08:51.144602 eFatura-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-23 12:08:19.000000 eFatura-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.140601 eFatura-1.0.3/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 12:08:19.000000 eFatura-1.0.3/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 12:08:19.000000 eFatura-1.0.3/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-23 12:08:19.000000 eFatura-1.0.3/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 12:08:19.000000 eFatura-1.0.3/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 12:08:51.144602 eFatura-1.0.3/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 12:08:51.000000 eFatura-1.0.3/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 12:08:51.144602 eFatura-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-23 12:08:19.000000 eFatura-1.0.3/setup.py
```

### Comparing `eFatura-1.0.2/PKG-INFO` & `eFatura-1.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,141 @@
-Metadata-Version: 2.1
-Name: eFatura
-Version: 1.0.2
-Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
-Home-page: https://github.com/keyiflerolsun/E-Fatura_Sorgu
-Author: keyiflerolsun
-Author-email: keyiflerolsun@gmail.com
-License: GPLv3+
-Keywords: eFatura,KekikAkademi,keyiflerolsun
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # 🔍 eFatura
 
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white)
-![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)
+[![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eFatura?logo=git&logoColor=white&label=Boyut)](#)
+[![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eFatura&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
-![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white)
-![License](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white)
-![Status](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white)
-
-[![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
-[![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura)
-
-[![Fonksiyon Testleri ve PyPI Yükle](https://github.com/keyiflerolsun/eFatura/actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/eFatura/actions/workflows/KekikFlow.yml)
+[![GitHub](https://img.shields.io/github/v/release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/keyiflerolsun/eFatura/releases)
+[![Fonksiyon Testleri ve PyPI Yükle](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml)
+[![Flatpak Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml)
+
+[![PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eFatura)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eFatura?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eFatura)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eFatura)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/eFatura?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu*
 
-![eFatura](https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)
+[![eFatura](https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)](#)
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🚀 Kurulum
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg"> PyPi (Lib - CLI - UI)
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg"></a> PyPI (Lib - CLI - UI)
 
 ```bash
 # Yüklemek
 pip install eFatura
 
 # Güncellemek
 pip install -U eFatura
 ```
 
 ## 📝 Kullanım
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"> Lib
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"></a> Lib
 
 ```python
 from eFatura import e_fatura
 
 print(e_fatura("11111111111")) # Vergi Numarası veya TC Kimlik Numarası
 
 >> True | False
 ```
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg"> CLI
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg"></a> CLI
 
 ```bash
 eFatura 11111111111
 
 # » [~] 11111111111 Numarası E-Fatura Mükellefi Değildir..
 ```
 
 ### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg"> UI
 
 ```bash
 eFaturaGUI
 ```
 
-## 📝 Proje Sahibi
-
-- ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
 
 ---
 
 <details>
     <summary style="font-weight: bold; font-size: 20px">
-      <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"> <b>Manuel Derlemek</b>
+      <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/buddy.svg"></a> <b>Kendiniz Paketlemek İsterseniz</b>
       <i>(genişletmek için tıklayın!)</i>
     </summary>
     <br/>
 
-### <img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"> Python
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg"></a> Python
 
 ```bash
 # Depoyu Çek
 https://github.com/keyiflerolsun/eFatura.git
 cd eFatura
 
 # Gerekli Ortamları Kur
-pip install -U pip setuptools wheel twine
+pip install -U pip setuptools wheel
 
 # Paketi Yükle
 pip install .
 
 # Artıkları Temizle
 rm -rf build *.egg-info
 
 # Çalıştır
 eFatura     # CLI
 eFaturaGUI  # GUI
 
 # Paketi Kaldır
 pip uninstall eFatura
 ```
+
+### <a href="#"><img width="16" src="https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/flatpak.svg"></a> FlatPak
+
+```bash
+# Depoyu Çek
+git clone https://github.com/keyiflerolsun/eFatura.git
+cd eFatura
+
+# Gerekli Dosyaları Al
+mv Shared/*.yml . && mv Shared/SRC .
+
+# Gerekli Ortamları Kur
+flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
+flatpak remote-add --if-not-exists flathub-beta https://flathub.org/beta-repo/flathub-beta.flatpakrepo
+flatpak update && flatpak upgrade
+flatpak install flathub org.gnome.{Platform,Sdk}//44
+
+# Paketle
+flatpak-builder --user --install --force-clean build-dir org.KekikAkademi.eFatura.yml
+
+# Artıkları Temizle
+rm -rf .flatpak* .vscode build-dir && find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
+
+# Çalıştır
+flatpak run org.KekikAkademi.eFatura
+
+# Paketi Kaldır
+flatpak uninstall org.KekikAkademi.eFatura
+```
+
 </details>
 
 ---
 
+## 📝 Proje Sahibi
+
+- ✅ **[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)**
+
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eFatura/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
 
 ## ♻️ İletişim
 
@@ -125,8 +143,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,57 +1,70 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.2 Summary: Vergi veya TC
-Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
-github.com/keyiflerolsun/E-Fatura_Sorgu Author: keyiflerolsun Author-email:
-keyiflerolsun@gmail.com License: GPLv3+ Keywords:
-eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
-Production/Stable Classifier: License :: OSI Approved :: GNU General Public
-License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10 Description-Content-Type: text/markdown # ð eFatura
-![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/
-eFatura?logo=git&logoColor=white) ![GÃ¶rÃ¼ntÃ¼lenme](https://
+# ð eFatura [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/
+eFatura?logo=git&logoColor=white&label=Boyut)](#) [![GÃ¶rÃ¼ntÃ¼lenme](https://
 hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/
-keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme) [https://img.shields.io/badge/
-âï¸-Kahve_Ismarla-ffdd00] ![Python Version](https://img.shields.io/pypi/
-pyversions/eFatura?logo=python&logoColor=white) ![License](https://
-img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white) ![Status](https://
-img.shields.io/pypi/status/eFatura?logo=windowsterminal&logoColor=white) [!
-[PyPI](https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white)](https:
-//pypi.org/project/eFatura) [![PyPI - Downloads](https://img.shields.io/pypi/
-dm/eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura) [!
-[PyPI - Wheel](https://img.shields.io/pypi/wheel/
-eFatura?logo=pypi&logoColor=white)](https://pypi.org/project/eFatura) [!
-[Fonksiyon Testleri ve PyPI YÃ¼kle](https://github.com/keyiflerolsun/eFatura/
-actions/workflows/KekikFlow.yml/badge.svg)](https://github.com/keyiflerolsun/
-eFatura/actions/workflows/KekikFlow.yml) *Vergi veya TC Kimlik NumarasÄ±ndan E-
-Fatura MÃ¼kellefiyet Sorgusu* ![eFatura](https://raw.githubusercontent.com/
-keyiflerolsun/eFatura/main/.github/icons/SS.png) [![ForTheBadge made-with-
-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://
-www.python.org/) [![ForTheBadge built-with-love](https://ForTheBadge.com/
-images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð
-Kurulum ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
-main/.github/icons/pypi.svg] PyPi (Lib - CLI - UI) ```bash # YÃ¼klemek pip
-install eFatura # GÃ¼ncellemek pip install -U eFatura ``` ## ð KullanÄ±m ###
-[https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
-python.svg] Lib ```python from eFatura import e_fatura print(e_fatura
-("11111111111")) # Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ```
-### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
-icons/iterm2.svg] CLI ```bash eFatura 11111111111 # Â» [~] 11111111111
-NumarasÄ± E-Fatura MÃ¼kellefi DeÄildir.. ``` ### [https://
-raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
-freedesktop.svg] UI ```bash eFaturaGUI ``` ## ð Proje Sahibi - â **
-[kmprens/CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ---
-[https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/
-buddy.svg] Manuel Derlemek (geniÅletmek iÃ§in tÄ±klayÄ±n!)
+keyiflerolsun/eFatura&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/
+âï¸-Kahve_Ismarla-ffdd00] [![GitHub](https://img.shields.io/github/v/
+release/keyiflerolsun/eFatura?logo=github&label=GitHub)](https://github.com/
+keyiflerolsun/eFatura/releases) [![Fonksiyon Testleri ve PyPI YÃ¼kle](https://
+img.shields.io/github/actions/workflow/status/keyiflerolsun/eFatura/
+test_ve_pypi.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/eFatura/actions/workflows/test_ve_pypi.yml) [![Flatpak
+YÃ¼kleyici](https://img.shields.io/github/actions/workflow/status/
+keyiflerolsun/eFatura/
+flatpakYukle.yml?label=Flatpak%20Y%C3%BCkleyici&logo=github)](https://
+github.com/keyiflerolsun/eFatura/actions/workflows/flatpakYukle.yml) [![PyPI]
+(https://img.shields.io/pypi/v/eFatura?logo=pypi&logoColor=white&label=PyPI)]
+(https://pypi.org/project/eFatura) [![PyPI - YÃ¼klenme](https://img.shields.io/
+pypi/dm/eFatura?logo=pypi&logoColor=white&label=YÃ¼klenme)](https://pypi.org/
+project/eFatura) [![PyPI - Wheel](https://img.shields.io/pypi/wheel/
+eFatura?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/
+eFatura) [![Python Version](https://img.shields.io/pypi/pyversions/
+eFatura?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/eFatura?logo=gnu&logoColor=white&label=Lisans)](#) [!
+[Durum](https://img.shields.io/pypi/status/
+eFatura?logo=windowsterminal&logoColor=white&label=Durum)](#) *Vergi veya TC
+Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu* [![eFatura](https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png)](#)
+[![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-
+with-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love]
+(https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Kurulum ### [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/pypi.svg]
+PyPI (Lib - CLI - UI) ```bash # YÃ¼klemek pip install eFatura # GÃ¼ncellemek
+pip install -U eFatura ``` ## ð KullanÄ±m ### [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/python.svg]
+Lib ```python from eFatura import e_fatura print(e_fatura("11111111111")) #
+Vergi NumarasÄ± veya TC Kimlik NumarasÄ± >> True | False ``` ### [https://
+raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/iterm2.svg]
+CLI ```bash eFatura 11111111111 # Â» [~] 11111111111 NumarasÄ± E-Fatura
+MÃ¼kellefi DeÄildir.. ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/freedesktop.svg] UI ```bash eFaturaGUI
+``` ---   [https://raw.githubusercontent.com/keyiflerolsun/eFatura/
+main/.github/icons/buddy.svg] Kendiniz Paketlemek Ä°sterseniz (geniÅletmek
+iÃ§in tÄ±klayÄ±n!)
 ### [https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/
 icons/python.svg] Python ```bash # Depoyu Ãek https://github.com/
 keyiflerolsun/eFatura.git cd eFatura # Gerekli OrtamlarÄ± Kur pip install -
-U pip setuptools wheel twine # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ±
-Temizle rm -rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI #
-Paketi KaldÄ±r pip uninstall eFatura ```  --- ## ð Telif HakkÄ± ve Lisans *
-*Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun)
-â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://
-github.com/keyiflerolsun/eFatura/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re
-lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
+U pip setuptools wheel # Paketi YÃ¼kle pip install . # ArtÄ±klarÄ± Temizle rm -
+rf build *.egg-info # ÃalÄ±ÅtÄ±r eFatura # CLI eFaturaGUI # GUI # Paketi
+KaldÄ±r pip uninstall eFatura ``` ### [https://raw.githubusercontent.com/
+keyiflerolsun/eFatura/main/.github/icons/flatpak.svg] FlatPak ```bash # Depoyu
+Ãek git clone https://github.com/keyiflerolsun/eFatura.git cd eFatura #
+Gerekli DosyalarÄ± Al mv Shared/*.yml . && mv Shared/SRC . # Gerekli OrtamlarÄ±
+Kur flatpak remote-add --if-not-exists flathub https://flathub.org/repo/
+flathub.flatpakrepo flatpak remote-add --if-not-exists flathub-beta https://
+flathub.org/beta-repo/flathub-beta.flatpakrepo flatpak update && flatpak
+upgrade flatpak install flathub org.gnome.{Platform,Sdk}//44 # Paketle flatpak-
+builder --user --install --force-clean build-dir org.KekikAkademi.eFatura.yml #
+ArtÄ±klarÄ± Temizle rm -rf .flatpak* .vscode build-dir && find . | grep -E "
+(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf # ÃalÄ±ÅtÄ±r flatpak run
+org.KekikAkademi.eFatura # Paketi KaldÄ±r flatpak uninstall
+org.KekikAkademi.eFatura ```  --- ## ð Proje Sahibi - â **[kmprens/
+CheckEinvoice](https://github.com/kmprens/CheckEinvoice)** ## ð Telif HakkÄ±
+ve Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eFatura/blob/master/LICENSE) *KoÅullarÄ±na
+gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek
 isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun]
 (https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https:/
 /KekikAkademi.org/Kahve)** *** > **[@KekikAkademi](https://t.me/KekikAkademi)**
 *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eFatura-1.0.2/eFatura/KekikGUI.py` & `eFatura-1.0.3/eFatura/GUI/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from gi import require_version
 require_version("Gtk", "3.0")
 
 from gi.repository import Gtk, GLib
 from eFatura       import e_fatura
+from ..Libs        import dosya_ver
 
 class KekikGUI(Gtk.Window):
-    def __init__(self, pencere_adi="eFatura", logo_yolu="logo.png", p_genislik=300, p_yukseklik=200):
+    def __init__(self):
         super().__init__()
-        self.set_title(pencere_adi)
+        self.set_title("eFatura")
         self.set_resizable(False)
-        self.set_default_size(p_genislik, p_yukseklik)
+        self.set_default_size(300, 200)
         self.set_position(Gtk.WindowPosition.CENTER)
         self.connect("delete-event", self.pencereyi_kapat)
-        self.set_icon_from_file(logo_yolu)
+        self.set_icon_from_file(dosya_ver("Assets/logo.png", ust_dizin=2))
 
         self.pencere = Gtk.Box(orientation=Gtk.Orientation.VERTICAL, spacing=10, margin=20)
         self.add(self.pencere)
 
         self.giris_alanlarini_olustur()
 
     def giris_alanlarini_olustur(self):
```

### Comparing `eFatura-1.0.2/eFatura/Oturum.py` & `eFatura-1.0.3/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.2/eFatura/__init__.py` & `eFatura-1.0.3/eFatura/Core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from .Oturum     import legacy_session
-from shutil      import copyfileobj
-from uuid        import uuid4
-from os          import remove
-from PIL         import Image
-from pytesseract import image_to_string
+from ..Libs.Oturum import legacy_session
+from shutil        import copyfileobj
+from uuid          import uuid4
+from os            import remove
+from PIL           import Image
+from pytesseract   import image_to_string
 
 def e_fatura(vergi_numarasi:str) -> bool:
     """Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu"""
     captcha_resmi = f"captcha_{uuid4()}.jpg"
 
     while True:
         oturum = legacy_session()
```

### Comparing `eFatura-1.0.2/eFatura/konsol.py` & `eFatura-1.0.3/eFatura/konsol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
-from Kekik.cli import konsol
-from eFatura   import e_fatura
-from sys       import argv
+from .Libs   import konsol
+from eFatura import e_fatura
+from sys     import argv
 
 def basla():
     print()
 
     if len(argv) != 2:
         konsol.print("[bold yellow2][!] Lütfen Vergi Numarası veya TC Kimlik Numarası Belirtin..")
         konsol.print("\n[turquoise2]Örn.: [pale_green1]eFatura 11111111111\n")
```

### Comparing `eFatura-1.0.2/setup.py` & `eFatura-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.2",
+    version      = "1.0.3",
     url          = "https://github.com/keyiflerolsun/E-Fatura_Sorgu",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -23,29 +23,36 @@
 
     # ? Paket Bilgileri
     packages         = ["eFatura"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
-        "Kekik",
+        "install_freedesktop",
+        "rich",
         "requests",
         "urllib3",
         "Pillow",
-        "pytesseract",
-        # "pygobject",
-        # "pygobject-stubs"
+        "pytesseract"
     ],
 
     # ? Konsoldan Çalıştırılabilir
     entry_points = {
         "console_scripts": [
             "eFatura    = eFatura.konsol:basla",
             "eFaturaGUI = eFatura.arayuz:basla"
         ]
     },
 
+    # ? Masaüstü Paketi
+    setup_requires = ["install_freedesktop"],
+    data_files     = [
+        ("share/appdata",                     ["Shared/org.KekikAkademi.eFatura.appdata.xml"]),
+        ("share/applications",                ["Shared/org.KekikAkademi.eFatura.desktop"]),
+        ("share/icons/hicolor/scalable/apps", ["Shared/org.KekikAkademi.eFatura.svg"])
+    ],
+
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
 )
```

