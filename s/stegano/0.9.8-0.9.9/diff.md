# Comparing `tmp/stegano-0.9.8.tar.gz` & `tmp/stegano-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stegano-0.9.8.tar", last modified: Fri Dec 20 08:43:48 2019, max compression
+gzip compressed data, was "stegano-0.9.9.tar", max compression
```

## Comparing `stegano-0.9.8.tar` & `stegano-0.9.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     6918 2019-12-15 14:52:01.879316 stegano-0.9.8/CHANGELOG.md
--rwxr-xr-x   0        0        0    35146 2015-12-23 12:14:16.863041 stegano-0.9.8/COPYING
--rw-r--r--   0        0        0     2674 2019-12-15 20:52:51.365896 stegano-0.9.8/README.md
--rw-r--r--   0        0        0        1 2019-12-20 07:52:38.783541 stegano-0.9.8/bin/__init__.py
--rwxr-xr-x   0        0        0     4377 2019-12-20 07:52:38.783541 stegano-0.9.8/bin/lsb.py
--rwxr-xr-x   0        0        0     7252 2019-12-20 07:52:38.783541 stegano-0.9.8/bin/lsbset.py
--rw-r--r--   0        0        0     1704 2019-12-20 08:11:50.874148 stegano-0.9.8/bin/parity.py
--rw-r--r--   0        0        0     2195 2019-12-20 08:11:20.590738 stegano-0.9.8/bin/red.py
--rw-r--r--   0        0        0     1710 2019-12-20 08:12:09.585786 stegano-0.9.8/bin/statistics.py
--rw-r--r--   0        0        0     5560 2015-12-23 12:14:16.863041 stegano-0.9.8/docs/Makefile
--rw-r--r--   0        0        0    11803 2018-02-28 21:52:20.371297 stegano-0.9.8/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0    16064 2019-12-15 14:51:44.715260 stegano-0.9.8/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0     3577 2019-12-15 14:51:44.715260 stegano-0.9.8/docs/_build/doctrees/installation.doctree
--rw-r--r--   0        0        0     9995 2019-12-15 14:51:44.715260 stegano-0.9.8/docs/_build/doctrees/module.doctree
--rw-r--r--   0        0        0    19366 2018-02-28 21:52:20.367297 stegano-0.9.8/docs/_build/doctrees/software.doctree
--rw-r--r--   0        0        0     3690 2018-02-28 21:52:20.371297 stegano-0.9.8/docs/_build/doctrees/steganalysis.doctree
--rw-r--r--   0        0        0    16835 2019-12-15 14:51:44.715260 stegano-0.9.8/docs/_build/doctrees/tutorial.doctree
--rw-r--r--   0        0        0      230 2018-02-28 21:52:20.763292 stegano-0.9.8/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0     2942 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/_sources/index.txt
--rw-r--r--   0        0        0      442 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/_sources/installation.txt
--rw-r--r--   0        0        0     3425 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/_sources/module.txt
--rw-r--r--   0        0        0     6859 2017-05-18 12:59:08.892334 stegano-0.9.8/docs/_build/html/_sources/software.txt
--rw-r--r--   0        0        0      633 2017-05-07 12:23:30.985410 stegano-0.9.8/docs/_build/html/_sources/steganalysis.txt
--rw-r--r--   0        0        0     5385 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/_sources/tutorial.txt
--rw-r--r--   0        0        0      673 2016-06-19 19:51:37.627984 stegano-0.9.8/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0        0        0       87 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/background_b01.png
--rw-r--r--   0        0        0     9633 2018-02-28 21:52:20.683293 stegano-0.9.8/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0     9570 2018-02-28 21:52:20.755292 stegano-0.9.8/docs/_build/html/_static/bizstyle.css
--rw-r--r--   0        0        0     1179 2018-02-28 21:52:20.735292 stegano-0.9.8/docs/_build/html/_static/bizstyle.js
--rw-r--r--   0        0        0     3500 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0        0        0     3578 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/comment-close.png
--rw-r--r--   0        0        0     3445 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/comment.png
--rw-r--r--   0        0        0    14939 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/css3-mediaqueries.js
--rw-r--r--   0        0        0    28629 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/css3-mediaqueries_src.js
--rw-r--r--   0        0        0     8166 2018-02-28 21:52:20.731292 stegano-0.9.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      347 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0        0        0      347 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/down.png
--rw-r--r--   0        0        0      358 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0   282766 2016-06-19 19:51:37.631984 stegano-0.9.8/docs/_build/html/_static/jquery-1.11.1.js
--rw-r--r--   0        0        0    95786 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/jquery.js
--rw-r--r--   0        0        0      173 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0      173 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     4149 2018-02-28 21:52:20.623294 stegano-0.9.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18862 2018-02-28 21:52:20.727292 stegano-0.9.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0    35168 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0        0        0    12140 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/underscore.js
--rw-r--r--   0        0        0      345 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0        0        0      345 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/up.png
--rw-r--r--   0        0        0    25351 2016-06-19 19:51:37.635984 stegano-0.9.8/docs/_build/html/_static/websupport.js
--rw-r--r--   0        0        0    10150 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/index.html
--rw-r--r--   0        0        0     4788 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/installation.html
--rw-r--r--   0        0        0    18803 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/module.html
--rw-r--r--   0        0        0      311 2018-02-28 21:52:20.767292 stegano-0.9.8/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     3306 2018-02-28 21:52:20.623294 stegano-0.9.8/docs/_build/html/search.html
--rw-r--r--   0        0        0     3337 2018-02-28 21:52:20.767292 stegano-0.9.8/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0    16499 2018-02-28 21:52:20.603294 stegano-0.9.8/docs/_build/html/software.html
--rw-r--r--   0        0        0     4785 2018-02-28 21:52:20.615294 stegano-0.9.8/docs/_build/html/steganalysis.html
--rw-r--r--   0        0        0    14747 2019-12-15 14:51:44.711260 stegano-0.9.8/docs/_build/html/tutorial.html
--rw-r--r--   0        0        0     7740 2019-01-26 16:23:49.956695 stegano-0.9.8/docs/conf.py
--rw-r--r--   0        0        0     2322 2019-10-27 21:11:57.715328 stegano-0.9.8/docs/index.rst
--rw-r--r--   0        0        0      404 2019-12-14 14:32:31.418471 stegano-0.9.8/docs/installation.rst
--rw-r--r--   0        0        0     5094 2015-12-23 12:14:16.863041 stegano-0.9.8/docs/make.bat
--rw-r--r--   0        0        0     3425 2019-10-27 21:12:19.930913 stegano-0.9.8/docs/module.rst
--rw-r--r--   0        0        0     7285 2019-01-26 16:23:49.964695 stegano-0.9.8/docs/software.rst
--rw-r--r--   0        0        0      633 2017-05-07 12:23:30.985410 stegano-0.9.8/docs/steganalysis.rst
--rw-r--r--   0        0        0     1421 2019-12-20 08:43:46.478679 stegano-0.9.8/pyproject.toml
--rwxr-xr-x   0        0        0      157 2019-06-07 20:49:24.812153 stegano-0.9.8/stegano/__init__.py
--rw-r--r--   0        0        0       73 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/exifHeader/__init__.py
--rw-r--r--   0        0        0     4740 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/exifHeader/exifHeader.py
--rw-r--r--   0        0        0       66 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/lsb/__init__.py
--rwxr-xr-x   0        0        0     4529 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/lsb/lsb.py
--rw-r--r--   0        0        0       69 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/lsbset/__init__.py
--rw-r--r--   0        0        0     5440 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/lsbset/generators.py
--rw-r--r--   0        0        0     4395 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/lsbset/lsbset.py
--rw-r--r--   0        0        0       66 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/red/__init__.py
--rwxr-xr-x   0        0        0     2996 2019-12-15 14:52:10.711344 stegano-0.9.8/stegano/red/red.py
--rw-r--r--   0        0        0       95 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/steganalysis/__init__.py
--rw-r--r--   0        0        0     1700 2019-12-15 14:52:10.711344 stegano-0.9.8/stegano/steganalysis/parity.py
--rw-r--r--   0        0        0     1889 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/steganalysis/statistics.py
--rwxr-xr-x   0        0        0     3741 2019-12-20 07:52:38.787541 stegano-0.9.8/stegano/tools.py
--rw-r--r--   0        0        0     3949 2019-12-20 08:43:48.916878 stegano-0.9.8/setup.py
--rw-r--r--   0        0        0     3750 2019-12-20 08:43:48.917277 stegano-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     7076 2021-07-02 21:53:22.805073 stegano-0.9.9/CHANGELOG.md
+-rwxr-xr-x   0        0        0    35146 2015-12-23 12:14:16.863041 stegano-0.9.9/COPYING
+-rw-r--r--   0        0        0     2670 2021-02-04 16:14:43.522481 stegano-0.9.9/README.md
+-rw-r--r--   0        0        0        1 2019-12-20 07:52:38.783541 stegano-0.9.9/bin/__init__.py
+-rwxr-xr-x   0        0        0     4377 2021-02-06 22:02:38.618874 stegano-0.9.9/bin/lsb.py
+-rwxr-xr-x   0        0        0     7252 2021-02-06 22:02:38.618874 stegano-0.9.9/bin/lsbset.py
+-rw-r--r--   0        0        0     1704 2021-02-06 22:02:38.618874 stegano-0.9.9/bin/parity.py
+-rw-r--r--   0        0        0     2195 2021-02-06 22:02:38.618874 stegano-0.9.9/bin/red.py
+-rw-r--r--   0        0        0     1710 2021-02-06 22:02:38.618874 stegano-0.9.9/bin/statistics.py
+-rw-r--r--   0        0        0     5560 2015-12-23 12:14:16.863041 stegano-0.9.9/docs/Makefile
+-rw-r--r--   0        0        0    11803 2018-02-28 21:52:20.371297 stegano-0.9.9/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0    16064 2019-12-15 14:51:44.715260 stegano-0.9.9/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0     3577 2019-12-15 14:51:44.715260 stegano-0.9.9/docs/_build/doctrees/installation.doctree
+-rw-r--r--   0        0        0     9995 2019-12-15 14:51:44.715260 stegano-0.9.9/docs/_build/doctrees/module.doctree
+-rw-r--r--   0        0        0    19366 2018-02-28 21:52:20.367297 stegano-0.9.9/docs/_build/doctrees/software.doctree
+-rw-r--r--   0        0        0     3690 2018-02-28 21:52:20.371297 stegano-0.9.9/docs/_build/doctrees/steganalysis.doctree
+-rw-r--r--   0        0        0    16835 2019-12-15 14:51:44.715260 stegano-0.9.9/docs/_build/doctrees/tutorial.doctree
+-rw-r--r--   0        0        0      230 2018-02-28 21:52:20.763292 stegano-0.9.9/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0     2942 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/_sources/index.txt
+-rw-r--r--   0        0        0      442 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/_sources/installation.txt
+-rw-r--r--   0        0        0     3425 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/_sources/module.txt
+-rw-r--r--   0        0        0     6859 2017-05-18 12:59:08.892334 stegano-0.9.9/docs/_build/html/_sources/software.txt
+-rw-r--r--   0        0        0      633 2017-05-07 12:23:30.985410 stegano-0.9.9/docs/_build/html/_sources/steganalysis.txt
+-rw-r--r--   0        0        0     5385 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/_sources/tutorial.txt
+-rw-r--r--   0        0        0      673 2016-06-19 19:51:37.627984 stegano-0.9.9/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0        0        0       87 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/background_b01.png
+-rw-r--r--   0        0        0     9633 2018-02-28 21:52:20.683293 stegano-0.9.9/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0     9570 2018-02-28 21:52:20.755292 stegano-0.9.9/docs/_build/html/_static/bizstyle.css
+-rw-r--r--   0        0        0     1179 2018-02-28 21:52:20.735292 stegano-0.9.9/docs/_build/html/_static/bizstyle.js
+-rw-r--r--   0        0        0     3500 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0        0        0     3578 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0        0        0     3445 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/comment.png
+-rw-r--r--   0        0        0    14939 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/css3-mediaqueries.js
+-rw-r--r--   0        0        0    28629 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/css3-mediaqueries_src.js
+-rw-r--r--   0        0        0     8166 2018-02-28 21:52:20.731292 stegano-0.9.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      347 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0        0        0      347 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/down.png
+-rw-r--r--   0        0        0      358 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0   282766 2016-06-19 19:51:37.631984 stegano-0.9.9/docs/_build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0        0        0    95786 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/jquery.js
+-rw-r--r--   0        0        0      173 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0      173 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     4149 2018-02-28 21:52:20.623294 stegano-0.9.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18862 2018-02-28 21:52:20.727292 stegano-0.9.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0    35168 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0        0        0    12140 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/underscore.js
+-rw-r--r--   0        0        0      345 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0        0        0      345 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/up.png
+-rw-r--r--   0        0        0    25351 2016-06-19 19:51:37.635984 stegano-0.9.9/docs/_build/html/_static/websupport.js
+-rw-r--r--   0        0        0    10150 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/index.html
+-rw-r--r--   0        0        0     4788 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/installation.html
+-rw-r--r--   0        0        0    18803 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/module.html
+-rw-r--r--   0        0        0      311 2018-02-28 21:52:20.767292 stegano-0.9.9/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     3306 2018-02-28 21:52:20.623294 stegano-0.9.9/docs/_build/html/search.html
+-rw-r--r--   0        0        0     3337 2018-02-28 21:52:20.767292 stegano-0.9.9/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0    16499 2018-02-28 21:52:20.603294 stegano-0.9.9/docs/_build/html/software.html
+-rw-r--r--   0        0        0     4785 2018-02-28 21:52:20.615294 stegano-0.9.9/docs/_build/html/steganalysis.html
+-rw-r--r--   0        0        0    14747 2019-12-15 14:51:44.711260 stegano-0.9.9/docs/_build/html/tutorial.html
+-rw-r--r--   0        0        0     5916 2021-04-10 09:44:09.374251 stegano-0.9.9/docs/conf.py
+-rw-r--r--   0        0        0     2222 2021-04-10 09:47:26.698733 stegano-0.9.9/docs/index.rst
+-rw-r--r--   0        0        0      402 2021-04-10 09:47:45.690403 stegano-0.9.9/docs/installation.rst
+-rw-r--r--   0        0        0     5094 2015-12-23 12:14:16.863041 stegano-0.9.9/docs/make.bat
+-rw-r--r--   0        0        0     3423 2021-04-10 09:48:17.321855 stegano-0.9.9/docs/module.rst
+-rw-r--r--   0        0        0     7275 2021-04-10 09:48:22.349769 stegano-0.9.9/docs/software.rst
+-rw-r--r--   0        0        0      633 2021-04-10 09:48:43.973397 stegano-0.9.9/docs/steganalysis.rst
+-rw-r--r--   0        0        0     1477 2021-07-02 21:53:44.192715 stegano-0.9.9/pyproject.toml
+-rwxr-xr-x   0        0        0      157 2019-06-07 20:49:24.812153 stegano-0.9.9/stegano/__init__.py
+-rw-r--r--   0        0        0       73 2019-12-20 07:52:38.787541 stegano-0.9.9/stegano/exifHeader/__init__.py
+-rw-r--r--   0        0        0     4740 2021-02-06 22:02:38.618874 stegano-0.9.9/stegano/exifHeader/exifHeader.py
+-rw-r--r--   0        0        0       66 2019-12-20 07:52:38.787541 stegano-0.9.9/stegano/lsb/__init__.py
+-rwxr-xr-x   0        0        0     4529 2021-02-06 22:02:38.418867 stegano-0.9.9/stegano/lsb/lsb.py
+-rw-r--r--   0        0        0       69 2019-12-20 07:52:38.787541 stegano-0.9.9/stegano/lsbset/__init__.py
+-rw-r--r--   0        0        0     5440 2021-02-06 22:02:38.618874 stegano-0.9.9/stegano/lsbset/generators.py
+-rw-r--r--   0        0        0     4395 2021-02-06 22:02:38.618874 stegano-0.9.9/stegano/lsbset/lsbset.py
+-rw-r--r--   0        0        0       66 2019-12-20 07:52:38.787541 stegano-0.9.9/stegano/red/__init__.py
+-rwxr-xr-x   0        0        0     2996 2021-02-06 22:02:38.418867 stegano-0.9.9/stegano/red/red.py
+-rw-r--r--   0        0        0       95 2019-12-20 07:52:38.787541 stegano-0.9.9/stegano/steganalysis/__init__.py
+-rw-r--r--   0        0        0     1700 2021-02-06 22:02:38.618874 stegano-0.9.9/stegano/steganalysis/parity.py
+-rw-r--r--   0        0        0     1889 2021-02-06 22:02:38.618874 stegano-0.9.9/stegano/steganalysis/statistics.py
+-rwxr-xr-x   0        0        0     3741 2021-02-06 22:02:38.418867 stegano-0.9.9/stegano/tools.py
+-rw-r--r--   0        0        0     3941 2021-07-02 21:57:18.347592 stegano-0.9.9/setup.py
+-rw-r--r--   0        0        0     3792 2021-07-02 21:57:18.347935 stegano-0.9.9/PKG-INFO
```

### Comparing `stegano-0.9.8/CHANGELOG.md` & `stegano-0.9.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 ## Release History
 
 
+### 0.9.9 (2021-07-02)
+
+* stegano now uses Pillow 8.3.0.
+
+
+### 0.9.8 (2019-12-20)
+
+* stegano is now using poetry;
+* minor improvements to the command line.
+
+
 ### 0.9.7 (2019-10-27)
 
