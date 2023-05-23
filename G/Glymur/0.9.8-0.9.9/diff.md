# Comparing `tmp/Glymur-0.9.8.tar.gz` & `tmp/Glymur-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Glymur-0.9.8.tar", last modified: Thu Mar 10 23:09:56 2022, max compression
+gzip compressed data, was "Glymur-0.9.9.tar", last modified: Thu Mar 24 13:44:28 2022, max compression
```

## Comparing `Glymur-0.9.8.tar` & `Glymur-0.9.9.tar`

### file list

```diff
@@ -1,137 +1,62 @@
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.297246 Glymur-0.9.8/
--rw-r--r--   0 jevans     (501) staff       (20)       55 2022-02-01 23:09:41.000000 Glymur-0.9.8/.gitignore
--rw-r--r--   0 jevans     (501) staff       (20)      102 2022-02-01 23:09:41.000000 Glymur-0.9.8/.readthedocs.yml
--rw-r--r--   0 jevans     (501) staff       (20)      881 2022-02-01 23:09:41.000000 Glymur-0.9.8/.travis.yml
--rw-r--r--   0 jevans     (501) staff       (20)     8955 2022-03-07 18:18:35.000000 Glymur-0.9.8/CHANGES.txt
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.080616 Glymur-0.9.8/Glymur.egg-info/
--rw-r--r--   0 jevans     (501) staff       (20)      940 2022-03-10 23:09:55.000000 Glymur-0.9.8/Glymur.egg-info/PKG-INFO
--rw-r--r--   0 jevans     (501) staff       (20)     3313 2022-03-10 23:09:56.000000 Glymur-0.9.8/Glymur.egg-info/SOURCES.txt
--rw-r--r--   0 jevans     (501) staff       (20)        1 2022-03-10 23:09:55.000000 Glymur-0.9.8/Glymur.egg-info/dependency_links.txt
--rw-r--r--   0 jevans     (501) staff       (20)       93 2022-03-10 23:09:55.000000 Glymur-0.9.8/Glymur.egg-info/entry_points.txt
--rw-r--r--   0 jevans     (501) staff       (20)        1 2021-12-22 22:45:26.000000 Glymur-0.9.8/Glymur.egg-info/not-zip-safe
--rw-r--r--   0 jevans     (501) staff       (20)       32 2022-03-10 23:09:55.000000 Glymur-0.9.8/Glymur.egg-info/requires.txt
--rw-r--r--   0 jevans     (501) staff       (20)       13 2022-03-10 23:09:56.000000 Glymur-0.9.8/Glymur.egg-info/top_level.txt
--rw-r--r--   0 jevans     (501) staff       (20)     1077 2018-05-12 12:02:44.000000 Glymur-0.9.8/LICENSE.txt
--rw-r--r--   0 jevans     (501) staff       (20)       92 2017-08-16 00:45:39.000000 Glymur-0.9.8/MANIFEST.in
--rw-r--r--   0 jevans     (501) staff       (20)      940 2022-03-10 23:09:56.297409 Glymur-0.9.8/PKG-INFO
--rw-r--r--   0 jevans     (501) staff       (20)      317 2022-02-01 23:09:41.000000 Glymur-0.9.8/README.md
--rw-r--r--   0 jevans     (501) staff       (20)     2828 2022-02-01 23:09:41.000000 Glymur-0.9.8/appveyor.yml
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.106471 Glymur-0.9.8/ci/
--rw-r--r--   0 jevans     (501) staff       (20)      127 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/doc.yml
--rw-r--r--   0 jevans     (501) staff       (20)     2970 2017-09-04 17:30:30.000000 Glymur-0.9.8/ci/install.ps1
--rwxr-xr-x   0 jevans     (501) staff       (20)      313 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/run_script.sh
--rw-r--r--   0 jevans     (501) staff       (20)     3600 2017-09-04 17:30:30.000000 Glymur-0.9.8/ci/run_with_env.cmd
--rwxr-xr-x   0 jevans     (501) staff       (20)     1782 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/setup_env.sh
--rw-r--r--   0 jevans     (501) staff       (20)      142 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-37-no-gdal.yaml
--rw-r--r--   0 jevans     (501) staff       (20)      148 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-37-no-opj.yaml
--rw-r--r--   0 jevans     (501) staff       (20)      172 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-37.yaml
--rw-r--r--   0 jevans     (501) staff       (20)      173 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-38.yaml
--rw-r--r--   0 jevans     (501) staff       (20)      154 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-39-opj2p4.yaml
--rw-r--r--   0 jevans     (501) staff       (20)      171 2022-02-01 23:09:41.000000 Glymur-0.9.8/ci/travis-39.yaml
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.110159 Glymur-0.9.8/docs/
--rw-r--r--   0 jevans     (501) staff       (20)     5573 2017-08-16 00:45:39.000000 Glymur-0.9.8/docs/Makefile
--rw-r--r--   0 jevans     (501) staff       (20)     5105 2017-08-16 00:45:39.000000 Glymur-0.9.8/docs/make.bat
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.142527 Glymur-0.9.8/docs/source/
--rw-r--r--   0 jevans     (501) staff       (20)     8632 2022-03-07 18:18:35.000000 Glymur-0.9.8/docs/source/conf.py
--rw-r--r--   0 jevans     (501) staff       (20)     2122 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/detailed_installation.rst
--rw-r--r--   0 jevans     (501) staff       (20)   491899 2017-08-16 00:45:39.000000 Glymur-0.9.8/docs/source/goodstuff_alpha.png
--rw-r--r--   0 jevans     (501) staff       (20)    32741 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/how_do_i.rst
--rw-r--r--   0 jevans     (501) staff       (20)      559 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/index.rst
--rw-r--r--   0 jevans     (501) staff       (20)     1144 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/introduction.rst
--rw-r--r--   0 jevans     (501) staff       (20)      480 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/roadmap.rst
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.155953 Glymur-0.9.8/docs/source/whatsnew/
--rw-r--r--   0 jevans     (501) staff       (20)     1524 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/whatsnew/0.5.rst
--rw-r--r--   0 jevans     (501) staff       (20)      929 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/whatsnew/0.6.rst
--rw-r--r--   0 jevans     (501) staff       (20)      676 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/whatsnew/0.7.rst
--rw-r--r--   0 jevans     (501) staff       (20)     3374 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/whatsnew/0.8.rst
--rw-r--r--   0 jevans     (501) staff       (20)     2161 2022-03-07 18:18:35.000000 Glymur-0.9.8/docs/source/whatsnew/0.9.rst
--rw-r--r--   0 jevans     (501) staff       (20)      212 2022-02-01 23:09:41.000000 Glymur-0.9.8/docs/source/whatsnew/index.rst
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.182097 Glymur-0.9.8/glymur/
--rw-r--r--   0 jevans     (501) staff       (20)      554 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/__init__.py
--rw-r--r--   0 jevans     (501) staff       (20)     4158 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/_iccprofile.py
--rw-r--r--   0 jevans     (501) staff       (20)    12587 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/_tiff.py
--rw-r--r--   0 jevans     (501) staff       (20)    59378 2022-02-04 00:50:46.000000 Glymur-0.9.8/glymur/codestream.py
--rw-r--r--   0 jevans     (501) staff       (20)     5458 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/command_line.py
--rw-r--r--   0 jevans     (501) staff       (20)     4366 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/config.py
--rw-r--r--   0 jevans     (501) staff       (20)     3639 2019-04-11 12:23:44.000000 Glymur-0.9.8/glymur/core.py
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.203037 Glymur-0.9.8/glymur/data/
--rw-r--r--   0 jevans     (501) staff       (20)     1031 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/data/__init__.py
--rw-r--r--   0 jevans     (501) staff       (20)   115220 2017-08-16 00:45:39.000000 Glymur-0.9.8/glymur/data/goodstuff.j2k
--rw-r--r--   0 jevans     (501) staff       (20)  1399071 2017-08-16 00:45:39.000000 Glymur-0.9.8/glymur/data/heliov.jpx
--rw-r--r--   0 jevans     (501) staff       (20)  1135519 2021-09-01 23:33:33.000000 Glymur-0.9.8/glymur/data/nemo.jp2
--rw-r--r--   0 jevans     (501) staff       (20)   111784 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/jp2box.py
--rw-r--r--   0 jevans     (501) staff       (20)    78955 2022-03-04 18:09:09.000000 Glymur-0.9.8/glymur/jp2k.py
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.219051 Glymur-0.9.8/glymur/lib/
--rw-r--r--   0 jevans     (501) staff       (20)      124 2022-02-01 22:43:51.000000 Glymur-0.9.8/glymur/lib/__init__.py
--rw-r--r--   0 jevans     (501) staff       (20)    43699 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/lib/openjp2.py
--rw-r--r--   0 jevans     (501) staff       (20)    36342 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/lib/tiff.py
--rw-r--r--   0 jevans     (501) staff       (20)     6393 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/options.py
--rw-r--r--   0 jevans     (501) staff       (20)    24820 2022-02-01 23:09:41.000000 Glymur-0.9.8/glymur/tiff.py
--rw-r--r--   0 jevans     (501) staff       (20)      981 2022-03-07 18:18:35.000000 Glymur-0.9.8/glymur/version.py
--rw-r--r--   0 jevans     (501) staff       (20)       90 2022-02-01 23:09:41.000000 Glymur-0.9.8/pyproject.toml
--rw-r--r--   0 jevans     (501) staff       (20)     1157 2022-03-10 23:09:56.298179 Glymur-0.9.8/setup.cfg
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.249201 Glymur-0.9.8/tests/
--rw-r--r--   0 jevans     (501) staff       (20)       56 2022-02-01 22:43:51.000000 Glymur-0.9.8/tests/__init__.py
-drwxr-xr-x   0 jevans     (501) staff       (20)        0 2022-03-10 23:09:56.296271 Glymur-0.9.8/tests/data/
--rw-r--r--   0 jevans     (501) staff       (20)        0 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/__init__.py
--rw-r--r--   0 jevans     (501) staff       (20)    65888 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/albers27-8.tif
--rw-r--r--   0 jevans     (501) staff       (20)    66643 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/albers27.tif
--rw-r--r--   0 jevans     (501) staff       (20)      353 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/decompression_parameters_type.txt
--rw-r--r--   0 jevans     (501) staff       (20)     1526 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/default_compression_parameters_type.txt
--rw-r--r--   0 jevans     (501) staff       (20)      494 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/default_progression_order_changes_type.txt
--rwxr-xr-x   0 jevans     (501) staff       (20)      499 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/degenerate_geotiff.tif
--rw-r--r--   0 jevans     (501) staff       (20)    17959 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/edf_c2_1178956.jp2
--rw-r--r--   0 jevans     (501) staff       (20)     1769 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/encoding_declaration.xml
--rw-r--r--   0 jevans     (501) staff       (20)      409 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/file1_xml.txt
--rw-r--r--   0 jevans     (501) staff       (20)      460 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/file1_xml_box.txt
--rw-r--r--   0 jevans     (501) staff       (20)    12927 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/flower-separated-planar-08.tif
--rw-r--r--   0 jevans     (501) staff       (20)     1234 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/geotiff_uuid.txt
--rw-r--r--   0 jevans     (501) staff       (20)     1312 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/geotiff_uuid_proj6.txt
--rw-r--r--   0 jevans     (501) staff       (20)     1645 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/goodstuff_codestream_header.txt
--rw-r--r--   0 jevans     (501) staff       (20)     3880 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/goodstuff_with_full_header.txt
--rw-r--r--   0 jevans     (501) staff       (20)    41308 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/issue142.j2k
--rw-r--r--   0 jevans     (501) staff       (20)      842 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/issue186_progression_order.txt
--rw-r--r--   0 jevans     (501) staff       (20)      414 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/issue392.jp2
--rw-r--r--   0 jevans     (501) staff       (20)      404 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/issue396.jp2
--rw-r--r--   0 jevans     (501) staff       (20)      380 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/issue398.dat
--rw-r--r--   0 jevans     (501) staff       (20)       80 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/issue405.dat
--rw-r--r--   0 jevans     (501) staff       (20)      625 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/issue438.jp2
--rw-r--r--   0 jevans     (501) staff       (20)      880 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/multiple_precinct_size.txt
--rw-r--r--   0 jevans     (501) staff       (20)     7772 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo.txt
--rw-r--r--   0 jevans     (501) staff       (20)     4102 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_dump_no_codestream.txt
--rw-r--r--   0 jevans     (501) staff       (20)      622 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_dump_no_codestream_no_xml.txt
--rw-r--r--   0 jevans     (501) staff       (20)     2228 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_dump_no_xml.txt
--rw-r--r--   0 jevans     (501) staff       (20)      272 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_dump_short.txt
--rw-r--r--   0 jevans     (501) staff       (20)     5708 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_with_codestream_header.txt
--rw-r--r--   0 jevans     (501) staff       (20)     3562 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/nemo_xmp_box.txt
--rw-r--r--   0 jevans     (501) staff       (20)     6183 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/p0_02.j2k
--rw-r--r--   0 jevans     (501) staff       (20)    12845 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/p0_03.j2k
--rw-r--r--   0 jevans     (501) staff       (20)    33826 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/p0_06.j2k
--rw-r--r--   0 jevans     (501) staff       (20)     3356 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/p1_06.j2k
--rw-r--r--   0 jevans     (501) staff       (20)      569 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/p1_07.j2k
--rw-r--r--   0 jevans     (501) staff       (20)      674 2022-02-01 23:09:41.000000 Glymur-0.9.8/tests/data/p1_07.txt
--rw-r--r--   0 jevans     (501) staff       (20)      416 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/sgray.icc
--rw-r--r--   0 jevans     (501) staff       (20)      410 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/data/simple_rdf.txt
--rw-r--r--   0 jevans     (501) staff       (20)    29911 2017-09-04 17:30:30.000000 Glymur-0.9.8/tests/data/text_GBR.jp2
--rw-r--r--   0 jevans     (501) staff       (20)      764 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/data/text_GBR_rreq.txt
--rw-r--r--   0 jevans     (501) staff       (20)      920 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/data/text_gbr_34.txt
--rw-r--r--   0 jevans     (501) staff       (20)     1134 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/data/text_gbr_35.txt
--rw-r--r--   0 jevans     (501) staff       (20)     5814 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/fixtures.py
--rw-r--r--   0 jevans     (501) staff       (20)     3032 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_callbacks.py
--rw-r--r--   0 jevans     (501) staff       (20)     5038 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_cinema.py
--rw-r--r--   0 jevans     (501) staff       (20)     5956 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_codestream.py
--rw-r--r--   0 jevans     (501) staff       (20)     7974 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_colour_specification_box.py
--rw-r--r--   0 jevans     (501) staff       (20)     9487 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_config.py
--rw-r--r--   0 jevans     (501) staff       (20)    51085 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_jp2box.py
--rw-r--r--   0 jevans     (501) staff       (20)    24233 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_jp2box_jpx.py
--rw-r--r--   0 jevans     (501) staff       (20)    13523 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_jp2box_uuid.py
--rw-r--r--   0 jevans     (501) staff       (20)     9438 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_jp2box_xml.py
--rw-r--r--   0 jevans     (501) staff       (20)    85855 2022-03-04 18:09:09.000000 Glymur-0.9.8/tests/test_jp2k.py
--rw-r--r--   0 jevans     (501) staff       (20)     1985 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_libtiff.py
--rw-r--r--   0 jevans     (501) staff       (20)    20378 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_openjp2.py
--rw-r--r--   0 jevans     (501) staff       (20)    63836 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_printing.py
--rw-r--r--   0 jevans     (501) staff       (20)     5364 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_set_decoded_components.py
--rw-r--r--   0 jevans     (501) staff       (20)    13753 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_slicing.py
--rw-r--r--   0 jevans     (501) staff       (20)    45137 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_tiff2jp2.py
--rw-r--r--   0 jevans     (501) staff       (20)    31567 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_warnings.py
--rw-r--r--   0 jevans     (501) staff       (20)     6131 2022-02-01 23:09:42.000000 Glymur-0.9.8/tests/test_writing_tiles.py
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.454928 Glymur-0.9.9/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     9040 2022-03-24 13:43:18.000000 Glymur-0.9.9/CHANGES.txt
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.448928 Glymur-0.9.9/Glymur.egg-info/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      940 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/PKG-INFO
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     1174 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/SOURCES.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)        1 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/dependency_links.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       93 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/entry_points.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)        1 2022-03-21 13:38:55.000000 Glymur-0.9.9/Glymur.egg-info/not-zip-safe
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       32 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/requires.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       13 2022-03-24 13:44:28.000000 Glymur-0.9.9/Glymur.egg-info/top_level.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     1077 2020-01-31 05:09:13.000000 Glymur-0.9.9/LICENSE.txt
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       92 2020-01-31 05:09:13.000000 Glymur-0.9.9/MANIFEST.in
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      940 2022-03-24 13:44:28.454928 Glymur-0.9.9/PKG-INFO
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      317 2021-11-05 11:55:58.000000 Glymur-0.9.9/README.md
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.449928 Glymur-0.9.9/glymur/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      554 2021-11-05 11:53:20.000000 Glymur-0.9.9/glymur/__init__.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     4158 2021-08-13 15:59:15.000000 Glymur-0.9.9/glymur/_iccprofile.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    12587 2021-11-05 11:53:20.000000 Glymur-0.9.9/glymur/_tiff.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    59378 2022-01-10 20:30:47.000000 Glymur-0.9.9/glymur/codestream.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     5458 2021-11-05 11:53:20.000000 Glymur-0.9.9/glymur/command_line.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     4366 2021-11-05 11:55:58.000000 Glymur-0.9.9/glymur/config.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     3639 2021-08-13 15:59:15.000000 Glymur-0.9.9/glymur/core.py
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.451928 Glymur-0.9.9/glymur/data/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     1031 2021-10-20 16:30:04.000000 Glymur-0.9.9/glymur/data/__init__.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)   115220 2020-01-31 05:09:13.000000 Glymur-0.9.9/glymur/data/goodstuff.j2k
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)  1399071 2020-01-31 05:09:13.000000 Glymur-0.9.9/glymur/data/heliov.jpx
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)  1135519 2020-01-31 05:09:13.000000 Glymur-0.9.9/glymur/data/nemo.jp2
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)   111784 2021-11-05 11:53:20.000000 Glymur-0.9.9/glymur/jp2box.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    78955 2022-01-10 20:30:47.000000 Glymur-0.9.9/glymur/jp2k.py
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.452928 Glymur-0.9.9/glymur/lib/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      124 2021-08-13 15:59:15.000000 Glymur-0.9.9/glymur/lib/__init__.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    43699 2021-11-05 11:55:58.000000 Glymur-0.9.9/glymur/lib/openjp2.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    36342 2022-03-23 17:33:26.000000 Glymur-0.9.9/glymur/lib/tiff.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     6393 2021-08-13 15:59:15.000000 Glymur-0.9.9/glymur/options.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    28601 2022-03-24 13:43:18.000000 Glymur-0.9.9/glymur/tiff.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)      981 2022-03-24 13:43:18.000000 Glymur-0.9.9/glymur/version.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       90 2022-01-10 20:30:47.000000 Glymur-0.9.9/pyproject.toml
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     1157 2022-03-24 13:44:28.455928 Glymur-0.9.9/setup.cfg
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.454928 Glymur-0.9.9/tests/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)       56 2021-08-13 15:59:15.000000 Glymur-0.9.9/tests/__init__.py
+drwxrwxr-x   0 jevans    (1000) jevans    (1000)        0 2022-03-24 13:44:28.454928 Glymur-0.9.9/tests/data/
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)        0 2021-08-13 15:59:15.000000 Glymur-0.9.9/tests/data/__init__.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     5814 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/fixtures.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     3032 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_callbacks.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     5038 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_cinema.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     5956 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_codestream.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     7974 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_colour_specification_box.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     9487 2021-11-05 11:55:58.000000 Glymur-0.9.9/tests/test_config.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    51085 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_jp2box.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    24233 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_jp2box_jpx.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    13523 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_jp2box_uuid.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     9438 2021-10-20 16:30:04.000000 Glymur-0.9.9/tests/test_jp2box_xml.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    85855 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_jp2k.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     1985 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_libtiff.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    20378 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_openjp2.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    63836 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_printing.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     5364 2021-11-05 11:55:58.000000 Glymur-0.9.9/tests/test_set_decoded_components.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    13753 2021-11-05 11:53:20.000000 Glymur-0.9.9/tests/test_slicing.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    45137 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_tiff2jp2.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)    31567 2021-10-20 16:30:04.000000 Glymur-0.9.9/tests/test_warnings.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     6131 2022-01-10 20:30:47.000000 Glymur-0.9.9/tests/test_writing_tiles.py
+-rw-rw-r--   0 jevans    (1000) jevans    (1000)     2621 2021-11-11 22:21:13.000000 Glymur-0.9.9/wisconsin.txt
```

### Comparing `Glymur-0.9.8/CHANGES.txt` & `Glymur-0.9.9/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+March 23, 2022 - v0.9.9
+    Fix bug retrieving some TIFF tags on big endian systems
+
 March 5, 2022 - v0.9.8
     Fix install requirements
 
 January 9, 2022 - v0.9.7.post1
     Fix setup.cfg issue
 
 December 27, 2021 - v0.9.7
