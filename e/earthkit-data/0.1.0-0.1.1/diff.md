# Comparing `tmp/earthkit-data-0.1.0.tar.gz` & `tmp/earthkit-data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-data-0.1.0.tar", last modified: Mon Apr 24 08:47:48 2023, max compression
+gzip compressed data, was "earthkit-data-0.1.1.tar", last modified: Tue May 23 09:20:46 2023, max compression
```

## Comparing `earthkit-data-0.1.0.tar` & `earthkit-data-0.1.1.tar`

### file list

```diff
@@ -1,206 +1,228 @@
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.656726 earthkit-data-0.1.0/
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.858701 earthkit-data-0.1.0/.github/
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.912762 earthkit-data-0.1.0/.github/workflows/
--rw-r--r--   0 mavj       (501) staff       (20)     3818 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/.github/workflows/on-push.yml
--rw-r--r--   0 mavj       (501) staff       (20)     7160 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/.gitignore
--rw-r--r--   0 mavj       (501) staff       (20)     1179 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 mavj       (501) staff       (20)    11382 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/LICENSE
--rw-r--r--   0 mavj       (501) staff       (20)      779 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/Makefile
--rw-r--r--   0 mavj       (501) staff       (20)     2288 2023-04-24 08:47:48.656832 earthkit-data-0.1.0/PKG-INFO
--rw-------   0 mavj       (501) staff       (20)     1582 2023-04-20 10:39:03.000000 earthkit-data-0.1.0/README.md
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.930561 earthkit-data-0.1.0/docs/
--rw-r--r--   0 mavj       (501) staff       (20)      634 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/Makefile
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.934776 earthkit-data-0.1.0/docs/_static/
--rw-r--r--   0 mavj       (501) staff       (20)        0 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/_static/.gitkeep
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.936261 earthkit-data-0.1.0/docs/_templates/
--rw-r--r--   0 mavj       (501) staff       (20)        0 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/_templates/.gitkeep
--rw-r--r--   0 mavj       (501) staff       (20)     2363 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/docs/conf.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.020284 earthkit-data-0.1.0/docs/examples/
--rw-r--r--   0 mavj       (501) staff       (20)    11749 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/bufr.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    44945 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/fdb_stream.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)   122682 2023-04-20 08:23:37.000000 earthkit-data-0.1.0/docs/examples/grib_basics.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)     8457 2023-04-20 08:23:37.000000 earthkit-data-0.1.0/docs/examples/grib_file_pattern.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    46033 2023-04-20 08:23:37.000000 earthkit-data-0.1.0/docs/examples/grib_from_stream.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    15073 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_indexing.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    72623 2023-04-20 08:23:37.000000 earthkit-data-0.1.0/docs/examples/grib_metadata.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)     5075 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_missing.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    16154 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_multi.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    44781 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_selection.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)     9265 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_tar.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)     2566 2023-04-20 08:23:37.000000 earthkit-data-0.1.0/docs/examples/grib_to_netcdf.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    28136 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/grib_url.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    34080 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/list_of_dict.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)     1200 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/missing.grib
--rw-r--r--   0 mavj       (501) staff       (20)    39003 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/netcdf.ipynb
--rw-r--r--   0 mavj       (501) staff       (20)    13530 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/temp_10.bufr
--rw-r--r--   0 mavj       (501) staff       (20)     1052 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/test.grib
--rw-r--r--   0 mavj       (501) staff       (20)     6504 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/test.nc
--rw-r--r--   0 mavj       (501) staff       (20)   521712 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/test4.grib
--rw-r--r--   0 mavj       (501) staff       (20)     1440 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/test6.grib
--rw-r--r--   0 mavj       (501) staff       (20)     4320 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/examples/tuv_pl.grib
--rw-------   0 mavj       (501) staff       (20)      259 2023-04-20 10:39:03.000000 earthkit-data-0.1.0/docs/index.md
--rw-r--r--   0 mavj       (501) staff       (20)      765 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/make.bat
--rw-r--r--   0 mavj       (501) staff       (20)      158 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.861030 earthkit-data-0.1.0/earthkit/
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.038433 earthkit-data-0.1.0/earthkit/data/
--rw-r--r--   0 mavj       (501) staff       (20)      970 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/__init__.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.057369 earthkit-data-0.1.0/earthkit/data/arguments/
--rw-r--r--   0 mavj       (501) staff       (20)      576 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     2523 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/args_kwargs.py
--rw-r--r--   0 mavj       (501) staff       (20)     2190 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/argument.py
--rw-r--r--   0 mavj       (501) staff       (20)    10135 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/earthkit_types.py
--rw-r--r--   0 mavj       (501) staff       (20)     5576 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/input_manager.py
--rw-r--r--   0 mavj       (501) staff       (20)     5802 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/arguments/transformers.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.092294 earthkit-data-0.1.0/earthkit/data/core/
--rw-r--r--   0 mavj       (501) staff       (20)     2707 2023-04-20 10:38:58.000000 earthkit-data-0.1.0/earthkit/data/core/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)    22874 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/caching.py
--rw-r--r--   0 mavj       (501) staff       (20)    14061 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/index.py
--rw-r--r--   0 mavj       (501) staff       (20)     3027 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/ipython.py
--rw-r--r--   0 mavj       (501) staff       (20)     5857 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/plugins.py
--rw-r--r--   0 mavj       (501) staff       (20)    11026 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/settings.py
--rw-r--r--   0 mavj       (501) staff       (20)     3203 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/statistics.py
--rw-r--r--   0 mavj       (501) staff       (20)     1502 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/temporary.py
--rw-r--r--   0 mavj       (501) staff       (20)     2708 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/core/thread.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:47.862152 earthkit-data-0.1.0/earthkit/data/data/
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.103099 earthkit-data-0.1.0/earthkit/data/data/css/
--rw-r--r--   0 mavj       (501) staff       (20)     2605 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/earthkit/data/data/css/tab.css
--rw-r--r--   0 mavj       (501) staff       (20)       74 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/earthkit/data/data/css/table.css
--rw-r--r--   0 mavj       (501) staff       (20)     5933 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/decorators.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.110561 earthkit-data-0.1.0/earthkit/data/indexing/
--rw-r--r--   0 mavj       (501) staff       (20)     1172 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/indexing/__init__.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.130247 earthkit-data-0.1.0/earthkit/data/indexing/database/
--rw-r--r--   0 mavj       (501) staff       (20)      858 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/indexing/database/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     1321 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/indexing/database/json.py
--rw-r--r--   0 mavj       (501) staff       (20)    14507 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/indexing/database/sql.py
--rw-r--r--   0 mavj       (501) staff       (20)      707 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/indexing/database/stdout.py
--rw-r--r--   0 mavj       (501) staff       (20)     5576 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/input_manager.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.152198 earthkit-data-0.1.0/earthkit/data/mergers/
--rw-r--r--   0 mavj       (501) staff       (20)     5535 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/mergers/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)      650 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/mergers/pandas.py
--rw-r--r--   0 mavj       (501) staff       (20)     2533 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/mergers/xarray.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.163759 earthkit-data-0.1.0/earthkit/data/mirrors/
--rw-r--r--   0 mavj       (501) staff       (20)     2819 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/mirrors/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     3089 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/mirrors/directory_mirror.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.227105 earthkit-data-0.1.0/earthkit/data/readers/
--rw-r--r--   0 mavj       (501) staff       (20)     5539 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     2077 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/archive.py
--rw-r--r--   0 mavj       (501) staff       (20)     2388 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/bufr.py
--rw-r--r--   0 mavj       (501) staff       (20)     4238 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/csv.py
--rw-r--r--   0 mavj       (501) staff       (20)     2542 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/directory.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.269952 earthkit-data-0.1.0/earthkit/data/readers/grib/
--rw-r--r--   0 mavj       (501) staff       (20)     1222 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)    14965 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/codes.py
--rw-r--r--   0 mavj       (501) staff       (20)     6489 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/fieldset.py
--rw-r--r--   0 mavj       (501) staff       (20)    11432 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/index.py
--rw-r--r--   0 mavj       (501) staff       (20)     3555 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/memory.py
--rw-r--r--   0 mavj       (501) staff       (20)     1361 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/pandas.py
--rw-r--r--   0 mavj       (501) staff       (20)     5252 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/parsing.py
--rw-r--r--   0 mavj       (501) staff       (20)     1242 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/reader.py
--rw-r--r--   0 mavj       (501) staff       (20)     4493 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/grib/xarray.py
--rw-r--r--   0 mavj       (501) staff       (20)    11392 2023-04-24 08:22:17.000000 earthkit-data-0.1.0/earthkit/data/readers/netcdf.py
--rw-r--r--   0 mavj       (501) staff       (20)     1275 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/numpy.py
--rw-r--r--   0 mavj       (501) staff       (20)      968 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/odb.py
--rw-r--r--   0 mavj       (501) staff       (20)     1105 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/tar.py
--rw-r--r--   0 mavj       (501) staff       (20)     1379 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/text.py
--rw-r--r--   0 mavj       (501) staff       (20)      774 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/unknown.py
--rw-r--r--   0 mavj       (501) staff       (20)     2802 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/readers/zip.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.353833 earthkit-data-0.1.0/earthkit/data/sources/
--rw-r--r--   0 mavj       (501) staff       (20)     3691 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)      378 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/earthkit/data/sources/dummy.grib
--rw-r--r--   0 mavj       (501) staff       (20)     6153 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/dummy_source.py
--rw-r--r--   0 mavj       (501) staff       (20)      567 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/empty.py
--rw-r--r--   0 mavj       (501) staff       (20)     1368 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/fdb.py
--rw-r--r--   0 mavj       (501) staff       (20)     6095 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/file.py
--rw-r--r--   0 mavj       (501) staff       (20)     3358 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/file_indexed.py
--rw-r--r--   0 mavj       (501) staff       (20)      909 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/file_pattern.py
--rw-r--r--   0 mavj       (501) staff       (20)     2026 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/indexed.py
--rw-r--r--   0 mavj       (501) staff       (20)     3710 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/list_of_dicts.py
--rw-r--r--   0 mavj       (501) staff       (20)     2693 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/memory.py
--rw-r--r--   0 mavj       (501) staff       (20)     4298 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/multi.py
--rw-r--r--   0 mavj       (501) staff       (20)     1155 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/multi_url.py
--rw-r--r--   0 mavj       (501) staff       (20)     1692 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/stream.py
--rw-r--r--   0 mavj       (501) staff       (20)     5493 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/url.py
--rw-r--r--   0 mavj       (501) staff       (20)      796 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/url_pattern.py
--rw-r--r--   0 mavj       (501) staff       (20)     4116 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/virtual.py
--rw-r--r--   0 mavj       (501) staff       (20)     6481 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/sources/virtual_directory.py
--rw-r--r--   0 mavj       (501) staff       (20)     3470 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/testing.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.437338 earthkit-data-0.1.0/earthkit/data/utils/
--rw-r--r--   0 mavj       (501) staff       (20)     4231 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     4959 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/availability.py
--rw-r--r--   0 mavj       (501) staff       (20)     5275 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/bbox.py
--rw-r--r--   0 mavj       (501) staff       (20)      701 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/conventions.py
--rw-r--r--   0 mavj       (501) staff       (20)     2671 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/dates.py
--rw-r--r--   0 mavj       (501) staff       (20)    19720 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/factorise.py
--rw-r--r--   0 mavj       (501) staff       (20)     2902 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/html.py
--rw-r--r--   0 mavj       (501) staff       (20)     7718 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/humanize.py
--rw-r--r--   0 mavj       (501) staff       (20)     2001 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/kwargs.py
--rw-r--r--   0 mavj       (501) staff       (20)     1742 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/lazy.py
--rw-r--r--   0 mavj       (501) staff       (20)     1887 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/parts.py
--rw-r--r--   0 mavj       (501) staff       (20)     4770 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/patterns.py
--rw-r--r--   0 mavj       (501) staff       (20)     1174 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/serialise.py
--rw-r--r--   0 mavj       (501) staff       (20)     5030 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/utils/summary.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.457101 earthkit-data-0.1.0/earthkit/data/vocabularies/
--rw-r--r--   0 mavj       (501) staff       (20)     2877 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/vocabularies/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     1151 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/vocabularies/aliases.py
--rw-r--r--   0 mavj       (501) staff       (20)      889 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/vocabularies/cf.py
--rw-r--r--   0 mavj       (501) staff       (20)     1908 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/earthkit/data/vocabularies/grib-paramid.csv
--rw-r--r--   0 mavj       (501) staff       (20)     1088 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/vocabularies/grib.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.468608 earthkit-data-0.1.0/earthkit/data/wrappers/
--rw-r--r--   0 mavj       (501) staff       (20)     1598 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/wrappers/__init__.py
--rw-r--r--   0 mavj       (501) staff       (20)     1825 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/earthkit/data/wrappers/string.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.473051 earthkit-data-0.1.0/earthkit_data.egg-info/
--rw-r--r--   0 mavj       (501) staff       (20)     2288 2023-04-24 08:47:47.000000 earthkit-data-0.1.0/earthkit_data.egg-info/PKG-INFO
--rw-r--r--   0 mavj       (501) staff       (20)     5382 2023-04-24 08:47:47.000000 earthkit-data-0.1.0/earthkit_data.egg-info/SOURCES.txt
--rw-r--r--   0 mavj       (501) staff       (20)        1 2023-04-24 08:47:47.000000 earthkit-data-0.1.0/earthkit_data.egg-info/dependency_links.txt
--rw-r--r--   0 mavj       (501) staff       (20)        7 2023-04-24 08:47:47.000000 earthkit-data-0.1.0/earthkit_data.egg-info/requires.txt
--rw-r--r--   0 mavj       (501) staff       (20)        9 2023-04-24 08:47:47.000000 earthkit-data-0.1.0/earthkit_data.egg-info/top_level.txt
--rw-r--r--   0 mavj       (501) staff       (20)      482 2023-04-24 08:43:43.000000 earthkit-data-0.1.0/environment.yml
--rw-r--r--   0 mavj       (501) staff       (20)      398 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/pyproject.toml
--rw-r--r--   0 mavj       (501) staff       (20)      414 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/pytest.ini
--rw-r--r--   0 mavj       (501) staff       (20)      890 2023-04-24 08:47:48.657352 earthkit-data-0.1.0/setup.cfg
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.476013 earthkit-data-0.1.0/tests/
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.478119 earthkit-data-0.1.0/tests/bufr/
--rw-r--r--   0 mavj       (501) staff       (20)     3532 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/bufr/test_bufr_summary.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.483054 earthkit-data-0.1.0/tests/core/
--rw-r--r--   0 mavj       (501) staff       (20)     1953 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/core/test_cache.py
--rw-r--r--   0 mavj       (501) staff       (20)      595 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/core/test_version.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.519621 earthkit-data-0.1.0/tests/data/
--rw-r--r--   0 mavj       (501) staff       (20)    22138 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/mercator.grib
--rw-r--r--   0 mavj       (501) staff       (20)    47520 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/ml_data.grib
--rw-r--r--   0 mavj       (501) staff       (20)     2400 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/rgg_small_subarea_cellarea_ref.grib
--rw-r--r--   0 mavj       (501) staff       (20)     1440 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/t_pl.grib
--rw-r--r--   0 mavj       (501) staff       (20)     3600 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/t_time_series.grib
--rw-r--r--   0 mavj       (501) staff       (20)      240 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/test_single.grib
--rw-r--r--   0 mavj       (501) staff       (20)    21233 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/test_single.nc
--rw-r--r--   0 mavj       (501) staff       (20)      360 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/test_single_with_missing.grib
--rw-r--r--   0 mavj       (501) staff       (20)     1440 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/u_pl.grib
--rw-r--r--   0 mavj       (501) staff       (20)     1440 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/data/v_pl.grib
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.525020 earthkit-data-0.1.0/tests/documentation/
--rw-r--r--   0 mavj       (501) staff       (20)     1304 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/documentation/test_examples.py
--rw-r--r--   0 mavj       (501) staff       (20)     1800 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/documentation/test_notebooks.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.541392 earthkit-data-0.1.0/tests/grib/
--rw-r--r--   0 mavj       (501) staff       (20)    21339 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/grib/test_grib_contents.py
--rw-r--r--   0 mavj       (501) staff       (20)     8458 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/grib/test_grib_sel.py
--rw-r--r--   0 mavj       (501) staff       (20)     5271 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/grib/test_grib_slice.py
--rw-r--r--   0 mavj       (501) staff       (20)    14359 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/grib/test_grib_summary.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.560444 earthkit-data-0.1.0/tests/indexing/
--rw-r--r--   0 mavj       (501) staff       (20)     4515 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/indexing/indexing_fixtures.py
--rw-r--r--   0 mavj       (501) staff       (20)     1707 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/indexing/test_indexing_isel.py
--rw-r--r--   0 mavj       (501) staff       (20)     2775 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/indexing/test_indexing_multi_file.py
--rw-r--r--   0 mavj       (501) staff       (20)     4874 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/indexing/test_indexing_order_by.py
--rw-r--r--   0 mavj       (501) staff       (20)     1657 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/indexing/test_indexing_serialisation.py
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.645731 earthkit-data-0.1.0/tests/readers/
--rw-r--r--   0 mavj       (501) staff       (20)     2583 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/readers/test_csv_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)     1417 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/readers/test_grib_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)     5626 2023-04-24 08:22:17.000000 earthkit-data-0.1.0/tests/readers/test_netcdf_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)      994 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/readers/test_tar_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)      993 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/readers/test_unknown_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)      644 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/readers/test_zip_reader.py
--rw-r--r--   0 mavj       (501) staff       (20)       83 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/readers/unknown_file.unknown_ext
--rw-r--r--   0 mavj       (501) staff       (20)       21 2023-04-13 09:21:25.000000 earthkit-data-0.1.0/tests/readers/unknown_text_file.unknown_ext
-drwxr-xr-x   0 mavj       (501) staff       (20)        0 2023-04-24 08:47:48.656479 earthkit-data-0.1.0/tests/sources/
--rw-r--r--   0 mavj       (501) staff       (20)     2555 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/sources/test_file.py
--rw-r--r--   0 mavj       (501) staff       (20)     4200 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/sources/test_multi.py
--rw-r--r--   0 mavj       (501) staff       (20)     3328 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/sources/test_url.py
--rw-r--r--   0 mavj       (501) staff       (20)     1304 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/sources/test_url_pattern.py
--rw-r--r--   0 mavj       (501) staff       (20)       97 2023-04-20 10:38:59.000000 earthkit-data-0.1.0/tests/test_00_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.279951 earthkit-data-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.235951 earthkit-data-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.243951 earthkit-data-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.github/workflows/notify_new_issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.github/workflows/notify_new_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 09:20:46.279951 earthkit-data-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.247951 earthkit-data-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.247951 earthkit-data-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.247951 earthkit-data-0.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.251951 earthkit-data-0.1.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/bufr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45108 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_fdb_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_file_pattern.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    46028 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_from_stream.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_indexing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    76257 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_metadata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_missing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16154 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_multi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   111937 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45664 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_selection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_tar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_to_netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28136 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/grib_url.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    34095 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/list_of_dict.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    39106 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/netcdf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/temp_10.bufr
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/test.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/test.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   521712 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/test4.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/test6.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples/tuv_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.239951 earthkit-data-0.1.1/earthkit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.251951 earthkit-data-0.1.1/earthkit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.251951 earthkit-data-0.1.1/earthkit/data/arguments/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/args_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/earthkit_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/input_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/arguments/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.255951 earthkit-data-0.1.1/earthkit/data/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/core/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.239951 earthkit-data-0.1.1/earthkit/data/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.255951 earthkit-data-0.1.1/earthkit/data/data/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/data/css/tab.css
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/data/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.255951 earthkit-data-0.1.1/earthkit/data/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/indexing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.259951 earthkit-data-0.1.1/earthkit/data/indexing/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/indexing/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/indexing/database/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19393 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/indexing/database/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/indexing/database/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/input_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.259951 earthkit-data-0.1.1/earthkit/data/mergers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/mergers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/mergers/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/mergers/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.259951 earthkit-data-0.1.1/earthkit/data/mirrors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/mirrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/mirrors/directory_mirror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.259951 earthkit-data-0.1.1/earthkit/data/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/bufr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.263951 earthkit-data-0.1.1/earthkit/data/readers/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/fieldset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.263951 earthkit-data-0.1.1/earthkit/data/readers/grib/index/
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/index/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/index/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/index/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/index/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/grib/xarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/odb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/readers/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.267951 earthkit-data-0.1.1/earthkit/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/dummy.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/dummy_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/fdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/file_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/file_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/list_of_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/multi_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/sources/virtual_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.267951 earthkit-data-0.1.1/earthkit/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/factorise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/parts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/serialise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/utils/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.267951 earthkit-data-0.1.1/earthkit/data/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/vocabularies/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/vocabularies/cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/vocabularies/grib-paramid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/vocabularies/grib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.267951 earthkit-data-0.1.1/earthkit/data/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/earthkit/data/wrappers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.271951 earthkit-data-0.1.1/earthkit_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-23 09:20:46.000000 earthkit-data-0.1.1/earthkit_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-23 09:20:46.000000 earthkit-data-0.1.1/earthkit_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:20:46.000000 earthkit-data-0.1.1/earthkit_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 09:20:46.000000 earthkit-data-0.1.1/earthkit_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 09:20:46.000000 earthkit-data-0.1.1/earthkit_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 09:20:46.279951 earthkit-data-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.271951 earthkit-data-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.271951 earthkit-data-0.1.1/tests/bufr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/bufr/test_bufr_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.271951 earthkit-data-0.1.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.271951 earthkit-data-0.1.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/mercator.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    47520 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/ml_data.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/rgg_small_subarea_cellarea_ref.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/t_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/t_time_series.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/test_icon.grib
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/test_single.grib
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/test_single.nc
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/test_single_with_missing.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/u_pl.grib
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/data/v_pl.grib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.275951 earthkit-data-0.1.1/tests/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/documentation/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/documentation/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.275951 earthkit-data-0.1.1/tests/grib/
+-rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8447 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_sel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/grib/test_grib_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.275951 earthkit-data-0.1.1/tests/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/indexing_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_indexing_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_indexing_isel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_indexing_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_indexing_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_order_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/indexing/test_selection_kwargs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.275951 earthkit-data-0.1.1/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_csv_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_grib_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_netcdf_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_tar_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_unknown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/test_zip_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/unknown_file.unknown_ext
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/readers/unknown_text_file.unknown_ext
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:20:46.279951 earthkit-data-0.1.1/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/sources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/sources/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/sources/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/sources/test_url_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 09:20:25.000000 earthkit-data-0.1.1/tests/test_00_version.py
```

### Comparing `earthkit-data-0.1.0/.gitignore` & `earthkit-data-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/.pre-commit-config.yaml` & `earthkit-data-0.1.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   - id: debug-statements
   - id: mixed-line-ending
 - repo: https://github.com/PyCQA/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/psf/black
-  rev: 22.6.0
+  rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/keewis/blackdoc
   rev: v0.3.4
   hooks:
   - id: blackdoc
     additional_dependencies: [black==22.3.0]
```

### Comparing `earthkit-data-0.1.0/LICENSE` & `earthkit-data-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/Makefile` & `earthkit-data-0.1.1/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 PROJECT := earthkit-data
 CONDA := conda
 CONDAFLAGS :=
 COV_REPORT := html
 
+setup:
+	pre-commit install
+
 default: qa unit-tests type-check
 
 qa:
 	pre-commit run --all-files
 
 unit-tests:
 	python -m pytest -vv -m 'not notebook' --cov=. --cov-report=$(COV_REPORT)
```

### Comparing `earthkit-data-0.1.0/PKG-INFO` & `earthkit-data-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -14,37 +14,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
+
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
-**earthkit-data** makes it simple to read, inspect and slice data from a wide range of
-geospatial input types (GRIB, netCDF, zarr and more) and transform them into
-familiar scientific Python objects (including numpy arrays, pandas dataframes,
-xarray datasets).
-
-```
-data = earthkit.data.from_source("my-data.nc")
-arr = data.to_numpy()
-df = data.to_pandas()
-dataset = data.to_xarray()
-```
-
-**earthkit-data** provides additional convenient methods for quickly inspecting certain
-features of your input data, such as data dimensionality, axes, coordinate
-reference systems and bounding boxes.
+The documentation can be found at https://earthkit-data.readthedocs.io/.
 
 ## License
 
 ```
 Copyright 2022, European Centre for Medium Range Weather Forecasts.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -54,8 +42,12 @@
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
+
+In applying this licence, ECMWF does not waive the privileges and immunities
+granted to it by virtue of its status as an intergovernmental organisation
+nor does it submit to any jurisdiction.
 ```
```

### Comparing `earthkit-data-0.1.0/docs/Makefile` & `earthkit-data-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/conf.py` & `earthkit-data-0.1.1/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,76 +2,60 @@
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Import and path setup ---------------------------------------------------
 
+import datetime
 import os
 import sys
 
-import earthkit.data
+# import earthkit.data
 
 sys.path.insert(0, os.path.abspath("../"))
 
 # -- Project information -----------------------------------------------------
 
 project = "earthkit-data"
-copyright = "2022, European Centre for Medium Range Weather Forecasts"
 author = "European Centre for Medium Range Weather Forecasts"
-version = earthkit.data.__version__
-release = earthkit.data.__version__
+
+year = datetime.datetime.now().year
+years = "2022-%s" % (year,)
+copyright = "%s, European Centre for Medium-Range Weather Forecasts (ECMWF)" % (years,)
+
+# version = earthkit.data.__version__
+# release = earthkit.data.__version__
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "autoapi.extension",
-    "myst_parser",
-    "sphinx.ext.autodoc",
-    "sphinx.ext.napoleon",
+    "sphinx_rtd_theme",
     "nbsphinx",
 ]
 
-# autodoc configuration
-autodoc_typehints = "none"
-
-# autoapi configuration
-autoapi_dirs = ["../earthkit/data"]
-autoapi_ignore = ["*/version.py"]
-autoapi_options = [
-    "members",
-    "inherited-members",
-    "undoc-members",
-    "show-inheritance",
-    "show-module-summary",
-    "imported-members",
-]
-autoapi_root = "_api"
-
-# napoleon configuration
-napoleon_google_docstring = False
-napoleon_numpy_docstring = True
-napoleon_preprocess_types = True
-
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
+# The suffix of source filenames.
+source_suffix = ".rst"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "pydata_sphinx_theme"
+html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
+# html_css_files = ["style.css"]
```

### Comparing `earthkit-data-0.1.0/docs/examples/bufr.ipynb` & `earthkit-data-0.1.1/docs/examples/bufr.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'cells'": "{1: {'source': ['## Using BUFR data']}}"}*

```diff
@@ -11,15 +11,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "102b1cf9-33a5-4310-af4d-bcd17d598d29",
             "metadata": {},
             "source": [
-                "## Handling BUFR data"
+                "## Using BUFR data"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e11bb141-5f5d-42c2-9083-3cccbf9b7799",
             "metadata": {},
             "source": [
```

### Comparing `earthkit-data-0.1.0/docs/examples/fdb_stream.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_fdb_stream.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9827215608465608%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'fad5f9b6-c33a-4d57-b982-95f5e3d64eff'), ('metadata', OrderedDict()), ('source', ['## "*

 * *            "Reading GRIB from FDB stream'])]))]}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'mpy38', 'name': 'mpy38'}, 'language_info': "*

 * *               "{'version': '3.8.16'}}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "fad5f9b6-c33a-4d57-b982-95f5e3d64eff",
