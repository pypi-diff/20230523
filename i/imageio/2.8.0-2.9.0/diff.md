# Comparing `tmp/imageio-2.8.0.tar.gz` & `tmp/imageio-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imageio-2.8.0.tar", last modified: Tue Feb 18 23:10:26 2020, max compression
+gzip compressed data, was "dist\imageio-2.9.0.tar", last modified: Mon Jul  6 13:20:34 2020, max compression
```

## Comparing `imageio-2.8.0.tar` & `imageio-2.9.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/
--rw-rw-rw-   0        0        0     1544 2019-02-06 10:36:59.000000 imageio-2.8.0/CONTRIBUTORS.txt
--rw-rw-rw-   0        0        0     1307 2020-02-18 22:38:25.000000 imageio-2.8.0/LICENSE
--rw-rw-rw-   0        0        0     2549 2020-02-18 23:10:26.000000 imageio-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5463 2020-02-18 22:42:46.000000 imageio-2.8.0/README.md
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/docs/
--rw-rw-rw-   0        0        0       20 2017-05-22 12:36:06.000000 imageio-2.8.0/docs/.requirements
--rw-rw-rw-   0        0        0     5568 2015-10-31 21:52:48.000000 imageio-2.8.0/docs/Makefile
--rw-rw-rw-   0        0        0      870 2018-02-19 14:22:40.000000 imageio-2.8.0/docs/cmdlinescripts.rst
--rw-rw-rw-   0        0        0     8443 2020-02-18 22:38:25.000000 imageio-2.8.0/docs/conf.py
--rw-rw-rw-   0        0        0      551 2015-10-31 21:52:49.000000 imageio-2.8.0/docs/devapi.rst
--rw-rw-rw-   0        0        0      659 2019-10-08 09:55:29.000000 imageio-2.8.0/docs/drop27.rst
--rw-rw-rw-   0        0        0     1275 2020-02-18 21:17:18.000000 imageio-2.8.0/docs/envvariables.rst
--rw-rw-rw-   0        0        0     8544 2020-02-18 15:43:23.000000 imageio-2.8.0/docs/examples.rst
--rw-rw-rw-   0        0        0     7345 2018-09-04 09:23:11.000000 imageio-2.8.0/docs/imageio_ext.py
--rw-rw-rw-   0        0        0      194 2015-10-31 21:52:49.000000 imageio-2.8.0/docs/index.rst
--rw-rw-rw-   0        0        0      959 2019-10-08 09:55:29.000000 imageio-2.8.0/docs/installation.rst
--rwxrwxrwx   0        0        0     5098 2015-10-31 21:52:49.000000 imageio-2.8.0/docs/make.bat
--rw-rw-rw-   0        0        0     1538 2018-09-04 12:21:12.000000 imageio-2.8.0/docs/scipy.rst
--rw-rw-rw-   0        0        0      157 2015-10-31 21:52:49.000000 imageio-2.8.0/docs/sec_developer.rst
--rw-rw-rw-   0        0        0      171 2020-02-18 22:38:25.000000 imageio-2.8.0/docs/sec_gettingstarted.rst
--rw-rw-rw-   0        0        0      230 2018-02-19 14:22:40.000000 imageio-2.8.0/docs/sec_reference.rst
--rw-rw-rw-   0        0        0      744 2015-10-31 21:52:49.000000 imageio-2.8.0/docs/userapi.rst
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/imageio/
--rw-rw-rw-   0        0        0     1272 2020-02-18 23:09:16.000000 imageio-2.8.0/imageio/__init__.py
--rw-rw-rw-   0        0        0     5399 2020-02-18 21:17:18.000000 imageio-2.8.0/imageio/__main__.py
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/imageio/core/
--rw-rw-rw-   0        0        0      639 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/core/__init__.py
--rw-rw-rw-   0        0        0     9187 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/core/fetching.py
--rw-rw-rw-   0        0        0     5506 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/core/findlib.py
--rw-rw-rw-   0        0        0    26004 2020-02-18 15:43:23.000000 imageio-2.8.0/imageio/core/format.py
--rw-rw-rw-   0        0        0    21221 2020-02-18 15:43:23.000000 imageio-2.8.0/imageio/core/functions.py
--rw-rw-rw-   0        0        0    20834 2020-02-18 21:46:53.000000 imageio-2.8.0/imageio/core/request.py
--rw-rw-rw-   0        0        0    18663 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/core/util.py
--rw-rw-rw-   0        0        0      170 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/freeze.py
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/imageio/plugins/
--rw-rw-rw-   0        0        0     3674 2020-02-18 21:17:18.000000 imageio-2.8.0/imageio/plugins/__init__.py
--rw-rw-rw-   0        0        0    32971 2019-02-05 22:11:00.000000 imageio-2.8.0/imageio/plugins/_bsdf.py
--rw-rw-rw-   0        0        0    33935 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/_dicom.py
--rw-rw-rw-   0        0        0    51834 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/_freeimage.py
--rw-rw-rw-   0        0        0    25758 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/_swf.py
--rw-rw-rw-   0        0        0   367400 2019-09-09 07:55:17.000000 imageio-2.8.0/imageio/plugins/_tifffile.py
--rw-rw-rw-   0        0        0    11422 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/bsdf.py
--rw-rw-rw-   0        0        0    10364 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/dicom.py
--rw-rw-rw-   0        0        0     5696 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/example.py
--rw-rw-rw-   0        0        0     3359 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/feisem.py
--rw-rw-rw-   0        0        0    28583 2020-02-18 15:43:23.000000 imageio-2.8.0/imageio/plugins/ffmpeg.py
--rw-rw-rw-   0        0        0     4775 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/fits.py
--rw-rw-rw-   0        0        0    18887 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/freeimage.py
--rw-rw-rw-   0        0        0    11745 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/freeimagemulti.py
--rw-rw-rw-   0        0        0     1711 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/gdal.py
--rw-rw-rw-   0        0        0     3250 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/grab.py
--rw-rw-rw-   0        0        0    24708 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/lytro.py
--rw-rw-rw-   0        0        0     3122 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/npz.py
--rw-rw-rw-   0        0        0    33002 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/pillow.py
--rw-rw-rw-   0        0        0    37399 2018-09-04 09:23:11.000000 imageio-2.8.0/imageio/plugins/pillow_info.py
--rw-rw-rw-   0        0        0    12571 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/pillowmulti.py
--rw-rw-rw-   0        0        0     4073 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/simpleitk.py
--rw-rw-rw-   0        0        0    15441 2020-01-13 11:53:41.000000 imageio-2.8.0/imageio/plugins/spe.py
--rw-rw-rw-   0        0        0    12295 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/plugins/swf.py
--rw-rw-rw-   0        0        0    11436 2020-02-18 15:43:23.000000 imageio-2.8.0/imageio/plugins/tifffile.py
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/imageio/resources/
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/imageio/resources/images/
--rw-rw-rw-   0        0        0   791555 2020-02-18 23:10:16.000000 imageio-2.8.0/imageio/resources/images/astronaut.png
--rw-rw-rw-   0        0        0   221294 2020-02-18 23:10:13.000000 imageio-2.8.0/imageio/resources/images/chelsea.png
--rw-rw-rw-   0        0        0   221318 2020-02-18 23:10:14.000000 imageio-2.8.0/imageio/resources/images/chelsea.zip
--rw-rw-rw-   0        0        0   728751 2020-02-18 23:10:19.000000 imageio-2.8.0/imageio/resources/images/cockatoo.mp4
--rw-rw-rw-   0        0        0   583374 2020-02-18 23:10:18.000000 imageio-2.8.0/imageio/resources/images/newtonscradle.gif
--rw-rw-rw-   0        0        0    96822 2020-02-18 23:10:21.000000 imageio-2.8.0/imageio/resources/images/realshort.mp4
--rw-rw-rw-   0        0        0   824612 2020-02-18 23:10:25.000000 imageio-2.8.0/imageio/resources/images/stent.npz
--rw-rw-rw-   0        0        0        0 2020-02-18 23:10:12.000000 imageio-2.8.0/imageio/resources/shipped_resources_go_here
--rw-rw-rw-   0        0        0     3419 2019-10-08 09:55:29.000000 imageio-2.8.0/imageio/testing.py
--rw-rw-rw-   0        0        0     6587 2020-02-18 22:38:25.000000 imageio-2.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-02-18 23:10:26.000000 imageio-2.8.0/tests/
--rw-rw-rw-   0        0        0      459 2016-01-13 10:47:50.000000 imageio-2.8.0/tests/README.md
--rw-rw-rw-   0        0        0     6010 2019-09-09 07:55:17.000000 imageio-2.8.0/tests/test_bsdf.py
--rw-rw-rw-   0        0        0    25953 2020-02-18 21:46:53.000000 imageio-2.8.0/tests/test_core.py
--rw-rw-rw-   0        0        0     5792 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_dicom.py
--rw-rw-rw-   0        0        0     1427 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_fei_tiff.py
--rw-rw-rw-   0        0        0    17768 2020-02-18 21:17:18.000000 imageio-2.8.0/tests/test_ffmpeg.py
--rw-rw-rw-   0        0        0     3873 2019-10-08 09:55:29.000000 imageio-2.8.0/tests/test_ffmpeg_info.py
--rw-rw-rw-   0        0        0     2114 2019-08-01 08:50:25.000000 imageio-2.8.0/tests/test_fits.py
--rw-rw-rw-   0        0        0    12101 2019-02-05 12:18:33.000000 imageio-2.8.0/tests/test_format.py
--rw-rw-rw-   0        0        0    17729 2019-06-06 06:52:39.000000 imageio-2.8.0/tests/test_freeimage.py
--rw-rw-rw-   0        0        0     3088 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_freeimage_suite.py
--rw-rw-rw-   0        0        0      819 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_gdal.py
--rw-rw-rw-   0        0        0     2673 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_grab.py
--rw-rw-rw-   0        0        0    24371 2018-09-11 09:14:35.000000 imageio-2.8.0/tests/test_lytro.py
--rw-rw-rw-   0        0        0     5648 2019-10-08 09:55:29.000000 imageio-2.8.0/tests/test_meta.py
--rw-rw-rw-   0        0        0     2231 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_npz.py
--rw-rw-rw-   0        0        0    14074 2019-06-06 06:52:39.000000 imageio-2.8.0/tests/test_pillow.py
--rw-rw-rw-   0        0        0     1320 2019-02-05 22:11:00.000000 imageio-2.8.0/tests/test_simpleitk.py
--rw-rw-rw-   0        0        0     1930 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_spe.py
--rw-rw-rw-   0        0        0     5781 2018-09-04 09:23:11.000000 imageio-2.8.0/tests/test_swf.py
--rw-rw-rw-   0        0        0     3869 2019-02-06 09:42:18.000000 imageio-2.8.0/tests/test_tifffile.py
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/
+-rw-rw-rw-   0        0        0     1544 2019-02-06 10:36:59.000000 imageio-2.9.0/CONTRIBUTORS.txt
+-rw-rw-rw-   0        0        0     1307 2020-02-18 22:38:25.000000 imageio-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0     2552 2020-07-06 13:20:34.000000 imageio-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5474 2020-06-08 11:09:32.000000 imageio-2.9.0/README.md
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/docs/
+-rw-rw-rw-   0        0        0       20 2017-05-22 12:36:06.000000 imageio-2.9.0/docs/.requirements
+-rw-rw-rw-   0        0        0     5568 2015-10-31 21:52:48.000000 imageio-2.9.0/docs/Makefile
+-rw-rw-rw-   0        0        0      870 2018-02-19 14:22:40.000000 imageio-2.9.0/docs/cmdlinescripts.rst
+-rw-rw-rw-   0        0        0     8443 2020-02-18 22:38:25.000000 imageio-2.9.0/docs/conf.py
+-rw-rw-rw-   0        0        0      551 2015-10-31 21:52:49.000000 imageio-2.9.0/docs/devapi.rst
+-rw-rw-rw-   0        0        0      659 2019-10-08 09:55:29.000000 imageio-2.9.0/docs/drop27.rst
+-rw-rw-rw-   0        0        0     1396 2020-07-06 12:38:25.000000 imageio-2.9.0/docs/envvariables.rst
+-rw-rw-rw-   0        0        0     8544 2020-02-18 15:43:23.000000 imageio-2.9.0/docs/examples.rst
+-rw-rw-rw-   0        0        0     7345 2018-09-04 09:23:11.000000 imageio-2.9.0/docs/imageio_ext.py
+-rw-rw-rw-   0        0        0      194 2015-10-31 21:52:49.000000 imageio-2.9.0/docs/index.rst
+-rw-rw-rw-   0        0        0      959 2019-10-08 09:55:29.000000 imageio-2.9.0/docs/installation.rst
+-rwxrwxrwx   0        0        0     5098 2015-10-31 21:52:49.000000 imageio-2.9.0/docs/make.bat
+-rw-rw-rw-   0        0        0     1538 2018-09-04 12:21:12.000000 imageio-2.9.0/docs/scipy.rst
+-rw-rw-rw-   0        0        0      157 2015-10-31 21:52:49.000000 imageio-2.9.0/docs/sec_developer.rst
+-rw-rw-rw-   0        0        0      171 2020-02-18 22:38:25.000000 imageio-2.9.0/docs/sec_gettingstarted.rst
+-rw-rw-rw-   0        0        0      230 2018-02-19 14:22:40.000000 imageio-2.9.0/docs/sec_reference.rst
+-rw-rw-rw-   0        0        0      744 2015-10-31 21:52:49.000000 imageio-2.9.0/docs/userapi.rst
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/imageio/
+-rw-rw-rw-   0        0        0     1273 2020-07-06 13:08:04.000000 imageio-2.9.0/imageio/__init__.py
+-rw-rw-rw-   0        0        0     5399 2020-02-18 21:17:18.000000 imageio-2.9.0/imageio/__main__.py
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/imageio/core/
+-rw-rw-rw-   0        0        0      639 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/core/__init__.py
+-rw-rw-rw-   0        0        0     9187 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/core/fetching.py
+-rw-rw-rw-   0        0        0     5544 2020-05-11 12:05:35.000000 imageio-2.9.0/imageio/core/findlib.py
+-rw-rw-rw-   0        0        0    26004 2020-02-18 15:43:23.000000 imageio-2.9.0/imageio/core/format.py
+-rw-rw-rw-   0        0        0    21221 2020-02-18 15:43:23.000000 imageio-2.9.0/imageio/core/functions.py
+-rw-rw-rw-   0        0        0    21190 2020-07-06 13:18:51.000000 imageio-2.9.0/imageio/core/request.py
+-rw-rw-rw-   0        0        0    18663 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/core/util.py
+-rw-rw-rw-   0        0        0      170 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/freeze.py
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/imageio/plugins/
+-rw-rw-rw-   0        0        0     3674 2020-02-18 21:17:18.000000 imageio-2.9.0/imageio/plugins/__init__.py
+-rw-rw-rw-   0        0        0    32971 2019-02-05 22:11:00.000000 imageio-2.9.0/imageio/plugins/_bsdf.py
+-rw-rw-rw-   0        0        0    33935 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/_dicom.py
+-rw-rw-rw-   0        0        0    51834 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/_freeimage.py
+-rw-rw-rw-   0        0        0    25758 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/_swf.py
+-rw-rw-rw-   0        0        0   367400 2019-09-09 07:55:17.000000 imageio-2.9.0/imageio/plugins/_tifffile.py
+-rw-rw-rw-   0        0        0    11422 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/bsdf.py
+-rw-rw-rw-   0        0        0    12190 2020-06-08 13:01:35.000000 imageio-2.9.0/imageio/plugins/dicom.py
+-rw-rw-rw-   0        0        0     5696 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/example.py
+-rw-rw-rw-   0        0        0     3392 2020-06-08 12:32:43.000000 imageio-2.9.0/imageio/plugins/feisem.py
+-rw-rw-rw-   0        0        0    28647 2020-06-08 12:32:43.000000 imageio-2.9.0/imageio/plugins/ffmpeg.py
+-rw-rw-rw-   0        0        0     4775 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/fits.py
+-rw-rw-rw-   0        0        0    18887 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/freeimage.py
+-rw-rw-rw-   0        0        0    11745 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/freeimagemulti.py
+-rw-rw-rw-   0        0        0     1711 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/gdal.py
+-rw-rw-rw-   0        0        0     3250 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/grab.py
+-rw-rw-rw-   0        0        0    24708 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/lytro.py
+-rw-rw-rw-   0        0        0     3122 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/npz.py
+-rw-rw-rw-   0        0        0    33002 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/pillow.py
+-rw-rw-rw-   0        0        0    37399 2018-09-04 09:23:11.000000 imageio-2.9.0/imageio/plugins/pillow_info.py
+-rw-rw-rw-   0        0        0    12571 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/pillowmulti.py
+-rw-rw-rw-   0        0        0     4349 2020-06-08 11:09:32.000000 imageio-2.9.0/imageio/plugins/simpleitk.py
+-rw-rw-rw-   0        0        0    15441 2020-01-13 11:53:41.000000 imageio-2.9.0/imageio/plugins/spe.py
+-rw-rw-rw-   0        0        0    12295 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/plugins/swf.py
+-rw-rw-rw-   0        0        0    11436 2020-02-18 15:43:23.000000 imageio-2.9.0/imageio/plugins/tifffile.py
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/imageio/resources/
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/imageio/resources/images/
+-rw-rw-rw-   0        0        0   791555 2020-07-06 13:20:28.000000 imageio-2.9.0/imageio/resources/images/astronaut.png
+-rw-rw-rw-   0        0        0   221294 2020-07-06 13:20:25.000000 imageio-2.9.0/imageio/resources/images/chelsea.png
+-rw-rw-rw-   0        0        0   221318 2020-07-06 13:20:26.000000 imageio-2.9.0/imageio/resources/images/chelsea.zip
+-rw-rw-rw-   0        0        0   728751 2020-07-06 13:20:31.000000 imageio-2.9.0/imageio/resources/images/cockatoo.mp4
+-rw-rw-rw-   0        0        0   583374 2020-07-06 13:20:29.000000 imageio-2.9.0/imageio/resources/images/newtonscradle.gif
+-rw-rw-rw-   0        0        0    96822 2020-07-06 13:20:31.000000 imageio-2.9.0/imageio/resources/images/realshort.mp4
+-rw-rw-rw-   0        0        0   824612 2020-07-06 13:20:33.000000 imageio-2.9.0/imageio/resources/images/stent.npz
+-rw-rw-rw-   0        0        0        0 2020-07-06 13:20:24.000000 imageio-2.9.0/imageio/resources/shipped_resources_go_here
+-rw-rw-rw-   0        0        0     3419 2019-10-08 09:55:29.000000 imageio-2.9.0/imageio/testing.py
+-rw-rw-rw-   0        0        0     6589 2020-02-18 23:40:06.000000 imageio-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-06 13:20:34.000000 imageio-2.9.0/tests/
+-rw-rw-rw-   0        0        0      459 2016-01-13 10:47:50.000000 imageio-2.9.0/tests/README.md
+-rw-rw-rw-   0        0        0     6010 2019-09-09 07:55:17.000000 imageio-2.9.0/tests/test_bsdf.py
+-rw-rw-rw-   0        0        0    25953 2020-02-18 21:46:53.000000 imageio-2.9.0/tests/test_core.py
+-rw-rw-rw-   0        0        0     5792 2020-06-08 11:18:59.000000 imageio-2.9.0/tests/test_dicom.py
+-rw-rw-rw-   0        0        0     1427 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_fei_tiff.py
+-rw-rw-rw-   0        0        0    17926 2020-06-08 12:32:43.000000 imageio-2.9.0/tests/test_ffmpeg.py
+-rw-rw-rw-   0        0        0     3886 2020-06-08 12:32:43.000000 imageio-2.9.0/tests/test_ffmpeg_info.py
+-rw-rw-rw-   0        0        0     2114 2019-08-01 08:50:25.000000 imageio-2.9.0/tests/test_fits.py
+-rw-rw-rw-   0        0        0    12101 2019-02-05 12:18:33.000000 imageio-2.9.0/tests/test_format.py
+-rw-rw-rw-   0        0        0    17729 2019-06-06 06:52:39.000000 imageio-2.9.0/tests/test_freeimage.py
+-rw-rw-rw-   0        0        0     3088 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_freeimage_suite.py
+-rw-rw-rw-   0        0        0      819 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_gdal.py
+-rw-rw-rw-   0        0        0     2673 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_grab.py
+-rw-rw-rw-   0        0        0    24371 2018-09-11 09:14:35.000000 imageio-2.9.0/tests/test_lytro.py
+-rw-rw-rw-   0        0        0     5648 2019-10-08 09:55:29.000000 imageio-2.9.0/tests/test_meta.py
+-rw-rw-rw-   0        0        0     2231 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_npz.py
+-rw-rw-rw-   0        0        0    14074 2019-06-06 06:52:39.000000 imageio-2.9.0/tests/test_pillow.py
+-rw-rw-rw-   0        0        0     1320 2019-02-05 22:11:00.000000 imageio-2.9.0/tests/test_simpleitk.py
+-rw-rw-rw-   0        0        0     1930 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_spe.py
+-rw-rw-rw-   0        0        0     5781 2018-09-04 09:23:11.000000 imageio-2.9.0/tests/test_swf.py
+-rw-rw-rw-   0        0        0     3869 2019-02-06 09:42:18.000000 imageio-2.9.0/tests/test_tifffile.py
```

### Comparing `imageio-2.8.0/CONTRIBUTORS.txt` & `imageio-2.9.0/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/LICENSE` & `imageio-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/PKG-INFO` & `imageio-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imageio
-Version: 2.8.0
+Version: 2.9.0
 Summary: Library for reading and writing a wide range of image, video, scientific, and volumetric data formats.
 Home-page: https://github.com/imageio/imageio
 Author: imageio contributors
 Author-email: almar.klein@gmail.com
 License: BSD-2-Clause
 Download-URL: http://pypi.python.org/pypi/imageio
 Description: 