-* fixed markdown of the previous release;
+* fixed markdown of the previous release.
 
 
 ### 0.9.6 (2019-10-27)
 
 * fixed markdown of the previous release;
```

### Comparing `stegano-0.9.8/COPYING` & `stegano-0.9.9/COPYING`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/README.md` & `stegano-0.9.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Stegano
 
 [![builds.sr.ht status](https://builds.sr.ht/~cedric/stegano.svg)](https://builds.sr.ht/~cedric/stegano)
 
 
-[Stegano](https://git.sr.ht/~cedric/stegano), a pure Python Steganography
+[Stegano](https://sr.ht/~cedric/stegano), a pure Python Steganography
 module.
 
 Steganography is the art and science of writing hidden messages in such a way
 that no one, apart from the sender and intended recipient, suspects the
 existence of the message, a form of security through obscurity. Consequently,
 functions provided by Stegano only hide messages, without encryption.
 Steganography is often used with cryptography.
@@ -16,23 +16,23 @@
 https://todo.sr.ht/~cedric/stegano
 
 
 ## Installation
 
 
 ```bash
-$ poetry install Stegano
+$ poetry install stegano
 ```
 
 You will be able to use Stegano in your Python programs.
 
 If you only want to install Stegano as a command line tool:
 
 ```bash