+            "metadata": {},
+            "source": [
+                "## Reading GRIB from FDB stream"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 1,
             "id": "sufficient-league",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyfdb \n",
@@ -977,27 +985,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "pyfdb",
+            "display_name": "mpy38",
             "language": "python",
-            "name": "pyfdb"
+            "name": "mpy38"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.12"
+            "version": "3.8.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_basics.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_overview.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910760799080394%*

 * *Differences: {"'cells'": "{1: {'source': ['## Using GRIB data overview']}, 11: {'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(1, '#T_cfd90 th {\\n'), (4, '#T_cfd90_row0_col0, "*

 * *            '#T_cfd90_row0_col1, #T_cfd90_row0_col2, #T_cfd90_row0_col3, #T_cfd90_row0_col4, '*

 * *            '#T_cfd90_row0_col5, #T_cfd90_row0_col6, #T_cfd90_row0_col7, #T_cfd90_row0_col8, '*

 * *            '#T_cfd90_row1_col0, #T_cfd90_row1_col1, #T_cfd90_row1_col2, #T_cfd90_row1_col3, '*

 * *            '#T_cfd90_row1_col4, #T_cfd90_row […]*

```diff
@@ -9,15 +9,15 @@
                 "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## GRIB handling basics"
+                "## Using GRIB data overview"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We load a GRIB file containing 6 messages from disk:"
@@ -258,35 +258,35 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_bf7a0 th {\n",
+                            "#T_cfd90 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_bf7a0_row0_col0, #T_bf7a0_row0_col1, #T_bf7a0_row0_col2, #T_bf7a0_row0_col3, #T_bf7a0_row0_col4, #T_bf7a0_row0_col5, #T_bf7a0_row0_col6, #T_bf7a0_row0_col7, #T_bf7a0_row0_col8, #T_bf7a0_row1_col0, #T_bf7a0_row1_col1, #T_bf7a0_row1_col2, #T_bf7a0_row1_col3, #T_bf7a0_row1_col4, #T_bf7a0_row1_col5, #T_bf7a0_row1_col6, #T_bf7a0_row1_col7, #T_bf7a0_row1_col8, #T_bf7a0_row2_col0, #T_bf7a0_row2_col1, #T_bf7a0_row2_col2, #T_bf7a0_row2_col3, #T_bf7a0_row2_col4, #T_bf7a0_row2_col5, #T_bf7a0_row2_col6, #T_bf7a0_row2_col7, #T_bf7a0_row2_col8 {\n",
+                            "#T_cfd90_row0_col0, #T_cfd90_row0_col1, #T_cfd90_row0_col2, #T_cfd90_row0_col3, #T_cfd90_row0_col4, #T_cfd90_row0_col5, #T_cfd90_row0_col6, #T_cfd90_row0_col7, #T_cfd90_row0_col8, #T_cfd90_row1_col0, #T_cfd90_row1_col1, #T_cfd90_row1_col2, #T_cfd90_row1_col3, #T_cfd90_row1_col4, #T_cfd90_row1_col5, #T_cfd90_row1_col6, #T_cfd90_row1_col7, #T_cfd90_row1_col8, #T_cfd90_row2_col0, #T_cfd90_row2_col1, #T_cfd90_row2_col2, #T_cfd90_row2_col3, #T_cfd90_row2_col4, #T_cfd90_row2_col5, #T_cfd90_row2_col6, #T_cfd90_row2_col7, #T_cfd90_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_bf7a0\">\n",
+                            "<table id=\"T_cfd90\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_bf7a0_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_cfd90_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_cfd90_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_cfd90_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_cfd90_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_cfd90_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_cfd90_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_cfd90_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_cfd90_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_cfd90_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -296,336 +296,69 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_bf7a0_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_bf7a0_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_bf7a0_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_bf7a0_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "      <th id=\"T_cfd90_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_cfd90_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_cfd90_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_cfd90_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_cfd90_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_cfd90_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_cfd90_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_cfd90_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_cfd90_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_cfd90_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_cfd90_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_bf7a0_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_bf7a0_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_bf7a0_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_bf7a0_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "      <th id=\"T_cfd90_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_cfd90_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_cfd90_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_cfd90_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_cfd90_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_cfd90_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_cfd90_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_cfd90_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_cfd90_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_cfd90_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_cfd90_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_bf7a0_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_bf7a0_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_bf7a0_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_bf7a0_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_cfd90_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_cfd90_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_cfd90_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_cfd90_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_cfd90_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_cfd90_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_cfd90_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_cfd90_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_cfd90_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_cfd90_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_cfd90_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x11f4ef730>"
+                            "<pandas.io.formats.style.Styler at 0x12cf4b220>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.describe()"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<style type=\"text/css\"> /* Based on:\n",
-                            " https://codepen.io/htmlcssfreebies/pen/WNpVeRK\n",
-                            " https://github.com/pydata/xarray/blob/main/xarray/static/css/style.css\n",
-                            " */\n",
-                            "\n",
-                            " :root {\n",
-                            "    --eh-font-color0: var(--jp-content-font-color0, rgba(0, 0, 0, 1));\n",
-                            "    --eh-font-color2: var(--jp-content-font-color2, rgba(0, 0, 0, 0.54));\n",
-                            "    --eh-font-color3: var(--jp-content-font-color3, rgba(0, 0, 0, 0.38));\n",
-                            "    --eh-border-color: var(--jp-border-color2, #e0e0e0);\n",
-                            "    --eh-disabled-color: var(--jp-layout-color3, #bdbdbd);\n",
-                            "    --eh-background-color: var(--jp-layout-color0, white);\n",
-                            "  }\n",
-                            "\n",
-                            "html[theme=dark],\n",
-                            "body[data-theme=dark],\n",
-                            "body.vscode-dark {\n",
-                            "  --eh-font-color0: rgba(255, 255, 255, 1);\n",
-                            "  --eh-font-color2: rgba(255, 255, 255, 0.54);\n",
-                            "  --eh-font-color3: rgba(255, 255, 255, 0.38);\n",
-                            "  --eh-border-color: #1F1F1F;\n",
-                            "  --eh-disabled-color: #515151;\n",
-                            "  --eh-background-color: #111111;\n",
-                            "}\n",
-                            "\n",
-                            " /* Reset */\n",
-                            " *,\n",
-                            " *::before,\n",
-                            " *::after {\n",
-                            "     box-sizing: border-box;\n",
-                            " }\n",
-                            "\n",
-                            " .eh-description {\n",
-                            "    color: var(--eh-font-color2);\n",
-                            " }\n",
-                            "\n",
-                            " .eh-section {\n",
-                            "    padding-left: 0px;\n",
-                            " }\n",
-                            "\n",
-                            " /* Tabs Container */\n",
-                            " .eh-tabs-container {\n",
-                            "     padding: 0px;\n",
-                            " }\n",
-                            "\n",
-                            " /* Tabs Block */\n",
-                            " .eh-tabs-block {\n",
-                            "     display: flex;\n",
-                            "     align-items: center;\n",
-                            "     justify-content: center;\n",
-                            "     padding-top: 4px;\n",
-                            " }\n",
-                            "\n",
-                            " /* Tabs */\n",
-                            " .eh-tabs {\n",
-                            "     display: flex;\n",
-                            "     flex-wrap: wrap;\n",
-                            "     width: 100%;\n",
-                            " }\n",
-                            "\n",
-                            " .eh-tabs label {\n",
-                            "     width: 100%;\n",
-                            "     display: flex;\n",
-                            "     align-items: center;\n",
-                            "     justify-content: center;\n",
-                            "     padding-left: 6px;\n",
-                            "     padding-right: 6px;\n",
-                            "     font-weight: 400;\n",
-                            "     cursor: pointer;\n",
-                            "     color: var(--eh-font-color2);\n",
-                            "     background-color: var(--eh-background-color);\n",
-                            "     border-top: 1px solid var(--eh-background-color);\n",
-                            "     border-bottom: 1px solid var(--eh-disabled-color);\n",
-                            " }\n",
-                            "\n",
-                            " /* Tab page contents */\n",
-                            " .eh-tabs .tab {\n",
-                            "     flex-grow: 1;\n",
-                            "     width: 100%;\n",
-                            "     height: 100%;\n",
-                            "     display: none;\n",
-                            "     padding: 2px 2px;\n",
-                            " }\n",
-                            "\n",
-                            " .eh-tabs [type=radio] {\n",
-                            "     display: none;\n",
-                            " }\n",
-                            "\n",
-                            " .eh-tabs [type=radio]:checked + label {\n",
-                            "     font-weight: 500;\n",
-                            "     color: var(--eh-font-color0);\n",
-                            "     border: 1px solid var(--eh-disabled-color);\n",
-                            " }\n",
-                            "\n",
-                            " .eh-tabs [type=radio]:checked + label + .tab {\n",
-                            "     display: block;\n",
-                            " }\n",
-                            "\n",
-                            " .eh-tabs [type=radio]:not(:checked) + label:hover {\n",
-                            "    color: var(--xr-font-color0);\n",
-                            " }\n",
-                            "\n",
-                            "\n",
-                            " @media (min-width: 768px) {\n",
-                            "\n",
-                            "     .eh-tabs-container {\n",
-                            "         padding: 1rem 1rem;\n",
-                            "     }\n",
-                            "\n",
-                            "     .eh-tabs label {\n",
-                            "         order: 1;\n",
-                            "         width: auto;\n",
-                            "     }\n",
-                            "\n",
-                            "     .eh-tabs .tab {\n",
-                            "         order: 9;\n",
-                            "     }\n",
-                            "\n",
-                            "     .eh-tabs [type=radio]:checked + label {\n",
-                            "         border-bottom: none;\n",
-                            "     }\n",
-                            " }\n",
-                            " @media (min-width: 992px) {\n",
-                            "\n",
-                            "     .eh-tabs {\n",
-                            "         width: 800px;\n",
-                            "     }\n",
-                            " }\n",
-                            "</style><div class=\"eh-description\">GribField</div>\n",
-                            "<div>\n",
-                            "<section class=\"eh-section>\n",
-                            "<div class=\"eh-tabs-container\">\n",
-                            "<div class=\"eh-tabs-block\">\n",
-                            "<div class=\"eh-tabs\">\n",
-                            "\n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"9dadc695-7dd1-4c28-8128-c8101fb4fd4f\"  />\n",
-                            "<label for=\"9dadc695-7dd1-4c28-8128-c8101fb4fd4f\" title=\"Keys in the ecCodes None namespace\">default</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>mybits</b></td><td>None</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"22287000-d072-4fca-8972-5d01bde30c6d\"  />\n",
-                            "<label for=\"22287000-d072-4fca-8972-5d01bde30c6d\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>edition</b></td><td>1</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>dataType</b></td><td>an</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"f003a52f-00fc-4b3e-9d74-9fd359d7f50d\"  />\n",
-                            "<label for=\"f003a52f-00fc-4b3e-9d74-9fd359d7f50d\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"adb4ac4d-e2be-44db-b533-643ee25f4336\"  />\n",
-                            "<label for=\"adb4ac4d-e2be-44db-b533-643ee25f4336\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>domain</b></td><td>g</td></tr> <tr><td><b>levtype</b></td><td>pl</td></tr> <tr><td><b>levelist</b></td><td>1000</td></tr> <tr><td><b>date</b></td><td>20180801</td></tr> <tr><td><b>time</b></td><td>1200</td></tr> <tr><td><b>step</b></td><td>0</td></tr> <tr><td><b>param</b></td><td>t</td></tr> <tr><td><b>class</b></td><td>od</td></tr> <tr><td><b>type</b></td><td>an</td></tr> <tr><td><b>stream</b></td><td>oper</td></tr> <tr><td><b>expver</b></td><td>0001</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"3408d86a-a413-41ea-93ad-085ca92affec\" checked />\n",
-                            "<label for=\"3408d86a-a413-41ea-93ad-085ca92affec\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"5dd09779-63a8-4ae5-befb-784ede1cf40b\"  />\n",
-                            "<label for=\"5dd09779-63a8-4ae5-befb-784ede1cf40b\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>max</b></td><td>320.5641784667969</td></tr> <tr><td><b>min</b></td><td>240.56417846679688</td></tr> <tr><td><b>avg</b></td><td>279.70703560965404</td></tr> <tr><td><b>sd</b></td><td>19.67421739058438</td></tr> <tr><td><b>skew</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurt</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>const</b></td><td>0.0</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"9fc40f55-f30b-474d-b595-68675b29d115\"  />\n",
-                            "<label for=\"9fc40f55-f30b-474d-b595-68675b29d115\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"0f662904-8e1c-499f-bd72-fb3f939a4ed6\"  />\n",
-                            "<label for=\"0f662904-8e1c-499f-bd72-fb3f939a4ed6\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
-                            "<div class=\"tab\">\n",
-                            "<style type=\"text/css\">table.eh td {\n",
-                            "    vertical-align: top;\n",
-                            "    text-align: left !important;\n",
-                            "}\n",
-                            "</style>\n",
-                            "<table class=\"eh-table\">\n",
-                            "<tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr>\n",
-                            "</table>\n",
-                            "</div>\n",
-                            "    \n",
-                            "</div>\n",
-                            "</div>\n",
-                            "</div>\n",
-                            "</section>\n",
-                            "</div>\n",
-                            "        "
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "execution_count": 7,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "fs[0].dump()"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Slicing"
             ]
         },
         {
@@ -633,36 +366,36 @@
             "metadata": {},
             "source": [
                 "Standard Python slicing is available. It does not involve any loading/copying of GRIB data. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "GribField(u,1000,20180801,1200,0,0)"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g = fs[1]\n",
                 "g"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -731,36 +464,36 @@
                             "1   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g = fs[1:3]\n",
                 "g.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "GribField(v,850,20180801,1200,0,0)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g = fs[-1]\n",
                 "g"
@@ -785,65 +518,65 @@
             "metadata": {},
             "source": [
                 "The values property always returns a flat array per field:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(84,)"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "v = fs[0].values\n",
                 "v.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "array([272.56417847, 272.56417847, 272.56417847, 272.56417847])"
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "v[0:4]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(6, 84)"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "v = fs.values\n",
                 "v.shape"
@@ -861,15 +594,15 @@
             "metadata": {},
             "source": [
                 "With to_numpy() the field shape is set on the array: "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "(7, 12)\n",
@@ -881,24 +614,24 @@
                 "v = fs[0].to_numpy()\n",
                 "print(v.shape)\n",
                 "print(fs[0].shape)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(6, 7, 12)"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "v = fs.to_numpy()\n",
                 "v.shape"
@@ -916,44 +649,44 @@
             "metadata": {},
             "source": [
                 "Metadata access works both on individual fields and slices:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'isobaricInhPa'"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0].metadata(\"typeOfLevel\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "[(1000, 130), (1000, 131)]"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0:2].metadata([\"level\", \"paramId\"])"
             ]
@@ -963,98 +696,98 @@
             "metadata": {},
             "source": [
                 "and on all the fields:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[1000, 1000, 1000, 850]"
+                            "[1000, 1000, 1000, 850, 850, 850]"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs[:4].metadata(\"level\")"
+                "fs.metadata(\"level\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[(1000, 130), (1000, 131), (1000, 132), (850, 130)]"
+                            "[(1000, 130), (1000, 131), (1000, 132), (850, 130), (850, 131), (850, 132)]"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs[:4].metadata([\"level\", \"paramId\"])"
+                "fs.metadata([\"level\", \"paramId\"])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Key qualifiers can be used to prescribe the required metadata type:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "('ecmf', 98, 'ecmf')"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs[0].metadata([\"centre\", \"centre\", \"centre:str\"], astype=(None, int, str))"
+                "fs[0].metadata([\"centre\", \"centre\", \"centre\"], astype=(None, int, str))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Metadata access with [] only works on individual fields:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'ecmf'"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0][\"centre\"]"
             ]
@@ -1071,15 +804,15 @@
             "metadata": {},
             "source": [
                 "Selection by metadata is always creating a \"view\", no copying of GRIB data is involved."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1148,27 +881,27 @@
                             "1   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 22,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g = fs.sel(shortName=[\"u\", \"v\"], level=850)\n",
                 "g.ls()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1237,15 +970,15 @@
                             "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 23,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "g = fs.sel(param=\"t\")\n",
                 "g.ls()"
@@ -1263,15 +996,15 @@
             "metadata": {},
             "source": [
                 "Xarray conversion does not involve disk writing. Under the hood it uses cfgrib."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -1639,60 +1372,60 @@
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    u              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    v              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-4cc48776-c4c8-48cb-a81f-601bc5ffe472' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-4cc48776-c4c8-48cb-a81f-601bc5ffe472' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-4e009685-a0c0-4b94-9bc6-f5515ef6c75c' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4e009685-a0c0-4b94-9bc6-f5515ef6c75c' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-f2e2d92d-e238-4662-8012-69a9dbd17156' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f2e2d92d-e238-4662-8012-69a9dbd17156' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-eaf63056-12a9-498e-b678-bfe6e9c1e84b' class='xr-var-data-in' type='checkbox'><label for='data-eaf63056-12a9-498e-b678-bfe6e9c1e84b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-99fb591c-6233-4ab4-a462-aabe54ef2cfd' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-99fb591c-6233-4ab4-a462-aabe54ef2cfd' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-357f733d-c821-445a-83f1-d8b528303d8e' class='xr-var-data-in' type='checkbox'><label for='data-357f733d-c821-445a-83f1-d8b528303d8e' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-c1f85ff8-aa2c-42c3-a200-d60613c79381' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-c1f85ff8-aa2c-42c3-a200-d60613c79381' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e9096202-efce-4843-b521-821011278f47' class='xr-var-data-in' type='checkbox'><label for='data-e9096202-efce-4843-b521-821011278f47' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-a617317b-8b52-44ba-a126-99ee7f0013a4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a617317b-8b52-44ba-a126-99ee7f0013a4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-81e30adc-a297-43a5-b316-9c3931a019de' class='xr-var-data-in' type='checkbox'><label for='data-81e30adc-a297-43a5-b316-9c3931a019de' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-5efe9b27-c8d7-401d-8f1a-cbfb96a42875' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5efe9b27-c8d7-401d-8f1a-cbfb96a42875' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-9859fa84-ac01-4b2f-a94f-624105210987' class='xr-var-data-in' type='checkbox'><label for='data-9859fa84-ac01-4b2f-a94f-624105210987' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-a1a6cb12-20df-40c9-bb18-f709de8ceb2b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a1a6cb12-20df-40c9-bb18-f709de8ceb2b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e238923e-029f-4ccc-a49b-a4a14e2a54df' class='xr-var-data-in' type='checkbox'><label for='data-e238923e-029f-4ccc-a49b-a4a14e2a54df' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-966f48c8-e658-4896-97d8-3d8be58b538e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-966f48c8-e658-4896-97d8-3d8be58b538e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d5613faf-3c2a-4740-8429-f7f6293f91dc' class='xr-var-data-in' type='checkbox'><label for='data-d5613faf-3c2a-4740-8429-f7f6293f91dc' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-51d5101a-976b-44f2-9d18-a8f6473d0953' class='xr-section-summary-in' type='checkbox'  checked><label for='section-51d5101a-976b-44f2-9d18-a8f6473d0953' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-b6fbb284-48eb-4802-897b-6b587c84370f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b6fbb284-48eb-4802-897b-6b587c84370f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-71a60ffa-bb17-4403-bed6-d4bdedce8af8' class='xr-var-data-in' type='checkbox'><label for='data-71a60ffa-bb17-4403-bed6-d4bdedce8af8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-20275099-3019-440d-96c8-8c609e0f5f62' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-20275099-3019-440d-96c8-8c609e0f5f62' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-05693561-9e14-4a5f-a810-d43fc1f595e4' class='xr-var-data-in' type='checkbox'><label for='data-05693561-9e14-4a5f-a810-d43fc1f595e4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-00de6ad1-2a2f-4f80-b442-980db9ac3ad3' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-00de6ad1-2a2f-4f80-b442-980db9ac3ad3' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f41926c3-51a5-4b74-a6c2-3e9271916bd5' class='xr-var-data-in' type='checkbox'><label for='data-f41926c3-51a5-4b74-a6c2-3e9271916bd5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d6e4e2c0-8349-443f-9945-c8385d8da96b' class='xr-section-summary-in' type='checkbox'  ><label for='section-d6e4e2c0-8349-443f-9945-c8385d8da96b' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-a5e2707b-ac0e-42ce-8c24-9ccf267a1ef9' class='xr-index-data-in' type='checkbox'/><label for='index-a5e2707b-ac0e-42ce-8c24-9ccf267a1ef9' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-ba75bcab-469d-4c88-abb0-c7b94432f388' class='xr-index-data-in' type='checkbox'/><label for='index-ba75bcab-469d-4c88-abb0-c7b94432f388' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-cb7dc903-b1d8-43c1-bf1d-51586eb00381' class='xr-index-data-in' type='checkbox'/><label for='index-cb7dc903-b1d8-43c1-bf1d-51586eb00381' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-025b0ff4-d9f5-44ca-80ae-dd5013622a23' class='xr-index-data-in' type='checkbox'/><label for='index-025b0ff4-d9f5-44ca-80ae-dd5013622a23' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-4d490346-f450-4f11-ab74-4594c88aa0af' class='xr-index-data-in' type='checkbox'/><label for='index-4d490346-f450-4f11-ab74-4594c88aa0af' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-069065ae-60a6-40b6-8581-b2292ffdf35c' class='xr-index-data-in' type='checkbox'/><label for='index-069065ae-60a6-40b6-8581-b2292ffdf35c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-db0e39c7-3033-4a18-81e8-84a3cf647fb7' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-db0e39c7-3033-4a18-81e8-84a3cf647fb7' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>number</span>: 1</li><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-17a6c222-0bdf-49e9-9a37-605c01177cb1' class='xr-section-summary-in' type='checkbox'  checked><label for='section-17a6c222-0bdf-49e9-9a37-605c01177cb1' class='xr-section-summary' >Coordinates: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>number</span></div><div class='xr-var-dims'>(number)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>0</div><input id='attrs-e5e8bc26-bf87-4870-98f3-324cce0f9bb7' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e5e8bc26-bf87-4870-98f3-324cce0f9bb7' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c0b95ce9-7659-44f5-92f8-db8b99bb6f6c' class='xr-var-data-in' type='checkbox'><label for='data-c0b95ce9-7659-44f5-92f8-db8b99bb6f6c' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>ensemble member numerical id</dd><dt><span>units :</span></dt><dd>1</dd><dt><span>standard_name :</span></dt><dd>realization</dd></dl></div><div class='xr-var-data'><pre>array([0])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-9ec6920a-7583-43e5-ad4b-1c9e44c48f05' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9ec6920a-7583-43e5-ad4b-1c9e44c48f05' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0574eef0-17fb-44b0-8ba2-30b1880d17e5' class='xr-var-data-in' type='checkbox'><label for='data-0574eef0-17fb-44b0-8ba2-30b1880d17e5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-0cfdd62d-907e-4e67-ae58-2258e25bf9da' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0cfdd62d-907e-4e67-ae58-2258e25bf9da' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-0dd74b66-c447-4bb7-959c-174f2b902c29' class='xr-var-data-in' type='checkbox'><label for='data-0dd74b66-c447-4bb7-959c-174f2b902c29' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-ab07721d-24f3-4fe5-837d-e0721ea5df7c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ab07721d-24f3-4fe5-837d-e0721ea5df7c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ee0c53ac-74f5-4d93-a30d-a3ac42c373ae' class='xr-var-data-in' type='checkbox'><label for='data-ee0c53ac-74f5-4d93-a30d-a3ac42c373ae' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-980e035e-f00e-43f4-8137-f38a11fd54c0' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-980e035e-f00e-43f4-8137-f38a11fd54c0' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-c32a02da-ed8d-4e78-a546-f15b4d8f4b03' class='xr-var-data-in' type='checkbox'><label for='data-c32a02da-ed8d-4e78-a546-f15b4d8f4b03' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-0bc9e819-b627-4b6d-b829-087606a5813e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0bc9e819-b627-4b6d-b829-087606a5813e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-ea7797bf-d267-4e4b-ab98-ae55b5479e15' class='xr-var-data-in' type='checkbox'><label for='data-ea7797bf-d267-4e4b-ab98-ae55b5479e15' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-b79add36-e2a0-40ff-9bf1-d8abbfb88711' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b79add36-e2a0-40ff-9bf1-d8abbfb88711' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-da901062-7f72-49d6-b95a-022578735e7f' class='xr-var-data-in' type='checkbox'><label for='data-da901062-7f72-49d6-b95a-022578735e7f' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-48c313e7-a24a-4465-a5a8-00cce3c434b3' class='xr-section-summary-in' type='checkbox'  checked><label for='section-48c313e7-a24a-4465-a5a8-00cce3c434b3' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-235ab54e-b4b8-45bc-99c7-e3cad3a9d680' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-235ab54e-b4b8-45bc-99c7-e3cad3a9d680' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-8c7d4c21-9061-4241-97c6-514072d4bcf4' class='xr-var-data-in' type='checkbox'><label for='data-8c7d4c21-9061-4241-97c6-514072d4bcf4' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-1ee7e1bd-50cf-4435-bd35-179936089503' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-1ee7e1bd-50cf-4435-bd35-179936089503' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-5404aa18-18e5-483a-85d1-c08862c97d28' class='xr-var-data-in' type='checkbox'><label for='data-5404aa18-18e5-483a-85d1-c08862c97d28' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(number, time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-2f3867f5-2027-4148-8264-841598cfbed4' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-2f3867f5-2027-4148-8264-841598cfbed4' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-eae0a5e1-a556-49e7-9d20-47939c94ff4b' class='xr-var-data-in' type='checkbox'><label for='data-eae0a5e1-a556-49e7-9d20-47939c94ff4b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a10d0606-54a1-4c97-93af-ed914118ddbe' class='xr-section-summary-in' type='checkbox'  ><label for='section-a10d0606-54a1-4c97-93af-ed914118ddbe' class='xr-section-summary' >Indexes: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>number</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-97013f57-9e3b-4a78-a3b5-599b61df78df' class='xr-index-data-in' type='checkbox'/><label for='index-97013f57-9e3b-4a78-a3b5-599b61df78df' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([0], dtype=&#x27;int64&#x27;, name=&#x27;number&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-282d7849-c5a4-4d6c-abb1-f4e44748c9ea' class='xr-index-data-in' type='checkbox'/><label for='index-282d7849-c5a4-4d6c-abb1-f4e44748c9ea' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-8bd8f5d1-d944-4f5a-a8f2-421508190093' class='xr-index-data-in' type='checkbox'/><label for='index-8bd8f5d1-d944-4f5a-a8f2-421508190093' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-747c0b6a-059b-4945-8789-1aa78050112a' class='xr-index-data-in' type='checkbox'/><label for='index-747c0b6a-059b-4945-8789-1aa78050112a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-003455f9-a696-4c08-a808-8a6e8e54ff74' class='xr-index-data-in' type='checkbox'/><label for='index-003455f9-a696-4c08-a808-8a6e8e54ff74' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-91e9a977-13b1-4de2-8030-47618eebdc76' class='xr-index-data-in' type='checkbox'/><label for='index-91e9a977-13b1-4de2-8030-47618eebdc76' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-75cf2309-6913-4cfd-8c36-a58e53ec3b95' class='xr-section-summary-in' type='checkbox'  checked><label for='section-75cf2309-6913-4cfd-8c36-a58e53ec3b95' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-4120d9a5-4080-4ca8-b5ab-b0835e3f38eb' class='xr-section-summary-in' type='checkbox'  checked><label for='section-4120d9a5-4080-4ca8-b5ab-b0835e3f38eb' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (number: 1, time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * number         (number) int64 0\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    u              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    v              (number, time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 24,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds = fs.to_xarray()\n",
                 "ds"
@@ -1703,15 +1436,15 @@
             "metadata": {},
             "source": [
                 "We can pass all the kwargs arguments cfgrib accepts. On top of that earthkit-data provides the **ignore_keys** option to omit keys from the default set of keys used by cfgrib:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 25,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div><svg style=\"position: absolute; width: 0; height: 0; overflow: hidden\">\n",
                             "<defs>\n",
@@ -2078,59 +1811,59 @@
                             "}\n",
                             "</style><pre class='xr-text-repr-fallback'>&lt;xarray.Dataset&gt;\n",
                             "Dimensions:        (time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    u              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    v              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-ef068533-c607-440e-ba29-2025a9c80732' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-ef068533-c607-440e-ba29-2025a9c80732' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-b1033360-5e6a-4d18-b49d-ef9e0a5d8b45' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b1033360-5e6a-4d18-b49d-ef9e0a5d8b45' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-4fa757b2-d1a3-493c-8717-883f6f647af5' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-4fa757b2-d1a3-493c-8717-883f6f647af5' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-3f34b28e-2639-425c-92fc-1a38c2f22a74' class='xr-var-data-in' type='checkbox'><label for='data-3f34b28e-2639-425c-92fc-1a38c2f22a74' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-49d6903b-97af-491c-8a54-f5ef01c86f11' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-49d6903b-97af-491c-8a54-f5ef01c86f11' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1cead2dc-bb19-4642-9184-0fcc14ffd4f5' class='xr-var-data-in' type='checkbox'><label for='data-1cead2dc-bb19-4642-9184-0fcc14ffd4f5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>1e+03 850.0</div><input id='attrs-9504333c-b753-422f-8aa8-b197baea0c8b' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-9504333c-b753-422f-8aa8-b197baea0c8b' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7d01f085-e650-4ca2-88d4-8d4796adba62' class='xr-var-data-in' type='checkbox'><label for='data-7d01f085-e650-4ca2-88d4-8d4796adba62' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000.,  850.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-d9f9710f-5ed0-48fd-ac10-385cde0fc49d' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d9f9710f-5ed0-48fd-ac10-385cde0fc49d' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-29f2b640-e821-4241-8360-90c194db10d0' class='xr-var-data-in' type='checkbox'><label for='data-29f2b640-e821-4241-8360-90c194db10d0' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-ac69a23a-147f-423e-989e-ad8341ab2020' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-ac69a23a-147f-423e-989e-ad8341ab2020' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-21819152-e957-4fe9-b07a-986671549e5a' class='xr-var-data-in' type='checkbox'><label for='data-21819152-e957-4fe9-b07a-986671549e5a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-417cc3f6-f268-4118-99b7-4f434f66ea47' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-417cc3f6-f268-4118-99b7-4f434f66ea47' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4c42ed07-9cf2-4de8-bee5-1a3db0d2d8fe' class='xr-var-data-in' type='checkbox'><label for='data-4c42ed07-9cf2-4de8-bee5-1a3db0d2d8fe' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-fc496526-e4c2-41f4-b81d-d3bf4e739de6' class='xr-section-summary-in' type='checkbox'  checked><label for='section-fc496526-e4c2-41f4-b81d-d3bf4e739de6' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-dd424e3b-fd11-475c-b2f4-17d14eb2cfe6' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-dd424e3b-fd11-475c-b2f4-17d14eb2cfe6' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-64b5ea80-ada5-43d2-a3e2-68eeeaa99da5' class='xr-var-data-in' type='checkbox'><label for='data-64b5ea80-ada5-43d2-a3e2-68eeeaa99da5' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-300229d5-c9d7-45eb-b855-2bfa30c79f0c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-300229d5-c9d7-45eb-b855-2bfa30c79f0c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-a170869f-a252-4c9a-a953-07b7c174e6ca' class='xr-var-data-in' type='checkbox'><label for='data-a170869f-a252-4c9a-a953-07b7c174e6ca' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-e13be213-c6b8-49d1-b5b7-e6e7f42b504c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e13be213-c6b8-49d1-b5b7-e6e7f42b504c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d945dbbf-e1e3-45c8-8ea4-0e1e083e72a6' class='xr-var-data-in' type='checkbox'><label for='data-d945dbbf-e1e3-45c8-8ea4-0e1e083e72a6' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-ba51f739-43cb-473f-890a-67a05d8c3459' class='xr-section-summary-in' type='checkbox'  ><label for='section-ba51f739-43cb-473f-890a-67a05d8c3459' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-862c1052-8bc7-4599-a51a-a6e14c3addab' class='xr-index-data-in' type='checkbox'/><label for='index-862c1052-8bc7-4599-a51a-a6e14c3addab' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bfcc584a-984f-4357-968d-c529d164530c' class='xr-index-data-in' type='checkbox'/><label for='index-bfcc584a-984f-4357-968d-c529d164530c' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-bd851b81-29ea-489e-8818-6025dab54463' class='xr-index-data-in' type='checkbox'/><label for='index-bd851b81-29ea-489e-8818-6025dab54463' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([1000.0, 850.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-64a01a2e-2ade-4353-a73d-5866a0fd2ca5' class='xr-index-data-in' type='checkbox'/><label for='index-64a01a2e-2ade-4353-a73d-5866a0fd2ca5' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-6ba6590d-b2e6-4b7a-b18b-fbb20532c884' class='xr-index-data-in' type='checkbox'/><label for='index-6ba6590d-b2e6-4b7a-b18b-fbb20532c884' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
+                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-01bdfa88-a320-4eb9-87ff-92f9ca26cc9f' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-01bdfa88-a320-4eb9-87ff-92f9ca26cc9f' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>time</span>: 1</li><li><span class='xr-has-index'>step</span>: 1</li><li><span class='xr-has-index'>isobaricInhPa</span>: 2</li><li><span class='xr-has-index'>latitude</span>: 7</li><li><span class='xr-has-index'>longitude</span>: 12</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-c55677d6-e1b1-4a75-b66f-a5bf09978944' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c55677d6-e1b1-4a75-b66f-a5bf09978944' class='xr-section-summary' >Coordinates: <span>(6)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>time</span></div><div class='xr-var-dims'>(time)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>2018-08-01T12:00:00</div><input id='attrs-0936b6a3-0026-4755-83f7-c22657d1d3f1' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0936b6a3-0026-4755-83f7-c22657d1d3f1' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b2d736eb-bdc3-44aa-9602-72a08cf7bb03' class='xr-var-data-in' type='checkbox'><label for='data-b2d736eb-bdc3-44aa-9602-72a08cf7bb03' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>initial time of forecast</dd><dt><span>standard_name :</span></dt><dd>forecast_reference_time</dd></dl></div><div class='xr-var-data'><pre>array([&#x27;2018-08-01T12:00:00.000000000&#x27;], dtype=&#x27;datetime64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>step</span></div><div class='xr-var-dims'>(step)</div><div class='xr-var-dtype'>timedelta64[ns]</div><div class='xr-var-preview xr-preview'>00:00:00</div><input id='attrs-0e8f705c-fb3e-4976-95a5-db37685f4384' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0e8f705c-fb3e-4976-95a5-db37685f4384' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e913d1ae-f4fd-4a36-bd8c-68f36e742abe' class='xr-var-data-in' type='checkbox'><label for='data-e913d1ae-f4fd-4a36-bd8c-68f36e742abe' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>time since forecast_reference_time</dd><dt><span>standard_name :</span></dt><dd>forecast_period</dd></dl></div><div class='xr-var-data'><pre>array([0], dtype=&#x27;timedelta64[ns]&#x27;)</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>int64</div><div class='xr-var-preview xr-preview'>1000 850</div><input id='attrs-0e43754b-54a9-4d7c-834a-37bb40160a60' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-0e43754b-54a9-4d7c-834a-37bb40160a60' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-b1223a41-0cc1-4abb-8444-a9e024db1732' class='xr-var-data-in' type='checkbox'><label for='data-b1223a41-0cc1-4abb-8444-a9e024db1732' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([1000,  850])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>latitude</span></div><div class='xr-var-dims'>(latitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>90.0 60.0 30.0 ... -60.0 -90.0</div><input id='attrs-d56113cd-12c4-412e-852c-f0af3f949732' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d56113cd-12c4-412e-852c-f0af3f949732' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-1a55ff7a-c6a0-4a81-9613-a4acfc299586' class='xr-var-data-in' type='checkbox'><label for='data-1a55ff7a-c6a0-4a81-9613-a4acfc299586' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd></dl></div><div class='xr-var-data'><pre>array([ 90.,  60.,  30.,   0., -30., -60., -90.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>longitude</span></div><div class='xr-var-dims'>(longitude)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>0.0 30.0 60.0 ... 270.0 300.0 330.0</div><input id='attrs-7f5a7bac-6972-49e4-9aa7-989e8529e899' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-7f5a7bac-6972-49e4-9aa7-989e8529e899' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-84f0b041-be5d-4580-8129-64f2dff39ef8' class='xr-var-data-in' type='checkbox'><label for='data-84f0b041-be5d-4580-8129-64f2dff39ef8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>array([  0.,  30.,  60.,  90., 120., 150., 180., 210., 240., 270., 300., 330.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>valid_time</span></div><div class='xr-var-dims'>(time, step)</div><div class='xr-var-dtype'>datetime64[ns]</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-28f336d8-f2a9-4d1b-b3b4-d9651a62ef8c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-28f336d8-f2a9-4d1b-b3b4-d9651a62ef8c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-11112970-9d92-4a0a-8610-d6e0df39b351' class='xr-var-data-in' type='checkbox'><label for='data-11112970-9d92-4a0a-8610-d6e0df39b351' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>standard_name :</span></dt><dd>time</dd><dt><span>long_name :</span></dt><dd>time</dd></dl></div><div class='xr-var-data'><pre>[1 values with dtype=datetime64[ns]]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-3b511f7a-b7ca-4be7-864f-86a2ec84c129' class='xr-section-summary-in' type='checkbox'  checked><label for='section-3b511f7a-b7ca-4be7-864f-86a2ec84c129' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-e59deb93-7f80-4370-997f-d2c929dd4d07' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-e59deb93-7f80-4370-997f-d2c929dd4d07' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d07b2021-a342-4a53-84dd-124e9f8ccbfe' class='xr-var-data-in' type='checkbox'><label for='data-d07b2021-a342-4a53-84dd-124e9f8ccbfe' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>air_temperature</dd><dt><span>GRIB_cfVarName :</span></dt><dd>t</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>Temperature</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>K</dd><dt><span>long_name :</span></dt><dd>Temperature</dd><dt><span>units :</span></dt><dd>K</dd><dt><span>standard_name :</span></dt><dd>air_temperature</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-acab4bb0-f031-4972-a89e-d572861d9e44' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-acab4bb0-f031-4972-a89e-d572861d9e44' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d243c247-5cbd-4b84-8f29-ffb5855a1a0b' class='xr-var-data-in' type='checkbox'><label for='data-d243c247-5cbd-4b84-8f29-ffb5855a1a0b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>eastward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>u</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>U component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>U component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>eastward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>v</span></div><div class='xr-var-dims'>(time, step, isobaricInhPa, latitude, longitude)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5372495d-a466-428d-9f52-1ef8962f3c07' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5372495d-a466-428d-9f52-1ef8962f3c07' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-bf420c93-6bc8-44c4-bd66-fd370e989d7d' class='xr-var-data-in' type='checkbox'><label for='data-bf420c93-6bc8-44c4-bd66-fd370e989d7d' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>132</dd><dt><span>GRIB_dataType :</span></dt><dd>an</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>84</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_stepUnits :</span></dt><dd>1</dd><dt><span>GRIB_stepType :</span></dt><dd>instant</dd><dt><span>GRIB_gridType :</span></dt><dd>regular_ll</dd><dt><span>GRIB_NV :</span></dt><dd>0</dd><dt><span>GRIB_Nx :</span></dt><dd>12</dd><dt><span>GRIB_Ny :</span></dt><dd>7</dd><dt><span>GRIB_cfName :</span></dt><dd>northward_wind</dd><dt><span>GRIB_cfVarName :</span></dt><dd>v</dd><dt><span>GRIB_gridDefinitionDescription :</span></dt><dd>Latitude/Longitude Grid</dd><dt><span>GRIB_iDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_iScansNegatively :</span></dt><dd>0</dd><dt><span>GRIB_jDirectionIncrementInDegrees :</span></dt><dd>30.0</dd><dt><span>GRIB_jPointsAreConsecutive :</span></dt><dd>0</dd><dt><span>GRIB_jScansPositively :</span></dt><dd>0</dd><dt><span>GRIB_latitudeOfFirstGridPointInDegrees :</span></dt><dd>90.0</dd><dt><span>GRIB_latitudeOfLastGridPointInDegrees :</span></dt><dd>-90.0</dd><dt><span>GRIB_longitudeOfFirstGridPointInDegrees :</span></dt><dd>0.0</dd><dt><span>GRIB_longitudeOfLastGridPointInDegrees :</span></dt><dd>330.0</dd><dt><span>GRIB_missingValue :</span></dt><dd>9999</dd><dt><span>GRIB_name :</span></dt><dd>V component of wind</dd><dt><span>GRIB_shortName :</span></dt><dd>v</dd><dt><span>GRIB_totalNumber :</span></dt><dd>0</dd><dt><span>GRIB_units :</span></dt><dd>m s**-1</dd><dt><span>long_name :</span></dt><dd>V component of wind</dd><dt><span>units :</span></dt><dd>m s**-1</dd><dt><span>standard_name :</span></dt><dd>northward_wind</dd></dl></div><div class='xr-var-data'><pre>[168 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2bb630e1-fa26-4967-b59c-f354837a9dcb' class='xr-section-summary-in' type='checkbox'  ><label for='section-2bb630e1-fa26-4967-b59c-f354837a9dcb' class='xr-section-summary' >Indexes: <span>(5)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>time</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-66fc280d-528b-49e0-bffe-ecf179b1ab77' class='xr-index-data-in' type='checkbox'/><label for='index-66fc280d-528b-49e0-bffe-ecf179b1ab77' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(DatetimeIndex([&#x27;2018-08-01 12:00:00&#x27;], dtype=&#x27;datetime64[ns]&#x27;, name=&#x27;time&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>step</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-fdbbb6f3-73b8-4562-a322-f8edec410372' class='xr-index-data-in' type='checkbox'/><label for='index-fdbbb6f3-73b8-4562-a322-f8edec410372' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(TimedeltaIndex([&#x27;0 days&#x27;], dtype=&#x27;timedelta64[ns]&#x27;, name=&#x27;step&#x27;, freq=None))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-a7784232-1a71-48d0-a148-b26a01343085' class='xr-index-data-in' type='checkbox'/><label for='index-a7784232-1a71-48d0-a148-b26a01343085' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Int64Index([1000, 850], dtype=&#x27;int64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>latitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-04c848f0-27a2-4a0d-9c0e-349cc5dc8b2a' class='xr-index-data-in' type='checkbox'/><label for='index-04c848f0-27a2-4a0d-9c0e-349cc5dc8b2a' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([90.0, 60.0, 30.0, 0.0, -30.0, -60.0, -90.0], dtype=&#x27;float64&#x27;, name=&#x27;latitude&#x27;))</pre></div></li><li class='xr-var-item'><div class='xr-index-name'><div>longitude</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-9c5ca668-c309-410f-94f3-5695f06974e3' class='xr-index-data-in' type='checkbox'/><label for='index-9c5ca668-c309-410f-94f3-5695f06974e3' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([0.0, 30.0, 60.0, 90.0, 120.0, 150.0, 180.0, 210.0, 240.0, 270.0,\n",
                             "              300.0, 330.0],\n",
-                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-52c558e3-2b4f-4b8d-90a8-5afeb8e36527' class='xr-section-summary-in' type='checkbox'  checked><label for='section-52c558e3-2b4f-4b8d-90a8-5afeb8e36527' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "             dtype=&#x27;float64&#x27;, name=&#x27;longitude&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-a4dfbfb4-d7ff-4c8e-a1f9-32f4e74a6649' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a4dfbfb4-d7ff-4c8e-a1f9-32f4e74a6649' class='xr-section-summary' >Attributes: <span>(7)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>GRIB_edition :</span></dt><dd>1</dd><dt><span>GRIB_centre :</span></dt><dd>ecmf</dd><dt><span>GRIB_centreDescription :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>GRIB_subCentre :</span></dt><dd>0</dd><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>institution :</span></dt><dd>European Centre for Medium-Range Weather Forecasts</dd><dt><span>history :</span></dt><dd>2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (time: 1, step: 1, isobaricInhPa: 2, latitude: 7,\n",
                             "                    longitude: 12)\n",
                             "Coordinates:\n",
                             "  * time           (time) datetime64[ns] 2018-08-01T12:00:00\n",
                             "  * step           (step) timedelta64[ns] 00:00:00\n",
-                            "  * isobaricInhPa  (isobaricInhPa) float64 1e+03 850.0\n",
+                            "  * isobaricInhPa  (isobaricInhPa) int64 1000 850\n",
                             "  * latitude       (latitude) float64 90.0 60.0 30.0 0.0 -30.0 -60.0 -90.0\n",
                             "  * longitude      (longitude) float64 0.0 30.0 60.0 90.0 ... 270.0 300.0 330.0\n",
                             "    valid_time     (time, step) datetime64[ns] ...\n",
                             "Data variables:\n",
                             "    t              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    u              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "    v              (time, step, isobaricInhPa, latitude, longitude) float32 ...\n",
                             "Attributes:\n",
                             "    GRIB_edition:            1\n",
                             "    GRIB_centre:             ecmf\n",
                             "    GRIB_centreDescription:  European Centre for Medium-Range Weather Forecasts\n",
                             "    GRIB_subCentre:          0\n",
                             "    Conventions:             CF-1.7\n",
                             "    institution:             European Centre for Medium-Range Weather Forecasts\n",
-                            "    history:                 2023-04-05T15:15 GRIB to CDM+CF via cfgrib-0.9.1..."
+                            "    history:                 2023-05-04T16:43 GRIB to CDM+CF via cfgrib-0.9.1..."
                         ]
                     },
-                    "execution_count": 25,
+                    "execution_count": 24,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ds = fs.to_xarray(xarray_open_dataset_kwargs={\"backend_kwargs\": {\"ignore_keys\": [\"number\"]}})\n",
                 "ds"
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_file_pattern.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_file_pattern.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/grib_from_stream.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_from_stream.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'cells'": "{1: {'source': ['## Reading GRIB from a stream']}}"}*

```diff
@@ -11,15 +11,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "recovered-organizer",
             "metadata": {},
             "source": [
-                "## Loading GRIB data from a stream"
+                "## Reading GRIB from a stream"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "sticky-refrigerator",
             "metadata": {},
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_indexing.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_indexing.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.981463823612072%*

 * *Differences: {"'cells'": "{13: {'outputs': {insert: [(0, OrderedDict([('name', 'stdout'), ('output_type', "*

 * *            "'stream'), ('text', ['coord_vals=[300, 400, 500, 700, 850, 1000] len=6\\n'])]))]}}, "*

 * *            "15: {'outputs': []}, 23: {'outputs': {0: {'data': {'text/html': {insert: [(36, '      "*

 * *            "<td>850</td>\\n'), (49, '      <td>500</td>\\n'), (62, '      <td>850</td>\\n'), (75, "*

 * *            "'      <td>500</td>\\n'), (88, '      <td>850</td>\\n'), (101, '      "*

 * *            "<td>500</td>\\n')] […]*

```diff
@@ -157,14 +157,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "coord_vals=[300, 400, 500, 700, 850, 1000] len=6\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
                             "3"
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
@@ -183,23 +190,15 @@
                 "When keys not present in the index db are used the functions above do not work:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "error: 'sel: GRIB key=gridType not found in index db'\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "try:\n",
                 "    a = fs.sel(gridType=\"regular_ll\")\n",
                 "except KeyError as e:\n",
                 "    print(f\"error: {e}\")   "
             ]
         },
@@ -412,99 +411,99 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>v</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>v</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
-                            "2   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
-                            "3   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
-                            "4   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
-                            "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
+                            "2   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
+                            "3   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
+                            "4   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "5   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
@@ -516,57 +515,14 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs = earthkit.data.from_source(\"file\", \"./_grib_dir_with_sql\", indexing=True, level=[500, 850], order_by=\"variable\")\n",
                 "fs.ls()"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Availability"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "The availability tells us what MARS settings we would need if we wanted to download the data from the MARS archive."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 15,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "'andate=None, anoffset=None, antime=None, channel=None, class=od, date=20180801, diagnostic=None, direction=None, domain=g, expver=0001, fcmonth=None, fcperiod=None, frequency=None, hdate=None, ident=None, instrument=None, iteration=None, leadtime=None, levelist=300, levtype=pl, method=None, number=None, obstype=None, opttime=None, origin=None, param=[t, u, v], quantile=None, range=None, reference=None, reportype=None, step=0, stream=oper, time=1200, type=an, verify=None\\n'"
-                        ]
-                    },
-                    "execution_count": 15,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "a.availability"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 16,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "x = fs.to_xarray()"
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "mpy38",
             "language": "python",
             "name": "mpy38"
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_metadata.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_metadata.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9776879369870426%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}}, 3: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}}, 8: {'metadata': {replace: OrderedDict([('tags', "*

 * *            "[])])}, 'outputs': {0: {'data': {'text/plain': {insert: [(0, '  centre shortName    "*

 * *            "typeOfLevel  level  dataDate  dataTime stepRange   \\n'), (1, '0   ecmf         t  "*

 * *            "isobaricInhPa   1000  20180801      1200         0  \\\\\\n')], delete: [1, 0]}}}}}, "*

 * *            "10: {'met […]*

```diff
@@ -1,13 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "code",
             "execution_count": 1,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "!test -f test6.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test6.grib"
             ]
         },
         {
             "cell_type": "markdown",
@@ -22,15 +24,17 @@
             "source": [
                 "We load a GRIB file containing 6 messages:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
                 "\n",
                 "fs = earthkit.data.from_source(\"file\", \"test6.grib\")"
             ]
         },
@@ -65,15 +69,17 @@
             "source": [
                 "head() displays the first 5 messages by default:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -171,16 +177,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
@@ -205,15 +211,17 @@
             "source": [
                 "The number of fields can be passed as an argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -272,16 +280,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -293,15 +301,17 @@
             "source": [
                 "fs.head(2)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
@@ -360,16 +370,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
@@ -382,20 +392,130 @@
                 "fs.head(n=2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The keys can be taken from an ecCodes GRIB namespace:"
+                "The keys can be taken from an [ecCodes GRIB namespace](https://confluence.ecmwf.int/display/UDOC/What+are+namespaces+-+ecCodes+GRIB+FAQ):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>max</th>\n",
+                            "      <th>min</th>\n",
+                            "      <th>avg</th>\n",
+                            "      <th>sd</th>\n",
+                            "      <th>skew</th>\n",
+                            "      <th>kurt</th>\n",
+                            "      <th>const</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>320.564178</td>\n",
+                            "      <td>240.564178</td>\n",
+                            "      <td>279.707036</td>\n",
+                            "      <td>19.674217</td>\n",
+                            "      <td>-0.731230</td>\n",
+                            "      <td>-0.169046</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>17.713120</td>\n",
+                            "      <td>-6.286880</td>\n",
+                            "      <td>-0.382119</td>\n",
+                            "      <td>5.605310</td>\n",
+                            "      <td>1.139004</td>\n",
+                            "      <td>1.018780</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>11.833481</td>\n",
+                            "      <td>-16.166519</td>\n",
+                            "      <td>-0.071281</td>\n",
+                            "      <td>6.140457</td>\n",
+                            "      <td>-0.217654</td>\n",
+                            "      <td>-0.839983</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>3</th>\n",
+                            "      <td>304.539169</td>\n",
+                            "      <td>232.539169</td>\n",
+                            "      <td>272.729646</td>\n",
+                            "      <td>19.241867</td>\n",
+                            "      <td>-0.998189</td>\n",
+                            "      <td>0.135718</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>4</th>\n",
+                            "      <td>27.101624</td>\n",
+                            "      <td>-12.898376</td>\n",
+                            "      <td>0.339719</td>\n",
+                            "      <td>8.141047</td>\n",
+                            "      <td>1.542573</td>\n",
+                            "      <td>1.864089</td>\n",
+                            "      <td>0.0</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "          max         min         avg         sd      skew      kurt  const\n",
+                            "0  320.564178  240.564178  279.707036  19.674217 -0.731230 -0.169046    0.0\n",
+                            "1   17.713120   -6.286880   -0.382119   5.605310  1.139004  1.018780    0.0\n",
+                            "2   11.833481  -16.166519   -0.071281   6.140457 -0.217654 -0.839983    0.0\n",
+                            "3  304.539169  232.539169  272.729646  19.241867 -0.998189  0.135718    0.0\n",
+                            "4   27.101624  -12.898376    0.339719   8.141047  1.542573  1.864089    0.0"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "fs.head(namespace=\"statistics\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -472,15 +592,15 @@
                             "0   ecmf      130        K          Temperature         t\n",
                             "1   ecmf      131  m s**-1  U component of wind         u\n",
                             "2   ecmf      132  m s**-1  V component of wind         v\n",
                             "3   ecmf      130        K          Temperature         t\n",
                             "4   ecmf      131  m s**-1  U component of wind         u"
                         ]
                     },
-                    "execution_count": 6,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.head(namespace=\"parameter\")"
             ]
@@ -490,15 +610,15 @@
             "metadata": {},
             "source": [
                 "The list of keys can be prescribed:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -539,15 +659,15 @@
                         ],
                         "text/plain": [
                             "   bitsPerValue  packingType\n",
                             "0             4  grid_simple\n",
                             "1             4  grid_simple"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.head(n=2, keys=[\"bitsPerValue\", \"packingType\"])"
             ]
@@ -557,15 +677,15 @@
             "metadata": {},
             "source": [
                 "The list of keys can also be extended:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -670,30 +790,30 @@
                             "      <td>131</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  paramId  \n",
                             "0       an       0  regular_ll      130  \n",
                             "1       an       0  regular_ll      131  \n",
                             "2       an       0  regular_ll      132  \n",
                             "3       an       0  regular_ll      130  \n",
                             "4       an       0  regular_ll      131  "
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.head(extra_keys=\"paramId\")"
             ]
@@ -710,15 +830,15 @@
             "metadata": {},
             "source": [
                 "tail() displays the last 5 messages by default:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -817,30 +937,30 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         u  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "3   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.tail(5)"
             ]
@@ -857,15 +977,15 @@
             "metadata": {},
             "source": [
                 "By default all the fields are listed:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -977,16 +1097,16 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
                             "3   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
                             "4   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
                             "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
@@ -994,15 +1114,15 @@
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
                             "5       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.ls()"
             ]
@@ -1012,15 +1132,15 @@
             "metadata": {},
             "source": [
                 "The number of fields to list can also be specified:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1080,35 +1200,35 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0  \\\n",
                             "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.ls(2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1168,24 +1288,24 @@
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
+                            "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange   \n",
+                            "0   ecmf         u  isobaricInhPa    850  20180801      1200         0  \\\n",
                             "1   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  "
                         ]
                     },
-                    "execution_count": 12,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.ls(-2)"
             ]
@@ -1202,42 +1322,42 @@
             "metadata": {},
             "source": [
                 "We can describe the whole object:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_02b8c th {\n",
+                            "#T_8ae4e th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_02b8c_row0_col0, #T_02b8c_row0_col1, #T_02b8c_row0_col2, #T_02b8c_row0_col3, #T_02b8c_row0_col4, #T_02b8c_row0_col5, #T_02b8c_row0_col6, #T_02b8c_row0_col7, #T_02b8c_row0_col8, #T_02b8c_row1_col0, #T_02b8c_row1_col1, #T_02b8c_row1_col2, #T_02b8c_row1_col3, #T_02b8c_row1_col4, #T_02b8c_row1_col5, #T_02b8c_row1_col6, #T_02b8c_row1_col7, #T_02b8c_row1_col8, #T_02b8c_row2_col0, #T_02b8c_row2_col1, #T_02b8c_row2_col2, #T_02b8c_row2_col3, #T_02b8c_row2_col4, #T_02b8c_row2_col5, #T_02b8c_row2_col6, #T_02b8c_row2_col7, #T_02b8c_row2_col8 {\n",
+                            "#T_8ae4e_row0_col0, #T_8ae4e_row0_col1, #T_8ae4e_row0_col2, #T_8ae4e_row0_col3, #T_8ae4e_row0_col4, #T_8ae4e_row0_col5, #T_8ae4e_row0_col6, #T_8ae4e_row0_col7, #T_8ae4e_row0_col8, #T_8ae4e_row1_col0, #T_8ae4e_row1_col1, #T_8ae4e_row1_col2, #T_8ae4e_row1_col3, #T_8ae4e_row1_col4, #T_8ae4e_row1_col5, #T_8ae4e_row1_col6, #T_8ae4e_row1_col7, #T_8ae4e_row1_col8, #T_8ae4e_row2_col0, #T_8ae4e_row2_col1, #T_8ae4e_row2_col2, #T_8ae4e_row2_col3, #T_8ae4e_row2_col4, #T_8ae4e_row2_col5, #T_8ae4e_row2_col6, #T_8ae4e_row2_col7, #T_8ae4e_row2_col8 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_02b8c\">\n",
+                            "<table id=\"T_8ae4e\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank\" >&nbsp;</th>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_02b8c_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
-                            "      <th id=\"T_02b8c_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
-                            "      <th id=\"T_02b8c_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
-                            "      <th id=\"T_02b8c_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
-                            "      <th id=\"T_02b8c_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
-                            "      <th id=\"T_02b8c_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
-                            "      <th id=\"T_02b8c_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
-                            "      <th id=\"T_02b8c_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
-                            "      <th id=\"T_02b8c_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col0\" class=\"col_heading level0 col0\" >level</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col1\" class=\"col_heading level0 col1\" >date</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col2\" class=\"col_heading level0 col2\" >time</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col3\" class=\"col_heading level0 col3\" >step</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col4\" class=\"col_heading level0 col4\" >paramId</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col5\" class=\"col_heading level0 col5\" >class</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col6\" class=\"col_heading level0 col6\" >stream</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col7\" class=\"col_heading level0 col7\" >type</th>\n",
+                            "      <th id=\"T_8ae4e_level0_col8\" class=\"col_heading level0 col8\" >experimentVersionNumber</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th class=\"index_name level0\" >shortName</th>\n",
                             "      <th class=\"index_name level1\" >typeOfLevel</th>\n",
                             "      <th class=\"blank col0\" >&nbsp;</th>\n",
                             "      <th class=\"blank col1\" >&nbsp;</th>\n",
                             "      <th class=\"blank col2\" >&nbsp;</th>\n",
@@ -1247,60 +1367,60 @@
                             "      <th class=\"blank col6\" >&nbsp;</th>\n",
                             "      <th class=\"blank col7\" >&nbsp;</th>\n",
                             "      <th class=\"blank col8\" >&nbsp;</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_02b8c_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
-                            "      <th id=\"T_02b8c_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_02b8c_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_02b8c_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
-                            "      <td id=\"T_02b8c_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
-                            "      <td id=\"T_02b8c_row0_col3\" class=\"data row0 col3\" >0</td>\n",
-                            "      <td id=\"T_02b8c_row0_col4\" class=\"data row0 col4\" >130</td>\n",
-                            "      <td id=\"T_02b8c_row0_col5\" class=\"data row0 col5\" >od</td>\n",
-                            "      <td id=\"T_02b8c_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
-                            "      <td id=\"T_02b8c_row0_col7\" class=\"data row0 col7\" >an</td>\n",
-                            "      <td id=\"T_02b8c_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_02b8c_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
-                            "      <th id=\"T_02b8c_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_02b8c_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_02b8c_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
-                            "      <td id=\"T_02b8c_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
-                            "      <td id=\"T_02b8c_row1_col3\" class=\"data row1 col3\" >0</td>\n",
-                            "      <td id=\"T_02b8c_row1_col4\" class=\"data row1 col4\" >131</td>\n",
-                            "      <td id=\"T_02b8c_row1_col5\" class=\"data row1 col5\" >od</td>\n",
-                            "      <td id=\"T_02b8c_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
-                            "      <td id=\"T_02b8c_row1_col7\" class=\"data row1 col7\" >an</td>\n",
-                            "      <td id=\"T_02b8c_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_02b8c_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
-                            "      <th id=\"T_02b8c_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
-                            "      <td id=\"T_02b8c_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
-                            "      <td id=\"T_02b8c_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
-                            "      <td id=\"T_02b8c_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
-                            "      <td id=\"T_02b8c_row2_col3\" class=\"data row2 col3\" >0</td>\n",
-                            "      <td id=\"T_02b8c_row2_col4\" class=\"data row2 col4\" >132</td>\n",
-                            "      <td id=\"T_02b8c_row2_col5\" class=\"data row2 col5\" >od</td>\n",
-                            "      <td id=\"T_02b8c_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
-                            "      <td id=\"T_02b8c_row2_col7\" class=\"data row2 col7\" >an</td>\n",
-                            "      <td id=\"T_02b8c_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
+                            "      <th id=\"T_8ae4e_level0_row0\" class=\"row_heading level0 row0\" >t</th>\n",
+                            "      <th id=\"T_8ae4e_level1_row0\" class=\"row_heading level1 row0\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_8ae4e_row0_col0\" class=\"data row0 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col1\" class=\"data row0 col1\" >20180801</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col2\" class=\"data row0 col2\" >1200</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col3\" class=\"data row0 col3\" >0</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col4\" class=\"data row0 col4\" >130</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col5\" class=\"data row0 col5\" >od</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col6\" class=\"data row0 col6\" >oper</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col7\" class=\"data row0 col7\" >an</td>\n",
+                            "      <td id=\"T_8ae4e_row0_col8\" class=\"data row0 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_8ae4e_level0_row1\" class=\"row_heading level0 row1\" >u</th>\n",
+                            "      <th id=\"T_8ae4e_level1_row1\" class=\"row_heading level1 row1\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_8ae4e_row1_col0\" class=\"data row1 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col1\" class=\"data row1 col1\" >20180801</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col2\" class=\"data row1 col2\" >1200</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col3\" class=\"data row1 col3\" >0</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col4\" class=\"data row1 col4\" >131</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col5\" class=\"data row1 col5\" >od</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col6\" class=\"data row1 col6\" >oper</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col7\" class=\"data row1 col7\" >an</td>\n",
+                            "      <td id=\"T_8ae4e_row1_col8\" class=\"data row1 col8\" >0001</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_8ae4e_level0_row2\" class=\"row_heading level0 row2\" >v</th>\n",
+                            "      <th id=\"T_8ae4e_level1_row2\" class=\"row_heading level1 row2\" >isobaricInhPa</th>\n",
+                            "      <td id=\"T_8ae4e_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col1\" class=\"data row2 col1\" >20180801</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col2\" class=\"data row2 col2\" >1200</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col3\" class=\"data row2 col3\" >0</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col4\" class=\"data row2 col4\" >132</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col5\" class=\"data row2 col5\" >od</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col6\" class=\"data row2 col6\" >oper</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col7\" class=\"data row2 col7\" >an</td>\n",
+                            "      <td id=\"T_8ae4e_row2_col8\" class=\"data row2 col8\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x11e4d8280>"
+                            "<pandas.io.formats.style.Styler at 0x1412bdb10>"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.describe()"
             ]
@@ -1310,164 +1430,164 @@
             "metadata": {},
             "source": [
                 "We can also describe a given parameter (defined by shortName or paramId):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_d6942 th {\n",
+                            "#T_ed832 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_d6942_row0_col0, #T_d6942_row1_col0, #T_d6942_row2_col0, #T_d6942_row3_col0, #T_d6942_row4_col0, #T_d6942_row5_col0, #T_d6942_row6_col0, #T_d6942_row7_col0, #T_d6942_row8_col0, #T_d6942_row9_col0, #T_d6942_row10_col0 {\n",
+                            "#T_ed832_row0_col0, #T_ed832_row1_col0, #T_ed832_row2_col0, #T_ed832_row3_col0, #T_ed832_row4_col0, #T_ed832_row5_col0, #T_ed832_row6_col0, #T_ed832_row7_col0, #T_ed832_row8_col0, #T_ed832_row9_col0, #T_ed832_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_d6942\">\n",
+                            "<table id=\"T_ed832\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_d6942_row0_col0\" class=\"data row0 col0\" >t</td>\n",
+                            "      <th id=\"T_ed832_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_ed832_row0_col0\" class=\"data row0 col0\" >t</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_d6942_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_ed832_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_ed832_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_d6942_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_ed832_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_ed832_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_d6942_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_ed832_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_ed832_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_d6942_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_ed832_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_ed832_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_d6942_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_ed832_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_ed832_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_d6942_row6_col0\" class=\"data row6 col0\" >130</td>\n",
+                            "      <th id=\"T_ed832_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_ed832_row6_col0\" class=\"data row6 col0\" >130</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_d6942_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_ed832_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_ed832_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_d6942_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_ed832_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_ed832_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_d6942_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_ed832_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_ed832_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_d6942_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_d6942_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_ed832_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_ed832_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x11e4d9250>"
+                            "<pandas.io.formats.style.Styler at 0x155bf6d50>"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.describe(\"t\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
-                            "#T_9660a th {\n",
+                            "#T_f5ed5 th {\n",
                             "  text-align: left;\n",
                             "}\n",
-                            "#T_9660a_row0_col0, #T_9660a_row1_col0, #T_9660a_row2_col0, #T_9660a_row3_col0, #T_9660a_row4_col0, #T_9660a_row5_col0, #T_9660a_row6_col0, #T_9660a_row7_col0, #T_9660a_row8_col0, #T_9660a_row9_col0, #T_9660a_row10_col0 {\n",
+                            "#T_f5ed5_row0_col0, #T_f5ed5_row1_col0, #T_f5ed5_row2_col0, #T_f5ed5_row3_col0, #T_f5ed5_row4_col0, #T_f5ed5_row5_col0, #T_f5ed5_row6_col0, #T_f5ed5_row7_col0, #T_f5ed5_row8_col0, #T_f5ed5_row9_col0, #T_f5ed5_row10_col0 {\n",
                             "  text-align: left;\n",
                             "}\n",
                             "</style>\n",
-                            "<table id=\"T_9660a\">\n",
+                            "<table id=\"T_f5ed5\">\n",
                             "  <thead>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
-                            "      <td id=\"T_9660a_row0_col0\" class=\"data row0 col0\" >u</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row0\" class=\"row_heading level0 row0\" >shortName</th>\n",
+                            "      <td id=\"T_f5ed5_row0_col0\" class=\"data row0 col0\" >u</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
-                            "      <td id=\"T_9660a_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row1\" class=\"row_heading level0 row1\" >typeOfLevel</th>\n",
+                            "      <td id=\"T_f5ed5_row1_col0\" class=\"data row1 col0\" >isobaricInhPa</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
-                            "      <td id=\"T_9660a_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row2\" class=\"row_heading level0 row2\" >level</th>\n",
+                            "      <td id=\"T_f5ed5_row2_col0\" class=\"data row2 col0\" >1000,850</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
-                            "      <td id=\"T_9660a_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row3\" class=\"row_heading level0 row3\" >date</th>\n",
+                            "      <td id=\"T_f5ed5_row3_col0\" class=\"data row3 col0\" >20180801</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
-                            "      <td id=\"T_9660a_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row4\" class=\"row_heading level0 row4\" >time</th>\n",
+                            "      <td id=\"T_f5ed5_row4_col0\" class=\"data row4 col0\" >1200</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
-                            "      <td id=\"T_9660a_row5_col0\" class=\"data row5 col0\" >0</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row5\" class=\"row_heading level0 row5\" >step</th>\n",
+                            "      <td id=\"T_f5ed5_row5_col0\" class=\"data row5 col0\" >0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
-                            "      <td id=\"T_9660a_row6_col0\" class=\"data row6 col0\" >131</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row6\" class=\"row_heading level0 row6\" >paramId</th>\n",
+                            "      <td id=\"T_f5ed5_row6_col0\" class=\"data row6 col0\" >131</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
-                            "      <td id=\"T_9660a_row7_col0\" class=\"data row7 col0\" >od</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row7\" class=\"row_heading level0 row7\" >class</th>\n",
+                            "      <td id=\"T_f5ed5_row7_col0\" class=\"data row7 col0\" >od</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
-                            "      <td id=\"T_9660a_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row8\" class=\"row_heading level0 row8\" >stream</th>\n",
+                            "      <td id=\"T_f5ed5_row8_col0\" class=\"data row8 col0\" >oper</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
-                            "      <td id=\"T_9660a_row9_col0\" class=\"data row9 col0\" >an</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row9\" class=\"row_heading level0 row9\" >type</th>\n",
+                            "      <td id=\"T_f5ed5_row9_col0\" class=\"data row9 col0\" >an</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_9660a_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
-                            "      <td id=\"T_9660a_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
+                            "      <th id=\"T_f5ed5_level0_row10\" class=\"row_heading level0 row10\" >experimentVersionNumber</th>\n",
+                            "      <td id=\"T_f5ed5_row10_col0\" class=\"data row10 col0\" >0001</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x11f9d1fa0>"
+                            "<pandas.io.formats.style.Styler at 0x1558ef190>"
                         ]
                     },
-                    "execution_count": 15,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.describe(131)"
             ]
@@ -1484,49 +1604,49 @@
             "metadata": {},
             "source": [
                 "metadata() with positional arguments works for both single and multiple fields. key type qualifiers are allowed to be used."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "['isobaricInhPa',\n",
                             " 'isobaricInhPa',\n",
                             " 'isobaricInhPa',\n",
                             " 'isobaricInhPa',\n",
                             " 'isobaricInhPa',\n",
                             " 'isobaricInhPa']"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs.metadata(\"typeOfLevel\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "('isobaricInhPa', 1000, 'ecmf', 98)"
                         ]
                     },
-                    "execution_count": 17,
+                    "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0].metadata([\"typeOfLevel\", \"level\", \"centre\", \"centre\"], astype=(None, None, str, int))"
             ]
@@ -1536,24 +1656,24 @@
             "metadata": {},
             "source": [
                 "For single fields the bracket operator can also be used:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "'t'"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0][\"param\"]"
             ]
@@ -1563,28 +1683,28 @@
             "metadata": {},
             "source": [
                 "Namespace keys can be fetched as a dict for single fields:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'centre': 'ecmf',\n",
                             " 'paramId': 130,\n",
                             " 'units': 'K',\n",
                             " 'name': 'Temperature',\n",
                             " 'shortName': 't'}"
                         ]
                     },
-                    "execution_count": 19,
+                    "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0].metadata(namespace=\"parameter\")"
             ]
