# Comparing `tmp/pretext-1.5.4.dev20230522.tar.gz` & `tmp/pretext-1.5.4.dev20230523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.5.4.dev20230522.tar", max compression
+gzip compressed data, was "pretext-1.5.4.dev20230523.tar", max compression
```

## Comparing `pretext-1.5.4.dev20230522.tar` & `pretext-1.5.4.dev20230523.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-05-22 06:18:14.773106 pretext-1.5.4.dev20230522/LICENSE
--rw-r--r--   0        0        0     9664 2023-05-22 06:18:14.773106 pretext-1.5.4.dev20230522/README.md
--rw-r--r--   0        0        0     1440 2023-05-22 06:18:46.221535 pretext-1.5.4.dev20230522/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/__main__.py
--rw-r--r--   0        0        0     7344 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/build.py
--rw-r--r--   0        0        0    22954 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-05-22 06:18:51.129639 pretext-1.5.4.dev20230522/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/core/resources.py
--rw-r--r--   0        0        0  1030816 2023-05-22 06:18:51.129639 pretext-1.5.4.dev20230522/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/generate.py
--rw-r--r--   0        0        0    24172 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/project.py
--rw-r--r--   0        0        0      516 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-05-22 06:18:51.177640 pretext-1.5.4.dev20230522/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-05-22 06:18:51.169639 pretext-1.5.4.dev20230522/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-05-22 06:18:51.181640 pretext-1.5.4.dev20230522/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-05-22 06:18:51.197640 pretext-1.5.4.dev20230522/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-05-22 06:18:51.185640 pretext-1.5.4.dev20230522/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18300 2023-05-22 06:18:14.777106 pretext-1.5.4.dev20230522/pretext/utils.py
--rw-r--r--   0        0        0     1119 2023-05-22 06:18:46.221535 pretext-1.5.4.dev20230522/pyproject.toml
--rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230522/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-05-23 06:18:10.323310 pretext-1.5.4.dev20230523/LICENSE
+-rw-r--r--   0        0        0     9664 2023-05-23 06:18:10.323310 pretext-1.5.4.dev20230523/README.md
+-rw-r--r--   0        0        0     1440 2023-05-23 06:18:44.099230 pretext-1.5.4.dev20230523/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/__main__.py
+-rw-r--r--   0        0        0     7344 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/build.py
+-rw-r--r--   0        0        0    22954 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-05-23 06:18:48.951208 pretext-1.5.4.dev20230523/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/core/resources.py
+-rw-r--r--   0        0        0  1030779 2023-05-23 06:18:48.951208 pretext-1.5.4.dev20230523/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/generate.py
+-rw-r--r--   0        0        0    24172 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-05-23 06:18:48.995208 pretext-1.5.4.dev20230523/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-05-23 06:18:48.987208 pretext-1.5.4.dev20230523/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-05-23 06:18:48.999208 pretext-1.5.4.dev20230523/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-05-23 06:18:49.015208 pretext-1.5.4.dev20230523/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-05-23 06:18:49.003208 pretext-1.5.4.dev20230523/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18300 2023-05-23 06:18:10.327310 pretext-1.5.4.dev20230523/pretext/utils.py
+-rw-r--r--   0        0        0     1119 2023-05-23 06:18:44.099230 pretext-1.5.4.dev20230523/pyproject.toml
+-rw-r--r--   0        0        0    10761 1970-01-01 00:00:00.000000 pretext-1.5.4.dev20230523/PKG-INFO
```

### Comparing `pretext-1.5.4.dev20230522/LICENSE` & `pretext-1.5.4.dev20230523/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/README.md` & `pretext-1.5.4.dev20230523/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/__init__.py` & `pretext-1.5.4.dev20230523/pretext/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
 