-$ pipx install Stegano
+$ pipx install stegano
 ```
 
 pipx installs scripts (system wide available) provided by Python packages into
 separate virtualenvs to shield them from your system and each other.
 
 
 ## Usage
@@ -98,10 +98,10 @@
 
 
 ## License
 
 This software is licensed under
 [GNU General Public License version 3](https://www.gnu.org/licenses/gpl-3.0.html)
 
-Copyright (C) 2010-2019 [Cédric Bonhomme](https://www.cedricbonhomme.org)
+Copyright (C) 2010-2021 [Cédric Bonhomme](https://www.cedricbonhomme.org)
 
 For more information, [the list of authors and contributors](CONTRIBUTORS.md) is available.
```

### Comparing `stegano-0.9.8/bin/lsb.py` & `stegano-0.9.9/bin/lsb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://github.com/cedricbonhomme/Stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/bin/lsbset.py` & `stegano-0.9.9/bin/lsbset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://github.com/cedricbonhomme/Stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/bin/parity.py` & `stegano-0.9.9/bin/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://github.com/cedricbonhomme/Stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -15,32 +15,34 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
-__author__ = "Cedric Bonhomme"
-__version__ = "$Revision: 0.7 $"
-__date__ = "$Date: 2016/08/25 $"
+__author__ = "Cédric Bonhomme"
+__version__ = "$Revision: 0.1 $"
+__date__ = "$Date: 2016/08/26 $"
+__revision__ = "$Date: 2016/08/26 $"
 __license__ = "GPLv3"
 
 from PIL import Image
 
 import argparse
 
 try:
-    from stegano.steganalysis import parity
+    from stegano.steganalysis import statistics
 except:
-    print("Install Stegano: pipx install Stegano")
+    print("Install Stegano: sudo pip install Stegano")
+
 
 def main():
     parser = argparse.ArgumentParser(prog='stegano-steganalysis-parity')
     parser.add_argument("-i", "--input", dest="input_image_file",
-                    required=True, help="Input image file.")
+                    help="Image file")
     parser.add_argument("-o", "--output", dest="output_image_file",
-                    required=True, help="Output image file.")
+                    help="Image file")
     arguments = parser.parse_args()
 
     input_image_file = Image.open(arguments.input_image_file)
-    output_image = parity.steganalyse(input_image_file)
+    output_image = statistics.steganalyse(input_image_file)
     output_image.save(arguments.output_image_file)
```

### Comparing `stegano-0.9.8/bin/red.py` & `stegano-0.9.9/bin/red.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://github.com/cedricbonhomme/Stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/bin/statistics.py` & `stegano-0.9.9/bin/parity.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://github.com/cedricbonhomme/Stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -15,34 +15,32 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
-__author__ = "Cédric Bonhomme"
-__version__ = "$Revision: 0.1 $"
-__date__ = "$Date: 2016/08/26 $"
-__revision__ = "$Date: 2016/08/26 $"
+__author__ = "Cedric Bonhomme"
+__version__ = "$Revision: 0.7 $"
+__date__ = "$Date: 2016/08/25 $"
 __license__ = "GPLv3"
 
 from PIL import Image
 
 import argparse
 
 try:
-    from stegano.steganalysis import statistics
+    from stegano.steganalysis import parity
 except:
-    print("Install Stegano: sudo pip install Stegano")
-
+    print("Install Stegano: pipx install Stegano")
 
 def main():
     parser = argparse.ArgumentParser(prog='stegano-steganalysis-parity')
     parser.add_argument("-i", "--input", dest="input_image_file",
-                    help="Image file")
+                    required=True, help="Input image file.")
     parser.add_argument("-o", "--output", dest="output_image_file",
-                    help="Image file")
+                    required=True, help="Output image file.")
     arguments = parser.parse_args()
 
     input_image_file = Image.open(arguments.input_image_file)
-    output_image = statistics.steganalyse(input_image_file)
+    output_image = parity.steganalyse(input_image_file)
     output_image.save(arguments.output_image_file)
```

### Comparing `stegano-0.9.8/docs/Makefile` & `stegano-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/environment.pickle` & `stegano-0.9.9/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/index.doctree` & `stegano-0.9.9/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/installation.doctree` & `stegano-0.9.9/docs/_build/doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/module.doctree` & `stegano-0.9.9/docs/_build/doctrees/module.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/software.doctree` & `stegano-0.9.9/docs/_build/doctrees/software.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/steganalysis.doctree` & `stegano-0.9.9/docs/_build/doctrees/steganalysis.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/doctrees/tutorial.doctree` & `stegano-0.9.9/docs/_build/doctrees/tutorial.doctree`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_sources/index.txt` & `stegano-0.9.9/docs/_build/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_sources/module.txt` & `stegano-0.9.9/docs/_build/html/_sources/module.txt`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_sources/software.txt` & `stegano-0.9.9/docs/_build/html/_sources/software.txt`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_sources/steganalysis.txt` & `stegano-0.9.9/docs/_build/html/_sources/steganalysis.txt`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_sources/tutorial.txt` & `stegano-0.9.9/docs/_build/html/_sources/tutorial.txt`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/ajax-loader.gif` & `stegano-0.9.9/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/basic.css` & `stegano-0.9.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/bizstyle.css` & `stegano-0.9.9/docs/_build/html/_static/bizstyle.css`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/bizstyle.js` & `stegano-0.9.9/docs/_build/html/_static/bizstyle.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/comment-bright.png` & `stegano-0.9.9/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/comment-close.png` & `stegano-0.9.9/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/comment.png` & `stegano-0.9.9/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/css3-mediaqueries.js` & `stegano-0.9.9/docs/_build/html/_static/css3-mediaqueries.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/css3-mediaqueries_src.js` & `stegano-0.9.9/docs/_build/html/_static/css3-mediaqueries_src.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/doctools.js` & `stegano-0.9.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/jquery-1.11.1.js` & `stegano-0.9.9/docs/_build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/jquery.js` & `stegano-0.9.9/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/pygments.css` & `stegano-0.9.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/searchtools.js` & `stegano-0.9.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/underscore-1.3.1.js` & `stegano-0.9.9/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/underscore.js` & `stegano-0.9.9/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/_static/websupport.js` & `stegano-0.9.9/docs/_build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/index.html` & `stegano-0.9.9/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/installation.html` & `stegano-0.9.9/docs/_build/html/installation.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/module.html` & `stegano-0.9.9/docs/_build/html/module.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/search.html` & `stegano-0.9.9/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/searchindex.js` & `stegano-0.9.9/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/software.html` & `stegano-0.9.9/docs/_build/html/software.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/steganalysis.html` & `stegano-0.9.9/docs/_build/html/steganalysis.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/_build/html/tutorial.html` & `stegano-0.9.9/docs/_build/html/tutorial.html`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/conf.py` & `stegano-0.9.9/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,24 +37,25 @@
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = u'Stegano'
-copyright = u'2010-2019, Cédric Bonhomme'
+copyright = u'2010-2021, Cédric Bonhomme'
+author = 'Cédric Bonhomme <cedric@cedricbonhomme.org>'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.8'
+version = '0.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.8.6'
+release = '0.9.4'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -76,26 +77,23 @@
 # unit titles (such as .. function::).
 #add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 #show_authors = False
 
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
 # A list of ignored prefixes for module index sorting.
 #modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'bizstyle'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -136,17 +134,14 @@
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
 #html_additional_pages = {}
 
 # If false, no module index is generated.
 #html_domain_indices = True
 
-# If false, no index is generated.
-html_use_index = False
-
 # If true, the index is split into individual pages for each letter.
 #html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
 #html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
@@ -159,84 +154,25 @@
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
 #html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 #html_file_suffix = None
 
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'Stgandoc'
-
 
 # -- Options for LaTeX output --------------------------------------------------
 
-latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-}
+latex_engine = 'pdflatex'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
   ('index', 'Stgan.tex', u'Stegano Documentation',
-   u'Cédric Bonhomme', 'manual'),
-]
-
-# The name of an image file (relative to this directory) to place at the top of
-# the title page.
-#latex_logo = None
-
-# For "manual" documents, if this is true, then toplevel headings are parts,
-# not chapters.
-#latex_use_parts = False
-
-# If true, show page references after internal links.
-#latex_show_pagerefs = False
-
-# If true, show URL addresses after external links.
-#latex_show_urls = False
-
-# Documents to append as an appendix to all manuals.
-#latex_appendices = []
-
-# If false, no module index is generated.
-#latex_domain_indices = True
-
-
-# -- Options for manual page output --------------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    ('index', 'stgan', u'Stéganô Documentation',
-     [u'Cédric Bonhomme'], 1)
-]
-
-# If true, show URL addresses after external links.
-#man_show_urls = False
-
-
-# -- Options for Texinfo output ------------------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-  ('index', 'Stgan', u'Stegano Documentation',
-   u'Cédric Bonhomme', 'Stgan', 'One line description of project.',
-   'Miscellaneous'),
+   u'Cédric Bonhomme', 'howto'),
 ]
 
-# Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
-
-# If false, no module index is generated.
-#texinfo_domain_indices = True
+latex_show_urls = True
+latex_show_pagerefs = True
 
-# How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+ADDITIONAL_PREAMBLE = """
+\setcounter{tocdepth}{3}
+"""
```