@@ -1601,16 +1721,18 @@
             "metadata": {},
             "source": [
                 "dump() gives a tabbed interface to inspect the various namespaces:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
-            "metadata": {},
+            "execution_count": 21,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\"> /* Based on:\n",
                             " https://codepen.io/htmlcssfreebies/pen/WNpVeRK\n",
                             " https://github.com/pydata/xarray/blob/main/xarray/static/css/style.css\n",
@@ -1742,107 +1864,107 @@
                             "</style><div class=\"eh-description\">GribField</div>\n",
                             "<div>\n",
                             "<section class=\"eh-section>\n",
                             "<div class=\"eh-tabs-container\">\n",
                             "<div class=\"eh-tabs-block\">\n",
                             "<div class=\"eh-tabs\">\n",
                             "\n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"9d595129-d2f8-45d2-acb4-b5c18dd92135\"  />\n",
-                            "<label for=\"9d595129-d2f8-45d2-acb4-b5c18dd92135\" title=\"Keys in the ecCodes None namespace\">default</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"bd2ba442-d557-48ff-b3a1-ba0971c1f9e7\"  />\n",
+                            "<label for=\"bd2ba442-d557-48ff-b3a1-ba0971c1f9e7\" title=\"Keys in the ecCodes None namespace\">default</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
-                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>mybits</b></td><td>None</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
+                            "<tr><td><b>globalDomain</b></td><td>g</td></tr> <tr><td><b>GRIBEditionNumber</b></td><td>1</td></tr> <tr><td><b>eps</b></td><td>0</td></tr> <tr><td><b>offsetSection0</b></td><td>0</td></tr> <tr><td><b>section0Length</b></td><td>8</td></tr> <tr><td><b>totalLength</b></td><td>150</td></tr> <tr><td><b>editionNumber</b></td><td>1</td></tr> <tr><td><b>WMO</b></td><td>0</td></tr> <tr><td><b>productionStatusOfProcessedData</b></td><td>0</td></tr> <tr><td><b>section1Length</b></td><td>52</td></tr> <tr><td><b>wrongPadding</b></td><td>0</td></tr> <tr><td><b>table2Version</b></td><td>128</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>centreDescription</b></td><td>European Centre for Medium-Range Weather Forecasts</td></tr> <tr><td><b>generatingProcessIdentifier</b></td><td>254</td></tr> <tr><td><b>gridDefinition</b></td><td>255</td></tr> <tr><td><b>indicatorOfParameter</b></td><td>130</td></tr> <tr><td><b>parameterName</b></td><td>Temperature</td></tr> <tr><td><b>parameterUnits</b></td><td>K</td></tr> <tr><td><b>indicatorOfTypeOfLevel</b></td><td>pl</td></tr> <tr><td><b>pressureUnits</b></td><td>hPa</td></tr> <tr><td><b>typeOfLevelECMF</b></td><td>isobaricInhPa</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>yearOfCentury</b></td><td>18</td></tr> <tr><td><b>month</b></td><td>8</td></tr> <tr><td><b>day</b></td><td>1</td></tr> <tr><td><b>hour</b></td><td>12</td></tr> <tr><td><b>minute</b></td><td>0</td></tr> <tr><td><b>second</b></td><td>0</td></tr> <tr><td><b>unitOfTimeRange</b></td><td>1</td></tr> <tr><td><b>P1</b></td><td>0</td></tr> <tr><td><b>P2</b></td><td>0</td></tr> <tr><td><b>timeRangeIndicator</b></td><td>0</td></tr> <tr><td><b>numberIncludedInAverage</b></td><td>0</td></tr> <tr><td><b>numberMissingFromAveragesOrAccumulations</b></td><td>0</td></tr> <tr><td><b>centuryOfReferenceTimeOfData</b></td><td>21</td></tr> <tr><td><b>subCentre</b></td><td>0</td></tr> <tr><td><b>paramIdECMF</b></td><td>130</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>cfNameECMF</b></td><td>air_temperature</td></tr> <tr><td><b>cfName</b></td><td>air_temperature</td></tr> <tr><td><b>cfVarNameECMF</b></td><td>t</td></tr> <tr><td><b>cfVarName</b></td><td>t</td></tr> <tr><td><b>unitsECMF</b></td><td>K</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>nameECMF</b></td><td>Temperature</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>decimalScaleFactor</b></td><td>0</td></tr> <tr><td><b>setLocalDefinition</b></td><td>0</td></tr> <tr><td><b>optimizeScaleFactor</b></td><td>0</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>year</b></td><td>2018</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>julianDay</b></td><td>2458332.0</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>marsParam</b></td><td>130.128</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr> <tr><td><b>deleteLocalDefinition</b></td><td>0</td></tr> <tr><td><b>localUsePresent</b></td><td>1</td></tr> <tr><td><b>reservedNeedNotBePresent</b></td><td>None</td></tr> <tr><td><b>localDefinitionNumber</b></td><td>1</td></tr> <tr><td><b>GRIBEXSection1Problem</b></td><td>0</td></tr> <tr><td><b>marsClass</b></td><td>od</td></tr> <tr><td><b>marsType</b></td><td>an</td></tr> <tr><td><b>marsStream</b></td><td>oper</td></tr> <tr><td><b>experimentVersionNumber</b></td><td>0001</td></tr> <tr><td><b>perturbationNumber</b></td><td>0</td></tr> <tr><td><b>numberOfForecastsInEnsemble</b></td><td>0</td></tr> <tr><td><b>padding_local1_1</b></td><td>None</td></tr> <tr><td><b>grib2LocalSectionNumber</b></td><td>1</td></tr> <tr><td><b>localExtensionPadding</b></td><td>None</td></tr> <tr><td><b>_x</b></td><td>None</td></tr> <tr><td><b>section1Padding</b></td><td>None</td></tr> <tr><td><b>shortNameECMF</b></td><td>t</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>ifsParam</b></td><td>130</td></tr> <tr><td><b>stepTypeForConversion</b></td><td>unknown</td></tr> <tr><td><b>md5Section1</b></td><td>3ae6b1f6f34f431c6134c40ec42f27fa</td></tr> <tr><td><b>md5Product</b></td><td>54697e1d910c88b76a8759b67e5c7a9c</td></tr> <tr><td><b>gridDescriptionSectionPresent</b></td><td>1</td></tr> <tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>angleSubdivisions</b></td><td>1000</td></tr> <tr><td><b>section2Length</b></td><td>32</td></tr> <tr><td><b>radius</b></td><td>6367470</td></tr> <tr><td><b>numberOfVerticalCoordinateValues</b></td><td>0</td></tr> <tr><td><b>neitherPresent</b></td><td>255</td></tr> <tr><td><b>pvlLocation</b></td><td>255</td></tr> <tr><td><b>dataRepresentationType</b></td><td>0</td></tr> <tr><td><b>gridDefinitionDescription</b></td><td>Latitude/Longitude Grid</td></tr> <tr><td><b>gridDefinitionTemplateNumber</b></td><td>0</td></tr> <tr><td><b>Ni</b></td><td>12</td></tr> <tr><td><b>Nj</b></td><td>7</td></tr> <tr><td><b>latitudeOfFirstGridPoint</b></td><td>90000</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPoint</b></td><td>0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>resolutionAndComponentFlags</b></td><td>128</td></tr> <tr><td><b>ijDirectionIncrementGiven</b></td><td>1</td></tr> <tr><td><b>earthIsOblate</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags3</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags4</b></td><td>0</td></tr> <tr><td><b>uvRelativeToGrid</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags6</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags7</b></td><td>0</td></tr> <tr><td><b>resolutionAndComponentFlags8</b></td><td>0</td></tr> <tr><td><b>latitudeOfLastGridPoint</b></td><td>-90000</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPoint</b></td><td>330000</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>jDirectionIncrement</b></td><td>30000</td></tr> <tr><td><b>scanningMode</b></td><td>0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>alternativeRowScanning</b></td><td>0</td></tr> <tr><td><b>iScansPositively</b></td><td>1</td></tr> <tr><td><b>jScansNegatively</b></td><td>1</td></tr> <tr><td><b>scanningMode4</b></td><td>0</td></tr> <tr><td><b>scanningMode5</b></td><td>0</td></tr> <tr><td><b>scanningMode6</b></td><td>0</td></tr> <tr><td><b>scanningMode7</b></td><td>0</td></tr> <tr><td><b>scanningMode8</b></td><td>0</td></tr> <tr><td><b>swapScanningAlternativeRows</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>numberOfDataPoints</b></td><td>84</td></tr> <tr><td><b>numberOfValues</b></td><td>84</td></tr> <tr><td><b>zeros</b></td><td></td></tr> <tr><td><b>PVPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_2</b></td><td>None</td></tr> <tr><td><b>PLPresent</b></td><td>0</td></tr> <tr><td><b>padding_sec2_1</b></td><td>None</td></tr> <tr><td><b>deletePV</b></td><td>1</td></tr> <tr><td><b>padding_sec2_3</b></td><td>None</td></tr> <tr><td><b>md5Section2</b></td><td>e09e4d6171c0ac85da1d256b2f8acf88</td></tr> <tr><td><b>lengthOfHeaders</b></td><td>85</td></tr> <tr><td><b>md5Headers</b></td><td>9160fb809a9d7b1efc95163bf36e6b51</td></tr> <tr><td><b>missingValue</b></td><td>9999</td></tr> <tr><td><b>tableReference</b></td><td>0</td></tr> <tr><td><b>section4Length</b></td><td>54</td></tr> <tr><td><b>halfByte</b></td><td>8</td></tr> <tr><td><b>dataFlag</b></td><td>8</td></tr> <tr><td><b>binaryScaleFactor</b></td><td>3</td></tr> <tr><td><b>referenceValue</b></td><td>240.56417846679688</td></tr> <tr><td><b>referenceValueError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>sphericalHarmonics</b></td><td>0</td></tr> <tr><td><b>complexPacking</b></td><td>0</td></tr> <tr><td><b>integerPointValues</b></td><td>0</td></tr> <tr><td><b>additionalFlagPresent</b></td><td>0</td></tr> <tr><td><b>orderOfSPD</b></td><td>2</td></tr> <tr><td><b>boustrophedonic</b></td><td>0</td></tr> <tr><td><b>hideThis</b></td><td>0</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>bitsPerValue</b></td><td>4</td></tr> <tr><td><b>constantFieldHalfByte</b></td><td>8</td></tr> <tr><td><b>bitMapIndicator</b></td><td>255</td></tr> <tr><td><b>numberOfCodedValues</b></td><td>84</td></tr> <tr><td><b>packingError</b></td><td>4.000007629394531</td></tr> <tr><td><b>unpackedError</b></td><td>1.52587890625e-05</td></tr> <tr><td><b>maximum</b></td><td>320.5641784667969</td></tr> <tr><td><b>minimum</b></td><td>240.56417846679688</td></tr> <tr><td><b>average</b></td><td>279.70703560965404</td></tr> <tr><td><b>standardDeviation</b></td><td>19.67421739058438</td></tr> <tr><td><b>skewness</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurtosis</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>isConstant</b></td><td>0.0</td></tr> <tr><td><b>numberOfMissing</b></td><td>0</td></tr> <tr><td><b>dataLength</b></td><td>5</td></tr> <tr><td><b>changeDecimalPrecision</b></td><td>0</td></tr> <tr><td><b>decimalPrecision</b></td><td>0</td></tr> <tr><td><b>bitsPerValueAndRepack</b></td><td>4</td></tr> <tr><td><b>scaleValuesBy</b></td><td>1.0</td></tr> <tr><td><b>offsetValuesBy</b></td><td>0.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr> <tr><td><b>getNumberOfValues</b></td><td>84</td></tr> <tr><td><b>padding_sec4_1</b></td><td>None</td></tr> <tr><td><b>md5Section4</b></td><td>7ea3331d80a962b5dc99276b76451eac</td></tr> <tr><td><b>section5Length</b></td><td>4</td></tr> <tr><td><b>7777</b></td><td>7777</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"5448f13a-677d-4bcb-822a-3a0717fae123\"  />\n",
-                            "<label for=\"5448f13a-677d-4bcb-822a-3a0717fae123\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"1f32e53f-cf32-467f-99a1-34f536fe3df2\"  />\n",
+                            "<label for=\"1f32e53f-cf32-467f-99a1-34f536fe3df2\" title=\"Keys in the ecCodes ls namespace\">ls</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>edition</b></td><td>1</td></tr> <tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>typeOfLevel</b></td><td>isobaricInhPa</td></tr> <tr><td><b>level</b></td><td>1000</td></tr> <tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>dataType</b></td><td>an</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr> <tr><td><b>packingType</b></td><td>grid_simple</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"c7b6e148-ca75-481c-bce7-b80186619cb3\"  />\n",
-                            "<label for=\"c7b6e148-ca75-481c-bce7-b80186619cb3\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"d41e79c9-324b-40e8-8afa-e91b3790f5e6\"  />\n",
+                            "<label for=\"d41e79c9-324b-40e8-8afa-e91b3790f5e6\" title=\"Keys in the ecCodes geography namespace\">geography</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>bitmapPresent</b></td><td>0</td></tr> <tr><td><b>latitudeOfFirstGridPointInDegrees</b></td><td>90.0</td></tr> <tr><td><b>longitudeOfFirstGridPointInDegrees</b></td><td>0.0</td></tr> <tr><td><b>latitudeOfLastGridPointInDegrees</b></td><td>-90.0</td></tr> <tr><td><b>longitudeOfLastGridPointInDegrees</b></td><td>330.0</td></tr> <tr><td><b>iScansNegatively</b></td><td>0</td></tr> <tr><td><b>jScansPositively</b></td><td>0</td></tr> <tr><td><b>jPointsAreConsecutive</b></td><td>0</td></tr> <tr><td><b>jDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>iDirectionIncrementInDegrees</b></td><td>30.0</td></tr> <tr><td><b>gridType</b></td><td>regular_ll</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"39b1424d-18b4-4aa0-a469-8d2c66803d7b\"  />\n",
-                            "<label for=\"39b1424d-18b4-4aa0-a469-8d2c66803d7b\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"5a953ecd-f4b9-44ac-a7b2-c7cabd0aeb46\"  />\n",
+                            "<label for=\"5a953ecd-f4b9-44ac-a7b2-c7cabd0aeb46\" title=\"Keys in the ecCodes mars namespace\">mars</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>domain</b></td><td>g</td></tr> <tr><td><b>levtype</b></td><td>pl</td></tr> <tr><td><b>levelist</b></td><td>1000</td></tr> <tr><td><b>date</b></td><td>20180801</td></tr> <tr><td><b>time</b></td><td>1200</td></tr> <tr><td><b>step</b></td><td>0</td></tr> <tr><td><b>param</b></td><td>t</td></tr> <tr><td><b>class</b></td><td>od</td></tr> <tr><td><b>type</b></td><td>an</td></tr> <tr><td><b>stream</b></td><td>oper</td></tr> <tr><td><b>expver</b></td><td>0001</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"963a2eab-99dd-4d50-949a-0bb9b90501ce\" checked />\n",
-                            "<label for=\"963a2eab-99dd-4d50-949a-0bb9b90501ce\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"db581bab-d814-40b0-ac67-d295c1615db9\" checked />\n",
+                            "<label for=\"db581bab-d814-40b0-ac67-d295c1615db9\" title=\"Keys in the ecCodes parameter namespace\">parameter</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>centre</b></td><td>ecmf</td></tr> <tr><td><b>paramId</b></td><td>130</td></tr> <tr><td><b>units</b></td><td>K</td></tr> <tr><td><b>name</b></td><td>Temperature</td></tr> <tr><td><b>shortName</b></td><td>t</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"dec462bb-4c39-4651-b6fe-716869f75c4e\"  />\n",
-                            "<label for=\"dec462bb-4c39-4651-b6fe-716869f75c4e\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"88d9241a-8e94-4df4-b0b6-955f6655e1cb\"  />\n",
+                            "<label for=\"88d9241a-8e94-4df4-b0b6-955f6655e1cb\" title=\"Keys in the ecCodes statistics namespace\">statistics</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>max</b></td><td>320.5641784667969</td></tr> <tr><td><b>min</b></td><td>240.56417846679688</td></tr> <tr><td><b>avg</b></td><td>279.70703560965404</td></tr> <tr><td><b>sd</b></td><td>19.67421739058438</td></tr> <tr><td><b>skew</b></td><td>-0.7312302105044429</td></tr> <tr><td><b>kurt</b></td><td>-0.16904561574741717</td></tr> <tr><td><b>const</b></td><td>0.0</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"5f0c466f-6e8e-4d95-bcab-392eaec32b2e\"  />\n",
-                            "<label for=\"5f0c466f-6e8e-4d95-bcab-392eaec32b2e\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"58056fef-26ca-44cf-a0d2-4a497af48c15\"  />\n",
+                            "<label for=\"58056fef-26ca-44cf-a0d2-4a497af48c15\" title=\"Keys in the ecCodes time namespace\">time</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
                             "<tr><td><b>dataDate</b></td><td>20180801</td></tr> <tr><td><b>dataTime</b></td><td>1200</td></tr> <tr><td><b>stepUnits</b></td><td>1</td></tr> <tr><td><b>stepType</b></td><td>instant</td></tr> <tr><td><b>stepRange</b></td><td>0</td></tr> <tr><td><b>startStep</b></td><td>0</td></tr> <tr><td><b>endStep</b></td><td>0</td></tr> <tr><td><b>validityDate</b></td><td>20180801</td></tr> <tr><td><b>validityTime</b></td><td>1200</td></tr>\n",
                             "</table>\n",
                             "</div>\n",
                             "     \n",
-                            "<input type=\"radio\" name=\"eh-tabs\" id=\"c5e93ddf-c2cd-4c3b-a192-c1dd233def31\"  />\n",
-                            "<label for=\"c5e93ddf-c2cd-4c3b-a192-c1dd233def31\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
+                            "<input type=\"radio\" name=\"eh-tabs\" id=\"3da2eefa-f60c-4b5a-a82c-067e2e1b367e\"  />\n",
+                            "<label for=\"3da2eefa-f60c-4b5a-a82c-067e2e1b367e\" title=\"Keys in the ecCodes vertical namespace\">vertical</label>\n",
                             "<div class=\"tab\">\n",
                             "<style type=\"text/css\">table.eh td {\n",
                             "    vertical-align: top;\n",
                             "    text-align: left !important;\n",
                             "}\n",
                             "</style>\n",
                             "<table class=\"eh-table\">\n",
@@ -1857,39 +1979,39 @@
                             "</div>\n",
                             "        "
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
-                    "execution_count": 20,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "fs[0].dump()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "mpy38",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "mpy38"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.16"
+            "version": "3.11.3"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_missing.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_missing.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979166666666667%*

 * *Differences: {"'cells'": "{1: {'source': ['## GRIB missing values']}}"}*

```diff
@@ -9,15 +9,15 @@
                 "!test -f missing.grib || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/missing.grib"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## GRIB missing values handling"
+                "## GRIB missing values"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We read a GRIB file containing 2 messages with missing values:"
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_multi.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_multi.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/grib_selection.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_selection.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9902246121657066%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(2, \'ds = earthkit.data.from_source("file", '*

 * *            '"tuv_pl.grib")\')], delete: [2]}}, 4: {\'source\': [\'len(ds)\']}, 7: {\'source\': '*

 * *            "{insert: [(0, 'a = ds.sel(level=500)\\n')], delete: [0]}}, 10: {'source': {insert: "*

 * *            '[(0, \'a = ds.sel({"level": 500, "shortName": "v"})\\n\')], delete: [0]}}, 12: '*

 * *            "{'source': {insert: [(0, 'a = ds.sel(level=[500, 850])\\n')], delete: [0]}}, 14: "*

 * *            '{\'source\': {insert: [(0, […]*

```diff
@@ -29,15 +29,15 @@
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
                 "\n",
-                "fs = earthkit.data.from_source(\"file\", \"tuv_pl.grib\")"
+                "ds = earthkit.data.from_source(\"file\", \"tuv_pl.grib\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -49,15 +49,15 @@
                     },
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "len(fs)"
+                "len(ds)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Using sel"
@@ -166,15 +166,15 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel(level=500)\n",
+                "a = ds.sel(level=500)\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
@@ -267,15 +267,15 @@
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel({\"level\": 500, \"shortName\": \"v\"})\n",
+                "a = ds.sel({\"level\": 500, \"shortName\": \"v\"})\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -423,15 +423,15 @@
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel(level=[500, 850])\n",
+                "a = ds.sel(level=[500, 850])\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -534,15 +534,15 @@
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel(param=\"t\", level=slice(500, 850))\n",
+                "a = ds.sel(param=\"t\", level=slice(500, 850))\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -596,71 +596,71 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
+                            "      <td>300</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
+                            "      <td>300</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>v</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>1000</td>\n",
+                            "      <td>300</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "1   ecmf         u  isobaricInhPa   1000  20180801      1200         0   \n",
-                            "2   ecmf         v  isobaricInhPa   1000  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    300  20180801      1200         0   \n",
+                            "1   ecmf         u  isobaricInhPa    300  20180801      1200         0   \n",
+                            "2   ecmf         v  isobaricInhPa    300  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
                     "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.isel(level=0)\n",
+                "a = ds.isel(level=0)\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
@@ -700,41 +700,41 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>700</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         u  isobaricInhPa    700  20180801      1200         0   \n",
+                            "0   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  "
                         ]
                     },
                     "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.isel({\"level\": 2, \"shortName\": 1})\n",
+                "a = ds.isel({\"level\": 2, \"shortName\": 1})\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
@@ -815,15 +815,15 @@
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.isel(level=[2,3], param=0)\n",
+                "a = ds.isel(level=[2,3], param=0)\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -870,71 +870,71 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>700</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>700</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>400</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         t  isobaricInhPa    400  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
                     "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.isel(level=slice(2,5), param=0)\n",
+                "a = ds.isel(level=slice(2,5), param=0)\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -1009,57 +1009,57 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>700</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>700</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>400</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         t  isobaricInhPa    400  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
@@ -1119,57 +1119,57 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>400</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>700</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>700</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    400  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
@@ -1230,57 +1230,57 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>400</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>700</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>700</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    400  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "2   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    700  20180801      1200         0   \n",
+                            "2   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  "
                         ]
                     },
