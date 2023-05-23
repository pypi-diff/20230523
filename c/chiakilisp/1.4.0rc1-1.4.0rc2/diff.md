# Comparing `tmp/chiakilisp-1.4.0rc1-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 26618 bytes, number of entries: 19
+Zip file size: 26615 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
 -rw-r--r--  2.0 unx    13791 b- defN 23-May-19 18:36 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
 -rw-r--r--  2.0 unx     3311 b- defN 23-May-15 20:31 chiakilisp/utils.py
 -rw-r--r--  2.0 unx     7173 b- defN 23-May-23 15:25 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
 -rw-r--r--  2.0 unx    30784 b- defN 23-May-19 18:35 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
 -rw-r--r--  2.0 unx     3778 b- defN 23-May-15 20:32 chiakilisp/models/literal.py
 -rw-r--r--  2.0 unx     1986 b- defN 23-May-15 20:31 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    12909 b- defN 23-May-23 18:17 chiakilisp-1.4.0rc1.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-23 18:17 chiakilisp-1.4.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-23 18:17 chiakilisp-1.4.0rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-23 18:17 chiakilisp-1.4.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-23 18:17 chiakilisp-1.4.0rc1.dist-info/RECORD
-19 files, 96343 bytes uncompressed, 24070 bytes compressed:  75.0%
+-rwxr-xr-x  2.0 unx    12909 b- defN 23-May-23 18:40 chiakilisp-1.4.0rc2.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-23 18:40 chiakilisp-1.4.0rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 18:40 chiakilisp-1.4.0rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-23 18:40 chiakilisp-1.4.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-23 18:40 chiakilisp-1.4.0rc2.dist-info/RECORD
+19 files, 96343 bytes uncompressed, 24067 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc1.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc2.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc1.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc1.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc1.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc1.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `chiakilisp-1.4.0rc1.data/scripts/chiakilang` & `chiakilisp-1.4.0rc2.data/scripts/chiakilang`

 * *Files identical despite different names*

## Comparing `chiakilisp-1.4.0rc1.dist-info/METADATA` & `chiakilisp-1.4.0rc2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc1
+Version: 1.4.0rc2
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
 Project-URL: Web Site, https://chiakilisp.jedi2light.moe
 Project-URL: Source, https://gitlab.com/jedi2light/chiakilisp.git
 Project-URL: Bug Tracker, https://gitlab.com/jedi2light/chiakilisp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Requires-Dist: hashedcolls (==1.1.0)
+Requires-Dist: hashedcolls (==1.1.1)
 
 # ChiakiLisp - Yet another LISP
 
 ## Demo
 
 ![alt Fujisaki Demo](demos/fujisaki.png)
```

## Comparing `chiakilisp-1.4.0rc1.dist-info/RECORD` & `chiakilisp-1.4.0rc2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/models/expression.py,sha256=xoOR1QQhTq19KwlVRmaedJnUL0u3Aqo5wwIk-eCBvTw,30784
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
 chiakilisp/models/literal.py,sha256=0m0FRZ9YLq23pH_DKjSSObey5gZIo73BUJP37F5svsA,3778
 chiakilisp/models/token.py,sha256=TYfdqCVn3_74aBCn6m5gPikjpwixUW65FeKrMLuvpvE,1986
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc1.data/scripts/chiakilang,sha256=kv-yjMEWm0XIoCB2DjaLrvLHX_lobI_IhZywiLuHYvM,12909
-chiakilisp-1.4.0rc1.dist-info/METADATA,sha256=UIS_X2R4PNdB1g31aL0dsI6phRWTPXId_-tbQbahIXk,1408
-chiakilisp-1.4.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc1.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc1.dist-info/RECORD,,
+chiakilisp-1.4.0rc2.data/scripts/chiakilang,sha256=kv-yjMEWm0XIoCB2DjaLrvLHX_lobI_IhZywiLuHYvM,12909
+chiakilisp-1.4.0rc2.dist-info/METADATA,sha256=fsIKRWeZ58tfAvfzdrWu21RznAlynProlaVPmdlRMR8,1408
+chiakilisp-1.4.0rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc2.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc2.dist-info/RECORD,,
```