### Comparing `stegano-0.9.8/docs/index.rst` & `stegano-0.9.9/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,27 @@
    sphinx-quickstart on Wed Jul 25 13:33:39 2012.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Presentation
 ============
 
-.. image:: https://builds.sr.ht/~cedric/Stegano.svg
-    :target: https://builds.sr.ht/~cedric/Stegano
+.. image:: https://builds.sr.ht/~cedric/stegano.svg
+    :target: https://builds.sr.ht/~cedric/stegano
 
 
 Stegano_ is a pure Python steganography_ module.
 
 Steganography is the art and science of writing hidden messages in such a way
 that no one, apart from the sender and intended recipient, suspects the
 existence of the message, a form of security through obscurity.
-Consequently, functions provided by Stéganô only hide messages,
+Consequently, functions provided by Stegano only hide messages,
 without encryption. Steganography is often used with cryptography.
 
-Stéganô implements these methods of hiding:
+Stegano implements these methods of hiding:
 
 - using the red portion of a pixel to hide ASCII messages;
 - using the `Least Significant Bit <http://en.wikipedia.org/wiki/Least_significant_bit>`_ (LSB) technique;
 - using the LSB technique with sets based on generators (Sieve for Eratosthenes, Fermat, Mersenne numbers, etc.);
 - using the description field of the image (JPEG and TIFF).
 
 Moreover some methods of steganalysis_ are provided:
@@ -49,36 +49,36 @@
 
     installation
     module
     software
     steganalysis
 
 You can have a look at the
-`unit tests <https://git.sr.ht/~cedric/Stegano/tree/master/tests>`_.
+`unit tests <https://git.sr.ht/~cedric/stegano/tree/master/tests>`_.
 
 
 License
 =======
 
 Stegano_ is under GPL v3 license.
 
 
 Donation
 ========
 
-If you wish and if you like Stegano, you can donate via bitcoin.
-My bitcoin address: `1GVmhR9fbBeEh7rP1qNq76jWArDdDQ3otZ <http://blockexplorer.com/address/1GVmhR9fbBeEh7rP1qNq76jWArDdDQ3otZ>`_
+If you wish and if you like Stegano, you can
+`donate <https://github.com/sponsors/cedricbonhomme>`_.
 
 
 
 Contact
 =======
 
 `My home page <https://www.cedricbonhomme.org>`_
 
 
 .. _Python: https://www.python.org
-.. _Stegano: https://git.sr.ht/~cedric/Stegano
+.. _Stegano: https://sr.ht/~cedric/stegano
 .. _`Pillow`: https://pypi.python.org/pypi/Pillow
 .. _`piexif`: https://pypi.python.org/pypi/piexif
 .. _steganography: http://en.wikipedia.org/wiki/Steganography
 .. _steganalysis: http://en.wikipedia.org/wiki/Steganalysis
```

### Comparing `stegano-0.9.8/docs/make.bat` & `stegano-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/docs/module.rst` & `stegano-0.9.9/docs/module.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-Using Stéganô as a Python module
+Using Stegano as a Python module
 ================================
 
 You can find more examples in the
-`unit tests directory <https://git.sr.ht/~cedric/Stegano/tree/master/tests>`_.
+`unit tests directory <https://git.sr.ht/~cedric/stegano/tree/master/tests>`_.
 
 LSB method
 ----------
 
 .. code-block:: python
 
     Python 3.5.1 (default, Dec  7 2015, 11:33:57)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `stegano-0.9.8/docs/software.rst` & `stegano-0.9.9/docs/software.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Using Stéganô in command line
+Using Stegano in command line
 =============================
 
 The command ``stegano-lsb``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Hide and reveal a message with the LSB method.
 
@@ -145,16 +145,16 @@
 (Fibonacci starts with 0, 1, 1, etc.). Or maybe you just want to add more complexity.
 In this case, simply use the optional arguments ``--shift``:
 
 
 .. code-block:: bash
 
     stegano-lsb-set reveal -i ./tests/sample-files/Lenna.png --generator fibonacci --shift 7
-    
-    
+
+
 List all available generators
 ------------------------------
 
 .. code-block:: bash
 
     $ stegano-lsb-set list-generators
     Generator id:
```

### Comparing `stegano-0.9.8/docs/steganalysis.rst` & `stegano-0.9.9/docs/steganalysis.rst`

 * *Files identical despite different names*

### Comparing `stegano-0.9.8/pyproject.toml` & `stegano-0.9.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "stegano"
-version = "0.9.8"
+version = "0.9.9"
 description = "A pure Python Steganography module."
 authors = [
     "Cédric Bonhomme <cedric@cedricbonhomme.org>"
 ]
 license = "GPL-3.0-or-later"
 
 readme = "README.md"
 
-homepage = "https://git.sr.ht/~cedric/stegano"
+homepage = "https://sr.ht/~cedric/stegano"
 repository = "https://git.sr.ht/~cedric/stegano"
 documentation = "https://stegano.readthedocs.io"
 
 keywords = ["steganography", "security", "stegano"]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Security",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 
 include = [
-    "CHANGELOG.md",
+    "README.md",
     "COPYING",
     "CHANGELOG.md",
     "docs/**/*",
     "bin/*"
 ]
 
 [tool.poetry.scripts]