@@ -1341,99 +1341,99 @@
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>t</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>u</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>v</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>500</td>\n",
+                            "      <td>850</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>5</th>\n",
                             "      <td>ecmf</td>\n",
                             "      <td>v</td>\n",
                             "      <td>isobaricInhPa</td>\n",
-                            "      <td>850</td>\n",
+                            "      <td>500</td>\n",
                             "      <td>20180801</td>\n",
                             "      <td>1200</td>\n",
                             "      <td>0</td>\n",
                             "      <td>an</td>\n",
                             "      <td>0</td>\n",
                             "      <td>regular_ll</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "  centre shortName    typeOfLevel  level  dataDate  dataTime stepRange  \\\n",
-                            "0   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
-                            "1   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
-                            "2   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
-                            "3   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
-                            "4   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
-                            "5   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "0   ecmf         t  isobaricInhPa    850  20180801      1200         0   \n",
+                            "1   ecmf         t  isobaricInhPa    500  20180801      1200         0   \n",
+                            "2   ecmf         u  isobaricInhPa    850  20180801      1200         0   \n",
+                            "3   ecmf         u  isobaricInhPa    500  20180801      1200         0   \n",
+                            "4   ecmf         v  isobaricInhPa    850  20180801      1200         0   \n",
+                            "5   ecmf         v  isobaricInhPa    500  20180801      1200         0   \n",
                             "\n",
                             "  dataType  number    gridType  \n",
                             "0       an       0  regular_ll  \n",
                             "1       an       0  regular_ll  \n",
                             "2       an       0  regular_ll  \n",
                             "3       an       0  regular_ll  \n",
                             "4       an       0  regular_ll  \n",