@@ -16,31 +16,31 @@
         
         
         Imageio is a Python library that provides an easy interface to read and
         write a wide range of image data, including animated images, volumetric
         data, and scientific formats. It is cross-platform, runs on Python 3.5+,
         and is easy to install.
         
-        Main website: http://imageio.github.io
+        Main website: https://imageio.github.io
         
         
         Release notes: hhttps://github.com/imageio/imageio/blob/master/CHANGELOG.md
         
         Example:
         
         .. code-block:: python
         
             >>> import imageio
             >>> im = imageio.imread('imageio:astronaut.png')
             >>> im.shape  # im is a numpy array
             (512, 512, 3)
             >>> imageio.imwrite('astronaut-gray.jpg', im[:, :, 0])
         
-        See the `user API <http://imageio.readthedocs.io/en/latest/userapi.html>`_
-        or `examples <http://imageio.readthedocs.io/en/latest/examples.html>`_
+        See the `user API <https://imageio.readthedocs.io/en/stable/userapi.html>`_
+        or `examples <https://imageio.readthedocs.io/en/stable/examples.html>`_
         for more information.
         
 Keywords: image video volume imread imwrite io animation ffmpeg
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -53,11 +53,11 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Provides: imageio
 Requires-Python: >=3.5
 Provides-Extra: fits