@@ -40,19 +41,20 @@
 stegano-lsb-set = "bin.lsbset:main"
 stegano-red = "bin.red:main"
 stegano-steganalysis-parity = "bin.parity:main"
 stegano-steganalysis-statistics = "bin.statistics:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pillow = "^6.2.1"
+pillow = "^8.2.0"
 piexif = "^1.1.3"
-crayons = "^0.3.0"
+crayons = "^0.4.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.750"
 flake8 = "^3.7.9"
 nose2 = "^0.9.1"
+Sphinx = "^3.5.3"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `stegano-0.9.8/stegano/exifHeader/exifHeader.py` & `stegano-0.9.9/stegano/exifHeader/exifHeader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/lsb/lsb.py` & `stegano-0.9.9/stegano/lsb/lsb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/lsbset/generators.py` & `stegano-0.9.9/stegano/lsbset/generators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/lsbset/lsbset.py` & `stegano-0.9.9/stegano/lsbset/lsbset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/red/red.py` & `stegano-0.9.9/stegano/red/red.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stéganô is a basic Python Steganography module.
-# Copyright (C) 2010-2019  Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021  Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/steganalysis/parity.py` & `stegano-0.9.9/stegano/steganalysis/parity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/steganalysis/statistics.py` & `stegano-0.9.9/stegano/steganalysis/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/stegano/tools.py` & `stegano-0.9.9/stegano/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Stegano - Stegano is a pure Python steganography module.
-# Copyright (C) 2010-2019 Cédric Bonhomme - https://www.cedricbonhomme.org
+# Copyright (C) 2010-2021 Cédric Bonhomme - https://www.cedricbonhomme.org
 #
 # For more information : https://git.sr.ht/~cedric/stegano
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `stegano-0.9.8/setup.py` & `stegano-0.9.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,33 +9,33 @@
  'stegano.red',
  'stegano.steganalysis']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['crayons>=0.3.0,<0.4.0', 'piexif>=1.1.3,<2.0.0', 'pillow>=6.2.1,<7.0.0']