@@ -1442,162 +1442,194 @@
                     },
                     "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "a = fs.sel(level=[500, 850]).order_by([\"shortName\"])\n",
+                "a = ds.sel(level=[500, 850]).order_by([\"shortName\"])\n",
                 "a.ls()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Using coords"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Coordinates are generated using almost all the MARS ecCodes keys."
+                "### Using indices"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The coords containing more than one values can be accessed as a property:"
+                "To get the unique values for predefined set of metadata keys (the MARS ecCodes keys) we can call *indices()*. By default it returns all the keys having valid values:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 18,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'levelist': (1000, 850, 700, 500, 400, 300), 'param': ('t', 'u', 'v')}"
+                            "{'class': ['od'],\n",
+                            " 'stream': ['oper'],\n",
+                            " 'levtype': ['pl'],\n",
+                            " 'type': ['an'],\n",
+                            " 'expver': ['0001'],\n",
+                            " 'date': [20180801],\n",
+                            " 'time': [1200],\n",
+                            " 'domain': ['g'],\n",
+                            " 'number': [0],\n",
+                            " 'levelist': [300, 400, 500, 700, 850, 1000],\n",
+                            " 'param': ['t', 'u', 'v'],\n",
+                            " 'shortName': ['t', 'u', 'v']}"
                         ]
                     },
                     "execution_count": 18,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "c = fs.coords\n",
-                "c"
+                "ds.indices()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The value of a given coord:"
+                "We can use the *squeeze* option to see only the keys having more than one values:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 19,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "('t', 'u', 'v')"
+                            "{'levelist': [300, 400, 500, 700, 850, 1000],\n",
+                            " 'param': ['t', 'u', 'v'],\n",
+                            " 'shortName': ['t', 'u', 'v']}"
                         ]
                     },
                     "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.coord(\"param\")"
+                "ds.indices(squeeze=True)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We can get the unique values for a given key:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 20,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(20180801,)"
+                            "['t', 'u', 'v']"
                         ]
                     },
                     "execution_count": 20,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.coord(\"date\")"
+                "ds.index(\"param\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 21,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[20180801]"
+                        ]
+                    },
+                    "execution_count": 21,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "ds.index(\"date\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Aliases can be used. E.g. instead of levelist we can use level:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "(1000, 850, 700, 500, 400, 300)"
+                            "[300, 400, 500, 700, 850, 1000]"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "fs.coord(\"level\")"
+                "ds.index(\"level\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Count the number of fields for each available level:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "level=1000 len=3\n",
-                        "level=850 len=3\n",
-                        "level=700 len=3\n",
-                        "level=500 len=3\n",
+                        "level=300 len=3\n",
                         "level=400 len=3\n",
-                        "level=300 len=3\n"
+                        "level=500 len=3\n",
+                        "level=700 len=3\n",
+                        "level=850 len=3\n",
+                        "level=1000 len=3\n"
                     ]
                 }
             ],
             "source": [
-                "for level in fs.coord(\"level\"):\n",
-                "    print(f\"level={level} len={len(fs.sel(level=level))}\")"
+                "for level in ds.index(\"level\"):\n",
+                "    print(f\"level={level} len={len(ds.sel(level=level))}\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_tar.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_tar.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946759259259259%*

 * *Differences: {"'cells'": "{1: {'source': ['## Reading GRIB in tar or zip archive']}, 4: {'source': ['The files "*

 * *            "are extracted and stored in the earthkit-data cache:']}, 8: {'outputs': {insert: [(0, "*

 * *            "OrderedDict([('name', 'stdout'), ('output_type', 'stream'), ('text', "*

 * *            '["args=() kwargs={\'levelist\': 500}\\n", "args=() kwargs={\'levelist\': '*

 * *            '500}\\n"])]))]}}}'}*

```diff
@@ -9,15 +9,15 @@
                 "!test -f test_gribs.tar || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test_gribs.tar"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Handling GRIB in tar or zip archive"
+                "## Reading GRIB in tar or zip archive"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We read a tar file containing 2 GRIB files:"
@@ -34,15 +34,15 @@
                 "fs = earthkit.data.from_source(\"file\", \"test_gribs.tar\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The files are extracted and stored in the emohawk cache:"
+                "The files are extracted and stored in the earthkit-data cache:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -217,14 +217,22 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "args=() kwargs={'levelist': 500}\n",
+                        "args=() kwargs={'levelist': 500}\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
                             "    .dataframe tbody tr th:only-of-type {\n",
                             "        vertical-align: middle;\n",
                             "    }\n",
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_to_netcdf.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_to_netcdf.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428572%*

 * *Differences: {"'cells'": "{1: {'source': ['## Converting GRIB to NetCDF']}}"}*

```diff
@@ -11,15 +11,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9c53d7c8-7f38-4a5f-93d0-e05919408b6e",
             "metadata": {},
             "source": [
-                "## Convert GRIB to NetCDF"
+                "## Converting GRIB to NetCDF"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "950b9aa8-6b76-47f8-b470-17476f99a733",
             "metadata": {},
```

### Comparing `earthkit-data-0.1.0/docs/examples/grib_url.ipynb` & `earthkit-data-0.1.1/docs/examples/grib_url.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/list_of_dict.ipynb` & `earthkit-data-0.1.1/docs/examples/list_of_dict.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987445849867724%*

 * *Differences: {"'cells'": '{8: {\'outputs\': {0: {\'data\': {\'text/html\': {insert: [(376, "    history:      '*

 * *            '2023-04-26T16:33 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes...</pre><div '*

 * *            "class='xr-wrap' style='display:none'><div class='xr-header'><div "*

 * *            "class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li "*

 * *            "class='xr-section-item'><input id='section-c58bcd02-2ec9-4806-98b2-7b2c04e5df94' "*

 * *            "class='xr-section-summary-in' type='checkbox' d […]*

```diff
@@ -728,15 +728,15 @@
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    t              (isobaricInhPa, values) float32 ...\n",
                             "    u              (isobaricInhPa, values) float32 ...\n",
                             "    d              (isobaricInhPa, values) float32 ...\n",
                             "Attributes:\n",
                             "    Conventions:  CF-1.7\n",
-                            "    history:      2023-04-05T15:18 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-5734b280-baa4-44ff-8825-d3697d961a08' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-5734b280-baa4-44ff-8825-d3697d961a08' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>isobaricInhPa</span>: 1</li><li><span>values</span>: 6</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-a48b7097-c141-48e5-b7c1-53d419978bce' class='xr-section-summary-in' type='checkbox'  checked><label for='section-a48b7097-c141-48e5-b7c1-53d419978bce' class='xr-section-summary' >Coordinates: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>500.0</div><input id='attrs-334d8ef0-073d-48f2-a659-332bba82f5ea' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-334d8ef0-073d-48f2-a659-332bba82f5ea' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e7022ba4-1903-424f-a909-5e9731e3c568' class='xr-var-data-in' type='checkbox'><label for='data-e7022ba4-1903-424f-a909-5e9731e3c568' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([500.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-91ddc010-d1c0-4dcd-9c07-845d1dcb8a8c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-91ddc010-d1c0-4dcd-9c07-845d1dcb8a8c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-e7ac50e4-dea4-4df8-8ff2-0b2ae4f6fee3' class='xr-var-data-in' type='checkbox'><label for='data-e7ac50e4-dea4-4df8-8ff2-0b2ae4f6fee3' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-5c3eb906-d2dd-42db-894d-72b72d2f048c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-5c3eb906-d2dd-42db-894d-72b72d2f048c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f4edc798-457f-4883-9a70-c88315d1e179' class='xr-var-data-in' type='checkbox'><label for='data-f4edc798-457f-4883-9a70-c88315d1e179' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float64]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-d7d896f6-795a-40c2-8b1c-41656a50d780' class='xr-section-summary-in' type='checkbox'  checked><label for='section-d7d896f6-795a-40c2-8b1c-41656a50d780' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-852033a4-974d-47a9-acb2-09b744ad753e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-852033a4-974d-47a9-acb2-09b744ad753e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-72ea0287-8d3c-41ee-b1c2-d82246070811' class='xr-var-data-in' type='checkbox'><label for='data-72ea0287-8d3c-41ee-b1c2-d82246070811' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 130</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-13f12ee8-ef92-4dc1-9afe-ddbcb94d507c' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-13f12ee8-ef92-4dc1-9afe-ddbcb94d507c' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-f8883df8-b9c9-4771-8123-8f5a294dafee' class='xr-var-data-in' type='checkbox'><label for='data-f8883df8-b9c9-4771-8123-8f5a294dafee' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 131</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>d</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-f51516ec-7c60-41c0-ab97-8d9298a2ce63' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-f51516ec-7c60-41c0-ab97-8d9298a2ce63' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-33a9655a-6da6-459f-a33a-378a0712429b' class='xr-var-data-in' type='checkbox'><label for='data-33a9655a-6da6-459f-a33a-378a0712429b' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>157</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>d</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 157</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-08c883bf-11e5-4d9c-8b1b-b741dc98956a' class='xr-section-summary-in' type='checkbox'  ><label for='section-08c883bf-11e5-4d9c-8b1b-b741dc98956a' class='xr-section-summary' >Indexes: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-95dfab88-dca0-4420-aa90-d19c492d373b' class='xr-index-data-in' type='checkbox'/><label for='index-95dfab88-dca0-4420-aa90-d19c492d373b' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([500.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-121f70b5-1a17-4570-b587-df95846cb88e' class='xr-section-summary-in' type='checkbox'  checked><label for='section-121f70b5-1a17-4570-b587-df95846cb88e' class='xr-section-summary' >Attributes: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>history :</span></dt><dd>2023-04-05T15:18 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
+                            "    history:      2023-04-26T16:33 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes...</pre><div class='xr-wrap' style='display:none'><div class='xr-header'><div class='xr-obj-type'>xarray.Dataset</div></div><ul class='xr-sections'><li class='xr-section-item'><input id='section-c58bcd02-2ec9-4806-98b2-7b2c04e5df94' class='xr-section-summary-in' type='checkbox' disabled ><label for='section-c58bcd02-2ec9-4806-98b2-7b2c04e5df94' class='xr-section-summary'  title='Expand/collapse section'>Dimensions:</label><div class='xr-section-inline-details'><ul class='xr-dim-list'><li><span class='xr-has-index'>isobaricInhPa</span>: 1</li><li><span>values</span>: 6</li></ul></div><div class='xr-section-details'></div></li><li class='xr-section-item'><input id='section-21cd8d91-e100-4176-bdcf-cf6e753c6f19' class='xr-section-summary-in' type='checkbox'  checked><label for='section-21cd8d91-e100-4176-bdcf-cf6e753c6f19' class='xr-section-summary' >Coordinates: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span class='xr-has-index'>isobaricInhPa</span></div><div class='xr-var-dims'>(isobaricInhPa)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>500.0</div><input id='attrs-a3249600-674f-4ee8-b352-8325bd0b444e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-a3249600-674f-4ee8-b352-8325bd0b444e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-19784380-b50e-4a40-83c3-42fd41e549e8' class='xr-var-data-in' type='checkbox'><label for='data-19784380-b50e-4a40-83c3-42fd41e549e8' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>long_name :</span></dt><dd>pressure</dd><dt><span>units :</span></dt><dd>hPa</dd><dt><span>positive :</span></dt><dd>down</dd><dt><span>stored_direction :</span></dt><dd>decreasing</dd><dt><span>standard_name :</span></dt><dd>air_pressure</dd></dl></div><div class='xr-var-data'><pre>array([500.])</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>latitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-14c940ac-0fd9-465c-ab34-c5eb987cd89f' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-14c940ac-0fd9-465c-ab34-c5eb987cd89f' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-82630d28-3ad5-4903-96af-50f6650915c9' class='xr-var-data-in' type='checkbox'><label for='data-82630d28-3ad5-4903-96af-50f6650915c9' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_north</dd><dt><span>standard_name :</span></dt><dd>latitude</dd><dt><span>long_name :</span></dt><dd>latitude</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float64]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>longitude</span></div><div class='xr-var-dims'>(values)</div><div class='xr-var-dtype'>float64</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-995317ee-af66-4f56-bc79-2ab24f8899fd' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-995317ee-af66-4f56-bc79-2ab24f8899fd' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-7cfbb7ae-22dd-4bf3-864a-e4548b672a2a' class='xr-var-data-in' type='checkbox'><label for='data-7cfbb7ae-22dd-4bf3-864a-e4548b672a2a' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>units :</span></dt><dd>degrees_east</dd><dt><span>standard_name :</span></dt><dd>longitude</dd><dt><span>long_name :</span></dt><dd>longitude</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float64]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-c6084a1e-61b6-486d-8607-96dd446a958b' class='xr-section-summary-in' type='checkbox'  checked><label for='section-c6084a1e-61b6-486d-8607-96dd446a958b' class='xr-section-summary' >Data variables: <span>(3)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-var-name'><span>t</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-d07fb32c-efdf-478a-9f61-15f68186bd61' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-d07fb32c-efdf-478a-9f61-15f68186bd61' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-4e2b8f1c-d03e-4355-8e0c-749819d9a628' class='xr-var-data-in' type='checkbox'><label for='data-4e2b8f1c-d03e-4355-8e0c-749819d9a628' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>130</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>t</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 130</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>u</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-efb72254-8c65-42d4-903b-5e5faee63433' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-efb72254-8c65-42d4-903b-5e5faee63433' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-591cd91f-7b83-4e4f-8f8a-e8b4086c9b23' class='xr-var-data-in' type='checkbox'><label for='data-591cd91f-7b83-4e4f-8f8a-e8b4086c9b23' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>131</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>u</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 131</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li><li class='xr-var-item'><div class='xr-var-name'><span>d</span></div><div class='xr-var-dims'>(isobaricInhPa, values)</div><div class='xr-var-dtype'>float32</div><div class='xr-var-preview xr-preview'>...</div><input id='attrs-b80eb5b3-9427-4b36-bee0-8e6f0fad3f2e' class='xr-var-attrs-in' type='checkbox' ><label for='attrs-b80eb5b3-9427-4b36-bee0-8e6f0fad3f2e' title='Show/Hide attributes'><svg class='icon xr-icon-file-text2'><use xlink:href='#icon-file-text2'></use></svg></label><input id='data-d603a24e-9e58-4480-875c-ab0b37b86f19' class='xr-var-data-in' type='checkbox'><label for='data-d603a24e-9e58-4480-875c-ab0b37b86f19' title='Show/Hide data repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-var-attrs'><dl class='xr-attrs'><dt><span>GRIB_paramId :</span></dt><dd>157</dd><dt><span>GRIB_numberOfPoints :</span></dt><dd>6</dd><dt><span>GRIB_typeOfLevel :</span></dt><dd>isobaricInhPa</dd><dt><span>GRIB_gridType :</span></dt><dd>reduced_gg</dd><dt><span>GRIB_shortName :</span></dt><dd>d</dd><dt><span>long_name :</span></dt><dd>original GRIB paramId: 157</dd><dt><span>units :</span></dt><dd>1</dd></dl></div><div class='xr-var-data'><pre>[6 values with dtype=float32]</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-2978e6b3-4ba6-4c23-9081-94f427002c1c' class='xr-section-summary-in' type='checkbox'  ><label for='section-2978e6b3-4ba6-4c23-9081-94f427002c1c' class='xr-section-summary' >Indexes: <span>(1)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><ul class='xr-var-list'><li class='xr-var-item'><div class='xr-index-name'><div>isobaricInhPa</div></div><div class='xr-index-preview'>PandasIndex</div><div></div><input id='index-a4c9307a-5151-45c0-a02f-0dba43bcfe73' class='xr-index-data-in' type='checkbox'/><label for='index-a4c9307a-5151-45c0-a02f-0dba43bcfe73' title='Show/Hide index repr'><svg class='icon xr-icon-database'><use xlink:href='#icon-database'></use></svg></label><div class='xr-index-data'><pre>PandasIndex(Float64Index([500.0], dtype=&#x27;float64&#x27;, name=&#x27;isobaricInhPa&#x27;))</pre></div></li></ul></div></li><li class='xr-section-item'><input id='section-b91defda-bf9b-4712-9269-58273c03aa61' class='xr-section-summary-in' type='checkbox'  checked><label for='section-b91defda-bf9b-4712-9269-58273c03aa61' class='xr-section-summary' >Attributes: <span>(2)</span></label><div class='xr-section-inline-details'></div><div class='xr-section-details'><dl class='xr-attrs'><dt><span>Conventions :</span></dt><dd>CF-1.7</dd><dt><span>history :</span></dt><dd>2023-04-26T16:33 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes-2.27.1 with {&quot;source&quot;: &quot;N/A&quot;, &quot;filter_by_keys&quot;: {}, &quot;encode_cf&quot;: [&quot;parameter&quot;, &quot;time&quot;, &quot;geography&quot;, &quot;vertical&quot;]}</dd></dl></div></li></ul></div></div>"
                         ],
                         "text/plain": [
                             "<xarray.Dataset>\n",
                             "Dimensions:        (isobaricInhPa: 1, values: 6)\n",
                             "Coordinates:\n",
                             "  * isobaricInhPa  (isobaricInhPa) float64 500.0\n",
                             "    latitude       (values) float64 ...\n",
@@ -744,24 +744,25 @@
                             "Dimensions without coordinates: values\n",
                             "Data variables:\n",
                             "    t              (isobaricInhPa, values) float32 ...\n",
                             "    u              (isobaricInhPa, values) float32 ...\n",
                             "    d              (isobaricInhPa, values) float32 ...\n",
                             "Attributes:\n",
                             "    Conventions:  CF-1.7\n",
-                            "    history:      2023-04-05T15:18 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes..."
+                            "    history:      2023-04-26T16:33 GRIB to CDM+CF via cfgrib-0.9.10.3/ecCodes..."
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "g.to_xarray()"
+                "r = g.to_xarray()\n",
+                "r"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `earthkit-data-0.1.0/docs/examples/missing.grib` & `earthkit-data-0.1.1/docs/examples/missing.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/netcdf.ipynb` & `earthkit-data-0.1.1/docs/examples/netcdf.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{insert: [(1, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['## Using NetCDF data'])]))]}"}*

```diff
@@ -6,14 +6,21 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "!test -f test.nc || wget https://get.ecmwf.int/repository/test-data/emohawk/examples/test.nc"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Using NetCDF data"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import earthkit.data\n",
                 "\n",
```

### Comparing `earthkit-data-0.1.0/docs/examples/temp_10.bufr` & `earthkit-data-0.1.1/docs/examples/temp_10.bufr`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/test.grib` & `earthkit-data-0.1.1/docs/examples/test.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/test.nc` & `earthkit-data-0.1.1/docs/examples/test.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/test4.grib` & `earthkit-data-0.1.1/docs/examples/test4.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/test6.grib` & `earthkit-data-0.1.1/docs/examples/test6.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/examples/tuv_pl.grib` & `earthkit-data-0.1.1/docs/examples/tuv_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/docs/make.bat` & `earthkit-data-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/__init__.py` & `earthkit-data-0.1.1/earthkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/__init__.py` & `earthkit-data-0.1.1/earthkit/data/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/args_kwargs.py` & `earthkit-data-0.1.1/earthkit/data/arguments/args_kwargs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self.kwargs = kwargs
         self.func = func
 
         self.positionals_only = []
         self.defaults = {}
 
     def add_default_values_and_kwargs(self):
-
         new_args = []
         new_kwargs = {}
 
         sig = inspect.signature(self.func)
         bnd = sig.bind(*self.args, **self.kwargs)
         parameters_names = list(sig.parameters)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/argument.py` & `earthkit-data-0.1.1/earthkit/data/arguments/argument.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/earthkit_types.py` & `earthkit-data-0.1.1/earthkit/data/arguments/earthkit_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,15 +364,14 @@
             return EnumSingleOrListType(values)
         if multiple is True:
             return EnumListType(values)
         if multiple is False:
             return EnumType(values)
 
     if values is None and isinstance(type, str):
-
         if multiple is None:
             try:
                 if type in SINGLE_OR_LIST_TYPES:
                     return SINGLE_OR_LIST_TYPES[type](**kwargs)
                 return {**LIST_TYPES, **NON_LIST_TYPES}[type](**kwargs)
             except Exception as e:
                 raise ValueError(f"Error building {type}({kwargs}): {e}")