```

### Comparing `Glymur-0.9.8/Glymur.egg-info/PKG-INFO` & `Glymur-0.9.9/Glymur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glymur
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/quintusdias/glymur
 Author: 'John Evans'
 Author-email: "John Evans" <john.g.evans.ne@gmail.com>
 License: 'MIT'
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `Glymur-0.9.8/LICENSE.txt` & `Glymur-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/PKG-INFO` & `Glymur-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Glymur
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/quintusdias/glymur
 Author: 'John Evans'
 Author-email: "John Evans" <john.g.evans.ne@gmail.com>
 License: 'MIT'
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `Glymur-0.9.8/glymur/__init__.py` & `Glymur-0.9.9/glymur/__init__.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/_iccprofile.py` & `Glymur-0.9.9/glymur/_iccprofile.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/_tiff.py` & `Glymur-0.9.9/glymur/_tiff.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/codestream.py` & `Glymur-0.9.9/glymur/codestream.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/command_line.py` & `Glymur-0.9.9/glymur/command_line.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/config.py` & `Glymur-0.9.9/glymur/config.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/core.py` & `Glymur-0.9.9/glymur/core.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/data/__init__.py` & `Glymur-0.9.9/glymur/data/__init__.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/data/goodstuff.j2k` & `Glymur-0.9.9/glymur/data/goodstuff.j2k`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/data/heliov.jpx` & `Glymur-0.9.9/glymur/data/heliov.jpx`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/data/nemo.jp2` & `Glymur-0.9.9/glymur/data/nemo.jp2`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/jp2box.py` & `Glymur-0.9.9/glymur/jp2box.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/jp2k.py` & `Glymur-0.9.9/glymur/jp2k.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/lib/openjp2.py` & `Glymur-0.9.9/glymur/lib/openjp2.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/lib/tiff.py` & `Glymur-0.9.9/glymur/lib/tiff.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/options.py` & `Glymur-0.9.9/glymur/options.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/glymur/tiff.py` & `Glymur-0.9.9/glymur/tiff.py`

 * *Files 15% similar despite different names*