+['crayons>=0.4.0,<0.5.0', 'piexif>=1.1.3,<2.0.0', 'pillow>=8.2.0,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['stegano-lsb = bin.lsb:main',
                      'stegano-lsb-set = bin.lsbset:main',
                      'stegano-red = bin.red:main',
                      'stegano-steganalysis-parity = bin.parity:main',
                      'stegano-steganalysis-statistics = bin.statistics:main']}
 
 setup_kwargs = {
     'name': 'stegano',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'A pure Python Steganography module.',
-    'long_description': '# Stegano\n\n[![builds.sr.ht status](https://builds.sr.ht/~cedric/stegano.svg)](https://builds.sr.ht/~cedric/stegano)\n\n\n[Stegano](https://git.sr.ht/~cedric/stegano), a pure Python Steganography\nmodule.\n\nSteganography is the art and science of writing hidden messages in such a way\nthat no one, apart from the sender and intended recipient, suspects the\nexistence of the message, a form of security through obscurity. Consequently,\nfunctions provided by Stegano only hide messages, without encryption.\nSteganography is often used with cryptography.\n\nFor reporting issues, visit the tracker here:\nhttps://todo.sr.ht/~cedric/stegano\n\n\n## Installation\n\n\n```bash\n$ poetry install Stegano\n```\n\nYou will be able to use Stegano in your Python programs.\n\nIf you only want to install Stegano as a command line tool:\n\n```bash\n$ pipx install Stegano\n```\n\npipx installs scripts (system wide available) provided by Python packages into\nseparate virtualenvs to shield them from your system and each other.\n\n\n## Usage\n\nA [tutorial](https://stegano.readthedocs.io) is available.\n\n\n## Use Stegano as a library in your Python program\n\nIf you want to use Stegano in your Python program you just have to import the\nappropriate steganography technique. For example:\n\n```python\n>>> from stegano import lsb\n>>> secret = lsb.hide("./tests/sample-files/Lenna.png", "Hello World")\n>>> secret.save("./Lenna-secret.png")\n>>>\n>>> clear_message = lsb.reveal("./Lenna-secret.png")\n```\n\n\n## Use Stegano as a command line tool\n\n### Hide and reveal a message\n\n```bash\n$ stegano-lsb hide -i ./tests/sample-files/Lenna.png -m "Secret Message" -o Lena1.png\n$ stegano-lsb reveal -i Lena1.png\nSecret Message\n```\n\n\n### Hide the message with the Sieve of Eratosthenes\n\n```bash\n$ stegano-lsb-set hide -i ./tests/sample-files/Lenna.png -m \'Secret Message\' --generator eratosthenes -o Lena2.png\n```\n\nThe message will be scattered in the picture, following a set described by the\nSieve of Eratosthenes. Other sets are available. You can also use your own\ngenerators.\n\nThis will make a steganalysis more complicated.\n\n\n## Running the tests\n\n```bash\n$ python -m unittest discover -v\n```\n\nRunning the static type checker:\n\n```bash\n$ python tools/run_mypy.py\n```\n\n\n## Contributions\n\nContributions are welcome. If you want to contribute to Stegano I highly\nrecommend you to install it in a Python virtual environment with poetry.\n\n\n## License\n\nThis software is licensed under\n[GNU General Public License version 3](https://www.gnu.org/licenses/gpl-3.0.html)\n\nCopyright (C) 2010-2019 [Cédric Bonhomme](https://www.cedricbonhomme.org)\n\nFor more information, [the list of authors and contributors](CONTRIBUTORS.md) is available.\n',
+    'long_description': '# Stegano\n\n[![builds.sr.ht status](https://builds.sr.ht/~cedric/stegano.svg)](https://builds.sr.ht/~cedric/stegano)\n\n\n[Stegano](https://sr.ht/~cedric/stegano), a pure Python Steganography\nmodule.\n\nSteganography is the art and science of writing hidden messages in such a way\nthat no one, apart from the sender and intended recipient, suspects the\nexistence of the message, a form of security through obscurity. Consequently,\nfunctions provided by Stegano only hide messages, without encryption.\nSteganography is often used with cryptography.\n\nFor reporting issues, visit the tracker here:\nhttps://todo.sr.ht/~cedric/stegano\n\n\n## Installation\n\n\n```bash\n$ poetry install stegano\n```\n\nYou will be able to use Stegano in your Python programs.\n\nIf you only want to install Stegano as a command line tool:\n\n```bash\n$ pipx install stegano\n```\n\npipx installs scripts (system wide available) provided by Python packages into\nseparate virtualenvs to shield them from your system and each other.\n\n\n## Usage\n\nA [tutorial](https://stegano.readthedocs.io) is available.\n\n\n## Use Stegano as a library in your Python program\n\nIf you want to use Stegano in your Python program you just have to import the\nappropriate steganography technique. For example:\n\n```python\n>>> from stegano import lsb\n>>> secret = lsb.hide("./tests/sample-files/Lenna.png", "Hello World")\n>>> secret.save("./Lenna-secret.png")\n>>>\n>>> clear_message = lsb.reveal("./Lenna-secret.png")\n```\n\n\n## Use Stegano as a command line tool\n\n### Hide and reveal a message\n\n```bash\n$ stegano-lsb hide -i ./tests/sample-files/Lenna.png -m "Secret Message" -o Lena1.png\n$ stegano-lsb reveal -i Lena1.png\nSecret Message\n```\n\n\n### Hide the message with the Sieve of Eratosthenes\n\n```bash\n$ stegano-lsb-set hide -i ./tests/sample-files/Lenna.png -m \'Secret Message\' --generator eratosthenes -o Lena2.png\n```\n\nThe message will be scattered in the picture, following a set described by the\nSieve of Eratosthenes. Other sets are available. You can also use your own\ngenerators.\n\nThis will make a steganalysis more complicated.\n\n\n## Running the tests\n\n```bash\n$ python -m unittest discover -v\n```\n\nRunning the static type checker:\n\n```bash\n$ python tools/run_mypy.py\n```\n\n\n## Contributions\n\nContributions are welcome. If you want to contribute to Stegano I highly\nrecommend you to install it in a Python virtual environment with poetry.\n\n\n## License\n\nThis software is licensed under\n[GNU General Public License version 3](https://www.gnu.org/licenses/gpl-3.0.html)\n\nCopyright (C) 2010-2021 [Cédric Bonhomme](https://www.cedricbonhomme.org)\n\nFor more information, [the list of authors and contributors](CONTRIBUTORS.md) is available.\n',
     'author': 'Cédric Bonhomme',
     'author_email': 'cedric@cedricbonhomme.org',
     'maintainer': None,
     'maintainer_email': None,
-    'url': 'https://git.sr.ht/~cedric/stegano',
+    'url': 'https://sr.ht/~cedric/stegano',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
```

### Comparing `stegano-0.9.8/PKG-INFO` & `stegano-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: stegano
-Version: 0.9.8
+Version: 0.9.9
 Summary: A pure Python Steganography module.
-Home-page: https://git.sr.ht/~cedric/stegano
+Home-page: https://sr.ht/~cedric/stegano
 License: GPL-3.0-or-later
 Keywords: steganography,security,stegano
 Author: Cédric Bonhomme
 Author-email: cedric@cedricbonhomme.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
-Requires-Dist: crayons (>=0.3.0,<0.4.0)
+Requires-Dist: crayons (>=0.4.0,<0.5.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
-Requires-Dist: pillow (>=6.2.1,<7.0.0)
+Requires-Dist: pillow (>=8.2.0,<9.0.0)
 Project-URL: Documentation, https://stegano.readthedocs.io
 Project-URL: Repository, https://git.sr.ht/~cedric/stegano
 Description-Content-Type: text/markdown
 
 # Stegano
 
 [![builds.sr.ht status](https://builds.sr.ht/~cedric/stegano.svg)](https://builds.sr.ht/~cedric/stegano)
 
 
-[Stegano](https://git.sr.ht/~cedric/stegano), a pure Python Steganography
+[Stegano](https://sr.ht/~cedric/stegano), a pure Python Steganography
 module.
 
 Steganography is the art and science of writing hidden messages in such a way
 that no one, apart from the sender and intended recipient, suspects the
 existence of the message, a form of security through obscurity. Consequently,
 functions provided by Stegano only hide messages, without encryption.
 Steganography is often used with cryptography.
@@ -43,23 +44,23 @@
 https://todo.sr.ht/~cedric/stegano
 
 
 ## Installation
 
 
 ```bash
-$ poetry install Stegano
+$ poetry install stegano
 ```
 
 You will be able to use Stegano in your Python programs.
 
 If you only want to install Stegano as a command line tool:
 
 ```bash
-$ pipx install Stegano
+$ pipx install stegano
 ```
 
 pipx installs scripts (system wide available) provided by Python packages into
 separate virtualenvs to shield them from your system and each other.
 
 
 ## Usage
@@ -125,11 +126,11 @@
 
 
 ## License
 
 This software is licensed under
 [GNU General Public License version 3](https://www.gnu.org/licenses/gpl-3.0.html)
 
-Copyright (C) 2010-2019 [Cédric Bonhomme](https://www.cedricbonhomme.org)
+Copyright (C) 2010-2021 [Cédric Bonhomme](https://www.cedricbonhomme.org)
 
 For more information, [the list of authors and contributors](CONTRIBUTORS.md) is available.
```