```

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/input_manager.py` & `earthkit-data-0.1.1/earthkit/data/arguments/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/arguments/transformers.py` & `earthkit-data-0.1.1/earthkit/data/arguments/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,15 @@
 import logging
 
 from earthkit.data.arguments.earthkit_types import Type
 from earthkit.data.vocabularies.aliases import unalias
 
 LOG = logging.getLogger(__name__)
 
-
-class _all:
-    def __repr__(self):
-        return "earthkit.ALL"
-
-
-ALL = _all()
+ALL = all
 
 
 class Action:
     def execute(self, kwargs):
         raise NotImplementedError()
 
     def execute_before_default(self, kwargs):
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/__init__.py` & `earthkit-data-0.1.1/earthkit/data/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
         for k, v in private_attributes.items():
             setattr(obj, k, kwargs.pop(k, v))
 
         return args, kwargs
 
 
 class Base(metaclass=MetaBase):
-
     # Convertors
     def to_numpy(self, **kwargs):
         self._not_implemented()
 
     @abstractmethod
     def to_xarray(self, **kwargs):
         self._not_implemented()
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/caching.py` & `earthkit-data-0.1.1/earthkit/data/core/caching.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
 CONNECTION = None
 CACHE = None
 
 
 class DiskUsage:
     def __init__(self, path):
-
         path = os.path.realpath(path)
         self.path = path
 
         if platform.system() == "Windows":
             avail = ctypes.c_ulonglong()
             total = ctypes.c_ulonglong()
             free = ctypes.c_ulonglong()
@@ -236,15 +235,14 @@
                     "SELECT MAX(creation_date) FROM cache WHERE size IS NOT NULL"
                 ).fetchone()[0]
             if latest is None:
                 latest = datetime.datetime.now()
             return latest
 
     def _purge_cache(self, matcher=None):
-
         if matcher is None:
             self._housekeeping(clean=True)
             # _update_cache(clean=True)
             self._decache(self._cache_size(), purge=True)
             return
 
         dump = self._dump_cache_database(matcher)
@@ -362,15 +360,14 @@
                     "orphans",
                     None,
                     parent,
                 )
         self._update_cache(clean=clean)
 
     def _delete_file(self, path):
-
         self._ensure_in_cache(path)
 
         try:
             if os.path.isdir(path) and not os.path.islink(path):
                 shutil.rmtree(path)
             else:
                 os.unlink(path)
@@ -448,15 +445,14 @@
             return 0
 
         LOG.warning("CliMetLab cache: trying to free %s", humanize.bytes(bytes))
 
         total = 0
 
         with self.connection as db:
-
             latest = datetime.datetime.now() if purge else self._latest_date()
 
             for stmt in (
                 "SELECT * FROM cache WHERE size IS NOT NULL AND owner='orphans' AND creation_date < ?",
                 "SELECT * FROM cache WHERE size IS NOT NULL AND creation_date < ? ORDER BY last_access ASC",
             ):
                 for entry in db.execute(stmt, (latest,)):
@@ -486,15 +482,14 @@
         -------
         changes :
             None or False if database does not need to be updated. TODO: clarify.
         """
         self._ensure_in_cache(path)
 
         with self.connection as db:
-
             now = datetime.datetime.now()
 
             args = json.dumps(args, default=default_serialiser)
 
             db.execute(
                 """
                 UPDATE cache
@@ -503,15 +498,14 @@
                 WHERE path=?""",
                 (now, path),
             )
 
             changes = db.execute("SELECT changes()").fetchone()[0]
 
             if not changes:
-
                 db.execute(
                     """
                     INSERT INTO cache(
                                     path,
                                     owner,
                                     args,
                                     creation_date,
@@ -533,15 +527,14 @@
                 size = 0
             return size
 
     def _decache_file(self, path):
         self._delete_entry(path)
 
     def _check_cache_size(self):
-
         # Check absolute limit
         size = self._cache_size()
         maximum = SETTINGS.get("maximum-cache-size")
         if maximum is not None and size > maximum:
             self._housekeeping()
             self._decache(size - maximum)
 
@@ -678,22 +671,20 @@
                 owner_data = json.loads(owner_data)
             force = force(args, path, owner_data)
 
         if force:
             decache_file(path)
 
     if not os.path.exists(path):
-
         lock = path + ".lock"
 
         with FileLock(lock):
             if not os.path.exists(
                 path
             ):  # Check again, another thread/process may have created the file
-
                 owner_data = create(path + ".tmp", args)
 
                 os.rename(path + ".tmp", path)
 
                 update_entry(path, owner_data)
 
                 check_cache_size()
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/index.py` & `earthkit-data-0.1.1/earthkit/data/core/index.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,439 +3,358 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-
-import hashlib
-import json
+import functools
 import logging
+import math
 from abc import abstractmethod
+from collections import defaultdict
+
+import numpy as np
 
-from earthkit.data.decorators import alias_argument
+import earthkit.data
+from earthkit.data.core.order import build_remapping, normalize_order_by
+from earthkit.data.core.select import normalize_selection, selection_from_index
 from earthkit.data.sources import Source
 
 LOG = logging.getLogger(__name__)
 
 
 class OrderOrSelection:
-    def __init__(self, *args, **kwargs):
-        """Parse args and kwargs to build a dictionary in self.order"""
-        self.dic = {}
-
-        for arg in args:
-            if isinstance(arg, dict):
-                arg = self.normalize_naming(**arg)
-            res_ok = self.parse_arg(arg)
-            if res_ok is False:
-                raise ValueError(f"Invalid argument of type({type(arg)}): {arg}")
-
-        kwargs = self.normalize_naming(**kwargs)
-        for k, v in kwargs.items():
-            self.parse_kwarg(k, v)
-
-    @alias_argument("levelist", ["level"])
-    @alias_argument("param", ["variable", "parameter"])
-    @alias_argument("number", ["realization", "realisation"])
-    @alias_argument("class", "klass")
-    def normalize_naming(self, **kwargs):
-        return kwargs
-
-    def parse_arg(self, arg):
-        # Returns True of argument has been parsed.
-        if arg is None:
-            return True
-        if isinstance(arg, dict):
-            for k, v in arg.items():
-                self.parse_kwarg(k, v)
-            return True
-        return False
+    actions = {}
 
     def __str__(self):
-        return f"{self.__class__.__name__}({self.dic})"
+        return f"{self.__class__.__name__}({self.actions})"
 
     @property
-    def is_empty(self):  # TODO: use __bool__ instead
-        if not self.dic:
-            return True
-        return False
-
-    def h(self, *args, **kwargs):
-        m = hashlib.sha256()
-        m.update(json.dumps(args, sort_keys=True).encode("utf-8"))
-        m.update(json.dumps(kwargs, sort_keys=True).encode("utf-8"))
-        m.update(json.dumps(self.dic, sort_keys=True).encode("utf-8"))
-        return m.hexdigest()
-
-    def keys(self):
-        return self.dic.keys()
+    def is_empty(self):
+        return not self.actions
 
 
 class Selection(OrderOrSelection):
-    @property
-    def selection(self):
-        return self.dic
+    def __init__(self, kwargs, remapping=None):
+        self.remapping = build_remapping(remapping)
 
-    def parse_kwarg(self, k, v):
-        if v is not None and not isinstance(v, (list, tuple, slice)):
-            v = [v]
-        if isinstance(v, (list, tuple)):
-            v = [str(_) for _ in v]
-        self.dic[k] = v
+        class InList:
+            def __init__(self, lst):
+                self.first = True
+                self.lst = lst  # lazy casting: lst will be modified
+
+            def __call__(self, x):
+                if self.first and x is not None:
+                    cast = type(x)
+                    self.lst = [cast(y) for y in self.lst]
+                    self.first = False
+                return x in self.lst
+
+        class InSlice:
+            def __init__(self, slc):
+                self.slc = slc
+                if self.slc.start is None and self.slc.stop is None:
+                    raise ValueError("Invalid selection value: slice(None, None)")
+
+                if (
+                    self.slc.start is not None
+                    and self.slc.stop is not None
+                    and self.slc.stop < self.slc.start
+                ):
+                    self.slc = slice(self.slc.stop, self.slc.start)
+
+            def __call__(self, x):
+                return not (
+                    (self.slc.start is not None and x < self.slc.start)
+                    or (self.slc.stop is not None and x > self.slc.stop)
+                )
 
-    def match_element(self, element):
-        for k, v in self.dic.items():
-            if v is None:
-                continue
-            value = element.metadata(k)
-            # value = grib_naming({key:value})[key]
-            if isinstance(v, slice):
-                if v.start is not None and value < v.start:
-                    return False
-                elif v.stop is not None and value > v.stop:
-                    return False
-                else:
-                    continue
-            if isinstance(v, (list, tuple)):
-                if value in v:
-                    continue
-                if str(value) in v:
-                    continue
-                return False
-            if value == v:
-                continue
-            if str(value) == v:
+        self.actions = {}
+        for k, v in kwargs.items():
+            if v is None or v is earthkit.data.ALL:
+                self.actions[k] = lambda x: True
                 continue
-            return False
-        return True
 
+            if callable(v):
+                self.actions[k] = v
+                continue
 
-class SelectionByIndex(Selection):
-    def __init__(self, coord_accessor, *args, **kwargs):
-        """Parse args and kwargs to build a dictionary in self.order"""
-        super().__init__(*args, **kwargs)
-        if not self.is_empty:
-            self._convert_index(coord_accessor)
+            if isinstance(v, slice):
+                self.actions[k] = InSlice(v)
+                continue
 
-    def parse_kwarg(self, k, v):
-        if v is not None and not isinstance(v, (list, tuple, slice)):
-            v = [int(v)]
-        if isinstance(v, (list, tuple)):
-            v = [int(_) for _ in v]
-        self.dic[k] = v
+            if not isinstance(v, (list, tuple, set)):
+                v = [v]
 
-    @property
-    def is_valid(self):
-        return all([len(v) > 0 for v in self.dic.values()])
+            v = set(v)
 
-    def _convert_index(self, coord_accessor):
-        if coord_accessor is None:
-            return
-        for k in list(self.dic.keys()):
-            v = self.dic[k]
-            try:
-                coord_vals = coord_accessor(k)
-                if coord_vals is None or len(coord_vals) == 0:
-                    self.dic = {k: []}
-                    return
-                else:
-                    if isinstance(v, slice):
-                        self.dic[k] = coord_vals[v]
-                    else:
-                        self.dic[k] = [coord_vals[i] for i in v]
-                    if None in self.dic[k]:
-                        self.dic = {k: []}
-                        return
-
-            except Exception as e:
-                raise IndexError(
-                    f"Invalid index={v}. Specified key={k} has {len(coord_accessor(k))} values. {e}"
-                )
+            self.actions[k] = InList(v)
 
+    def match_element(self, element):
+        metadata = self.remapping(element.metadata)
+        return all(v(metadata(k, default=None)) for k, v in self.actions.items())
 
-class Order(OrderOrSelection):
-    def __init__(self, *args, **kwargs):
-        self._rankers = None
-        if args and all([isinstance(a, str) for a in args]):
-            args = [args]
-        super().__init__(*args, **kwargs)
 
-    @property
-    def order(self):
-        return self.dic
+class OrderBase(OrderOrSelection):
+    def __init__(self, kwargs, remapping):
+        self.actions = self.build_actions(kwargs)
+        self.remapping = remapping
 
-    def update(self, other):
-        assert isinstance(other, Order), other
-        self.dic.update(other.dic)
-
-    def items(self):
-        if self.is_empty:
-            return
-
-        from earthkit.data.indexing.database.sql import GRIB_INDEX_KEYS
-
-        for k, v in self.dic.items():
-            yield k, v
-
-        for k in GRIB_INDEX_KEYS:
-            if k in self.dic:
-                continue  # already yielded above
-            yield k, self[k]
-
-    def __getitem__(self, key):
-        # Default is ascending order
-        return self.dic.get(key, "ascending")
-
-    def parse_arg(self, arg):
-        if super().parse_arg(arg):
-            return True
-        if isinstance(arg, str):
-            self.dic[arg] = "ascending"
-            return True
-        if isinstance(arg, (list, tuple)):
-            dic = {}
-            for k in arg:
-                assert isinstance(k, str), k
-                assert len(k) > 0, k
-                if k[0] == "-":
-                    dic[k[1:]] = "descending"
-                    continue
-                if k[0] == "+":
-                    dic[k[1:]] = "ascending"
-                    continue
-                dic[k] = "ascending"
-            dic = self.normalize_naming(**dic)
-            return self.parse_arg(dic)
-        return False
-
-    def parse_kwarg(self, k, v):
-        if isinstance(v, (list, tuple)):
-            v = [str(_) for _ in v]  # processing only strings from now.
-        if (v == "ascending") or (v == "descending") or isinstance(v, (list, tuple)):
-            self.dic[k] = v
-            return
-
-        if v is None:
-            self.dic[k] = "ascending"
-            return
-
-        self.dic[k] = "ascending"
-        return
-        # raise ValueError(f"Invalid argument for {k}: {v} ({type(v)})")
-
-    def build_rankers(self):
-        if self._rankers is not None:
-            return self._rankers
-
-        from earthkit.data.indexing.database.sql import GRIB_INDEX_KEYS
-
-        keys = [_ for _ in self.dic.keys()]
-        keys += [_ for _ in GRIB_INDEX_KEYS if _ not in keys]
-
-        key_types = {}
-        dict_of_dicts = dict()
-
-        for key in keys:
-            lst = self.dic.get(key, None)
-
-            if isinstance(lst, (tuple, list)):
-                dict_of_dicts[key] = dict(zip(lst, range(len(lst))))
-                key_types[key] = "explicit"
-                continue
+    @abstractmethod
+    def build_actions(self, kwargs):
+        raise NotImplementedError()
 
-            if lst == "ascending" or lst is None:
-                dict_of_dicts[key] = lambda value: value
-                key_types[key] = "ascending"
-                continue
+    def compare_elements(self, a, b):
+        a_metadata = self.remapping(a.metadata)
+        b_metadata = self.remapping(b.metadata)
+        for k, v in self.actions.items():
+            n = v(a_metadata(k, default=None), b_metadata(k, default=None))
+            if n != 0:
+                return n
+        return 0
+
+
+class Order(OrderBase):
+    def build_actions(self, kwargs):
+        actions = {}
+
+        def ascending(a, b):
+            if a == b:
+                return 0
+            if a > b:
+                return 1
+            if a < b:
+                return -1
+            raise ValueError(f"{a},{b}")
+
+        def descending(a, b):
+            if a == b:
+                return 0
+            if a > b:
+                return -1
+            if a < b:
+                return 1
+            raise ValueError(f"{a},{b}")
+
+        class Compare:
+            def __init__(self, order):
+                self.order = order
 
-            raise ValueError(f"Invalid argument {lst}")
+            def __call__(self, a, b):
+                return ascending(self.get(a), self.get(b))
 
-        self._rankers = keys, key_types, dict_of_dicts
-        return self._rankers
+            def get(self, x):
+                return self.order[x]
 
-    def get_element_ranking(self, element):
-        keys, key_types, dict_of_dicts = self.build_rankers()
-        ranks = []
-        for k in keys:
-            value = element.metadata(k)
+        for k, v in kwargs.items():
+            if v == "ascending" or v is None:
+                actions[k] = ascending
+                continue
 
-            if key_types[k] == "ascending":
-                ranks.append(value)
+            if v == "descending":
+                actions[k] = descending
                 continue
 
-            if key_types[k] == "explicit":
-                value = str(value)
-                ranks.append(dict_of_dicts[k][value])
+            if callable(v):
+                actions[k] = v
                 continue
 
-            assert False, (k, key_types[k], element)
+            assert isinstance(
+                v, (list, tuple)
+            ), f"Invalid argument for {k}: {v} ({type(v)})"
+
+            order = {}
+            for i, key in enumerate(v):
+                order[str(key)] = i
+                try:
+                    order[int(key)] = i
+                except ValueError:
+                    pass
+                try:
+                    order[float(key)] = i
+                except ValueError:
+                    pass
+            actions[k] = Compare(order)
 
-        return tuple(ranks)
+        return actions
 
 
 class Index(Source):
     @classmethod
     def new_mask_index(self, *args, **kwargs):
-        print("new_mask_index")
         return MaskIndex(*args, **kwargs)
 
-    def __init__(self, *args, order_by=None, **kwargs):
-        self._init_args = args
-        self._init_kwargs = kwargs
-        self._init_order_by = order_by
-        self._coords = {}
-
-    def mutate(self):
-        source = self
-        source = source.sel(*self._init_args, **self._init_kwargs)
-        source = source.order_by(*self._init_args, **self._init_kwargs)
-        source = source.order_by(self._init_order_by)
-        return source
-
-    @abstractmethod
-    def __getitem__(self, n):
-        self._not_implemented()
-
     @abstractmethod
     def __len__(self):
         self._not_implemented()
 
+    def _normalize_kwargs_names(**kwargs):
+        return kwargs
+
     @abstractmethod
     def sel(self, *args, **kwargs):
         """Filter elements on their metadata(), according to kwargs.
         Returns a new index object.
         """
-        selection = Selection(*args, **kwargs)
+        kwargs = normalize_selection(*args, **kwargs)
+        kwargs = self._normalize_kwargs_names(**kwargs)
+        if not kwargs:
+            return self
+
+        selection = Selection(kwargs)
         if selection.is_empty:
             return self
 
-        indices = []
-        for i, element in enumerate(self):
-            if selection.match_element(element):
-                indices.append(i)
+        indices = (
+            i for i, element in enumerate(self) if selection.match_element(element)
+        )
 
         return self.new_mask_index(self, indices)
 
     @abstractmethod
     def isel(self, *args, **kwargs):
         """Filter elements on their metadata() using indices, according to kwargs.
         Returns a new index object.
         """
-        selection = SelectionByIndex(self.coord, *args, **kwargs)
-        if selection.is_empty:
+        kwargs = normalize_selection(*args, **kwargs)
+        kwargs = self._normalize_kwargs_names(**kwargs)
+        if not kwargs:
             return self
-        elif not selection.is_valid:
-            self.new_mask_index(self, [])
 
-        return self.sel(selection.selection)
+        kwargs = selection_from_index(self.index, kwargs)
+
+        if not kwargs:
+            return self.new_mask_index(self, [])
 
-    def order_by(self, *args, **kwargs):
+        return self.sel(**kwargs)
+
+    def order_by(self, *args, remapping=None, **kwargs):
         """Default order_by method.
         It expects that calling self[i] returns an element that and Order object can rank
         (i.e. order.get_element_ranking(element) -> tuple).
         then it sorts the elements according to the tuples.
 
         Returns a new index object.
         """
-        order = Order(*args, **kwargs)
-        if order.is_empty:
+        kwargs = normalize_order_by(*args, **kwargs)
+        kwargs = self._normalize_kwargs_names(**kwargs)
+
+        remapping = build_remapping(remapping)
+
+        if not kwargs:
             return self
 
-        for k, v in order.order.items():
-            assert isinstance(v, (tuple, list)) or v in [
-                "ascending",
-                None,
-            ], f"Unsupported order: {v}, Supported values: 'ascending'."
-
-        class Sorter:
-            def __init__(_self, index, order):
-                """Uses the order to sort the index"""
-                _self.index = index
-                _self.order = order
-                _self._cache = [None] * len(_self.index)
-
-            def __call__(_self, i):
-                if _self._cache[i] is None:
-                    element = _self.index[i]
-                    _self._cache[i] = _self.order.get_element_ranking(element)
-                return _self._cache[i]
+        order = Order(kwargs, remapping=remapping)
+        # order = Order(*args, **kwargs)
+        if order.is_empty:
+            return self
 
-        sorter = Sorter(self, order)
+        def cmp(i, j):
+            return order.compare_elements(self[i], self[j])
 
-        result = list(range(len(self)))
-        indices = sorted(result, key=sorter)
+        indices = list(range(len(self)))
+        indices = sorted(indices, key=functools.cmp_to_key(cmp))
         return self.new_mask_index(self, indices)
 
-    def subindex(self, idx):
-        def _make_subindex(num, idx):
-            import numpy as np
+    def __getitem__(self, n):
+        if isinstance(n, slice):
+            return self.from_slice(n)
+        if isinstance(n, (tuple, list, np.ndarray)):
+            return self.from_multi(n)
+        if isinstance(n, dict):
+            return self.from_dict(n)
+        return self._getitem(n)
 
-            indices = np.arange(0, num if num > 0 else 0)
-            return indices[idx].tolist()
+    def from_slice(self, s):
+        indices = range(len(self))[s]
+        return self.new_mask_index(self, indices)
 
-        if isinstance(int, str):
-            raise ValueError(f"subindex: invalid idx type={type(idx)} specified")
+    def from_mask(self, lst):
+        indices = [i for i, x in enumerate(lst) if x]
+        return self.new_mask_index(self, indices)
 
-        indices = _make_subindex(len(self), idx)
+    def from_multi(self, a):
+        # will raise IndexError if an index is out of bounds
+        n = len(self)
+        indices = np.arange(0, n if n > 0 else 0)
+        indices = indices[a].tolist()
         return self.new_mask_index(self, indices)
 
+    def from_dict(self, dic):
+        return self.sel(dic)
+
+    @classmethod
+    def merge(cls, sources):
+        assert all(isinstance(_, Index) for _ in sources)
+        return MultiIndex(sources)
+
+    def to_numpy(self, *args, **kwargs):
+        import numpy as np
+
+        return np.array([f.to_numpy(*args, **kwargs) for f in self])
+
+    def full(self, *coords):
+        return FullIndex(self, *coords)
+
 
 class MaskIndex(Index):
     def __init__(self, index, indices):
         self.index = index
-        self.indices = indices
-        super().__init__(
-            *self.index._init_args,
-            order_by=self.index._init_order_by,
-            **self.index._init_kwargs,
-        )
+        self.indices = list(indices)
+        # super().__init__(
+        #     *self.index._init_args,
+        #     order_by=self.index._init_order_by,
+        #     **self.index._init_kwargs,
+        # )
 
-    def __getitem__(self, n):
+    def _getitem(self, n):
         n = self.indices[n]
         return self.index[n]
 
     def __len__(self):
         return len(self.indices)
 
+    def __repr__(self):
+        return "MaskIndex(%r,%s)" % (self.index, self.indices)
+
 
 class MultiIndex(Index):
     def __init__(self, indexes, *args, **kwargs):
         self.indexes = list(indexes)
         super().__init__(*args, **kwargs)
         # self.indexes = list(i for i in indexes if len(i))
         # TODO: propagate  index._init_args, index._init_order_by, index._init_kwargs, for each i in indexes?
 
     def sel(self, *args, **kwargs):
-        selection = Selection(*args, **kwargs)
-        if selection.is_empty:
+        if not args and not kwargs:
             return self
         return self.__class__(i.sel(*args, **kwargs) for i in self.indexes)
 
-    def __getitem__(self, n):
-        if isinstance(n, int):
-            if n < 0:
-                n = len(self) + n
-            k = 0
-            while n >= len(self.indexes[k]):
-                n -= len(self.indexes[k])
-                k += 1
-            return self.indexes[k][n]
-        else:
-            return self.subindex(n)
+    def _getitem(self, n):
+        k = 0
+        while n >= len(self.indexes[k]):
+            n -= len(self.indexes[k])
+            k += 1
+        return self.indexes[k][n]
 
     def __len__(self):
         return sum(len(i) for i in self.indexes)
 
     def graph(self, depth=0):
         print(" " * depth, self.__class__.__name__)
         for s in self.indexes:
             s.graph(depth + 3)
 
+    def __repr__(self):
+        return "%s(%s)" % (
+            self.__class__.__name__,
+            ",".join(repr(i) for i in self.indexes),
+        )
+
 
 class ForwardingIndex(Index):
     def __init__(self, index):
         self.index = index
 
     def __len__(self):
         return len(self.index)
@@ -455,7 +374,42 @@
     def __init__(self, index, offset, scaling):
         super().__init__(index)
         self.offset = offset
         self.scaling = scaling
 
     def __getitem__(self, n):
         return ScaledField(self.index[n], self.offset, self.scaling)
+
+
+class FullIndex(Index):
+    def __init__(self, index, *coords):
+        import numpy as np
+
+        self.index = index
+
+        # Pass1, unique values
+        unique = index.unique_values(*coords)
+        shape = tuple(len(v) for v in unique.values())
+
+        name_to_index = defaultdict(dict)
+
+        for k, v in unique.items():
+            for i, e in enumerate(v):
+                name_to_index[k][e] = i
+
+        self.size = math.prod(shape)
+        self.shape = shape
+        self.holes = np.full(shape, False)
+
+        for f in index:
+            idx = tuple(name_to_index[k][f.metadata(k, default=None)] for k in coords)
+            self.holes[idx] = True
+
+        self.holes = self.holes.flatten()
+        print("+++++++++", self.holes.shape, coords, self.shape)
+
+    def __len__(self):
+        return self.size
+
+    def _getitem(self, n):
+        assert self.holes[n], f"Attempting to access hole {n}"
+        return self.index[sum(self.holes[:n])]
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/ipython.py` & `earthkit-data-0.1.1/earthkit/data/core/ipython.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/core/plugins.py` & `earthkit-data-0.1.1/earthkit/data/core/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
                 if ext == ".yaml":
                     candidates.add(base)
                     if base == name:
                         full = os.path.join(directory, path, f)
                         return loader.load_yaml(full)
 
                 if ext == ".py" and base[0] != "_":
-
                     full = os.path.join(path, base)
 
                     if sys.platform == "win32":
                         full = full.replace("\\", "/")
 
                     if full[0] != "/":
                         full = "/" + full
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/settings.py` & `earthkit-data-0.1.1/earthkit/data/core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         self.none_ok = none_ok
         self.kind = kind if kind is not None else type(default)
 
     def kind(self):
         return type(self.default)
 
     def save(self, name, value, f):
-
         for n in self.description.split("\n"):
             print(f"# {n.strip()}", file=f)
         print(file=f)
         comment = yaml.dump({name: self.default}, default_flow_style=False)
         for n in comment.split("\n"):
             if n:
                 print(f"# {n}", file=f)
@@ -293,15 +292,14 @@
         for cb in self._callbacks:
             cb()
 
     def on_change(self, callback: Callable[[], None]):
         self._callbacks.append(callback)
 
     def _save(self):
-
         if self._settings_yaml is None:
             return
 
         try:
             save_settings(self._settings_yaml, self._settings)
         except Exception:
             LOG.error(
```

### Comparing `earthkit-data-0.1.0/earthkit/data/core/statistics.py` & `earthkit-data-0.1.1/earthkit/data/core/statistics.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/core/temporary.py` & `earthkit-data-0.1.1/earthkit/data/core/temporary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/core/thread.py` & `earthkit-data-0.1.1/earthkit/data/core/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
                 self._condition.notify_all()
 
         with self._lock:
             self._active = False
             self._error = error
 
     def submit(self, func, *args, **kwargs):  # submit
-
         with self._lock:
             if not self._active:
                 self.start()
 
         with self._condition:
             s = Future(func, args, kwargs)
             self._queue.append(s)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/data/css/tab.css` & `earthkit-data-0.1.1/earthkit/data/data/css/tab.css`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/decorators.py` & `earthkit-data-0.1.1/earthkit/data/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         with LOCK:
             return func(*args, **kwargs)
 
     return wrapped
 
 
 class Decorator:
-
     is_availability = False
 
     def __call__(self, func):
         from earthkit.data.arguments import InputManager
 
         if not callable(func):
             manager = InputManager(decorators=[self])
```

### Comparing `earthkit-data-0.1.0/earthkit/data/indexing/__init__.py` & `earthkit-data-0.1.1/earthkit/data/indexing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,11 +26,10 @@
 
 
 class PerUrlIndex:
     def __init__(
         self,
         pattern,
     ) -> None:
-
         # warnings.warn( "PerUrlIndex is obsolete.")
 
         self.pattern = pattern
```

### Comparing `earthkit-data-0.1.0/earthkit/data/indexing/database/stdout.py` & `earthkit-data-0.1.1/earthkit/data/indexing/database/stdout.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/input_manager.py` & `earthkit-data-0.1.1/earthkit/data/input_manager.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/mergers/__init__.py` & `earthkit-data-0.1.1/earthkit/data/mergers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 LOG = logging.getLogger(__name__)
 
 FORWARDS = ("to_xarray", "to_pandas", "to_tfdataset")
 
 
 def _nearest_common_class(objects):
-
     # mro() is "method resolution order"
     mros = [type(o).mro() for o in objects]
 
     first = mros[0]
     rest = mros[1:]
     for c in first:
         if all(c in m for m in rest):
@@ -44,15 +43,14 @@
 def merge_by_class(sources):
     common = _nearest_common_class(sources)
     return common.merge(sources)
 
 
 class Merger:
     def __init__(self, sources):
-
         assert sources
 
         self.sources = list(_flatten(sources))
         assert self.sources, sources
 
         self.paths = None
         self.reader_class = None
@@ -177,15 +175,14 @@
     for a in args:
         k, v = a.split("=")
         kwargs[k] = v
     return kwargs
 
 
 def make_merger(merger, sources):
-
     for fwd in FORWARDS:
         if hasattr(merger, fwd) and callable(getattr(merger, fwd)):
             LOG.debug("Merger %s has method in %s()", merger, fwd)
             return ObjMerger(merger, sources)
 
     if callable(merger):
         LOG.debug("Merger %s is callable", merger)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/mergers/pandas.py` & `earthkit-data-0.1.1/earthkit/data/mergers/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/mergers/xarray.py` & `earthkit-data-0.1.1/earthkit/data/mergers/xarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
 def merge(
     sources=None,
     paths=None,
     reader_class=None,
     **kwargs,
 ):
-
     assert sources
 
     options = infer_open_mfdataset_kwargs(
         sources=sources,
         paths=paths,
         reader_class=reader_class,
         user_kwargs=kwargs,
```

### Comparing `earthkit-data-0.1.0/earthkit/data/mirrors/__init__.py` & `earthkit-data-0.1.1/earthkit/data/mirrors/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         LOG.info(
             f"Not implemented. Not creating anything for {self.source} in mirror {self.mirror}."
         )
         return None
 
 
 class BaseMirror:
-
     _prefetch = False
 
     def __enter__(self):
         self.activate(prefetch=self._prefetch)
         return self
 
     def __exit__(self, *args, **kwargs):
```

### Comparing `earthkit-data-0.1.0/earthkit/data/mirrors/directory_mirror.py` & `earthkit-data-0.1.1/earthkit/data/mirrors/directory_mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from . import BaseMirror, MirrorConnection
 
 LOG = logging.getLogger(__name__)
 
 
 def strict_init(cls):
-
     sig = inspect.signature(cls.__init__)
 
     def check_type(name, value):
         type = sig.parameters[name].annotation
         if type == inspect._empty:
             return
         assert isinstance(value, type), (value, type)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/__init__.py` & `earthkit-data-0.1.1/earthkit/data/readers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 
 
 class ReaderMeta(type(Base), type(os.PathLike)):
     pass
 
 
 class Reader(Base, os.PathLike, metaclass=ReaderMeta):
-
     appendable = False  # Set to True if the data can be appened to and existing file
     binary = True
 
     def __init__(self, source, path):
-
         LOG.debug("Reader for %s is %s", path, self.__class__.__name__)
 
         self._source = weakref.ref(source)
         self.path = path
 
     @property
     def source(self):
@@ -90,20 +88,18 @@
 
 # TODO: Add plugins
 @locked
 def _readers(method_name):
     if not _READERS:
         here = os.path.dirname(__file__)
         for path in sorted(os.listdir(here)):
-
             if path[0] in ("_", "."):
                 continue
 
             if path.endswith(".py") or os.path.isdir(os.path.join(here, path)):
-
                 name, _ = os.path.splitext(path)
                 try:
                     for method in ["reader", "memory_reader", "stream_reader"]:
                         module = import_module(f".{name}", package=__name__)
                         if hasattr(module, method):
                             _READERS[(name, method)] = getattr(module, method)
                             if hasattr(module, "aliases"):
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/archive.py` & `earthkit-data-0.1.1/earthkit/data/readers/archive.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/bufr.py` & `earthkit-data-0.1.1/earthkit/data/readers/bufr.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/csv.py` & `earthkit-data-0.1.1/earthkit/data/readers/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     path,
     probe_size=4096,
     compression=None,
     for_is_csv=False,
     minimum_columns=2,
     minimum_rows=2,
 ):
-
     OPENS = {
         None: open,
         "zip": ZipProbe,
     }
 
     try:
         import gzip
@@ -114,15 +113,14 @@
         return None, False
 
     except csv.Error:
         return None, False
 
 
 def is_csv(path, probe_size=4096, compression=None):
-
     _, extension = os.path.splitext(path)
 
     if extension in (".xml",):
         return False
 
     dialect, _ = probe_csv(path, probe_size, compression, for_is_csv=True)
     return dialect is not None
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/directory.py` & `earthkit-data-0.1.1/earthkit/data/readers/directory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/__init__.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/codes.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
 def missing_is_none(x):
     return None if x == 2147483647 else x
 
 
 # This does not belong here, should be in the C library
 def get_messages_positions(path):