-CORE_COMMIT = 'ac42cd57a6136165d0dd3773a9207287a5e124a7'
+CORE_COMMIT = '0f4bed37ad9f6cf42e4aeb5e75e437cc4004cf19'
 
 
 def activate():
     """
     This function was provided by the original `pretext` package
     deployed to PyPI by Alex Willmer. Thanks to their generosity,
     we were allowed to adopt this namespace as of 1.0, so we raise an error here
```

### Comparing `pretext-1.5.4.dev20230522/pretext/build.py` & `pretext-1.5.4.dev20230523/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/cli.py` & `pretext-1.5.4.dev20230523/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/codechat.py` & `pretext-1.5.4.dev20230523/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/config/xml_overlay.py` & `pretext-1.5.4.dev20230523/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/core/pretext.py` & `pretext-1.5.4.dev20230523/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/core/resources.py` & `pretext-1.5.4.dev20230523/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/core/resources.zip` & `pretext-1.5.4.dev20230523/pretext/core/resources.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,142 +1,142 @@
-Zip file size: 1030816 bytes, number of entries: 140
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 script/mjsre/
--rw-r--r--  2.0 unx      258 b- defN 23-May-22 06:18 script/README.md
--rw-r--r--  2.0 unx     2666 b- defN 23-May-22 06:18 script/mbx
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 06:18 script/mjsre/update-sre
--rw-r--r--  2.0 unx      481 b- defN 23-May-22 06:18 script/mjsre/README.md
--rw-r--r--  2.0 unx      116 b- defN 23-May-22 06:18 script/mjsre/package.json
--rw-r--r--  2.0 unx     9251 b- defN 23-May-22 06:18 script/mjsre/mj-sre-page.js
--rw-r--r--  2.0 unx    18421 b- defN 23-May-22 06:18 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    58086 b- defN 23-May-22 06:18 schema/pretext.rnc
--rw-r--r--  2.0 unx    25290 b- defN 23-May-22 06:18 schema/pretext-validation-plus.xsl
--rw-r--r--  2.0 unx   134043 b- defN 23-May-22 06:18 schema/pretext.xml
--rw-r--r--  2.0 unx     1180 b- defN 23-May-22 06:18 schema/README.md
--rw-r--r--  2.0 unx   125135 b- defN 23-May-22 06:18 schema/pretext.xsd
--rw-r--r--  2.0 unx      326 b- defN 23-May-22 06:18 schema/xml.xsd
--rw-r--r--  2.0 unx    34210 b- defN 23-May-22 06:18 schema/pretext-dev.rng
--rw-r--r--  2.0 unx   101829 b- defN 23-May-22 06:18 schema/pretext.rng
--rw-r--r--  2.0 unx    17587 b- defN 23-May-22 06:18 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx     3135 b- defN 23-May-22 06:18 schema/build.sh
--rw-r--r--  2.0 unx     1367 b- defN 23-May-22 06:18 pretext/README.md
--rw-r--r--  2.0 unx   172432 b- defN 23-May-22 06:18 pretext/pretext.py
--rw-r--r--  2.0 unx     1955 b- defN 23-May-22 06:18 pretext/module-test.py
--rw-r--r--  2.0 unx    30908 b- defN 23-May-22 06:18 pretext/pretext
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 06:18 pretext/__init__.py
--rw-r--r--  2.0 unx    35449 b- defN 23-May-22 06:18 pretext/braille_format.py
--rw-r--r--  2.0 unx     2566 b- defN 23-May-22 06:18 pretext/pretext.cfg
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/utilities/
--rw-r--r--  2.0 unx     9787 b- defN 23-May-22 06:18 xsl/entities.ent
--rw-r--r--  2.0 unx     3239 b- defN 23-May-22 06:18 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-May-22 06:18 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-May-22 06:18 xsl/README.md
--rw-r--r--  2.0 unx   139486 b- defN 23-May-22 06:18 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-May-22 06:18 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-May-22 06:18 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-May-22 06:18 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-May-22 06:18 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-May-22 06:18 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx   262798 b- defN 23-May-22 06:18 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   104457 b- defN 23-May-22 06:18 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-May-22 06:18 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-May-22 06:18 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-May-22 06:18 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   541384 b- defN 23-May-22 06:18 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-May-22 06:18 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-May-22 06:18 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-May-22 06:18 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx    67275 b- defN 23-May-22 06:18 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-May-22 06:18 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-May-22 06:18 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx   111553 b- defN 23-May-22 06:18 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-May-22 06:18 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-May-22 06:18 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx   544780 b- defN 23-May-22 06:18 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-May-22 06:18 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-May-22 06:18 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx    13186 b- defN 23-May-22 06:18 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-May-22 06:18 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-May-22 06:18 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-May-22 06:18 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-May-22 06:18 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   606258 b- defN 23-May-22 06:18 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-May-22 06:18 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-May-22 06:18 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-May-22 06:18 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-May-22 06:18 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-May-22 06:18 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-May-22 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-May-22 06:18 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx    14482 b- defN 23-May-22 06:18 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-May-22 06:18 xsl/latex/pretext-latex-guide.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/support/play-button/
--rw-r--r--  2.0 unx      504 b- defN 23-May-22 06:18 xsl/support/README.md
--rw-r--r--  2.0 unx    10306 b- defN 23-May-22 06:18 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-May-22 06:18 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-May-22 06:18 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-May-22 06:18 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5800 b- defN 23-May-22 06:18 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx     5065 b- defN 23-May-22 06:18 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     2657 b- defN 23-May-22 06:18 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx      722 b- defN 23-May-22 06:18 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     6621 b- defN 23-May-22 06:18 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16518 b- defN 23-May-22 06:18 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-May-22 06:18 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-May-22 06:18 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-May-22 06:18 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-May-22 06:18 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-May-22 06:18 xsl/localizations/README.md
--rw-r--r--  2.0 unx    15938 b- defN 23-May-22 06:18 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-May-22 06:18 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16236 b- defN 23-May-22 06:18 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-May-22 06:18 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-May-22 06:18 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-May-22 06:18 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx    15736 b- defN 23-May-22 06:18 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-May-22 06:18 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-May-22 06:18 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-May-22 06:18 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-May-22 06:18 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx     1810 b- defN 23-May-22 06:18 xsl/utilities/README.md
--rw-r--r--  2.0 unx    30257 b- defN 23-May-22 06:18 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-May-22 06:18 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-May-22 06:18 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx     4299 b- defN 23-May-22 06:18 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx      787 b- defN 23-May-22 06:18 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx     1276 b- defN 23-May-22 06:18 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx     7761 b- defN 23-May-22 06:18 css/style_default.css
--rw-r--r--  2.0 unx     3473 b- defN 23-May-22 06:18 css/style_soundwriting.css
--rw-r--r--  2.0 unx    63664 b- defN 23-May-22 06:18 css/mathbook-add-on.css
--rw-r--r--  2.0 unx     1865 b- defN 23-May-22 06:18 css/README.md
--rw-r--r--  2.0 unx     1280 b- defN 23-May-22 06:18 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_blue_red.css
--rw-r--r--  2.0 unx   435680 b- defN 23-May-22 06:18 css/mathbook-3.css
--rw-r--r--  2.0 unx   146685 b- defN 23-May-22 06:18 css/mathbook-content.css
--rw-r--r--  2.0 unx    22438 b- defN 23-May-22 06:18 css/pretext.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_green_plum.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     4308 b- defN 23-May-22 06:18 css/colors_blue_green.css
--rw-r--r--  2.0 unx    71198 b- defN 23-May-22 06:18 css/pretext_add_on.css
--rw-r--r--  2.0 unx     2608 b- defN 23-May-22 06:18 css/colors_default.css
--rw-r--r--  2.0 unx     2438 b- defN 23-May-22 06:18 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-22 06:18 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_orange_navy.css
--rw-r--r--  2.0 unx    12567 b- defN 23-May-22 06:18 css/style_oscarlevin.css
--rw-r--r--  2.0 unx      691 b- defN 23-May-22 06:18 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     1338 b- defN 23-May-22 06:18 css/colors_red_blue.css
--rw-r--r--  2.0 unx    14069 b- defN 23-May-22 06:18 css/setcolors.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2446 b- defN 23-May-22 06:18 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1362 b- defN 23-May-22 06:18 css/epub.css
--rw-r--r--  2.0 unx     2441 b- defN 23-May-22 06:18 css/kindle.css
--rw-r--r--  2.0 unx     2397 b- defN 23-May-22 06:18 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx     4021 b- defN 23-May-22 06:18 css/update_css
-140 files, 4816921 bytes uncompressed, 1013488 bytes compressed:  79.0%
+Zip file size: 1030779 bytes, number of entries: 140
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-May-23 06:18 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-May-23 06:18 script/mbx
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 06:18 script/mjsre/update-sre
+-rw-r--r--  2.0 unx      481 b- defN 23-May-23 06:18 script/mjsre/README.md
+-rw-r--r--  2.0 unx      116 b- defN 23-May-23 06:18 script/mjsre/package.json
+-rw-r--r--  2.0 unx     9251 b- defN 23-May-23 06:18 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx    18421 b- defN 23-May-23 06:18 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-May-23 06:18 schema/pretext.rnc
+-rw-r--r--  2.0 unx    25290 b- defN 23-May-23 06:18 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx   134043 b- defN 23-May-23 06:18 schema/pretext.xml
+-rw-r--r--  2.0 unx     1180 b- defN 23-May-23 06:18 schema/README.md
+-rw-r--r--  2.0 unx   125135 b- defN 23-May-23 06:18 schema/pretext.xsd
+-rw-r--r--  2.0 unx      326 b- defN 23-May-23 06:18 schema/xml.xsd
+-rw-r--r--  2.0 unx    34210 b- defN 23-May-23 06:18 schema/pretext-dev.rng
+-rw-r--r--  2.0 unx   101829 b- defN 23-May-23 06:18 schema/pretext.rng
+-rw-r--r--  2.0 unx    17587 b- defN 23-May-23 06:18 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx     3135 b- defN 23-May-23 06:18 schema/build.sh
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-23 06:18 pretext/README.md
+-rw-r--r--  2.0 unx   172432 b- defN 23-May-23 06:18 pretext/pretext.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-May-23 06:18 pretext/module-test.py
+-rw-r--r--  2.0 unx    30908 b- defN 23-May-23 06:18 pretext/pretext
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 06:18 pretext/__init__.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-May-23 06:18 pretext/braille_format.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-May-23 06:18 pretext/pretext.cfg
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/utilities/
+-rw-r--r--  2.0 unx     9787 b- defN 23-May-23 06:18 xsl/entities.ent
+-rw-r--r--  2.0 unx     3239 b- defN 23-May-23 06:18 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-May-23 06:18 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-May-23 06:18 xsl/README.md
+-rw-r--r--  2.0 unx   139486 b- defN 23-May-23 06:18 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-May-23 06:18 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-May-23 06:18 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-May-23 06:18 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-May-23 06:18 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-May-23 06:18 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx   262798 b- defN 23-May-23 06:18 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   103661 b- defN 23-May-23 06:18 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-May-23 06:18 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-May-23 06:18 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-May-23 06:18 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   541384 b- defN 23-May-23 06:18 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-May-23 06:18 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-May-23 06:18 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-May-23 06:18 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-May-23 06:18 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-May-23 06:18 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-May-23 06:18 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx   111553 b- defN 23-May-23 06:18 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-23 06:18 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-May-23 06:18 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx   544780 b- defN 23-May-23 06:18 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-23 06:18 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-May-23 06:18 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-May-23 06:18 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-May-23 06:18 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-May-23 06:18 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-May-23 06:18 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-May-23 06:18 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx   606816 b- defN 23-May-23 06:18 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-May-23 06:18 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-May-23 06:18 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-May-23 06:18 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-May-23 06:18 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx     7526 b- defN 23-May-23 06:18 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-May-23 06:18 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-May-23 06:18 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-May-23 06:18 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-May-23 06:18 xsl/latex/pretext-latex-guide.xsl
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/support/play-button/
+-rw-r--r--  2.0 unx      504 b- defN 23-May-23 06:18 xsl/support/README.md
+-rw-r--r--  2.0 unx    10306 b- defN 23-May-23 06:18 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx     5241 b- defN 23-May-23 06:18 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-May-23 06:18 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-May-23 06:18 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     5800 b- defN 23-May-23 06:18 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx     5065 b- defN 23-May-23 06:18 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     2657 b- defN 23-May-23 06:18 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx      722 b- defN 23-May-23 06:18 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx     6621 b- defN 23-May-23 06:18 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx    16518 b- defN 23-May-23 06:18 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-May-23 06:18 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-May-23 06:18 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-May-23 06:18 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-May-23 06:18 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-May-23 06:18 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    15938 b- defN 23-May-23 06:18 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-May-23 06:18 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-May-23 06:18 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-May-23 06:18 xsl/localizations/en-US.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-May-23 06:18 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-May-23 06:18 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    15736 b- defN 23-May-23 06:18 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-May-23 06:18 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    17065 b- defN 23-May-23 06:18 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-May-23 06:18 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    16296 b- defN 23-May-23 06:18 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx     1810 b- defN 23-May-23 06:18 xsl/utilities/README.md
+-rw-r--r--  2.0 unx    30257 b- defN 23-May-23 06:18 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-May-23 06:18 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-May-23 06:18 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     4299 b- defN 23-May-23 06:18 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx      787 b- defN 23-May-23 06:18 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     1276 b- defN 23-May-23 06:18 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-May-23 06:18 css/style_default.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-May-23 06:18 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-May-23 06:18 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-May-23 06:18 css/README.md
+-rw-r--r--  2.0 unx     1280 b- defN 23-May-23 06:18 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_blue_red.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-May-23 06:18 css/mathbook-3.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-May-23 06:18 css/mathbook-content.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-May-23 06:18 css/pretext.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_green_plum.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-May-23 06:18 css/colors_blue_green.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-May-23 06:18 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     2608 b- defN 23-May-23 06:18 css/colors_default.css
+-rw-r--r--  2.0 unx     2438 b- defN 23-May-23 06:18 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-23 06:18 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-May-23 06:18 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx      691 b- defN 23-May-23 06:18 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1338 b- defN 23-May-23 06:18 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-May-23 06:18 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-May-23 06:18 css/colors_martiansands.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-May-23 06:18 css/epub.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-May-23 06:18 css/kindle.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-May-23 06:18 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-May-23 06:18 css/update_css
+140 files, 4816683 bytes uncompressed, 1013451 bytes compressed:  79.0%
```

#### xsl/pretext-runestone.xsl

##### xsl/pretext-runestone.xsl

```diff
@@ -210,31 +210,17 @@
           <!-- no .python3 -->
           <!-- no .jobehost -->
           <!-- no .proxyuri_runs -->
           <!-- no .proxyuri_files -->
           <!-- no .enable_chatcodes -->
         </script>
         <xsl:text/>
-        <!-- Google Ads: only on Runestone server, only visible in -->
-        <!-- *non-login* versions of books hosted at Runestone     -->
-        <!--                                                       -->
-        <!-- @data-ad-client attribute of upcoming script tag is   -->
-        <!-- templated for Runestone serving.  We form it as a     -->
-        <!-- variable, so that we can place it using an XSL AVT    -->
-        <xsl:variable name="id-attr">
-          <xsl:value-of select="$rso"/>
-          <xsl:text>settings.adsenseid</xsl:text>
-          <xsl:value-of select="$rsc"/>
-        </xsl:variable>
-        <!--  -->
-        <xsl:text/>
-        <xsl:text>{% if serve_ad and settings.adsenseid %}</xsl:text>
-        <script data-ad-client="{$id-attr}" async="" src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"/>
-        <xsl:text/>
-        <xsl:text>{% endif %}</xsl:text>
+        <!-- Ethical Ads: only on Runestone server, only visible in -->
+        <!-- *non-login* versions of books hosted at Runestone      -->
+        <script src="https://media.ethicalads.io/media/client/ethicalads.min.js"/>
         <!-- We only show the Runestone "bust" menu icon if we are building        -->
         <!-- for a Runestone server, so this CSS is only needed in that case.      -->
         <!-- Perhaps it should exist in Runestone's CSS or maybe in PreTeXt's CSS? -->
         <style>
           <xsl:text>.dropdown {</xsl:text>
           <xsl:text>position: relative;</xsl:text>
           <xsl:text>display: inline-block;</xsl:text>
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -6604,14 +6604,15 @@
               <!-- responsive videos they grow to be much bigger -->
               <div id="ptx-content" class="ptx-content" style="max-width: 1600px">
                 <!-- This is content passed in as a parameter -->
                 <xsl:copy-of select="$content"/>
               </div>
             </main>
           </div>
+          <xsl:call-template name="runestone-ethical-ads"/>
           <!-- analytics services, if requested -->
           <xsl:call-template name="statcounter"/>
           <xsl:call-template name="google-classic"/>
           <xsl:call-template name="google-universal"/>
           <xsl:call-template name="google-gst"/>
           <xsl:call-template name="extra-js-footer"/>
         </body>
@@ -10120,14 +10121,15 @@
           <!-- formerly "extra" -->
           <div id="ptx-page-footer" class="ptx-page-footer">
             <xsl:apply-templates select="." mode="feedback-button"/>
             <xsl:call-template name="pretext-link"/>
             <xsl:call-template name="runestone-link"/>
             <xsl:call-template name="mathjax-link"/>
           </div>
+          <xsl:call-template name="runestone-ethical-ads"/>
           <!-- analytics services, if requested -->
           <xsl:call-template name="statcounter"/>
           <xsl:call-template name="google-classic"/>
           <xsl:call-template name="google-universal"/>
           <xsl:call-template name="google-gst"/>
           <xsl:call-template name="aim-login-footer"/>
           <xsl:call-template name="extra-js-footer"/>
@@ -11578,14 +11580,24 @@
     </a>
   </xsl:template>
   <xsl:template name="mathjax-link">
     <a class="mathjax-link" href="https://www.mathjax.org" title="MathJax">
       <img class="logo" src="https://www.mathjax.org/badge/badge-square-2.png"/>
     </a>
   </xsl:template>
+  <!-- Runestone build only, revenue generator -->
+  <xsl:template name="runestone-ethical-ads">
+    <xsl:if test="$b-host-runestone">
+      <xsl:text>{% if show_ethical_ad %}</xsl:text>
+      <div style="width: 100%">
+        <div data-ea-publisher="runestoneacademy" data-ea-type="image" style="display: flex; justify-content: center"/>
+      </div>
+      <xsl:text>{% endif %}</xsl:text>
+    </xsl:if>
+  </xsl:template>
   <!-- Tooltip Text -->
   <!-- Text for an HTML "title" attribute      -->
   <!-- Always leverage the PreTeXt title, e.g. -->
   <!-- don't use "caption", it could be BIG    -->
   <xsl:template match="*" mode="tooltip-text">
     <xsl:apply-templates select="." mode="type-name"/>
     <xsl:variable name="num">
```

### Comparing `pretext-1.5.4.dev20230522/pretext/generate.py` & `pretext-1.5.4.dev20230523/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/project.py` & `pretext-1.5.4.dev20230523/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/__init__.py` & `pretext-1.5.4.dev20230523/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/.gitignore` & `pretext-1.5.4.dev20230523/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/article.zip` & `pretext-1.5.4.dev20230523/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/
--rw-r--r--  2.0 unx       86 b- defN 23-May-22 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-22 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-22 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-22 06:18 .gitignore
--rw-r--r--  2.0 unx   154806 b- defN 23-May-22 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     2059 b- defN 23-May-22 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-May-22 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-May-22 06:18 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-May-22 06:18 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-May-22 06:18 source/section-2.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/
+-rw-r--r--  2.0 unx       86 b- defN 23-May-23 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-23 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-23 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-23 06:18 .gitignore
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-23 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-23 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-May-23 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-May-23 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      449 b- defN 23-May-23 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-May-23 06:18 source/section-2.ptx
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/book.zip` & `pretext-1.5.4.dev20230523/pretext/templates/resources/book.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-22 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-22 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-22 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-22 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6114 b- defN 23-May-22 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-May-22 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-23 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-23 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-23 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-23 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-23 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-May-23 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-May-23 06:18 source/main.ptx
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/demo.zip` & `pretext-1.5.4.dev20230523/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/
--rw-r--r--  2.0 unx       82 b- defN 23-May-22 06:18 README.md
--rw-r--r--  2.0 unx     1710 b- defN 23-May-22 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-22 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-22 06:18 .gitignore
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-May-22 06:18 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-May-22 06:18 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     2059 b- defN 23-May-22 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx     6092 b- defN 23-May-22 06:18 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/images/
--rw-r--r--  2.0 unx      847 b- defN 23-May-22 06:18 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-May-22 06:18 source/main.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-May-22 06:18 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-May-22 06:18 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-May-22 06:18 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-May-22 06:18 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-May-22 06:18 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-May-22 06:18 source/frontmatter.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-May-22 06:18 source/ch-features.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-May-22 06:18 source/ch-generate.ptx
--rw-r--r--  2.0 unx      867 b- defN 23-May-22 06:18 source/sec-features.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-May-22 06:18 source/backmatter.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-May-22 06:18 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-May-22 06:18 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-May-22 06:18 source/ex-first.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-May-22 06:18 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-May-22 06:18 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-May-22 06:18 source/images/cflag.asy
--rw-r--r--  2.0 unx      357 b- defN 23-May-22 06:18 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-May-22 06:18 source/images/sageplot3d.sage
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/
+-rw-r--r--  2.0 unx       82 b- defN 23-May-23 06:18 README.md
+-rw-r--r--  2.0 unx     1710 b- defN 23-May-23 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-23 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-23 06:18 .gitignore
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-May-23 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-May-23 06:18 assets/jsxgraph/infinity.js
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-23 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-May-23 06:18 publication/publication.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/images/
+-rw-r--r--  2.0 unx      847 b- defN 23-May-23 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-23 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-May-23 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      375 b- defN 23-May-23 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-May-23 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-May-23 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-May-23 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-May-23 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-May-23 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-May-23 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-May-23 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-May-23 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-May-23 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-May-23 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-May-23 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-May-23 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx       10 b- defN 23-May-23 06:18 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-May-23 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-May-23 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       93 b- defN 23-May-23 06:18 source/images/sageplot3d.sage
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/devcontainer.json` & `pretext-1.5.4.dev20230523/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/hello.zip` & `pretext-1.5.4.dev20230523/pretext/templates/resources/hello.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/
--rw-r--r--  2.0 unx       69 b- defN 23-May-22 06:18 README.md
--rw-r--r--  2.0 unx     1217 b- defN 23-May-22 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-22 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-22 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-22 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      242 b- defN 23-May-22 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-May-22 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/
+-rw-r--r--  2.0 unx       69 b- defN 23-May-23 06:18 README.md
+-rw-r--r--  2.0 unx     1217 b- defN 23-May-23 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-23 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-23 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-23 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-May-23 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-May-23 06:18 source/main.ptx
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/project.ptx` & `pretext-1.5.4.dev20230523/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pretext/templates/resources/slideshow.zip` & `pretext-1.5.4.dev20230523/pretext/templates/resources/slideshow.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-22 06:18 xsl/
--rw-r--r--  2.0 unx      784 b- defN 23-May-22 06:18 project.ptx
--rw-r--r--  2.0 unx     2268 b- defN 23-May-22 06:18 codechat_config.yaml
--rw-r--r--  2.0 unx     1676 b- defN 23-May-22 06:18 .gitignore
--rw-r--r--  2.0 unx     2059 b- defN 23-May-22 06:18 .devcontainer/devcontainer.json
--rw-r--r--  2.0 unx      190 b- defN 23-May-22 06:18 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-May-22 06:18 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-May-22 06:18 source/main.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-23 06:18 xsl/
+-rw-r--r--  2.0 unx      784 b- defN 23-May-23 06:18 project.ptx
+-rw-r--r--  2.0 unx     2268 b- defN 23-May-23 06:18 codechat_config.yaml
+-rw-r--r--  2.0 unx     1676 b- defN 23-May-23 06:18 .gitignore
+-rw-r--r--  2.0 unx     2059 b- defN 23-May-23 06:18 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      190 b- defN 23-May-23 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2097 b- defN 23-May-23 06:18 publication/publication.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-May-23 06:18 source/main.ptx
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

### Comparing `pretext-1.5.4.dev20230522/pretext/utils.py` & `pretext-1.5.4.dev20230523/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.5.4.dev20230522/pyproject.toml` & `pretext-1.5.4.dev20230523/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.5.4.dev20230522"
+version = "1.5.4.dev20230523"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.5.4.dev20230522/PKG-INFO` & `pretext-1.5.4.dev20230523/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.5.4.dev20230522
+Version: 1.5.4.dev20230523
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