+Provides-Extra: gdal
 Provides-Extra: itk
 Provides-Extra: ffmpeg
 Provides-Extra: full
-Provides-Extra: gdal
```

### Comparing `imageio-2.8.0/README.md` & `imageio-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 # IMAGEIO
 
 [![PyPI Version](https://img.shields.io/pypi/v/imageio.svg)](https://pypi.python.org/pypi/imageio/)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/imageio.svg)](https://pypi.python.org/pypi/imageio/)
 [![Build Status](https://travis-ci.org/imageio/imageio.svg?branch=master)](https://travis-ci.org/imageio/imageio)
-[![Coverage Status](https://coveralls.io/repos/imageio/imageio/badge.png?branch=master)](https://coveralls.io/r/imageio/imageio?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/imageio/imageio/badge.svg?branch=master)](https://coveralls.io/github/imageio/imageio?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/imageio/badge/?version=latest)](https://imageio.readthedocs.io)
 [![PyPi Download stats](http://pepy.tech/badge/imageio)](http://pepy.tech/project/imageio)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1488561.svg)](https://doi.org/10.5281/zenodo.1488561)
 
-Website: http://imageio.github.io
+Website: https://imageio.github.io
 
 <!-- From below ends up on the website Keep this ---- DIVIDER ---- -->
 
 <p class='summary'>
 Imageio is a Python library that provides an easy interface to read and
 write a wide range of image data, including animated images, video,
 volumetric data, and scientific formats. It is cross-platform, runs on
 Python 3.5+, and is easy to install.
 </p>
 
 <h2>Example</h2>
 Here's a minimal example of how to use imageio. See the docs for
-<a href='http://imageio.readthedocs.io/en/latest/examples.html'>more examples</a>.
-<pre>
+<a href='https://imageio.readthedocs.io/en/stable/examples.html'>more examples</a>.
+
+```python
 import imageio
 im = imageio.imread('imageio:chelsea.png')  # read a standard image
-im.shape  # im is a numpy array
+im.shape  # im is a NumPy array
 >> (300, 451, 3)
 imageio.imwrite('~/chelsea-gray.jpg', im[:, :, 0])
-</pre>
+```
 
 <h2>API in a nutshell</h2>
-As a user, you just have to remember a handfull of functions:
+As a user, you just have to remember a handful of functions:
 
 <ul>
     <li>imread() and imwrite() - for single images</li>
     <li>mimread() and mimwrite() - for image series (animations)</li>
     <li>volread() and volwrite() - for volumetric image data</li>
     <li>get_reader() and get_writer() - for more control (e.g. streaming or compression)</li>
-    <li>See the <a href='http://imageio.readthedocs.io/en/latest/userapi.html'>user api</a> for more information</li>
+    <li>See the <a href='https://imageio.readthedocs.io/en/stable/userapi.html'>user api</a> for more information</li>
 </ul>
 
 
 <h2>Features</h2>
 <ul>
     <li>Simple interface via a consise set of functions.</li>
-    <li>Easy to <a href='http://imageio.readthedocs.io/en/latest/installation.html'>install</a> using conda or pip.</li>
-    <li>Few dependencies (only Numpy and Pillow).</li>
-    <li>Pure Python, runs on Python 3.5+, and Pypy</li>
+    <li>Easy to <a href='https://imageio.readthedocs.io/en/stable/installation.html'>install</a> using Conda or pip</li>
+    <li>Few dependencies (only NumPy and Pillow)</li>
+    <li>Pure Python, runs on Python 3.5+, and PyPy</li>
     <li>Cross platform, runs on Windows, Linux, macOS</li>
-    <li>Lots of supported <a href='http://imageio.readthedocs.io/en/latest/formats.html'>formats</a>.</li>
-    <li>Can read from file names, file objects, zipfiles, http/ftp, and raw bytes.</li>
-    <li>Easy to extend using plugins.</li>
-    <li>Code quality is maintained with many tests and continuous integration.</li>
+    <li>Lots of supported <a href='https://imageio.readthedocs.io/en/stable/formats.html'>formats</a></li>
+    <li>Can read from file names, file objects, zipfiles, http/ftp, and raw bytes</li>
+    <li>Easy to extend using plugins</li>
+    <li>Code quality is maintained with many tests and continuous integration</li>
 </ul>
 
 
 <h2>Dependencies</h2>
 
 Minimal requirements:
 <ul>
     <li>Python 3.5+</li>
-    <li>Numpy</li>
+    <li>NumPy</li>
     <li>Pillow</li>
 </ul>
 
 Optional Python packages:
 <ul>
     <li>imageio-ffmpeg (for working with video files)</li>
     <li>itk or SimpleITK (for ITK formats)</li>
@@ -88,15 +89,15 @@
 To report a security vulnerability, please use the
 <a href='https://tidelift.com/security'>Tidelift security contact</a>.
 Tidelift will coordinate the fix and disclosure.
 
 
 <h2>imageio for enterprise</h2>
 
-Available as part of the Tidelift Subscription
+Available as part of the Tidelift Subscription.
 
 The maintainers of imageio and thousands of other packages are working with Tidelift to deliver commercial support and maintenance for the open source dependencies you use to build your applications. Save time, reduce risk, and improve code health, while paying the maintainers of the exact dependencies you use.
 <a href='https://tidelift.com/subscription/pkg/pypi-imageio?utm_source=pypi-imageio&utm_medium=referral&utm_campaign=readme'>Learn more</a>.
 
 
 <h2>Details</h2>
 <p>
@@ -114,31 +115,31 @@
 </p>
 
 
 <h2>Contributing</h2>
 
 <p>Install a complete development environment:</p>
 
-<pre>
+```bash
 pip install -r requirements.txt
 pip install -e .
-</pre>
+```
 
 <p><i>N.B. this does not include GDAL because it has awkward compiled dependencies</i></p>
 
 <p>You may see failing test(s) due to missing installed components.
 On ubuntu, do <code>sudo apt install libfreeimage3</code></p>
 
 <p>
 Style checks, unit tests and coverage are controlled by <code>invoke</code>.
 Before committing, check these with:</p>
 
-<pre>
+```bash
 # reformat code on python 3.6+
 invoke autoformat
 # check there are no style errors
 invoke test --style
 # check the tests pass
 invoke test --unit
 # check test coverage (re-runs tests)
 invoke test --cover
-</pre>
+```
```

#### html2text {}

```diff
@@ -1,53 +1,51 @@
 # IMAGEIO [![PyPI Version](https://img.shields.io/pypi/v/imageio.svg)](https://
 pypi.python.org/pypi/imageio/) [![Supported Python Versions](https://
 img.shields.io/pypi/pyversions/imageio.svg)](https://pypi.python.org/pypi/
 imageio/) [![Build Status](https://travis-ci.org/imageio/
 imageio.svg?branch=master)](https://travis-ci.org/imageio/imageio) [![Coverage
-Status](https://coveralls.io/repos/imageio/imageio/badge.png?branch=master)]
-(https://coveralls.io/r/imageio/imageio?branch=master) [![Documentation Status]
-(https://readthedocs.org/projects/imageio/badge/?version=latest)](https://
-imageio.readthedocs.io) [![PyPi Download stats](http://pepy.tech/badge/
-imageio)](http://pepy.tech/project/imageio) [![DOI](https://zenodo.org/badge/
-DOI/10.5281/zenodo.1488561.svg)](https://doi.org/10.5281/zenodo.1488561)
-Website: http://imageio.github.io
+Status](https://coveralls.io/repos/github/imageio/imageio/
+badge.svg?branch=master)](https://coveralls.io/github/imageio/
+imageio?branch=master) [![Documentation Status](https://readthedocs.org/
+projects/imageio/badge/?version=latest)](https://imageio.readthedocs.io) [!
+[PyPi Download stats](http://pepy.tech/badge/imageio)](http://pepy.tech/
+project/imageio) [![DOI](https://zenodo.org/badge/DOI/10.5281/
+zenodo.1488561.svg)](https://doi.org/10.5281/zenodo.1488561) Website: https://
+imageio.github.io
 Imageio is a Python library that provides an easy interface to read and write a
 wide range of image data, including animated images, video, volumetric data,
 and scientific formats. It is cross-platform, runs on Python 3.5+, and is easy
 to install.
 ***** Example *****
 Here's a minimal example of how to use imageio. See the docs for more_examples.
-import imageio
-im = imageio.imread('imageio:chelsea.png')  # read a standard image
-im.shape  # im is a numpy array
->> (300, 451, 3)
-imageio.imwrite('~/chelsea-gray.jpg', im[:, :, 0])
+```python import imageio im = imageio.imread('imageio:chelsea.png') # read a
+standard image im.shape # im is a NumPy array >> (300, 451, 3) imageio.imwrite
+('~/chelsea-gray.jpg', im[:, :, 0]) ```
 ***** API in a nutshell *****
-As a user, you just have to remember a handfull of functions:
+As a user, you just have to remember a handful of functions:
     * imread() and imwrite() - for single images
     * mimread() and mimwrite() - for image series (animations)
     * volread() and volwrite() - for volumetric image data
     * get_reader() and get_writer() - for more control (e.g. streaming or
       compression)
     * See the user_api for more information
 ***** Features *****
     * Simple interface via a consise set of functions.
-    * Easy to install using conda or pip.
-    * Few dependencies (only Numpy and Pillow).
-    * Pure Python, runs on Python 3.5+, and Pypy
+    * Easy to install using Conda or pip
+    * Few dependencies (only NumPy and Pillow)
+    * Pure Python, runs on Python 3.5+, and PyPy
     * Cross platform, runs on Windows, Linux, macOS
-    * Lots of supported formats.
-    * Can read from file names, file objects, zipfiles, http/ftp, and raw
-      bytes.
-    * Easy to extend using plugins.
-    * Code quality is maintained with many tests and continuous integration.
+    * Lots of supported formats
+    * Can read from file names, file objects, zipfiles, http/ftp, and raw bytes
+    * Easy to extend using plugins
+    * Code quality is maintained with many tests and continuous integration
 ***** Dependencies *****
 Minimal requirements:
     * Python 3.5+
-    * Numpy
+    * NumPy
     * Pillow
 Optional Python packages:
     * imageio-ffmpeg (for working with video files)
     * itk or SimpleITK (for ITK formats)
     * astropy (for FITS plugin)
     * osgeo (for GDAL plugin)
 Still on an earlier version of Python? Imageio version 2.6.x supports Python
@@ -55,15 +53,15 @@
 ***** Citing imageio *****
 If you use imageio for scientific work, we would appreciate a citation. We have
 a DOI!
 ***** Security contact information *****
 To report a security vulnerability, please use the Tidelift_security_contact.
 Tidelift will coordinate the fix and disclosure.
 ***** imageio for enterprise *****
-Available as part of the Tidelift Subscription The maintainers of imageio and
+Available as part of the Tidelift Subscription. The maintainers of imageio and
 thousands of other packages are working with Tidelift to deliver commercial
 support and maintenance for the open source dependencies you use to build your
 applications. Save time, reduce risk, and improve code health, while paying the
 maintainers of the exact dependencies you use. Learn_more.
 ***** Details *****
 Imageio has a relatively simple core that provides a common interface to
 different file formats. This core takes care of reading from different sources
@@ -72,22 +70,16 @@
 registered.
 Imageio provides a wide range of image formats, including scientific formats.
 Any help with implementing more formats is very welcome!
 The codebase adheres to (a subset of) the PEP8 style guides. We strive for
 maximum test coverage (100% for the core, >95% for each plugin).
 ***** Contributing *****
 Install a complete development environment:
-pip install -r requirements.txt
-pip install -e .
+```bash pip install -r requirements.txt pip install -e . ```
 N.B. this does not include GDAL because it has awkward compiled dependencies
 You may see failing test(s) due to missing installed components. On ubuntu, do
 sudo apt install libfreeimage3
 Style checks, unit tests and coverage are controlled by invoke. Before
 committing, check these with:
-# reformat code on python 3.6+
-invoke autoformat
-# check there are no style errors
-invoke test --style
-# check the tests pass
-invoke test --unit
-# check test coverage (re-runs tests)
-invoke test --cover
+```bash # reformat code on python 3.6+ invoke autoformat # check there are no
+style errors invoke test --style # check the tests pass invoke test --unit #
+check test coverage (re-runs tests) invoke test --cover ```
```

### Comparing `imageio-2.8.0/docs/Makefile` & `imageio-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/cmdlinescripts.rst` & `imageio-2.9.0/docs/cmdlinescripts.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/conf.py` & `imageio-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/devapi.rst` & `imageio-2.9.0/docs/devapi.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/drop27.rst` & `imageio-2.9.0/docs/drop27.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/envvariables.rst` & `imageio-2.9.0/docs/envvariables.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 * ``IMAGEIO_FFMPEG_EXE``: Set the path to the ffmpeg executable. Set
   to simply "ffmpeg" to use your system ffmpeg executable.
 * ``IMAGEIO_FREEIMAGE_LIB``: Set the path to the freeimage library. If
   not given, will prompt user to download the freeimage library.
 * ``IMAGEIO_FORMAT_ORDER``: Determine format preference. E.g. setting this
   to ``"TIFF, -FI"`` will prefer the FreeImage plugin over the Pillow plugin,
   but still prefer TIFF over that. Also see the ``formats.sort()`` method.
+* ``IMAGEIO_REQUEST_TIMEOUT``: Set the timeout of http/ftp request in seconds.
+  If not set, this defaults to 5 seconds.
 * ``IMAGEIO_USERDIR``: Set the path to the default user directory. If not
   given, imageio will try ``~`` and if that's not available ``/var/tmp``.
```

### Comparing `imageio-2.8.0/docs/examples.rst` & `imageio-2.9.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/imageio_ext.py` & `imageio-2.9.0/docs/imageio_ext.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/installation.rst` & `imageio-2.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/make.bat` & `imageio-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/scipy.rst` & `imageio-2.9.0/docs/scipy.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/docs/userapi.rst` & `imageio-2.9.0/docs/userapi.rst`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/__init__.py` & `imageio-2.9.0/imageio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 # the page on Pypi:
 """
 Imageio is a Python library that provides an easy interface to read and
 write a wide range of image data, including animated images, volumetric
 data, and scientific formats. It is cross-platform, runs on Python 3.5+,
 and is easy to install.
 
-Main website: http://imageio.github.io
+Main website: https://imageio.github.io
 """
 
 # flake8: noqa
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
 
 # Load some bits from core
 from .core import FormatManager, RETURN_BYTES
 
 # Instantiate format manager
 formats = FormatManager()
```

### Comparing `imageio-2.8.0/imageio/__main__.py` & `imageio-2.9.0/imageio/__main__.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/core/__init__.py` & `imageio-2.9.0/imageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/core/fetching.py` & `imageio-2.9.0/imageio/core/fetching.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/core/findlib.py` & `imageio-2.9.0/imageio/core/findlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     lib_dirs = lib_dirs or []
 
     # Get system dirs to search
     sys_lib_dirs = [
         "/lib",
         "/usr/lib",
         "/usr/lib/x86_64-linux-gnu",
+        "/usr/lib/aarch64-linux-gnu",
         "/usr/local/lib",
         "/opt/local/lib",
     ]
 
     # Get Python dirs to search (shared if for Pyzo)
     py_sub_dirs = ["lib", "DLLs", "Library/bin", "shared"]
     py_lib_dirs = [os.path.join(sys.prefix, d) for d in py_sub_dirs]
```

### Comparing `imageio-2.8.0/imageio/core/format.py` & `imageio-2.9.0/imageio/core/format.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/core/functions.py` & `imageio-2.9.0/imageio/core/functions.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/core/request.py` & `imageio-2.9.0/imageio/core/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 RETURN_BYTES = "<bytes>"
 
 # Example images that will be auto-downloaded
 EXAMPLE_IMAGES = {
     "astronaut.png": "Image of the astronaut Eileen Collins",
     "camera.png": "Classic grayscale image of a photographer",
     "checkerboard.png": "Black and white image of a chekerboard",
+    "wood.jpg": "A (repeatable) texture of wooden planks",
+    "bricks.jpg": "A (repeatable) texture of stone bricks",
     "clock.png": "Photo of a clock with motion blur (Stefan van der Walt)",
     "coffee.png": "Image of a cup of coffee (Rachel Michetti)",
     "chelsea.png": "Image of Stefan's cat",
     "wikkie.png": "Image of Almar's cat",
     "coins.png": "Image showing greek coins from Pompeii",
     "horse.png": "Image showing the silhouette of a horse (Andreas Preuss)",
     "hubble_deep_field.png": "Photograph taken by Hubble telescope (NASA)",
@@ -49,14 +51,15 @@
     "page.png": "A scanned page of text",
     "text.png": "A photograph of handdrawn text",
     "chelsea.zip": "The chelsea.png in a zipfile (for testing)",
     "chelsea.bsdf": "The chelsea.png in a BSDF file(for testing)",
     "newtonscradle.gif": "Animated GIF of a newton's cradle",
     "cockatoo.mp4": "Video file of a cockatoo",
     "stent.npz": "Volumetric image showing a stented abdominal aorta",
+    "meadow_cube.jpg": "A cubemap image of a meadow, e.g. to render a skybox.",
 }
 
 
 class Request(object):
     """ Request(uri, mode, **kwargs)
 
     Represents a request for reading or saving an image resource. This
@@ -340,15 +343,18 @@
                 # Open zipfile and open new file object for specific file
                 self._zipfile = zipfile.ZipFile(filename, "r")
                 self._file = self._zipfile.open(name, "r")
                 self._file = SeekableFileObject(self._file)
 
         elif self._uri_type in [URI_HTTP or URI_FTP]:
             assert not want_to_write  # This should have been tested in init
-            self._file = urlopen(self.filename, timeout=5)
+            timeout = os.getenv('IMAGEIO_REQUEST_TIMEOUT')
+            if timeout is None or not timeout.isdigit():
+                timeout = 5
+            self._file = urlopen(self.filename, timeout=float(timeout))
             self._file = SeekableFileObject(self._file)
 
         return self._file
 
     def get_local_filename(self):
         """ get_local_filename()
         If the filename is an existing file on this filesystem, return
```

### Comparing `imageio-2.8.0/imageio/core/util.py` & `imageio-2.9.0/imageio/core/util.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/__init__.py` & `imageio-2.9.0/imageio/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/_bsdf.py` & `imageio-2.9.0/imageio/plugins/_bsdf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/_dicom.py` & `imageio-2.9.0/imageio/plugins/_dicom.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/_freeimage.py` & `imageio-2.9.0/imageio/plugins/_freeimage.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/_swf.py` & `imageio-2.9.0/imageio/plugins/_swf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/_tifffile.py` & `imageio-2.9.0/imageio/plugins/_tifffile.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/bsdf.py` & `imageio-2.9.0/imageio/plugins/bsdf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/dicom.py` & `imageio-2.9.0/imageio/plugins/dicom.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,34 +43,70 @@
         "c:\\dcmtk",
         "c:\\Program Files",
         "c:\\Program Files\\dcmtk",
         "c:\\Program Files (x86)\\dcmtk",
     ):
         filename = os.path.join(dir, fname)
         if os.path.isfile(filename):
-            return filename
+            return [filename]
 
     try:
         subprocess.check_call([fname, "--version"])
-        return fname
+        return [fname]
     except Exception:
         return None
 
 
+def get_gdcmconv_exe():
+    fname = "gdcmconv" + ".exe" * sys.platform.startswith("win")
+    # Maybe it's on the path
+    try:
+        subprocess.check_call([fname, "--version"])
+        return [fname, "--raw"]
+    except Exception:
+        pass
+    # Select directories where it could be
+    candidates = []
+    base_dirs = [r"c:\Program Files"]
+    for base_dir in base_dirs:
+        if os.path.isdir(base_dir):
+            for dname in os.listdir(base_dir):
+                if dname.lower().startswith("gdcm"):
+                    suffix = dname[4:].strip()
+                    candidates.append((suffix, os.path.join(base_dir, dname)))
+    # Sort, so higher versions are tried earlier
+    candidates.sort(reverse=True)
+    # Select executable
+    filename = None
+    for _, dirname in candidates:
+        exe1 = os.path.join(dirname, "gdcmconv.exe")
+        exe2 = os.path.join(dirname, "bin", "gdcmconv.exe")
+        if os.path.isfile(exe1):
+            filename = exe1
+            break
+        if os.path.isfile(exe2):
+            filename = exe2
+            break
+    else:
+        return None
+    return [filename, "--raw"]
+
+
 class DicomFormat(Format):
     """ A format for reading DICOM images: a common format used to store
     medical image data, such as X-ray, CT and MRI.
 
-    This format borrows some code (and ideas) from the pydicom project,
-    and (to the best of our knowledge) has the same limitations as
-    pydicom with regard to the type of files that it can handle. However,
+    This format borrows some code (and ideas) from the pydicom project. However,
     only a predefined subset of tags are extracted from the file. This allows
     for great simplifications allowing us to make a stand-alone reader, and
-    also results in a much faster read time. We plan to allow reading all
-    tags in the future (by using pydicom).
+    also results in a much faster read time.
+
+    By default, only uncompressed and deflated transfer syntaxes are supported.
+    If gdcm or dcmtk is installed, these will be used to automatically convert
+    the data. See https://github.com/malaterre/GDCM/releases for installing GDCM.
 
     This format provides functionality to group images of the same
     series together, thus extracting volumes (and multiple volumes).
     Using volread will attempt to yield a volume. If multiple volumes
     are present, the first one is given. Using mimread will simply yield
     all images in the given directory (not taking series into account).
 
@@ -103,43 +139,55 @@
         # We cannot save yet. May be possible if we will used pydicom as
         # a backend.
         return False
 
     # --
 
     class Reader(Format.Reader):
+
+        _compressed_warning_dirs = set()
+
         def _open(self, progress=True):
             if not _dicom:
                 load_lib()
             if os.path.isdir(self.request.filename):
                 # A dir can be given if the user used the format explicitly
                 self._info = {}
                 self._data = None
             else:
                 # Read the given dataset now ...
                 try:
                     dcm = _dicom.SimpleDicomReader(self.request.get_file())
                 except _dicom.CompressedDicom as err:
-                    if "JPEG" in str(err):
-                        exe = get_dcmdjpeg_exe()
-                        if not exe:
-                            raise
+                    # We cannot do this on our own. Perhaps with some help ...
+                    cmd = get_gdcmconv_exe()
+                    if not cmd and "JPEG" in str(err):
+                        cmd = get_dcmdjpeg_exe()
+                    if not cmd:
+                        msg = err.args[0].replace("using", "installing")
+                        msg = msg.replace("convert", "auto-convert")
+                        err.args = (msg,)
+                        raise
+                    else:
                         fname1 = self.request.get_local_filename()
                         fname2 = fname1 + ".raw"
                         try:
-                            subprocess.check_call([exe, fname1, fname2])
+                            subprocess.check_call(cmd + [fname1, fname2])
                         except Exception:
                             raise err
-                        logger.warning(
-                            "DICOM file contained compressed data. "
-                            "Used dcmtk to convert it."
-                        )
+                        d = os.path.dirname(fname1)
+                        if d not in self._compressed_warning_dirs:
+                            self._compressed_warning_dirs.add(d)
+                            logger.warning(
+                                "DICOM file contained compressed data. "
+                                + "Autoconverting with "
+                                + cmd[0]
+                                + " (this warning is shown once for each directory)"
+                            )
                         dcm = _dicom.SimpleDicomReader(fname2)
-                    else:
-                        raise
 
                 self._info = dcm._info
                 self._data = dcm.get_numpy_array()
 
             # Initialize series, list of DicomSeries objects
             self._series = None  # only created if needed
```

### Comparing `imageio-2.8.0/imageio/plugins/example.py` & `imageio-2.9.0/imageio/plugins/example.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/feisem.py` & `imageio-2.9.0/imageio/plugins/feisem.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,28 +52,28 @@
             metadata : dict
                 Dictionary of metadata.
             """
             md = {"root": {}}
             current_tag = "root"
             reading_metadata = False
             filename = self.request.get_local_filename()
-            with open(filename, "rb") as fin:
+            with open(filename, encoding="utf8", errors="ignore") as fin:
                 for line in fin:
                     if not reading_metadata:
-                        if not line.startswith(b"Date="):
+                        if not line.startswith("Date="):
                             continue
                         else:
                             reading_metadata = True
-                    line = line.rstrip().decode()
+                    line = line.rstrip()
                     if line.startswith("["):
                         current_tag = line.lstrip("[").rstrip("]")
                         md[current_tag] = {}
                     else:
-                        if line and line != "\x00":  # ignore blank lines
-                            key, val = line.split("=")
+                        if "=" in line:  # ignore empty and irrelevant lines
+                            key, val = line.split("=", maxsplit=1)
                             for tag_type in (int, float):
                                 try:
                                     val = tag_type(val)
                                 except ValueError:
                                     continue
                                 else:
                                     break
```

### Comparing `imageio-2.8.0/imageio/plugins/ffmpeg.py` & `imageio-2.9.0/imageio/plugins/ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
             # Write "_video"_arg - indicating webcam support
             self.request._video = None
             if self.request.filename in ["<video%i>" % i for i in range(10)]:
                 self.request._video = self.request.filename
             # Specify input framerate?
             if self.request._video:
                 if "-framerate" not in str(self._arg_input_params):
-                    self._arg_input_params.extend(["-framerate", str(float(fps or 15))])
+                    self._arg_input_params.extend(["-framerate", str(float(fps or 30))])
             # Get local filename
             if self.request._video:
                 index = int(self.request._video[-2])
                 self._filename = self._get_cam_inputname(index)
             else:
                 self._filename = self.request.get_local_filename()
                 # When passed to ffmpeg on command line, carets need to be escaped.
@@ -454,15 +454,17 @@
                         if "Unknown input format: 'avfoundation'" in err_text:
                             err_text += (
                                 "Try installing FFMPEG using "
                                 "home brew to get a version with "
                                 "support for cameras."
                             )
                     raise IndexError(
-                        "No camera at {}.\n\n{}".format(self.request._video, err_text)
+                        "No (working) camera at {}.\n\n{}".format(
+                            self.request._video, err_text
+                        )
                     )
                 else:
                     self._meta.update(meta)
             elif index == 0:
                 self._meta.update(self._read_gen.__next__())
             else:
                 self._read_gen.__next__()  # we already have meta data
```

### Comparing `imageio-2.8.0/imageio/plugins/fits.py` & `imageio-2.9.0/imageio/plugins/fits.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/freeimage.py` & `imageio-2.9.0/imageio/plugins/freeimage.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/freeimagemulti.py` & `imageio-2.9.0/imageio/plugins/freeimagemulti.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/gdal.py` & `imageio-2.9.0/imageio/plugins/gdal.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/grab.py` & `imageio-2.9.0/imageio/plugins/grab.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/lytro.py` & `imageio-2.9.0/imageio/plugins/lytro.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/npz.py` & `imageio-2.9.0/imageio/plugins/npz.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/pillow.py` & `imageio-2.9.0/imageio/plugins/pillow.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/pillow_info.py` & `imageio-2.9.0/imageio/plugins/pillow_info.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/pillowmulti.py` & `imageio-2.9.0/imageio/plugins/pillowmulti.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/simpleitk.py` & `imageio-2.9.0/imageio/plugins/simpleitk.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     ".mha",
     ".mhd",
     ".nhdr",
     "nia",
     "hdr",
     ".nrrd",
     ".nii",
+    ".nii.gz",
+    ".img",
+    ".img.gz",
     ".vtk",
     "hdf5",
     "lsm",
     "mnc",
     "mnc2",
     "mgh",
     "mnc",
@@ -102,18 +105,23 @@
             return True
         if has_module("itk.ImageIOBase") or has_module("SimpleITK"):
             return request.extension in ALL_FORMATS
 
     # -- reader
 
     class Reader(Format.Reader):
-        def _open(self, **kwargs):
+        def _open(self, pixel_type=None, fallback_only=None, **kwargs):
             if not _itk:
                 load_lib()
-            self._img = _read_function(self.request.get_local_filename())
+            args = ()
+            if pixel_type is not None:
+                args += (pixel_type,)
+                if fallback_only is not None:
+                    args += (fallback_only,)
+            self._img = _read_function(self.request.get_local_filename(), *args)
 
         def _get_length(self):
             return 1
 
         def _close(self):
             pass
```

### Comparing `imageio-2.8.0/imageio/plugins/spe.py` & `imageio-2.9.0/imageio/plugins/spe.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/swf.py` & `imageio-2.9.0/imageio/plugins/swf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/plugins/tifffile.py` & `imageio-2.9.0/imageio/plugins/tifffile.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/astronaut.png` & `imageio-2.9.0/imageio/resources/images/astronaut.png`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/chelsea.png` & `imageio-2.9.0/imageio/resources/images/chelsea.png`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/chelsea.zip` & `imageio-2.9.0/imageio/resources/images/chelsea.zip`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/cockatoo.mp4` & `imageio-2.9.0/imageio/resources/images/cockatoo.mp4`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/newtonscradle.gif` & `imageio-2.9.0/imageio/resources/images/newtonscradle.gif`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/realshort.mp4` & `imageio-2.9.0/imageio/resources/images/realshort.mp4`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/resources/images/stent.npz` & `imageio-2.9.0/imageio/resources/images/stent.npz`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/imageio/testing.py` & `imageio-2.9.0/imageio/testing.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/setup.py` & `imageio-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
 
     >>> import imageio
     >>> im = imageio.imread('imageio:astronaut.png')
     >>> im.shape  # im is a numpy array
     (512, 512, 3)
     >>> imageio.imwrite('astronaut-gray.jpg', im[:, :, 0])
 
-See the `user API <http://imageio.readthedocs.io/en/latest/userapi.html>`_
-or `examples <http://imageio.readthedocs.io/en/latest/examples.html>`_
+See the `user API <https://imageio.readthedocs.io/en/stable/userapi.html>`_
+or `examples <https://imageio.readthedocs.io/en/stable/examples.html>`_
 for more information.
 """
 
 # Prepare resources dir
 package_data = [
     "resources/shipped_resources_go_here",
     "resources/*.*",
```

### Comparing `imageio-2.8.0/tests/test_bsdf.py` & `imageio-2.9.0/tests/test_bsdf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_core.py` & `imageio-2.9.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_dicom.py` & `imageio-2.9.0/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_fei_tiff.py` & `imageio-2.9.0/tests/test_fei_tiff.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_ffmpeg.py` & `imageio-2.9.0/tests/test_ffmpeg.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from io import BytesIO
 import os
 import sys
 import gc
 import time
 import threading
-
+import platform
 import psutil
 
 import numpy as np
 
 from pytest import raises, skip
 from imageio.testing import run_tests_if_main, get_test_dir
 
@@ -38,30 +38,33 @@
 
 
 def setup_module():
     pass
 
 
 def test_get_exe_installed():
-    import imageio_ffmpeg
-
-    # backup any user-defined path
-    if "IMAGEIO_FFMPEG_EXE" in os.environ:
-        oldpath = os.environ["IMAGEIO_FFMPEG_EXE"]
+    if platform.machine() == "aarch64":
+        skip("Skip for aarch64")
     else:
-        oldpath = ""
-    # Test if download works
-    os.environ["IMAGEIO_FFMPEG_EXE"] = ""
-    path = imageio_ffmpeg.get_ffmpeg_exe()
-    # cleanup
-    os.environ.pop("IMAGEIO_FFMPEG_EXE")
-    if oldpath:
-        os.environ["IMAGEIO_FFMPEG_EXE"] = oldpath
-    print(path)
-    assert os.path.isfile(path)
+        import imageio_ffmpeg
+
+        # backup any user-defined path
+        if "IMAGEIO_FFMPEG_EXE" in os.environ:
+            oldpath = os.environ["IMAGEIO_FFMPEG_EXE"]
+        else:
+            oldpath = ""
+        # Test if download works
+        os.environ["IMAGEIO_FFMPEG_EXE"] = ""
+        path = imageio_ffmpeg.get_ffmpeg_exe()
+        # cleanup
+        os.environ.pop("IMAGEIO_FFMPEG_EXE")
+        if oldpath:
+            os.environ["IMAGEIO_FFMPEG_EXE"] = oldpath
+        print(path)
+        assert os.path.isfile(path)
 
 
 def test_get_exe_env():
     import imageio_ffmpeg
 
     # backup any user-defined path
     if "IMAGEIO_FFMPEG_EXE" in os.environ:
```

### Comparing `imageio-2.8.0/tests/test_ffmpeg_info.py` & `imageio-2.9.0/tests/test_ffmpeg_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,22 @@
     device_names = imageio.plugins.ffmpeg.parse_device_names(sample)
 
     # Assert that the device_names list has the correct length
     assert len(device_names) == 2
 
 
 def test_overload_fps():
-
     need_internet()
 
     # Native
     r = imageio.get_reader("imageio:cockatoo.mp4")
     assert r.count_frames() == 280  # native
     assert int(r._meta["fps"] * r._meta["duration"] + 0.5) == 280
     ims = [im for im in r]
-    assert len(ims) == 280
+    assert len(ims) in (280, 281)
     # imageio.mimwrite('~/parot280.gif', ims[:30])
 
     # Less
     r = imageio.get_reader("imageio:cockatoo.mp4", fps=8)
     # assert r.count_frames() == 112  # cant :(
     assert int(r._meta["fps"] * r._meta["duration"] + 0.5) == 112  # note the mismatch
     ims = [im for im in r]
@@ -72,15 +71,15 @@
     # imageio.mimwrite('~/parot112.gif', ims[:30])
 
     # More
     r = imageio.get_reader("imageio:cockatoo.mp4", fps=24)
     # assert r.count_frames() == 336  # cant :(
     ims = [im for im in r]
     assert int(r._meta["fps"] * r._meta["duration"] + 0.5) == 336
-    assert len(ims) == 336
+    assert len(ims) in (336, 337)
     # imageio.mimwrite('~/parot336.gif', ims[:30])
 
     # Do we calculate nframes correctly? To be fair, the reader wont try to
     # read beyond what it thinks how many frames it has. But this at least
     # makes sure that this works.
     for fps in (8.0, 8.02, 8.04, 8.06, 8.08):
         r = imageio.get_reader("imageio:cockatoo.mp4", fps=fps)
```

### Comparing `imageio-2.8.0/tests/test_fits.py` & `imageio-2.9.0/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_format.py` & `imageio-2.9.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_freeimage.py` & `imageio-2.9.0/tests/test_freeimage.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_freeimage_suite.py` & `imageio-2.9.0/tests/test_freeimage_suite.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_gdal.py` & `imageio-2.9.0/tests/test_gdal.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_grab.py` & `imageio-2.9.0/tests/test_grab.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_lytro.py` & `imageio-2.9.0/tests/test_lytro.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_meta.py` & `imageio-2.9.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_npz.py` & `imageio-2.9.0/tests/test_npz.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_pillow.py` & `imageio-2.9.0/tests/test_pillow.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_simpleitk.py` & `imageio-2.9.0/tests/test_simpleitk.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_spe.py` & `imageio-2.9.0/tests/test_spe.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_swf.py` & `imageio-2.9.0/tests/test_swf.py`

 * *Files identical despite different names*

### Comparing `imageio-2.8.0/tests/test_tifffile.py` & `imageio-2.9.0/tests/test_tifffile.py`

 * *Files identical despite different names*