-
     fd = os.open(path, os.O_RDONLY)
     try:
 
         def get(count):
             buf = os.read(fd, count)
             assert len(buf) == count
             return int.from_bytes(
@@ -107,31 +106,30 @@
         super().__init__(handle)
         self.path = path
         self.offset = offset
 
     # TODO: just a wrapper around the base class implementation to handle the
     # s,l,d qualifiers. Once these are implemented in the base class this method can
     # be removed. md5GridSection is also handled!
-    def get(self, name, default=None, ktype=None):
-
+    def get(self, name, ktype=None, **kwargs):
         if name == "values":
             return self.get_values()
         elif name == "md5GridSection":
             return self.get_md5GridSection()
 
         if ktype is None:
-            name_part, _, key_type_str = name.partition(":")
+            name, _, key_type_str = name.partition(":")
             if key_type_str in CodesHandle.KEY_TYPES:
-                return super().get(
-                    name_part,
-                    default=default,
-                    ktype=CodesHandle.KEY_TYPES[key_type_str],
-                )
+                ktype = CodesHandle.KEY_TYPES[key_type_str]
 
-        return super().get(name, default=default, ktype=ktype)
+        if "default" in kwargs:
+            return super().get(name, ktype=ktype, **kwargs)
+        else:
+            # this will throw if name is not available
+            return super()._get(name, ktype=ktype)
 
     def get_md5GridSection(self):
         # Special case because:
         #
         # 1) eccodes is returning size > 1 for 'md5GridSection'
         # (size = 16 : it is the number of bytes of the value)
         # This is already fixed in eccodes 2.27.1
@@ -212,29 +210,33 @@
 class ReaderLRUCache(dict):
     def __init__(self, size):
         self.readers = dict()
         self.lock = threading.Lock()
         self.size = size
 
     def __getitem__(self, path):
+        key = (
+            path,
+            os.getpid(),
+        )
         with self.lock:
             try:
-                return super().__getitem__(path)
+                return super().__getitem__(key)
             except KeyError:
                 pass
 
-            c = self[path] = CodesReader(path)
+            c = self[key] = CodesReader(path)
             while len(self) >= self.size:
-                oldest = min((v.last, v.path) for v in self.values())
-                del self[oldest[1]]
+                _, oldest = min((v.last, k) for k, v in self.items())
+                del self[oldest]
 
             return c
 
 
-cache = ReaderLRUCache(512)  # TODO: Add to config
+cache = ReaderLRUCache(32)  # TODO: Add to config
 
 
 class CodesReader:
     def __init__(self, path):
         self.path = path
         self.lock = threading.Lock()
         # print("OPEN", self.path)
@@ -259,28 +261,25 @@
             handle = eccodes.codes_new_from_file(
                 self.file,
                 eccodes.CODES_PRODUCT_GRIB,
             )
             assert handle is not None
             return CodesHandle(handle, self.path, offset)
 
+    def __repr__(self):
+        return f"{self.__class__.__name__}({self.path}"
+
 
 class GribField(Base):
     def __init__(self, path, offset, length):
         self.path = path
         self._offset = offset
         self._length = length
         self._handle = None
 
-    # def __enter__(self):
-    #     return self
-
-    # def __exit__(self, exc_type, exc_val, exc_tb):
-    #     pass
-
     @property
     def handle(self):
         if self._handle is None:
             assert self._offset is not None
             self._handle = CodesReader.from_cache(self.path).at_offset(self._offset)
         return self._handle
 
@@ -292,18 +291,19 @@
     def offset(self):
         if self._offset is None:
             self._offset = int(self.handle.get("offset"))
         return self._offset
 
     @property
     def shape(self):
-        Nj = missing_is_none(self.handle.get("Nj"))
-        Ni = missing_is_none(self.handle.get("Ni"))
+        Nj = missing_is_none(self.handle.get("Nj", default=None))
+        Ni = missing_is_none(self.handle.get("Ni", default=None))
         if Ni is None or Nj is None:
-            return self.handle.get("numberOfDataPoints")
+            n = self.handle.get("numberOfDataPoints", default=None)
+            return (n,)  # shape must be a tuple
         return (Nj, Ni)
 
     def data(self, *args, flatten=False):
         keys = dict(
             lat=self.handle.get_latitudes,
             lon=self.handle.get_longitudes,
             value=self.handle.get_values,
@@ -324,78 +324,77 @@
 
     def to_points(self, flatten=True):
         lon, lat = self.data("lon", "lat", flatten=flatten)
         return dict(lon=lon, lat=lat)
 
     def __repr__(self):
         return "GribField(%s,%s,%s,%s,%s,%s)" % (
-            self.handle.get("shortName"),
-            self.handle.get("levelist"),
-            self.handle.get("date"),
-            self.handle.get("time"),
-            self.handle.get("step"),
-            self.handle.get("number"),
+            self.handle.get("shortName", default=None),
+            self.handle.get("levelist", default=None),
+            self.handle.get("date", default=None),
+            self.handle.get("time", default=None),
+            self.handle.get("step", default=None),
+            self.handle.get("number", default=None),
         )
 
     def datetime(self, **kwargs):
         return {
             "base_time": self._base_datetime(),
             "valid_time": self._valid_datetime(),
         }
 
     def _base_datetime(self):
-        date = self.handle.get("date")
-        time = self.handle.get("time")
+        date = self.handle.get("date", default=None)
+        time = self.handle.get("time", default=None)
         return datetime.datetime(
             date // 10000,
             date % 10000 // 100,
             date % 100,
             time // 100,
             time % 100,
         )
 
     def _valid_datetime(self):
-        step = self.handle.get("endStep")
+        step = self.handle.get("endStep", default=None)
         return self._base_datetime() + datetime.timedelta(hours=step)
 
     def proj_string(self):
         return self.proj_target_string()
 
     def proj_source_string(self):
-        return self.handle.get("projSourceString")
+        return self.handle.get("projSourceString", default=None)
 
     def proj_target_string(self):
-        return self.handle.get("projTargetString")
+        return self.handle.get("projTargetString", default=None)
 
     def bounding_box(self):
         return BoundingBox(
-            north=self.handle.get("latitudeOfFirstGridPointInDegrees"),
-            south=self.handle.get("latitudeOfLastGridPointInDegrees"),
-            west=self.handle.get("longitudeOfFirstGridPointInDegrees"),
-            east=self.handle.get("longitudeOfLastGridPointInDegrees"),
+            north=self.handle.get("latitudeOfFirstGridPointInDegrees", default=None),
+            south=self.handle.get("latitudeOfLastGridPointInDegrees", default=None),
+            west=self.handle.get("longitudeOfFirstGridPointInDegrees", default=None),
+            east=self.handle.get("longitudeOfLastGridPointInDegrees", default=None),
         )
 
     def _attributes(self, names):
         result = {}
         for name in names:
-            result[name] = self.handle.get(name)
+            result[name] = self.handle.get(name, default=None)
         return result
 
     def _get(self, name):
         """Private, for testing only"""
         # paramId is renamed as param to get rid of the
         # additional '.128' (in earthkit/data/scripts/grib.py)
         if name == "param":
             name = "paramId"
         return self.handle.get(name)
 
     # TODO: move it into core or util
     @staticmethod
     def _parse_metadata_args(*args, namespace=None, astype=None):
-
         key = []
         for k in args:
             if isinstance(k, str):
                 key.append(k)
             elif isinstance(k, (list, tuple)):
                 key.extend(k)
             else:
@@ -422,15 +421,15 @@
         if namespace is None:
             namespace = []
         elif isinstance(namespace, str):
             namespace = [namespace]
 
         return (key, namespace, astype)
 
-    def metadata(self, *args, namespace=None, astype=None):
+    def metadata(self, *args, namespace=None, astype=None, **kwargs):
         def _key_name(key):
             if key == "param":
                 key = "shortName"
             elif key == "_param_id":
                 key = "paramId"
             return key
 
@@ -442,15 +441,18 @@
         assert isinstance(namespace, (list, tuple))
 
         if key:
             assert isinstance(astype, (list, tuple))
             if namespace:
                 key = [namespace[0] + "." + k for k in key]
 
-            r = [self.handle.get(_key_name(k), ktype=kt) for k, kt in zip(key, astype)]
+            r = [
+                self.handle.get(_key_name(k), ktype=kt, **kwargs)
+                for k, kt in zip(key, astype)
+            ]
             return tuple(r) if len(r) > 1 else r[0]
         else:
             if len(namespace) == 0:
                 namespace = GRIB_NAMESPACES
             r = {ns: self.handle.as_namespace(ns) for ns in namespace}
             if len(r) == 1:
                 return r[namespace[0]]
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/memory.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/pandas.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/pandas.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/parsing.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/parsing.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,55 +2,114 @@
 #
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
+
+import datetime
+import fnmatch
 import logging
 import os
 
-from earthkit.data.readers.grib.codes import CodesHandle
-from earthkit.data.utils import progress_bar, tqdm
+from tqdm import tqdm
 
 LOG = logging.getLogger(__name__)
 
 
+def post_process_valid_date(field, h):
+    date = h.get("validityDate")
+    time = h.get("validityTime")
+    field["datetime"] = datetime.datetime(
+        date // 10000,
+        date % 10000 // 100,
+        date % 100,
+        time // 100,
+        time % 100,
+    )
+    # Note that we do not create a script here:
+    # There is no ".isoformat()". Because the sql database
+    # takes care of this conversion back and forth.
+    return field
+
+
+def post_process_parameter_level(field, h):
+    param = field.get("param", None)
+    if param is None:
+        field["param_level"] = None
+        return field
+
+    level = field.get("levelist", None)
+    if level is None:
+        field["param_level"] = param
+        return field
+
+    field["param_level"] = f"{param}_{level}"
+    return field
+
+
+def post_process_statistics(field, h):
+    values = h.get("values")
+    field["mean"] = values.mean()
+    field["std"] = values.std()
+    field["min"] = values.min()
+    field["max"] = values.max()
+    field["shape"] = ",".join([str(_) for _ in values.shape])
+    return field
+
+
 def _index_grib_file(
     path,
     with_statistics=False,
+    with_valid_date=True,
+    with_parameter_level=True,
 ):
     import eccodes
 
-    # TODO: deduplicate this code
+    from earthkit.data.readers.grib.codes import CodesHandle
+
+    post_process_mars = []
+    if with_valid_date:
+        post_process_mars.append(post_process_valid_date)
+    if with_parameter_level:
+        post_process_mars.append(post_process_parameter_level)
+    if with_statistics:
+        post_process_mars.append(post_process_statistics)
 
     def parse_field(h):
         field = h.as_namespace("mars")
 
+        if post_process_mars:
+            for f in post_process_mars:
+                field = f(field, h)
+
         field["_path"] = path
         field["_offset"] = h.get_long("offset")
         field["_length"] = h.get_long("totalLength")
         field["_param_id"] = h.get_string("paramId")
         field["md5_grid_section"] = h.get("md5GridSection")
 
         # eccodes.codes_get_string(h, "number") returns "0"
         # when "number" is not in the iterator
         # remove? field["number"] = h.get("number")
 
-        if with_statistics:
-            values = h.get("values")
-            field["mean"] = values.mean()
-            field["std"] = values.std()
-            field["min"] = values.min()
-            field["max"] = values.max()
-
         return field
 
     size = os.path.getsize(path)
-    pbar = progress_bar(desc=f"Parsing {path}", total=size)
+    pbar = tqdm(
+        desc=f"Parsing {path}",
+        total=size,
+        unit_scale=True,
+        unit_divisor=1024,
+        unit="B",
+        leave=False,
+        # position=TQDM_POSITION,
+        dynamic_ncols=True,
+    )
 
     with open(path, "rb") as f:
         old_position = f.tell()
         h = eccodes.codes_grib_new_from_file(f)
 
         while h:
             yield parse_field(CodesHandle(h, path, offset=old_position))
@@ -60,17 +119,17 @@
             old_position = position
             h = eccodes.codes_grib_new_from_file(f)
 
     pbar.close()
 
 
 def _index_url(url):
-    import earthkit.data as cml
+    import earthkit.data
 
-    path = cml.from_source("url", url).path
+    path = earthkit.data.from_source("url", url).path
     # TODO: should use download_and_cache
     # path = download_and_cache(url)
     for entry in _index_grib_file(path):
         del entry["_path"]
         yield entry
 
 
@@ -85,23 +144,30 @@
 
 class PathParserIterator:
     """Delays parsing the directory for the list of files
     until the iterator is actually used (calling __iter__)
     """
 
     def __init__(
-        self, path, relative_paths, ignore=None, followlinks=True, verbose=False
+        self,
+        path,
+        relative_paths,
+        ignore=None,
+        followlinks=True,
+        verbose=False,
+        with_statistics=True,
     ):
         if ignore is None:
             ignore = []
         self.ignore = ignore
         self.path = path
         self.relative_paths = relative_paths
         self.followlinks = followlinks
         self.verbose = verbose
+        self.with_statistics = with_statistics
 
         self._tasks = None
 
     def __iter__(self):
         for path in tqdm(self.tasks, dynamic_ncols=True):
             for entry in self.process_one_task(path):
                 yield entry
@@ -111,14 +177,20 @@
         if self._tasks is not None:
             return self._tasks
 
         LOG.debug(f"Parsing files in path={self.path}")
         assert os.path.exists(self.path), f"{self.path} does not exist"
         # assert os.path.isdir(self.path), f"{self.path} is not a directory"
 
+        def _ignore(path):
+            for ignore in self.ignore:
+                if fnmatch.fnmatch(os.path.basename(path), ignore):
+                    return True
+            return False
+
         tasks = []
 
         if not os.path.isdir(self.path):
             tasks.append(self.path)
         else:
             for root, _, files in os.walk(self.path, followlinks=self.followlinks):
                 for name in files:
@@ -156,15 +228,15 @@
             # grib-index auxiliary file in the cache.
             # Indexing 1M grib files lead to 1M in cache.
             #
             # We would need either to refactor the grib reader.
 
             from earthkit.data.readers.grib.parsing import _index_grib_file
 
-            for field in _index_grib_file(path, with_statistics=True):
+            for field in _index_grib_file(path, with_statistics=self.with_statistics):
                 field["_path"] = _path
                 yield field
         except PermissionError as e:
             LOG.error(f"Could not read {path}: {e}")
             return
         except Exception as e:
             print(f"(grib-parsing) Ignoring {path}, {e}")
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/grib/xarray.py` & `earthkit-data-0.1.1/earthkit/data/readers/grib/xarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     def xarray_open_dataset_kwargs(self):
         return dict(
             cache=True,  # Set to false to prevent loading the whole dataset
             chunks=None,  # Set to 'auto' for lazy loading
         )
 
     def to_xarray(self, **kwargs):
-
         import xarray as xr
 
         xarray_open_dataset_kwargs = {}
 
         if "xarray_open_mfdataset_kwargs" in kwargs:
             warnings.warn(
                 "xarray_open_mfdataset_kwargs is deprecated, please use xarray_open_dataset_kwargs instead."
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/netcdf.py` & `earthkit-data-0.1.1/earthkit/data/readers/netcdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,21 @@
 
     def __getitem__(self, key):
         if key not in self._cache:
             self._cache[key] = self._ds[key]
         return self._cache[key]
 
     def bbox(self, variable):
-
         data_array = self[variable]
         dims = data_array.dims
 
         lat = dims[-2]
         lon = dims[-1]
 
         if (lat, lon) not in self._bbox:
-
             dims = data_array.dims
 
             latitude = data_array[lat]
             longitude = data_array[lon]
 
             self._bbox[(lat, lon)] = (
                 np.amax(latitude.data),
@@ -143,15 +141,14 @@
             )
 
         return self._bbox[(lat, lon)]
 
 
 class NetCDFField(Base):
     def __init__(self, path, ds, variable, slices, non_dim_coords):
-
         data_array = ds[variable]
 
         self._ds = ds
         self._da = data_array
 
         self.north, self.west, self.south, self.east = ds.bbox(variable)
 
@@ -169,15 +166,14 @@
         )
 
         self.time = non_dim_coords.get("valid_time", non_dim_coords.get("time"))
 
         # print('====', non_dim_coords)
 
         for s in self.slices:
-
             if isinstance(s, TimeSlice):
                 self.time = s.value
 
             if s.is_info:
                 self.title += " (" + s.name + "=" + str(s.value) + ")"
 
     def __repr__(self):
@@ -277,39 +273,37 @@
         for name in ds.data_vars:
             v = ds[name]
             skip.update(getattr(v, "coordinates", "").split(" "))
             skip.update(getattr(v, "bounds", "").split(" "))
             skip.update(getattr(v, "grid_mapping", "").split(" "))
 
         for name in ds.data_vars:
-
             if name in skip:
                 continue
 
             v = ds[name]
 
             coordinates = []
 
             # self.log.info('Scanning file: %s var=%s coords=%s', self.path, name, v.coords)
 
             info = [value for value in v.coords if value not in v.dims]
             non_dim_coords = {}
             for coord in v.coords:
-
                 if coord not in v.dims:
                     non_dim_coords[coord] = ds[coord].values
                     continue
 
                 c = ds[coord]
 
                 # self.log.info("COORD %s %s %s %s", coord, type(coord), hasattr(c, 'calendar'), c)
 
-                standard_name = getattr(c, "standard_name", None)
-                axis = getattr(c, "axis", None)
-                long_name = getattr(c, "long_name", None)
+                standard_name = getattr(c, "standard_name", "")
+                axis = getattr(c, "axis", "")
+                long_name = getattr(c, "long_name", "")
 
                 use = False
 
                 if (
                     standard_name.lower() in GEOGRAPHIC_COORDS["x"]
                     or (long_name == "longitude")
                     or (axis == "X")
@@ -346,15 +340,14 @@
                     coordinates.append(OtherCoordinate(c, coord in info))
 
             if not (has_lat and has_lon):
                 # self.log.info("NetCDFReader: skip %s (Not a 2 field)", name)
                 continue
 
             for values in product(*[c.values for c in coordinates]):
-
                 slices = []
                 for value, coordinate in zip(values, coordinates):
                     slices.append(coordinate.make_slice(value))
 
                 fields.append(NetCDFField(self.path, ds, name, slices, non_dim_coords))
 
         if not fields:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/numpy.py` & `earthkit-data-0.1.1/earthkit/data/readers/numpy.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/odb.py` & `earthkit-data-0.1.1/earthkit/data/readers/odb.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/tar.py` & `earthkit-data-0.1.1/earthkit/data/readers/tar.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/text.py` & `earthkit-data-0.1.1/earthkit/data/readers/text.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/unknown.py` & `earthkit-data-0.1.1/earthkit/data/readers/unknown.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/readers/zip.py` & `earthkit-data-0.1.1/earthkit/data/readers/zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,30 +50,28 @@
 
         self._mutate = None
 
         with ZipFile(path, "r") as zip:
             members = zip.infolist()
 
             if len(members) == 1:
-
                 _, ext = os.path.splitext(members[0].filename)
                 if ext in (".csv",):
                     self._mutate = CSVReader(source, path, compression="zip")
                     return  # Pandas can read zipped files directly
 
             if ".zattrs" in members:
                 return  # Zarr can read zipped files directly
 
             self.expand(zip, members)
 
     def check(self, member):
         return super().check(InfoWrapper(member))
 
     def mutate(self):
-
         if self._mutate:
             return self._mutate
 
         return super().mutate()
 
     def mutate_source(self):
         # zarr can read data from a zip file
@@ -83,15 +81,14 @@
         return None
 
 
 EXTENSIONS_TO_SKIP = (".npz",)  # Numpy arrays
 
 
 def reader(source, path, magic=None, deeper_check=False):
-
     if magic is None:  # Bypass check and force
         return ZIPReader(source, path)
 
     _, extension = os.path.splitext(path)
 
     if magic[:4] == b"PK\x03\x04" and extension not in EXTENSIONS_TO_SKIP:
         return ZIPReader(source, path)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/__init__.py` & `earthkit-data-0.1.1/earthkit/data/sources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
         return table(self)
 
     def graph(self, depth=0):
         print(" " * depth, self)
 
 
 class SourceLoader:
-
     kind = "source"
 
     def load_module(self, module):
         return import_module(module, package=__name__).source
 
     def load_entry(self, entry):
         entry = entry.load()
@@ -129,15 +128,14 @@
         return self(name.replace("_", "-"))
 
 
 get_source = SourceMaker()
 
 
 def from_source(name: str, *args, lazily=False, **kwargs) -> Source:
-
     if lazily:
         return from_source_lazily(name, *args, **kwargs)
 
     prev = None
     src = get_source(name, *args, **kwargs)
     while src is not prev:
         prev = src
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/dummy_source.py` & `earthkit-data-0.1.1/earthkit/data/sources/dummy_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     import json
 
     with open(target, "w") as f:
         print(json.dumps(kwargs), file=f)
 
 
 def generate_zeros(target, size=1024 * 1024, chunk_size=1024 * 1024, **kwargs):
-
     chunk_size = min(chunk_size, size)
     zeros = bytes(chunk_size)
 
     with open(target, "wb") as f:
         while size > 0:
             bufsize = min(size, chunk_size)
             f.write(zeros[:bufsize])
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/empty.py` & `earthkit-data-0.1.1/earthkit/data/sources/empty.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/fdb.py` & `earthkit-data-0.1.1/earthkit/data/sources/fdb.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/file.py` & `earthkit-data-0.1.1/earthkit/data/sources/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         if "reader" in kwargs:
             setattr(obj, "reader", kwargs.pop("reader"))
 
         return super().patch(obj, *args, **kwargs)
 
 
 class FileSource(Source, os.PathLike, metaclass=FileSourceMeta):
-
     _reader_ = None
 
     def __init__(self, path=None, filter=None, merger=None, **kwargs):
         Source.__init__(self, **kwargs)
         self.path = path
         self.filter = filter
         self.merger = merger
@@ -141,20 +140,19 @@
 
     def __fspath__(self):
         return self.path
 
     def metadata(self, *args, **kwargs):
         return self._reader.metadata(*args, **kwargs)
 
-    @property
-    def coords(self):
-        return self._reader.coords
+    def indices(self, *args, **kwargs):
+        return self._reader.indices(*args, **kwargs)
 
-    def coord(self, *args, **kwargs):
-        return self._reader.coord(*args, **kwargs)
+    def index(self, *args, **kwargs):
+        return self._reader.index(*args, **kwargs)
 
     def head(self, n=5, **kwargs):
         if n <= 0:
             raise ValueError("head: n must be > 0")
         return self.ls(n=n, **kwargs)
 
     def tail(self, n=5, **kwargs):
@@ -191,17 +189,15 @@
         expand_vars=False,
         unix_glob=True,
         recursive_glob=True,
         filter=None,
         merger=None,
         **kwargs,
     ):
-
         if not isinstance(path, (list, tuple)):
-
             if expand_user:
                 path = os.path.expanduser(path)
 
             if expand_vars:
                 path = os.path.expandvars(path)
 
             if unix_glob and set(path).intersection(set("[]?*")):
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/file_indexed.py` & `earthkit-data-0.1.1/earthkit/data/sources/file_indexed.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 import logging
 import os
 
-from earthkit.data.readers.grib.index import FieldsetInFilesWithSqlIndex
+from earthkit.data.readers.grib.index.sql import FieldsetInFilesWithSqlIndex
 from earthkit.data.readers.grib.parsing import GribIndexingPathParserIterator
 from earthkit.data.sources.indexed import IndexedSource
 
 LOG = logging.getLogger(__name__)
 
 
 def make_absolute(filename, root_dir, default):
@@ -92,8 +92,9 @@
         # Create the db_path file in cache (or used the cached one)
         LOG.info(f"Did not find index files in {db_path} or {index_file}")
         ignore = [self.DEFAULT_DB_FILE, self.DEFAULT_JSON_FILE, db_path, index_file]
         index = self.INDEX_CLASS.from_iterator(
             GribIndexingPathParserIterator(path, ignore=ignore, relative_paths=False),
             cache_metadata={"directory": self.path},
         )
+
         super().__init__(index, **kwargs)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/file_pattern.py` & `earthkit-data-0.1.1/earthkit/data/sources/file_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/indexed.py` & `earthkit-data-0.1.1/earthkit/data/sources/indexed.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from earthkit.data.sources import Source
 
 LOG = logging.getLogger(__name__)
 
 
 class IndexedSource(Source):
-
     _reader_ = None
 
     def __init__(self, index, order_by=None, filter=None, merger=None, **kwargs):
         LOG.debug(f"New IndexedSource order={order_by} kwargs={kwargs}")
 
         def _build_order_by_from_selection(selection):
             if not selection:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/list_of_dicts.py` & `earthkit-data-0.1.1/earthkit/data/sources/list_of_dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 from earthkit.data.readers.grib.index import FieldSet
 
 LOG = logging.getLogger(__name__)
 
 
 class VirtualGribField(dict):
-
     KEY_TYPES = {
         "s": str,
         "l": int,
         "d": float,
         "str": str,
         "int": int,
         "float": float,
@@ -33,15 +32,15 @@
         "level": "levelist",
         "step": "endStep",
     }
 
     for k in list(NAME_LOOKUP.keys()):
         NAME_LOOKUP[NAME_LOOKUP[k]] = k
 
-    def metadata(self, name):
+    def metadata(self, name, **kwargs):
         name, _, key_type_str = name.partition(":")
         try:
             key_type = self.KEY_TYPES[key_type_str]
         except KeyError:
             raise ValueError(f"Key type={key_type_str} not supported")
 
         try:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/memory.py` & `earthkit-data-0.1.1/earthkit/data/sources/memory.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/multi.py` & `earthkit-data-0.1.1/earthkit/data/sources/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         for s in self.sources:
             s._set_dataset(dataset)
 
     def __iter__(self):
         return itertools.chain(*self.sources)
 
     def __getitem__(self, n):
-
         if n < 0:
             n = len(self) + n
 
         i = 0
         while n >= self._length(i):
             n -= self._length(i)
             i += 1
@@ -121,15 +120,14 @@
         if nthreads < 2:
             return [s() for s in sources]
 
         def _call(s, *args, **kwargs):
             return s(*args, **kwargs)
 
         with SoftThreadPool(nthreads=nthreads) as pool:
-
             futures = [pool.submit(_call, s, observer=pool) for s in sources]
 
             iterator = (f.result() for f in futures)
             sources = list(tqdm(iterator, leave=False, total=len(futures)))
 
         return sources
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/multi_url.py` & `earthkit-data-0.1.1/earthkit/data/sources/multi_url.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/stream.py` & `earthkit-data-0.1.1/earthkit/data/sources/stream.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/url.py` & `earthkit-data-0.1.1/earthkit/data/sources/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     chunk_size=1024 * 1024,
     range_method="auto",
     http_headers=None,
     update_if_out_of_date=False,
     fake_headers=None,  # When HEAD is not allowed but you know the size
     **kwargs,
 ):
-
     # TODO: re-enable this feature
     extension = None
 
     LOG.debug("URL %s", url)
 
     downloader = Downloader(
         url,
@@ -115,15 +114,14 @@
         force=None,
         chunk_size=1024 * 1024,
         range_method="auto",
         http_headers=None,
         update_if_out_of_date=False,
         fake_headers=None,  # When HEAD is not allowed but you know the size
     ):
-
         super().__init__(filter=filter, merger=merger)
 
         # TODO: re-enable this feature
         extension = None
 
         self.url = url
         self.parts = parts
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/url_pattern.py` & `earthkit-data-0.1.1/earthkit/data/sources/url_pattern.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/virtual.py` & `earthkit-data-0.1.1/earthkit/data/sources/virtual.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,25 +118,23 @@
                 "latitude": 721,
                 "longitude": 1440,
             },
             lock=NoLock(),
         )
 
     def full_month(self, date):
-
         yyyymm = date // 100
 
         with self.lock:
             if yyyymm in self.fields:
                 return self.fields[yyyymm]
             if yyyymm not in self.locks:
                 self.locks[yyyymm] = threading.Lock()
 
         with self.locks[yyyymm]:
-
             # Some other threads may have created that in the meantime
 
             if yyyymm in self.fields:
                 return self.fields[yyyymm]
 
             yyyy = yyyymm // 100
             mm = yyyymm % 100
```

### Comparing `earthkit-data-0.1.0/earthkit/data/sources/virtual_directory.py` & `earthkit-data-0.1.1/earthkit/data/sources/virtual_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,14 @@
             return self[key]
 
     def __str__(self):
         return f"{self.field} (cached)"
 
 
 class VirtualField:  # Should inherit from GribField
-
     _real_item = None
 
     def __init__(self, i, owner):
         self.i = i
         self.owner = owner
         self.item_metadata = owner.get_metadata(i)
 
@@ -167,15 +166,14 @@
 
         return item
 
     def get_real_item(self, n):
         return super().__getitem__(n)
 
     def _get_metadata_for_item(self, key, item):
-
         func = METADATA_FUNCS[key]
 
         try:
             value = func(key, item)
         except Exception as e:
             LOG.exception(f"Exception reading {key}:{str(e)}")
             return None
```

### Comparing `earthkit-data-0.1.0/earthkit/data/testing.py` & `earthkit-data-0.1.1/earthkit/data/testing.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/__init__.py` & `earthkit-data-0.1.1/earthkit/data/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
 
 def _dummy(**kwargs):
     pass
 
 
 def consume_args(func1, func2, *args, **kwargs):
-
     # print("=====>", args, kwargs)
 
     if func1 is None:
         func1 = _dummy
 
     if func2 is None:
         func2 = _dummy
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/availability.py` & `earthkit-data-0.1.1/earthkit/data/utils/availability.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/bbox.py` & `earthkit-data-0.1.1/earthkit/data/utils/bbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         lon -= 360
 
     return lon
 
 
 class BoundingBox:
     def __init__(self, *, north, west, south, east):
-
         # Convert to float as these values may come from Numpy
         self.north = min(float(north), 90.0)
         self.south = max(float(south), -90.0)
 
         self.is_periodic_west_east = (east - west) == 360
         self.west = _normalize(float(west), -180)  # Or 0?
 
@@ -70,15 +69,14 @@
 
     @property
     def height(self):
         return self.north - self.south
 
     @classmethod
     def multi_merge(cls, bboxes):
-
         north = max(z.north for z in bboxes)
         south = min(z.south for z in bboxes)
 
         first = bboxes[0]
 
         origin = first.east % 360
         full = BoundingBox(
@@ -89,15 +87,14 @@
         )
 
         # Build the list of provided [west, east] intervals
 
         boundaries = list()
         stacked_intervals = set()  # To keep track of overlapping intervals
         for i, b in enumerate(bboxes):
-
             if b.east - b.west == 360:
                 return full
 
             west = (b.west - origin) % 360
             east = (b.east - origin) % 360
 
             if west > east:
@@ -113,15 +110,14 @@
         west = 0
         east = 0
 
         # Find the longest interval *outside* the provided [west, east] intervals
         # It's complement will be the result
 
         for cursor, entering, interval in boundaries:
-
             if entering:
                 if not stacked_intervals:
                     distance = cursor - start
                     if distance > best:
                         best = distance
                         west = cursor
                         east = start
@@ -145,15 +141,14 @@
             east=origin + east,
         )
 
     def merge(self, other):
         return self.multi_merge([self, other])
 
     def add_margins(self, margins):
-
         if isinstance(margins, str) and margins[-1] == "%":
             margins = int(margins[:-1]) / 100.0
             margins = max(
                 (self.north - self.south) * margins, (self.east - self.west) * margins
             )
 
         # TODO:check east/west
@@ -177,15 +172,14 @@
         return (self.north, self.west, self.south, self.east)
 
     def as_dict(self):
         return dict(north=self.north, west=self.west, south=self.south, east=self.east)
 
 
 def bounding_box(obj):
-
     if isinstance(obj, BoundingBox):
         return obj
 
     if isinstance(obj, (list, tuple)):
         return BoundingBox(north=obj[0], west=obj[1], south=obj[2], east=obj[3])
 
     obj = get_wrapper(obj)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/conventions.py` & `earthkit-data-0.1.1/earthkit/data/utils/conventions.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 
 from earthkit.data.vocabularies import VOCABULARIES
 
 LOG = logging.getLogger(__name__)
 
 
 def normalise_string(key, convention="cf"):
-
     vocabulary = VOCABULARIES[convention]
 
     new = vocabulary.normalise(key)
     LOG.debug(f"Normalising '{key}' into '{new}' ({convention} convention)")
     return new
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/dates.py` & `earthkit-data-0.1.1/earthkit/data/utils/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     while start <= end:
         result.append(start)
         start = start + datetime.timedelta(days=by)
     return result
 
 
 def to_datetime_list(datetimes):  # noqa C901