```diff
@@ -67,14 +67,17 @@
 
         self.jp2_filename = jp2_filename
         self.tilesize = tilesize
         self.create_uuid = create_uuid
 
         self.kwargs = kwargs
 
+        self.setup_logging(verbosity)
+
+    def setup_logging(self, verbosity):
         self.logger = logging.getLogger('tiff2jp2')
         self.logger.setLevel(verbosity)
         ch = logging.StreamHandler()
         ch.setLevel(verbosity)
         self.logger.addHandler(ch)
 
     def __enter__(self):
@@ -82,31 +85,34 @@
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         libtiff.close(self.tiff_fp)
 
     def run(self):
 
+        self.get_main_ifd()
         self.copy_image()
 
         if self.create_uuid:
             self.copy_metadata()
 
     def copy_metadata(self):
         """
         Copy over the TIFF IFD.  Place it in a UUID box.  Append to the JPEG
         2000 file.
         """
         # create a bytesio object for the IFD
         b = io.BytesIO()
 
-        with open(self.tiff_filename, 'rb') as tfp:
+        # write this 32-bit header into the UUID, no matter if we had bigtiff
+        # or regular tiff or big endian
+        data = struct.pack('<BBHI', 73, 73, 42, 8)
+        b.write(data)
 
-            endian = self._process_header(b, tfp)
-            self._process_tags(b, tfp, endian)
+        self._process_tags(b)
 
         if self.found_geotiff_tags:
             # geotiff UUID
             uuid = UUID('b14bf8bd-083d-4b43-a5ae-8cd7d5a6ce03')
             payload = b.getvalue()
         else:
             # Make it an exif UUID.
@@ -117,81 +123,154 @@
         # to store the length of the box and the box ID
         box_length = len(payload) + 8
 
         uuid_box = UUIDBox(uuid, payload, box_length)
         with open(self.jp2_filename, mode='ab') as f:
             uuid_box.write(f)
 
-    def _process_tags(self, b, tfp, endian):
+    def get_main_ifd(self):
+        """
+        Read all the tags in the main IFD.  We do it this way because of the
+        difficulty in using TIFFGetFieldDefaulted when the datatype of a tag
+        can differ.
+        """
+
+        with open(self.tiff_filename, 'rb') as tfp:
+
+            self.get_endianness(tfp)
+
+            self.found_geotiff_tags = False
+
+            tag_length = 20 if self.version == _BIGTIFF else 12
+
+            # how many tags?
+            if self.version == _BIGTIFF:
+                buffer = tfp.read(8)
+                num_tags, = struct.unpack(self.endian + 'Q', buffer)
+            else:
+                buffer = tfp.read(2)
+                num_tags, = struct.unpack(self.endian + 'H', buffer)
+
+            # Ok, so now we have the IFD main body, but following that we have
+            # the tag payloads that cannot fit into 4 bytes.
+
+            # the IFD main body in the TIFF.  As it might be big endian, we
+            # cannot just process it as one big chunk.
+            buffer = tfp.read(num_tags * tag_length)
+
+            if self.version == _BIGTIFF:
+                tag_format_str = self.endian + 'HHQQ'
+                tag_payload_offset = 12
+                max_tag_payload_length = 8
+            else:
+                tag_format_str = self.endian + 'HHII'
+                tag_payload_offset = 8
+                max_tag_payload_length = 4
+
+            self.tags = {}
+
+            for idx in range(num_tags):
+
+                self.logger.debug(f'tag #: {idx}')
 
-        self.found_geotiff_tags = False
+                tag_data = buffer[idx * tag_length:(idx + 1) * tag_length]
 
-        tag_length = 20 if self.version == _BIGTIFF else 12
+                tag, dtype, nvalues, offset = struct.unpack(tag_format_str, tag_data)  # noqa : E501
+
+                if tag == 34735:
+                    self.found_geotiff_tags = True
+
+                payload_length = tag_dtype[dtype]['nbytes'] * nvalues
+
+                if payload_length > max_tag_payload_length:
+                    # the payload does not fit into the tag entry, so use the
+                    # offset to seek to that position
+                    current_position = tfp.tell()
+                    tfp.seek(offset)
+                    payload_buffer = tfp.read(payload_length)
+                    tfp.seek(current_position)
+
+                    # read the payload from the TIFF
+                    payload_format = tag_dtype[dtype]['format'] * nvalues
+                    payload = struct.unpack(
+                        self.endian + payload_format, payload_buffer
+                    )
+
+                else:
+                    # the payload DOES fit into the TIFF tag entry
+                    payload_buffer = tag_data[tag_payload_offset:]
+
+                    # read ALL of the payload buffer
+                    payload_format = (
+                        tag_dtype[dtype]['format']
+                        * int(max_tag_payload_length / tag_dtype[dtype]['nbytes'])  # noqa : E501
+                    )
+
+                    payload = struct.unpack(
+                        self.endian + payload_format, payload_buffer
+                    )
+
+                    # Extract the actual payload.  Two things going
+                    # on here.  First of all, not all of the items may
+                    # be used.  For example, if the payload length is
+                    # 4 bytes but the format string was HHH, the that
+                    # last 16 bit value is not wanted, so we should
+                    # discard it.  Second thing is that the signed and
+                    # unsigned rational datatypes effectively have twice
+                    # the number of values so we need to account for that.
+                    if dtype in [5, 10]:
+                        payload = payload[:2 * nvalues]
+                    else:
+                        payload = payload[:nvalues]
+
+                self.tags[tag] = {
+                    'dtype': dtype,
+                    'nvalues': nvalues,
+                    'payload': payload
+                }
+
+    def _process_tags(self, b):
 
         # keep this for writing to the UUID, which will always be 32-bit
         little_tiff_tag_length = 12
 
-        # how many tags?
-        if self.version == _BIGTIFF:
-            buffer = tfp.read(8)
-            num_tags, = struct.unpack(endian + 'Q', buffer)
-        else:
-            buffer = tfp.read(2)
-            num_tags, = struct.unpack(endian + 'H', buffer)
+        num_tags = len(self.tags)
 
         write_buffer = struct.pack('<H', num_tags)
         b.write(write_buffer)
 
         # Ok, so now we have the IFD main body, but following that we have
         # the tag payloads that cannot fit into 4 bytes.
 
         # the IFD main body in the TIFF.  As it might be big endian, we cannot
         # just process it as one big chunk.
-        buffer = tfp.read(num_tags * tag_length)
-
-        start_of_tags_position = b.tell()
-        after_ifd_position = start_of_tags_position + len(buffer)
-
-        if self.version == _BIGTIFF:
-            tag_format_str = endian + 'HHQQ'
-            tag_payload_offset = 12
-            max_tag_payload_length = 8
-        else:
-            tag_format_str = endian + 'HHII'
-            tag_payload_offset = 8
-            max_tag_payload_length = 4
 
-        for idx in range(num_tags):
+        tag_start_loc = b.tell()
+        after_ifd_position = tag_start_loc + num_tags * little_tiff_tag_length
 
-            self.logger.debug(f'tag #: {idx}')
+        # We write a little-TIFF IFD
+        max_tag_payload_length = 4
 
-            b.seek(start_of_tags_position + idx * little_tiff_tag_length)
+        for idx, tag in enumerate(self.tags):
 
-            tag_data = buffer[idx * tag_length:(idx + 1) * tag_length]
+            self.logger.debug(f'tag #: {tag}')
 
-            tag, dtype, nvalues, offset = struct.unpack(tag_format_str, tag_data)  # noqa : E501
+            b.seek(tag_start_loc + idx * little_tiff_tag_length)
 
-            if tag == 34735:
-                self.found_geotiff_tags = True
+            dtype = self.tags[tag]['dtype']
+            nvalues = self.tags[tag]['nvalues']
+            payload = self.tags[tag]['payload']
 
             payload_length = tag_dtype[dtype]['nbytes'] * nvalues
 
             if payload_length > max_tag_payload_length:
-                # the payload does not fit into the tag entry, so use the
-                # offset to seek to that position
-                current_position = tfp.tell()
-                tfp.seek(offset)
-                payload_buffer = tfp.read(payload_length)
-                tfp.seek(current_position)
+                # the payload does not fit into the tag entry
 
                 # read the payload from the TIFF
                 payload_format = tag_dtype[dtype]['format'] * nvalues
-                payload = struct.unpack(
-                    endian + payload_format, payload_buffer
-                )
 
                 # write the tag entry to the UUID
                 new_offset = after_ifd_position
                 outbuffer = struct.pack(
                     '<HHII', tag, dtype, nvalues, new_offset
                 )
                 b.write(outbuffer)
@@ -207,38 +286,21 @@
 
                 # keep track of the next position to write out-of-IFD data
                 after_ifd_position = b.tell()
                 b.seek(cpos)
 
             else:
                 # the payload DOES fit into the TIFF tag entry
-                payload_buffer = tag_data[tag_payload_offset:]
 
                 # read ALL of the payload buffer
                 payload_format = (
                     tag_dtype[dtype]['format']
                     * int(max_tag_payload_length / tag_dtype[dtype]['nbytes'])
                 )
 
-                payload = struct.unpack(
-                    endian + payload_format, payload_buffer
-                )
-
-                # Extract the actual payload.  Two things going on here.  First
-                # of all, not all of the items may be used.  For example, if
-                # the payload length is 4 bytes but the format string was HHH,
-                # the that last 16 bit value is not wanted, so we should
-                # discard it.  Second thing is that the signed and unsigned
-                # rational datatypes effectively have twice the number of
-                # values so we need to account for that.
-                if dtype in [5, 10]:
-                    payload = payload[:2 * nvalues]
-                else:
-                    payload = payload[:nvalues]
-
                 # Does it fit into the UUID tag entry (4 bytes)?
                 if payload_length <= 4:
 
                     # so write it back into the tag entry in the UUID
                     outbuffer = struct.pack('<HHI', tag, dtype, nvalues)
                     b.write(outbuffer)
 
@@ -270,14 +332,49 @@
                     outbuffer = struct.pack(out_format, *payload)
                     b.write(outbuffer)
 
                     # keep track of the next position to write out-of-IFD data
                     after_ifd_position = b.tell()
                     b.seek(cpos)
 
+    def get_endianness(self, tfp):
+        """
+        Set the endian-ness of the TIFF
+        """
+
+        buffer = tfp.read(4)
+        data = struct.unpack('BB', buffer[:2])
+
+        # big endian or little endian?
+        if data[0] == 73 and data[1] == 73:
+            # little endian
+            self.endian = '<'
+        elif data[0] == 77 and data[1] == 77:
+            # big endian
+            self.endian = '>'
+        else:
+            msg = (
+                f"The byte order indication in the TIFF header "
+                f"({data}) is invalid.  It should be either "
+                f"{bytes([73, 73])} or {bytes([77, 77])}."
+            )
+            raise RuntimeError(msg)
+
+        # version number and offset to the first IFD
+        version, = struct.unpack(self.endian + 'H', buffer[2:4])
+        self.version = _TIFF if version == 42 else _BIGTIFF
+
+        if self.version == _BIGTIFF:
+            buffer = tfp.read(12)
+            _, _, offset = struct.unpack(self.endian + 'HHQ', buffer)
+        else:
+            buffer = tfp.read(4)
+            offset, = struct.unpack(self.endian + 'I', buffer)
+        tfp.seek(offset)
+
     def _process_header(self, b, tfp):
 
         buffer = tfp.read(4)
         data = struct.unpack('BB', buffer[:2])
 
         # big endian or little endian?
         if data[0] == 73 and data[1] == 73:
@@ -309,32 +406,53 @@
         # write this 32-bit header into the UUID, no matter if we had bigtiff
         # or regular tiff or big endian
         data = struct.pack('<BBHI', 73, 73, 42, 8)
         b.write(data)
 
         return endian
 
+    def get_tag_value(self, tagnum):
+        """
+        Return the value associated with the tag.  Some tags are not actually
+        written into the IFD, but are instead "defaulted".
+
+        Returns
+        -------
+        tag value
+        """
+
+        if tagnum not in self.tags and tagnum == 284:
+            # PlanarConfig is not always written into the IFD, defaults to 1
+            return 1
+
+        if tagnum not in self.tags and tagnum == 339:
+            # SampleFormat is not always written into the IFD, defaults to 1
+            return 1
+
+        # The tag value is always stored as a tuple with at least one member.
+        return self.tags[tagnum]['payload'][0]
+
     def copy_image(self):
         """
         Transfer the image data from the TIFF to the JPEG 2000 file.  If the
         TIFF has a stripped configuration, this may be somewhat inefficient.
         """
 
         if libtiff.isTiled(self.tiff_fp):
             isTiled = True
         else:
             isTiled = False
 
-        photo = libtiff.getFieldDefaulted(self.tiff_fp, 'Photometric')
-        imagewidth = libtiff.getFieldDefaulted(self.tiff_fp, 'ImageWidth')
-        imageheight = libtiff.getFieldDefaulted(self.tiff_fp, 'ImageLength')
-        spp = libtiff.getFieldDefaulted(self.tiff_fp, 'SamplesPerPixel')
-        sf = libtiff.getFieldDefaulted(self.tiff_fp, 'SampleFormat')
-        bps = libtiff.getFieldDefaulted(self.tiff_fp, 'BitsPerSample')
-        planar = libtiff.getFieldDefaulted(self.tiff_fp, 'PlanarConfig')
+        photo = self.get_tag_value(262)
+        imagewidth = self.get_tag_value(256)
+        imageheight = self.get_tag_value(257)
+        spp = self.get_tag_value(277)
+        sf = self.get_tag_value(339)
+        bps = self.get_tag_value(258)
+        planar = self.get_tag_value(284)
 
         if sf not in [libtiff.SampleFormat.UINT, libtiff.SampleFormat.VOID]:
             sampleformat_str = self.tagvalue2str(libtiff.SampleFormat, sf)
 
             msg = (
                 f"The TIFF SampleFormat is {sampleformat_str}.  Only UINT "
                 "and VOID are supported."
@@ -360,19 +478,19 @@
             msg = (
                 "A separated planar configuration is not supported when a "
                 "tile size is specified."
             )
             raise RuntimeError(msg)
 
         if libtiff.isTiled(self.tiff_fp):
-            tw = libtiff.getFieldDefaulted(self.tiff_fp, 'TileWidth')
-            th = libtiff.getFieldDefaulted(self.tiff_fp, 'TileLength')
+            tw = self.get_tag_value(322)
+            th = self.get_tag_value(323)
         else:
             tw = imagewidth
-            rps = libtiff.getFieldDefaulted(self.tiff_fp, 'RowsPerStrip')
+            rps = self.get_tag_value(278)
             num_strips = libtiff.numberOfStrips(self.tiff_fp)
 
         if self.tilesize is not None:
             jth, jtw = self.tilesize
 
             num_jp2k_tile_rows = int(np.ceil(imagewidth / jtw))
             num_jp2k_tile_cols = int(np.ceil(imagewidth / jtw))
@@ -424,15 +542,17 @@
                 photostr = self.tagvalue2str(libtiff.Photometric, photo)
                 msg = (
                     "Beware, the RGBA interface to attempt to read this TIFF "
                     f"when it has a PhotometricInterpretation of {photostr}."
                 )
                 warnings.warn(msg)
 
-            image = libtiff.readRGBAImageOriented(self.tiff_fp)
+            image = libtiff.readRGBAImageOriented(
+                self.tiff_fp, imagewidth, imageheight
+            )
 
             if spp < 4:
                 image = image[:, :, :3]
 
             jp2[:] = image
 
         elif isTiled and self.tilesize is not None:
```

### Comparing `Glymur-0.9.8/glymur/version.py` & `Glymur-0.9.9/glymur/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Local imports ...
 from .lib import openjp2 as opj2
 from .lib import tiff
 
 # Do not change the format of this next line!  Doing so risks breaking
 # setup.py
-version = "0.9.8"
+version = "0.9.9"
 
 version_tuple = parse(version).release
 
 openjpeg_version = opj2.version()
 openjpeg_version_tuple = parse(openjpeg_version).release
 
 tiff_version = tiff.getVersion()
```

### Comparing `Glymur-0.9.8/setup.cfg` & `Glymur-0.9.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Glymur
-version = 0.9.8
+version = 0.9.9
 author = 'John Evans'
 author_email = "John Evans" <john.g.evans.ne@gmail.com>
 license = 'MIT'
 long_description_content_type = text/markdown
 long_description = 
 	**glymur** contains a Python interface to the OpenJPEG library which
 	allows one to read and write JPEG 2000 files.
```

### Comparing `Glymur-0.9.8/tests/fixtures.py` & `Glymur-0.9.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_callbacks.py` & `Glymur-0.9.9/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_cinema.py` & `Glymur-0.9.9/tests/test_cinema.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_codestream.py` & `Glymur-0.9.9/tests/test_codestream.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_colour_specification_box.py` & `Glymur-0.9.9/tests/test_colour_specification_box.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_config.py` & `Glymur-0.9.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_jp2box.py` & `Glymur-0.9.9/tests/test_jp2box.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_jp2box_jpx.py` & `Glymur-0.9.9/tests/test_jp2box_jpx.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_jp2box_uuid.py` & `Glymur-0.9.9/tests/test_jp2box_uuid.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_jp2box_xml.py` & `Glymur-0.9.9/tests/test_jp2box_xml.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_jp2k.py` & `Glymur-0.9.9/tests/test_jp2k.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_libtiff.py` & `Glymur-0.9.9/tests/test_libtiff.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_openjp2.py` & `Glymur-0.9.9/tests/test_openjp2.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_printing.py` & `Glymur-0.9.9/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_set_decoded_components.py` & `Glymur-0.9.9/tests/test_set_decoded_components.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_slicing.py` & `Glymur-0.9.9/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_tiff2jp2.py` & `Glymur-0.9.9/tests/test_tiff2jp2.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_warnings.py` & `Glymur-0.9.9/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `Glymur-0.9.8/tests/test_writing_tiles.py` & `Glymur-0.9.9/tests/test_writing_tiles.py`

 * *Files identical despite different names*