-
     if isinstance(datetimes, (datetime.datetime, np.datetime64)):
         return to_datetime_list([datetimes])
 
     if isinstance(datetimes, (list, tuple)):
         if (
             len(datetimes) == 3
             and isinstance(datetimes[1], str)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/factorise.py` & `earthkit-data-0.1.1/earthkit/data/utils/factorise.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
             result = [r for r in result if r is not None]
 
         return tuple(result)
 
     def __repr__(self):
         if isinstance(self.start, datetime.date):
-
             if self.start == self.end:
                 return self.start.strftime("%Y-%m-%d")
 
             return "%s/%s" % (
                 self.start.strftime("%Y-%m-%d"),
                 self.end.strftime("%Y-%m-%d"),
             )
@@ -146,15 +145,14 @@
         return (self.start, self.end) != (other.start, other.end)
 
     def __hash__(self):
         return hash((self.start, self.end))
 
 
 def _cleanup(x):
-
     if isinstance(x, (list, tuple)):
         return [_cleanup(a) for a in x]
 
     if isinstance(x, dict):
         return {_cleanup(k): _cleanup(v) for k, v in x.items()}
 
     if isinstance(x, (str, int, float)):
@@ -290,19 +288,17 @@
             if k in self._intervals:
                 request[k] = _as_interval(v)
             else:
                 request[k] = _as_tuple(v)
         return request
 
     def count(self, _kwargs=None, **kwargs):
-
         return self._count(self._kwargs_to_request(_kwargs, **kwargs))
 
     def _count(self, request):
-
         if not self._values and not self._children:
             return 0
 
         ok, matches = self._match(request)
         if not ok:
             return 0
 
@@ -361,15 +357,14 @@
         s = [_from_hashable(x) for x in user.difference(user.intersection(tree))]
 
         return _factorise(s, intervals=self._intervals)
 
     def _match(self, request):
         matches = {}
         for name, values in [(n, v) for (n, v) in request.items() if n in self._values]:
-
             if name in self._intervals:
                 common = Interval.intersection(values, self._values[name])
             else:
                 common = set(values).intersection(set(self._values[name]))
 
             if len(common) == 0:
                 return False, None
@@ -399,15 +394,14 @@
             return self._children[0]
         return self
 
     def factorise(self):
         return _factorise(list(self._flatten_tree()), intervals=self._intervals)
 
     def tree(self):
-
         text = []
         indent = {}
         order = {}
 
         def V(request, depth):
             if not request:
                 return
@@ -483,15 +477,14 @@
 
     def __repr__(self):
         return "Column(%s,%s,%s,%s)" % (self.title, self.values, self.prio, self.diff)
 
 
 class Table(object):
     def __init__(self, other=None, a=None, b=None):
-
         self.tree = Tree()
 
         if other is not None:
             self.depth = other.depth + 1
             self.cols = copy(other.cols)
             self.colidx = copy(other.colidx)
             self.rowidx = other.rowidx[a:b]
@@ -645,15 +638,14 @@
             c.append(value)
         n += m
 
     return n
 
 
 def _as_requests(r):
-
     s = {}
     for k, v in r.items():
         if not isinstance(v, (tuple, list)):
             s[k] = [v]
         else:
             s[k] = v
 
@@ -663,15 +655,14 @@
 def factorise(req, *, intervals=None):
     # Make a copy so we don't modify the original
     safe = [dict(**r) for r in req]
     return _factorise(safe, intervals=intervals)
 
 
 def _factorise(req, intervals=None):
-
     if intervals is None:
         intervals = []
 
     if not isinstance(intervals, (list, tuple, set)):
         intervals = [intervals]
 
     if intervals:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/html.py` & `earthkit-data-0.1.1/earthkit/data/utils/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 
 def tr(key, value):
     return f"<tr>{td(bold(key))}{td(value)}</tr>"
 
 
 def table(obj):
-
     style = css("table")
 
     table = """
 <h4>{name}</h4>
 <table class="eh">
 <tr><td><b>Home page</b></td><td>{home_page}</td></tr>
 <tr><td><b>Documentation</b></td><td>{documentation}</td></tr>
@@ -53,15 +52,14 @@
         documentation=urlify(obj.documentation),
     )
 
     return style + table
 
 
 def table_from_dict(vals, title=None):
-
     if not isinstance(vals, dict):
         raise TypeError(f"table_from_dict: vals must be a dict not type={type(vals)}")
 
     t = ""
     if title is not None and title:
         t = f"<h4>{title}</h4>"
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/humanize.py` & `earthkit-data-0.1.1/earthkit/data/utils/humanize.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     if count > 1:
         return "s"
     else:
         return ""
 
 
 def seconds(seconds):
-
     if isinstance(seconds, datetime.timedelta):
         seconds = seconds.total_seconds()
 
     if seconds == 0:
         return "instantaneous"
 
     if seconds < 0.1:
@@ -240,22 +239,20 @@
                 d[i - 1, j - 1] + cost,
             )
 
     return d[m, n]
 
 
 def did_you_mean(word, vocabulary):
-
     distance, best = min((string_distance(word, w), w) for w in vocabulary)
     # if distance < min(len(word), len(best)):
     return best
 
 
 def dict_to_human(query):
-
     lst = [f"{k}={v}" for k, v in sorted(query.items())]
 
     return list_to_human(lst)
 
 
 def list_to_human(lst):
     if not lst:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/kwargs.py` & `earthkit-data-0.1.1/earthkit/data/utils/kwargs.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/lazy.py` & `earthkit-data-0.1.1/earthkit/data/utils/lazy.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
         self.args = args
         self.kwargs = kwargs
         self._source = None
         self._exception = None
 
     @property
     def source(self):
-
         if self._source is None:
             try:
                 self._source = from_source(
                     self.name,
                     lazily=False,
                     *self.args,
                     **self.kwargs,
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/parts.py` & `earthkit-data-0.1.1/earthkit/data/utils/parts.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/patterns.py` & `earthkit-data-0.1.1/earthkit/data/utils/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
         return self.format % value
 
 
 TYPES = {"": Any, "int": Int, "float": Float, "date": Datetime, "enum": Enum}
 
 
 class Constant:
-
     name = None
 
     def __init__(self, value):
         self.value = value
 
     def substitute(self, params):
         return self.value
@@ -156,15 +155,14 @@
             result.append(p.substitute(params))
         if used and not self.ignore_missing_keys:
             raise ValueError("Unused parameter(s): {}".format(used))
 
         return "".join(str(x) for x in result)
 
     def _substitute_many(self, params):
-
         for k, v in list(params.items()):
             if not isinstance(v, list):
                 params[k] = [v]
 
         seen = set()
         result = []
         for n in (
```

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/serialise.py` & `earthkit-data-0.1.1/earthkit/data/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/utils/summary.py` & `earthkit-data-0.1.1/earthkit/data/utils/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 def make_unique(x, full=False):
     v = set(x)
     r = [str(t) for t in v]
     return format_list(r, full=full)
 
 
 def ls(metadata_proc, default_keys, n=None, keys=None, extra_keys=None, **kwargs):
-
     do_print = kwargs.pop("print", False)
 
     if kwargs:
         raise ValueError(f"ls: unsupported arguments={kwargs}")
 
     _keys = {}
     if isinstance(default_keys, (list, tuple)):
@@ -139,15 +138,14 @@
         return df
     elif do_print:
         print(df)
     return df
 
 
 def format_info(data, selected=None, details=None, **kwargs):
-
     do_print = kwargs.pop("print", True)
     html = kwargs.pop("html", True)
     raw = kwargs.pop("_as_raw", False)
 
     rv = {item["title"]: item["data"] for item in data}
 
     if ipython_active:
```

### Comparing `earthkit-data-0.1.0/earthkit/data/vocabularies/__init__.py` & `earthkit-data-0.1.1/earthkit/data/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/vocabularies/aliases.py` & `earthkit-data-0.1.1/earthkit/data/vocabularies/aliases.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/vocabularies/cf.py` & `earthkit-data-0.1.1/earthkit/data/vocabularies/cf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,9 @@
     xmldoc = minidom.parse(path)
     entries = xmldoc.getElementsByTagName("entry")
     for entry in entries:
         yield entry.attributes["id"].value
 
 
 if __name__ == "__main__":
-
     for n in cf_standard_names():
         print(n)
```

### Comparing `earthkit-data-0.1.0/earthkit/data/vocabularies/grib-paramid.csv` & `earthkit-data-0.1.1/earthkit/data/vocabularies/grib-paramid.csv`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/vocabularies/grib.py` & `earthkit-data-0.1.1/earthkit/data/vocabularies/grib.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,12 +35,11 @@
 
 def param_id_to_short_name(param_id):
     entry = param_id_to_dict(param_id)
     return entry["param_shortName"]
 
 
 if __name__ == "__main__":
-
     import sys
 
     for i in sys.argv[1:]:
         print(param_id_to_short_name(int(i)))
```

### Comparing `earthkit-data-0.1.0/earthkit/data/wrappers/__init__.py` & `earthkit-data-0.1.1/earthkit/data/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/earthkit/data/wrappers/string.py` & `earthkit-data-0.1.1/earthkit/data/wrappers/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from earthkit.data.wrappers import Wrapper
 
 VALID_DATE = re.compile(r"\d\d\d\d-?\d\d-?\d\d([T\s]\d\d:\d\d(:\d\d)?)?Z?")
 
 
 def parse_date(dt):
-
     if not VALID_DATE.match(dt):
         raise ValueError(f"Invalid datetime '{dt}'")
 
     try:
         return datetime.datetime.fromisoformat(dt)
     except Exception:
         pass
```

### Comparing `earthkit-data-0.1.0/earthkit_data.egg-info/PKG-INFO` & `earthkit-data-0.1.1/earthkit_data.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: A format-agnostic Python interface for geospatial data
 License: Apache License 2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -14,37 +14,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # earthkit-data
 
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/earthkit-data.svg)](https://pypi.python.org/pypi/earthkit-data/)
+
 A format-agnostic interface for geospatial data with a focus on meteorology and
 climate science.
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
 
-**earthkit-data** makes it simple to read, inspect and slice data from a wide range of
-geospatial input types (GRIB, netCDF, zarr and more) and transform them into
-familiar scientific Python objects (including numpy arrays, pandas dataframes,
-xarray datasets).
-
-```
-data = earthkit.data.from_source("my-data.nc")
-arr = data.to_numpy()
-df = data.to_pandas()
-dataset = data.to_xarray()
-```
-
-**earthkit-data** provides additional convenient methods for quickly inspecting certain
-features of your input data, such as data dimensionality, axes, coordinate
-reference systems and bounding boxes.
+The documentation can be found at https://earthkit-data.readthedocs.io/.
 
 ## License
 
 ```
 Copyright 2022, European Centre for Medium Range Weather Forecasts.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -54,8 +42,12 @@
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
+
+In applying this licence, ECMWF does not waive the privileges and immunities
+granted to it by virtue of its status as an intergovernmental organisation
+nor does it submit to any jurisdiction.
 ```
```

### Comparing `earthkit-data-0.1.0/earthkit_data.egg-info/SOURCES.txt` & `earthkit-data-0.1.1/earthkit_data.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yml
 LICENSE
 Makefile
 README.md
 environment.yml
 pyproject.toml
 pytest.ini
 setup.cfg
-.github/workflows/on-push.yml
+.github/workflows/ci.yml
+.github/workflows/label-public-pr.yml
+.github/workflows/notify_new_issue.yml
+.github/workflows/notify_new_pr.yml
 docs/Makefile
 docs/conf.py
-docs/index.md
+docs/contributing.rst
+docs/examples.rst
+docs/index.rst
+docs/install.rst
+docs/licence.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/.gitkeep
+docs/_static/style.css
 docs/_templates/.gitkeep
 docs/examples/bufr.ipynb
-docs/examples/fdb_stream.ipynb
-docs/examples/grib_basics.ipynb
+docs/examples/grib_fdb_stream.ipynb
 docs/examples/grib_file_pattern.ipynb
 docs/examples/grib_from_stream.ipynb
 docs/examples/grib_indexing.ipynb
 docs/examples/grib_metadata.ipynb
 docs/examples/grib_missing.ipynb
 docs/examples/grib_multi.ipynb
+docs/examples/grib_overview.ipynb
 docs/examples/grib_selection.ipynb
 docs/examples/grib_tar.ipynb
 docs/examples/grib_to_netcdf.ipynb
 docs/examples/grib_url.ipynb
 docs/examples/list_of_dict.ipynb
 docs/examples/missing.grib
 docs/examples/netcdf.ipynb
@@ -45,17 +54,20 @@
 earthkit/data/arguments/args_kwargs.py
 earthkit/data/arguments/argument.py
 earthkit/data/arguments/earthkit_types.py
 earthkit/data/arguments/input_manager.py
 earthkit/data/arguments/transformers.py
 earthkit/data/core/__init__.py
 earthkit/data/core/caching.py
+earthkit/data/core/constants.py
 earthkit/data/core/index.py
 earthkit/data/core/ipython.py
+earthkit/data/core/order.py
 earthkit/data/core/plugins.py
+earthkit/data/core/select.py
 earthkit/data/core/settings.py
 earthkit/data/core/statistics.py
 earthkit/data/core/temporary.py
 earthkit/data/core/thread.py
 earthkit/data/data/css/tab.css
 earthkit/data/data/css/table.css
 earthkit/data/indexing/__init__.py
@@ -79,20 +91,24 @@
 earthkit/data/readers/tar.py
 earthkit/data/readers/text.py
 earthkit/data/readers/unknown.py
 earthkit/data/readers/zip.py
 earthkit/data/readers/grib/__init__.py
 earthkit/data/readers/grib/codes.py
 earthkit/data/readers/grib/fieldset.py
-earthkit/data/readers/grib/index.py
 earthkit/data/readers/grib/memory.py
 earthkit/data/readers/grib/pandas.py
 earthkit/data/readers/grib/parsing.py
 earthkit/data/readers/grib/reader.py
 earthkit/data/readers/grib/xarray.py
+earthkit/data/readers/grib/index/__init__.py
+earthkit/data/readers/grib/index/db.py
+earthkit/data/readers/grib/index/file.py
+earthkit/data/readers/grib/index/json.py
+earthkit/data/readers/grib/index/sql.py
 earthkit/data/sources/__init__.py
 earthkit/data/sources/dummy.grib
 earthkit/data/sources/dummy_source.py
 earthkit/data/sources/empty.py
 earthkit/data/sources/fdb.py
 earthkit/data/sources/file.py
 earthkit/data/sources/file_indexed.py
@@ -138,30 +154,35 @@
 tests/core/test_cache.py
 tests/core/test_version.py
 tests/data/mercator.grib
 tests/data/ml_data.grib
 tests/data/rgg_small_subarea_cellarea_ref.grib
 tests/data/t_pl.grib
 tests/data/t_time_series.grib
+tests/data/test_icon.grib
 tests/data/test_single.grib
 tests/data/test_single.nc
 tests/data/test_single_with_missing.grib
 tests/data/u_pl.grib
 tests/data/v_pl.grib
 tests/documentation/test_examples.py
 tests/documentation/test_notebooks.py
 tests/grib/test_grib_contents.py
+tests/grib/test_grib_convert.py
+tests/grib/test_grib_order_by.py
 tests/grib/test_grib_sel.py
 tests/grib/test_grib_slice.py
 tests/grib/test_grib_summary.py
 tests/indexing/indexing_fixtures.py
+tests/indexing/test_indexing_db.py
 tests/indexing/test_indexing_isel.py
-tests/indexing/test_indexing_multi_file.py
 tests/indexing/test_indexing_order_by.py
 tests/indexing/test_indexing_serialisation.py
+tests/indexing/test_order_kwargs.py
+tests/indexing/test_selection_kwargs.py
 tests/readers/test_csv_reader.py
 tests/readers/test_grib_reader.py
 tests/readers/test_netcdf_reader.py
 tests/readers/test_tar_reader.py
 tests/readers/test_unknown_reader.py
 tests/readers/test_zip_reader.py
 tests/readers/unknown_file.unknown_ext
```

### Comparing `earthkit-data-0.1.0/setup.cfg` & `earthkit-data-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/bufr/test_bufr_summary.py` & `earthkit-data-0.1.1/tests/bufr/test_bufr_summary.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/core/test_cache.py` & `earthkit-data-0.1.1/tests/core/test_cache.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/core/test_version.py` & `earthkit-data-0.1.1/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/mercator.grib` & `earthkit-data-0.1.1/tests/data/mercator.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/ml_data.grib` & `earthkit-data-0.1.1/tests/data/ml_data.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/rgg_small_subarea_cellarea_ref.grib` & `earthkit-data-0.1.1/tests/data/rgg_small_subarea_cellarea_ref.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/t_pl.grib` & `earthkit-data-0.1.1/tests/data/t_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/t_time_series.grib` & `earthkit-data-0.1.1/tests/data/t_time_series.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/test_single.nc` & `earthkit-data-0.1.1/tests/data/test_single.nc`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/u_pl.grib` & `earthkit-data-0.1.1/tests/data/u_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/data/v_pl.grib` & `earthkit-data-0.1.1/tests/data/v_pl.grib`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/documentation/test_examples.py` & `earthkit-data-0.1.1/tests/documentation/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,30 +23,28 @@
     "settings-2-set.py",
 ]
 
 EXAMPLES = earthkit_file("docs")
 
 
 def example_list():
-
     examples = []
     for root, _, files in os.walk(EXAMPLES):
         for file in files:
             path = os.path.join(root, file)
             if path.endswith(".py") and file not in IGNORE:
                 n = len(EXAMPLES) + 1
                 examples.append(path[n:])
 
     return sorted(examples)
 
 
 # @pytest.mark.skipif(not IN_GITHUB, reason="Not on GITHUB")
 @pytest.mark.parametrize("path", example_list())
 def test_example(path):
-
     full = os.path.join(EXAMPLES, path)
     with open(full) as f:
         exec(f.read(), dict(__file__=full), {})
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
```

### Comparing `earthkit-data-0.1.0/tests/documentation/test_notebooks.py` & `earthkit-data-0.1.1/tests/documentation/test_notebooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 from earthkit.data.testing import MISSING, earthkit_file
 
 # See https://www.blog.pythonlibrary.org/2018/10/16/testing-jupyter-notebooks/
 
 
 EXAMPLES = earthkit_file("docs", "examples")
 
-SKIP = "fdb_stream.ipynb"
+SKIP = "grib_fdb_stream.ipynb"
 
 
 def notebooks_list():
-
     notebooks = []
     for path in os.listdir(EXAMPLES):
         if re.match(r".+\.ipynb$", path):
             # if re.match(r"^\d\d-.*\.ipynb$", path):
             if "Copy" not in path:
                 notebooks.append(path)
```

### Comparing `earthkit-data-0.1.0/tests/grib/test_grib_contents.py` & `earthkit-data-0.1.1/tests/grib/test_grib_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -597,15 +597,14 @@
     # y
     assert v["lat"].shape == (7, 12)
     for i, y in enumerate(v["lat"]):
         assert np.allclose(y, np.ones(12) * (90 - i * 30))
 
 
 def test_grib_datetime():
-
     s = from_source("file", earthkit_examples_file("test.grib"))
 
     ref = {
         "base_time": [datetime.datetime(2020, 5, 13, 12)],
         "valid_time": [datetime.datetime(2020, 5, 13, 12)],
     }
     assert s.datetime() == ref
@@ -767,47 +766,11 @@
         assert len(fs) == 6
         with temp_file() as tmp:
             fs.save(tmp)
             fs_saved = from_source("file", tmp)
             assert len(fs) == len(fs_saved)
 
 
-def test_grib_to_pandas():
-    f = from_source("file", earthkit_test_data_file("test_single.grib"))
-
-    # all points
-    df = f.to_pandas()
-    assert len(df) == 84
-    cols = [
-        "lat",
-        "lon",
-        "value",
-        "datetime",
-        "domain",
-        "levtype",
-        "date",
-        "time",
-        "step",
-        "param",
-        "class",
-        "type",
-        "stream",
-        "expver",
-    ]
-    assert list(df.columns) == cols
-    assert np.allclose(df["lat"][0:2], [90, 90])
-    assert np.allclose(df["lon"][0:2], [0, 30])
-    assert np.allclose(df["value"][0:2], [260.435608, 260.435608])
-
-    # specific location
-    df = f.to_pandas(latitude=90, longitude=30)
-    assert len(df) == 1
-    assert list(df.columns) == cols
-    assert np.isclose(df["lat"][0], 90)
-    assert np.isclose(df["lon"][0], 30)
-    assert np.isclose(df["value"][0], 260.435608)
-
-
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit-data-0.1.0/tests/grib/test_grib_sel.py` & `earthkit-data-0.1.1/tests/grib/test_grib_sel.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             keys = metadata_keys
 
         assert g.metadata(keys) == expected_meta
     return
 
 
 def test_grib_sel_single_file_2():
-
     f = from_source("file", earthkit_file("tests/data/t_time_series.grib"))
 
     g = f.sel(shortName=["t"], step=[3, 6])
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "step:l"]) == [
         ("t", 1000, 3),
         ("t", 1000, 6),
@@ -169,16 +168,16 @@
     assert len(r) == 1
     assert r[0].metadata("shortName") == "2t"
 
 
 @pytest.mark.parametrize(
     "params,expected_meta,metadata_keys",
     [
-        (dict(shortName=1, level=2), [("u", 700)], []),
-        (dict(paramId=1, level=2), [(131, 700)], []),
+        (dict(shortName=1, level=2), [("u", 500)], []),
+        (dict(paramId=1, level=2), [(131, 500)], []),
         (
             dict(shortName=[0, 1], level=[2, 3]),
             [
                 ("t", 700),
                 ("u", 700),
                 ("t", 500),
                 ("u", 500),
@@ -194,17 +193,17 @@
                 ("t", 500, "an"),
             ],
             ["shortName", "level:l", "marsType"],
         ),
         (
             dict(level=-1),
             [
-                ("t", 300),
-                ("u", 300),
-                ("v", 300),
+                ("t", 1000),
+                ("u", 1000),
+                ("v", 1000),
             ],
             ["shortName", "level:l"],
         ),
     ],
 )
 def test_grib_isel_single_file(params, expected_meta, metadata_keys):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
@@ -213,26 +212,25 @@
     assert len(g) == len(expected_meta)
     if len(expected_meta) > 0:
         keys = list(params.keys())
         if metadata_keys:
             keys = metadata_keys
 
         assert g.metadata(keys) == expected_meta
-    return
 
 
 @pytest.mark.parametrize(
     "param_id,level,expected_meta",
     [
-        (1, (slice(2)), [(131, 1000), (131, 850)]),
-        (1, (slice(None, 2)), [(131, 1000), (131, 850)]),
-        (1, (slice(2, 3)), [(131, 700)]),
+        (1, (slice(2)), [(131, 400), (131, 300)]),
+        (1, (slice(None, 2)), [(131, 400), (131, 300)]),
+        (1, (slice(2, 3)), [(131, 500)]),
         (1, (slice(2, 4)), [(131, 700), (131, 500)]),
-        (1, (slice(4, None)), [(131, 400), (131, 300)]),
-        (1, (slice(None, None, 2)), [(131, 1000), (131, 700), (131, 400)]),
+        (1, (slice(4, None)), [(131, 1000), (131, 850)]),
+        (1, (slice(None, None, 2)), [(131, 850), (131, 500), (131, 300)]),
     ],
 )
 def test_grib_isel_slice_single_file(param_id, level, expected_meta):
     f = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
 
     g = f.isel(paramId=param_id, level=level)
     assert len(g) == len(expected_meta)
@@ -252,33 +250,33 @@
 
 def test_grib_isel_multi_file():
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
     # single resulting field
-    g = f.isel(shortName=0, level=21)
+    g = f.isel(shortName=1, level=21)
     assert len(g) == 1
-    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [("t", 61, "hybrid")]
+    assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [("t", 85, "hybrid")]
 
-    g1 = f[34]
+    g1 = f[40]
     d = g.to_numpy() - g1.to_numpy()
     assert np.allclose(d, np.zeros(len(d)))
 
 
 def test_grib_isel_slice_multi_file():
     f1 = from_source("file", earthkit_file("docs/examples/tuv_pl.grib"))
     f2 = from_source("file", earthkit_file("tests/data/ml_data.grib"))
     f = from_source("multi", [f1, f2])
 
-    g = f.isel(shortName=0, level=slice(20, 22))
+    g = f.isel(shortName=1, level=slice(20, 22))
     assert len(g) == 2
     assert g.metadata(["shortName", "level:l", "typeOfLevel"]) == [
-        ("t", 57, "hybrid"),
-        ("t", 61, "hybrid"),
+        ("t", 81, "hybrid"),
+        ("t", 85, "hybrid"),
     ]
 
 
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     main()
```

### Comparing `earthkit-data-0.1.0/tests/grib/test_grib_slice.py` & `earthkit-data-0.1.1/tests/grib/test_grib_slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,28 @@
     # v = r.values
     # assert v.shape == (3, 84)
     # check the original fieldset
     assert len(f) == 6
     assert f.metadata("shortName") == ["2t", "msl", "t", "z", "t", "z"]
 
 
-@pytest.mark.parametrize("indexes", [(np.array([1, 16, 5, 9])), ([1, 16, 5, 9])])
-def test_grib_array_indexing(indexes):
+@pytest.mark.parametrize(
+    "indexes1,indexes2",
+    [(np.array([1, 16, 5, 9]), np.array([1, 3])), ([1, 16, 5, 9], [1, 3])],
+)
+def test_grib_array_indexing(indexes1, indexes2):
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
-    r = f[indexes]
+    r = f[indexes1]
     assert len(r) == 4
     assert r.metadata("shortName") == ["u", "u", "v", "t"]
 
+    r1 = r[indexes2]
+    assert len(r1) == 2
+    assert r1.metadata("shortName") == ["u", "t"]
+
 
 @pytest.mark.parametrize("indexes", [(np.array([1, 19, 5, 9])), ([1, 19, 5, 9])])
 def test_grib_array_indexing_bad(indexes):
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
     with pytest.raises(IndexError):
         f[indexes]
```

### Comparing `earthkit-data-0.1.0/tests/grib/test_grib_summary.py` & `earthkit-data-0.1.1/tests/grib/test_grib_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.testing import earthkit_examples_file
 
 
 def test_grib_describe():
-
     f = from_source("file", earthkit_examples_file("tuv_pl.grib"))
 
     # full contents
     df = f.describe(print=False)
     df = df.data
 
     ref = {
```

### Comparing `earthkit-data-0.1.0/tests/readers/test_csv_reader.py` & `earthkit-data-0.1.1/tests/readers/test_csv_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     )
 
     print(s.to_pandas())
 
 
 @pytest.mark.skipif(True, reason="Test not yet implemented")
 def test_csv_icoads():
-
     r = {
         "class": "e2",
         "date": "1662-10-01/to/1663-12-31",
         "dataset": "icoads",
         "expver": "1608",
         "groupid": "17",
         "reportype": "16008",
@@ -94,15 +93,14 @@
     }
 
     source = cml.from_source("mars", **r)
     print(source)
 
 
 def test_csv_text():
-
     s = cml.from_source(
         "dummy-source",
         "csv",
         headers=["a", "b", "c"],
         quote_strings=True,
         lines=[
             [1, "x", 3],
```

### Comparing `earthkit-data-0.1.0/tests/readers/test_grib_reader.py` & `earthkit-data-0.1.1/tests/readers/test_grib_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/readers/test_netcdf_reader.py` & `earthkit-data-0.1.1/tests/readers/test_netcdf_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
 import datetime
 import os
+import tempfile
 
 import numpy as np
 import pytest
 
 from earthkit.data import from_source
 from earthkit.data.readers.netcdf import NetCDFField
 from earthkit.data.testing import (
@@ -211,12 +212,34 @@
     assert (
         r[0]
         == "+proj=laea +lat_0=52 +lon_0=10 +x_0=4321000 +y_0=3210000 +ellps=GRS80 +units=m +no_defs"
     )
     assert r[1] == "+proj=eqc +datum=WGS84 +units=m +no_defs"
 
 
+def test_get_fields_missing_standard_name_attr_in_coord_array():
+    """test _get_fields() can handle a missing 'standard_name' attr in coordinate data arrays"""
+
+    # example dataset
+    fs = from_source("file", earthkit_examples_file("test.nc"))
+    ds = fs.to_xarray()
+
+    # delete 'standard_name' attribute (if exists) in any coordinate data arrays
+    for coord_name in ds.coords:
+        try:
+            del ds.coords[coord_name].attrs["standard_name"]
+        except Exception as e:
+            print(e)
+
+    # save updates to disk and try read that file source
+    with tempfile.TemporaryDirectory() as tmp_dir:
+        fpath = os.path.join(tmp_dir, "tmp.nc")
+        ds.to_netcdf(fpath)
+        fs = from_source("file", earthkit_test_data_file(fpath))
+        assert len(fs) == 2
+
+
 if __name__ == "__main__":
     from earthkit.data.testing import main
 
     # test_datetime()
     main(__file__)
```

### Comparing `earthkit-data-0.1.0/tests/readers/test_tar_reader.py` & `earthkit-data-0.1.1/tests/readers/test_tar_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/readers/test_unknown_reader.py` & `earthkit-data-0.1.1/tests/readers/test_unknown_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/readers/test_zip_reader.py` & `earthkit-data-0.1.1/tests/readers/test_zip_reader.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/sources/test_file.py` & `earthkit-data-0.1.1/tests/sources/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,18 @@
 from earthkit.data.testing import earthkit_file
 
 LOG = logging.getLogger(__name__)
 
 
 @pytest.mark.long_test
 def test_file_source_grib():
-
     s = from_source("file", earthkit_file("docs/examples/test.grib"))
     from earthkit.data.readers.grib.reader import GRIBReader
 
-    assert isinstance(s._reader, GRIBReader), s
+    assert isinstance(s, GRIBReader), s
     assert len(s) == 2
 
 
 def test_file_source_netcdf():
     s = from_source("file", earthkit_file("docs/examples/test.nc"))
     assert len(s) == 2
```

### Comparing `earthkit-data-0.1.0/tests/sources/test_multi.py` & `earthkit-data-0.1.1/tests/sources/test_multi.py`

 * *Files identical despite different names*

### Comparing `earthkit-data-0.1.0/tests/sources/test_url.py` & `earthkit-data-0.1.1/tests/sources/test_url.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
         "url",
         "https://get.ecmwf.int/repository/test-data/emohawk/examples/test_gribs.tar",
     )
     assert len(ds) == 6
 
 
 def test_part_url():
-
     ds = from_source(
         "url",
         "https://get.ecmwf.int/repository/test-data/emohawk/test-data/temp.bufr",
     )
 
     ds = from_source(
         "url",
```

### Comparing `earthkit-data-0.1.0/tests/sources/test_url_pattern.py` & `earthkit-data-0.1.1/tests/sources/test_url_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,26 +20,24 @@
         "https://get.ecmwf.int/repository/test-data/emohawk/examples/test.{format}",
         {"format": ["nc", "grib"]},
     )
     # source.to_xarray()
 
 
 def test_url_pattern_int():
-
     fs = from_source(
         "url-pattern",
         "https://get.ecmwf.int/repository/test-data/emohawk/examples/test{id}.grib",
         {"id": [4, 6]},
     )
 
     assert len(fs) == 10
 
 
 def test_url_pattern_date():
-
     fs = from_source(
         "url-pattern",
         "https://get.ecmwf.int/repository/test-data/emohawk/test-data/"
         "test_{my_date:date(%Y-%m-%d)}_{name}.grib",
         {"my_date": datetime.datetime(2020, 5, 13), "name": ["t2", "msl"]},
     )
```

