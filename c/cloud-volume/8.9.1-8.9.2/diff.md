# Comparing `tmp/cloud-volume-8.9.1.tar.gz` & `tmp/cloud-volume-8.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-volume-8.9.1.tar", last modified: Thu Aug 18 21:51:11 2022, max compression
+gzip compressed data, was "cloud-volume-8.9.2.tar", last modified: Tue Sep  6 22:03:19 2022, max compression
```

## Comparing `cloud-volume-8.9.1.tar` & `cloud-volume-8.9.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.589029 cloud-volume-8.9.1/
--rw-r--r--   0 wms        (501) staff       (20)      423 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     1558 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       25 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)    47002 2022-08-18 21:51:11.588800 cloud-volume-8.9.1/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    40821 2022-08-04 21:36:58.000000 cloud-volume-8.9.1/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.561480 cloud-volume-8.9.1/cloud_volume.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    47002 2022-08-18 21:51:11.000000 cloud-volume-8.9.1/cloud_volume.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     3106 2022-08-18 21:51:11.000000 cloud-volume-8.9.1/cloud_volume.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2022-08-18 21:51:11.000000 cloud-volume-8.9.1/cloud_volume.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)      752 2022-08-18 21:51:11.000000 cloud-volume-8.9.1/cloud_volume.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       12 2022-08-18 21:51:11.000000 cloud-volume-8.9.1/cloud_volume.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.567954 cloud-volume-8.9.1/cloudvolume/
--rw-r--r--   0 wms        (501) staff       (20)     2938 2022-08-18 21:51:01.000000 cloud-volume-8.9.1/cloudvolume/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    17118 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/cacheservice.py
--rw-r--r--   0 wms        (501) staff       (20)    10905 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/cloudvolume/chunks.py
--rw-r--r--   0 wms        (501) staff       (20)    13015 2022-07-14 18:33:05.000000 cloud-volume-8.9.1/cloudvolume/cloudvolume.py
--rw-r--r--   0 wms        (501) staff       (20)       36 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/cloudvolume/compression.py
--rw-r--r--   0 wms        (501) staff       (20)     3525 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/connectionpools.py
--rw-r--r--   0 wms        (501) staff       (20)     5727 2021-08-19 18:41:54.000000 cloud-volume-8.9.1/cloudvolume/dask.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.568208 cloud-volume-8.9.1/cloudvolume/datasource/
--rw-r--r--   0 wms        (501) staff       (20)     3519 2022-08-18 21:43:40.000000 cloud-volume-8.9.1/cloudvolume/datasource/__init__.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.569053 cloud-volume-8.9.1/cloudvolume/datasource/boss/
--rw-r--r--   0 wms        (501) staff       (20)     1434 2021-07-02 00:29:28.000000 cloud-volume-8.9.1/cloudvolume/datasource/boss/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     4394 2022-08-04 21:34:36.000000 cloud-volume-8.9.1/cloudvolume/datasource/boss/image.py
--rw-r--r--   0 wms        (501) staff       (20)     2379 2021-05-13 23:31:42.000000 cloud-volume-8.9.1/cloudvolume/datasource/boss/metadata.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.569872 cloud-volume-8.9.1/cloudvolume/datasource/graphene/
--rw-r--r--   0 wms        (501) staff       (20)     2929 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/__init__.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.570973 cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/
--rw-r--r--   0 wms        (501) staff       (20)     1244 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)      189 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/metadata.py
--rw-r--r--   0 wms        (501) staff       (20)    11156 2022-05-24 23:35:13.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/sharded.py
--rw-r--r--   0 wms        (501) staff       (20)     9158 2021-08-09 21:54:31.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/unsharded.py
--rw-r--r--   0 wms        (501) staff       (20)    13984 2022-02-08 18:06:56.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/metadata.py
--rw-r--r--   0 wms        (501) staff       (20)      415 2021-02-04 04:10:15.000000 cloud-volume-8.9.1/cloudvolume/datasource/graphene/sharding.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.571814 cloud-volume-8.9.1/cloudvolume/datasource/n5/
--rw-r--r--   0 wms        (501) staff       (20)     1737 2022-08-04 21:34:36.000000 cloud-volume-8.9.1/cloudvolume/datasource/n5/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     4502 2022-08-04 21:34:36.000000 cloud-volume-8.9.1/cloudvolume/datasource/n5/image.py
--rw-r--r--   0 wms        (501) staff       (20)     2342 2022-08-04 21:34:36.000000 cloud-volume-8.9.1/cloudvolume/datasource/n5/metadata.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.573403 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/
--rw-r--r--   0 wms        (501) staff       (20)     3439 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     1270 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/common.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.574820 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/
--rw-r--r--   0 wms        (501) staff       (20)    19768 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     6497 2022-07-14 22:25:50.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/common.py
--rw-r--r--   0 wms        (501) staff       (20)    24044 2022-05-25 15:58:55.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/rx.py
--rw-r--r--   0 wms        (501) staff       (20)    11897 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/tx.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.576040 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/
--rw-r--r--   0 wms        (501) staff       (20)     1915 2021-10-26 01:40:21.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)      474 2021-07-01 03:46:14.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/common.py
--rw-r--r--   0 wms        (501) staff       (20)     2457 2022-01-03 22:40:19.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/metadata.py
--rw-r--r--   0 wms        (501) staff       (20)    16199 2022-05-24 23:35:13.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/multilod.py
--rw-r--r--   0 wms        (501) staff       (20)     7316 2022-04-20 04:34:25.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/unsharded.py
--rw-r--r--   0 wms        (501) staff       (20)    24305 2022-08-18 21:50:08.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/metadata.py
--rw-r--r--   0 wms        (501) staff       (20)    14165 2021-11-11 04:03:30.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mmh3.py
--rw-r--r--   0 wms        (501) staff       (20)    27172 2022-05-25 15:58:55.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/sharding.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.577119 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/
--rw-r--r--   0 wms        (501) staff       (20)     1349 2021-10-26 01:40:21.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     2963 2022-02-23 06:56:57.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/metadata.py
--rw-r--r--   0 wms        (501) staff       (20)     2228 2021-10-18 21:22:19.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/sharded.py
--rw-r--r--   0 wms        (501) staff       (20)     3722 2022-05-24 23:35:13.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/unsharded.py
--rw-r--r--   0 wms        (501) staff       (20)    16409 2022-06-05 07:57:22.000000 cloud-volume-8.9.1/cloudvolume/datasource/precomputed/spatial_index.py
--rw-r--r--   0 wms        (501) staff       (20)     3431 2022-03-01 21:03:42.000000 cloud-volume-8.9.1/cloudvolume/exceptions.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.578027 cloud-volume-8.9.1/cloudvolume/frontends/
--rw-r--r--   0 wms        (501) staff       (20)       89 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/frontends/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    24339 2022-05-25 15:58:55.000000 cloud-volume-8.9.1/cloudvolume/frontends/graphene.py
--rw-r--r--   0 wms        (501) staff       (20)    33042 2022-08-10 00:36:35.000000 cloud-volume-8.9.1/cloudvolume/frontends/precomputed.py
--rw-r--r--   0 wms        (501) staff       (20)    27739 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/lib.py
--rw-r--r--   0 wms        (501) staff       (20)     7637 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/lru.py
--rw-r--r--   0 wms        (501) staff       (20)    14285 2022-05-12 02:08:16.000000 cloud-volume-8.9.1/cloudvolume/mesh.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.580818 cloud-volume-8.9.1/cloudvolume/microviewer/
--rw-r--r--   0 wms        (501) staff       (20)     5524 2021-11-11 04:03:30.000000 cloud-volume-8.9.1/cloudvolume/microviewer/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    34643 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/cloudvolume/microviewer/datacube.js
--rw-r--r--   0 wms        (501) staff       (20)     1911 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/microviewer/favicon.ico
--rw-r--r--   0 wms        (501) staff       (20)    17074 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/cloudvolume/microviewer/index.html
--rw-r--r--   0 wms        (501) staff       (20)    86926 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/microviewer/jquery-3.3.1.js
--rw-r--r--   0 wms        (501) staff       (20)     5640 2022-08-04 21:34:36.000000 cloud-volume-8.9.1/cloudvolume/paths.py
--rw-r--r--   0 wms        (501) staff       (20)     3799 2021-02-11 23:00:42.000000 cloud-volume-8.9.1/cloudvolume/provenance.py
--rw-r--r--   0 wms        (501) staff       (20)    10721 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/py_compressed_segmentation.py
--rw-r--r--   0 wms        (501) staff       (20)     2639 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/scheduler.py
--rw-r--r--   0 wms        (501) staff       (20)     6070 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/secrets.py
--rw-r--r--   0 wms        (501) staff       (20)     2463 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/server.py
--rw-r--r--   0 wms        (501) staff       (20)     6708 2021-07-21 05:29:44.000000 cloud-volume-8.9.1/cloudvolume/sharedmemory.py
--rw-r--r--   0 wms        (501) staff       (20)    33156 2022-08-18 21:49:59.000000 cloud-volume-8.9.1/cloudvolume/skeleton.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.582189 cloud-volume-8.9.1/cloudvolume/storage/
--rw-r--r--   0 wms        (501) staff       (20)      908 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/cloudvolume/storage/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    20968 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/cloudvolume/storage/storage.py
--rw-r--r--   0 wms        (501) staff       (20)    15097 2021-07-21 05:29:44.000000 cloud-volume-8.9.1/cloudvolume/storage/storage_interfaces.py
--rw-r--r--   0 wms        (501) staff       (20)     7173 2022-02-11 05:36:41.000000 cloud-volume-8.9.1/cloudvolume/threaded_queue.py
--rw-r--r--   0 wms        (501) staff       (20)      175 2022-03-01 22:13:19.000000 cloud-volume-8.9.1/cloudvolume/types.py
--rw-r--r--   0 wms        (501) staff       (20)     3349 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/cloudvolume/volumecutout.py
--rw-r--r--   0 wms        (501) staff       (20)      506 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/requirements.txt
--rw-r--r--   0 wms        (501) staff       (20)       38 2022-08-18 21:51:11.589098 cloud-volume-8.9.1/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     2408 2022-08-18 21:51:01.000000 cloud-volume-8.9.1/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-08-18 21:51:11.588183 cloud-volume-8.9.1/test/
--rw-r--r--   0 wms        (501) staff       (20)     4805 2022-05-10 21:12:56.000000 cloud-volume-8.9.1/test/test_chunks.py
--rw-r--r--   0 wms        (501) staff       (20)    49288 2022-08-04 21:34:38.000000 cloud-volume-8.9.1/test/test_cloudvolume.py
--rw-r--r--   0 wms        (501) staff       (20)     1759 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/test/test_connectionpools.py
--rw-r--r--   0 wms        (501) staff       (20)     3441 2021-08-19 18:41:54.000000 cloud-volume-8.9.1/test/test_dask.py
--rw-r--r--   0 wms        (501) staff       (20)    15455 2022-05-10 21:12:57.000000 cloud-volume-8.9.1/test/test_graphene.py
--rw-r--r--   0 wms        (501) staff       (20)     7282 2021-07-21 05:29:44.000000 cloud-volume-8.9.1/test/test_lib.py
--rw-r--r--   0 wms        (501) staff       (20)     1500 2022-05-10 21:12:57.000000 cloud-volume-8.9.1/test/test_lru.py
--rw-r--r--   0 wms        (501) staff       (20)     5811 2022-03-02 05:51:29.000000 cloud-volume-8.9.1/test/test_meshing.py
--rw-r--r--   0 wms        (501) staff       (20)     5777 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/test/test_paths.py
--rw-r--r--   0 wms        (501) staff       (20)     1674 2021-07-01 19:28:07.000000 cloud-volume-8.9.1/test/test_precomputed_multilod.py
--rw-r--r--   0 wms        (501) staff       (20)     3204 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/test/test_provenance.py
--rw-r--r--   0 wms        (501) staff       (20)     6214 2021-07-01 19:28:05.000000 cloud-volume-8.9.1/test/test_sharding.py
--rw-r--r--   0 wms        (501) staff       (20)     3099 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/test/test_sharedmemory.py
--rw-r--r--   0 wms        (501) staff       (20)    19866 2021-12-27 22:30:59.000000 cloud-volume-8.9.1/test/test_skeletons.py
--rw-r--r--   0 wms        (501) staff       (20)     9576 2021-06-11 02:56:35.000000 cloud-volume-8.9.1/test/test_storage.py
--rw-r--r--   0 wms        (501) staff       (20)     2092 2021-01-11 02:21:16.000000 cloud-volume-8.9.1/test/test_threadedqueue.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.991366 cloud-volume-8.9.2/
+-rw-r--r--   0 wms        (501) staff       (20)      423 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     1558 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       25 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)    47002 2022-09-06 22:03:19.991187 cloud-volume-8.9.2/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    40821 2022-08-04 21:36:58.000000 cloud-volume-8.9.2/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.965472 cloud-volume-8.9.2/cloud_volume.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    47002 2022-09-06 22:03:19.000000 cloud-volume-8.9.2/cloud_volume.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     3106 2022-09-06 22:03:19.000000 cloud-volume-8.9.2/cloud_volume.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2022-09-06 22:03:19.000000 cloud-volume-8.9.2/cloud_volume.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)      745 2022-09-06 22:03:19.000000 cloud-volume-8.9.2/cloud_volume.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       12 2022-09-06 22:03:19.000000 cloud-volume-8.9.2/cloud_volume.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.972013 cloud-volume-8.9.2/cloudvolume/
+-rw-r--r--   0 wms        (501) staff       (20)     2938 2022-09-06 22:03:00.000000 cloud-volume-8.9.2/cloudvolume/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    17118 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/cacheservice.py
+-rw-r--r--   0 wms        (501) staff       (20)    10905 2022-08-04 21:34:38.000000 cloud-volume-8.9.2/cloudvolume/chunks.py
+-rw-r--r--   0 wms        (501) staff       (20)    13015 2022-07-14 18:33:05.000000 cloud-volume-8.9.2/cloudvolume/cloudvolume.py
+-rw-r--r--   0 wms        (501) staff       (20)       36 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/cloudvolume/compression.py
+-rw-r--r--   0 wms        (501) staff       (20)     3525 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/connectionpools.py
+-rw-r--r--   0 wms        (501) staff       (20)     5727 2021-08-19 18:41:54.000000 cloud-volume-8.9.2/cloudvolume/dask.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.972372 cloud-volume-8.9.2/cloudvolume/datasource/
+-rw-r--r--   0 wms        (501) staff       (20)     3519 2022-08-18 21:43:40.000000 cloud-volume-8.9.2/cloudvolume/datasource/__init__.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.973167 cloud-volume-8.9.2/cloudvolume/datasource/boss/
+-rw-r--r--   0 wms        (501) staff       (20)     1434 2021-07-02 00:29:28.000000 cloud-volume-8.9.2/cloudvolume/datasource/boss/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     4394 2022-08-04 21:34:36.000000 cloud-volume-8.9.2/cloudvolume/datasource/boss/image.py
+-rw-r--r--   0 wms        (501) staff       (20)     2379 2021-05-13 23:31:42.000000 cloud-volume-8.9.2/cloudvolume/datasource/boss/metadata.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.974039 cloud-volume-8.9.2/cloudvolume/datasource/graphene/
+-rw-r--r--   0 wms        (501) staff       (20)     2929 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/__init__.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.975265 cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/
+-rw-r--r--   0 wms        (501) staff       (20)     1244 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)      189 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/metadata.py
+-rw-r--r--   0 wms        (501) staff       (20)    11156 2022-05-24 23:35:13.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/sharded.py
+-rw-r--r--   0 wms        (501) staff       (20)     9158 2021-08-09 21:54:31.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/unsharded.py
+-rw-r--r--   0 wms        (501) staff       (20)    13984 2022-02-08 18:06:56.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/metadata.py
+-rw-r--r--   0 wms        (501) staff       (20)      415 2021-02-04 04:10:15.000000 cloud-volume-8.9.2/cloudvolume/datasource/graphene/sharding.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.976095 cloud-volume-8.9.2/cloudvolume/datasource/n5/
+-rw-r--r--   0 wms        (501) staff       (20)     1737 2022-08-04 21:34:36.000000 cloud-volume-8.9.2/cloudvolume/datasource/n5/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     4502 2022-08-04 21:34:36.000000 cloud-volume-8.9.2/cloudvolume/datasource/n5/image.py
+-rw-r--r--   0 wms        (501) staff       (20)     2342 2022-08-04 21:34:36.000000 cloud-volume-8.9.2/cloudvolume/datasource/n5/metadata.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.977910 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/
+-rw-r--r--   0 wms        (501) staff       (20)     3439 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     1270 2022-08-04 21:34:38.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/common.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.979160 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/
+-rw-r--r--   0 wms        (501) staff       (20)    19768 2022-08-04 21:34:38.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     6497 2022-07-14 22:25:50.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/common.py
+-rw-r--r--   0 wms        (501) staff       (20)    24044 2022-05-25 15:58:55.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/rx.py
+-rw-r--r--   0 wms        (501) staff       (20)    11897 2022-08-04 21:34:38.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/tx.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.980826 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/
+-rw-r--r--   0 wms        (501) staff       (20)     1915 2021-10-26 01:40:21.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)      474 2021-07-01 03:46:14.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/common.py
+-rw-r--r--   0 wms        (501) staff       (20)     2457 2022-01-03 22:40:19.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/metadata.py
+-rw-r--r--   0 wms        (501) staff       (20)    16199 2022-05-24 23:35:13.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/multilod.py
+-rw-r--r--   0 wms        (501) staff       (20)     7316 2022-09-02 20:38:36.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/unsharded.py
+-rw-r--r--   0 wms        (501) staff       (20)    24305 2022-08-18 21:50:08.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/metadata.py
+-rw-r--r--   0 wms        (501) staff       (20)    14165 2021-11-11 04:03:30.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mmh3.py
+-rw-r--r--   0 wms        (501) staff       (20)    27172 2022-05-25 15:58:55.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/sharding.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.981700 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/
+-rw-r--r--   0 wms        (501) staff       (20)     1349 2021-10-26 01:40:21.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     2963 2022-02-23 06:56:57.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/metadata.py
+-rw-r--r--   0 wms        (501) staff       (20)     2228 2021-10-18 21:22:19.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/sharded.py
+-rw-r--r--   0 wms        (501) staff       (20)     3722 2022-05-24 23:35:13.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/unsharded.py
+-rw-r--r--   0 wms        (501) staff       (20)    16409 2022-06-05 07:57:22.000000 cloud-volume-8.9.2/cloudvolume/datasource/precomputed/spatial_index.py
+-rw-r--r--   0 wms        (501) staff       (20)     3431 2022-03-01 21:03:42.000000 cloud-volume-8.9.2/cloudvolume/exceptions.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.982547 cloud-volume-8.9.2/cloudvolume/frontends/
+-rw-r--r--   0 wms        (501) staff       (20)       89 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/frontends/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    24339 2022-05-25 15:58:55.000000 cloud-volume-8.9.2/cloudvolume/frontends/graphene.py
+-rw-r--r--   0 wms        (501) staff       (20)    33042 2022-08-10 00:36:35.000000 cloud-volume-8.9.2/cloudvolume/frontends/precomputed.py
+-rw-r--r--   0 wms        (501) staff       (20)    27920 2022-09-06 21:57:59.000000 cloud-volume-8.9.2/cloudvolume/lib.py
+-rw-r--r--   0 wms        (501) staff       (20)     7637 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/lru.py
+-rw-r--r--   0 wms        (501) staff       (20)    14285 2022-05-12 02:08:16.000000 cloud-volume-8.9.2/cloudvolume/mesh.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.984622 cloud-volume-8.9.2/cloudvolume/microviewer/
+-rw-r--r--   0 wms        (501) staff       (20)     5524 2021-11-11 04:03:30.000000 cloud-volume-8.9.2/cloudvolume/microviewer/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    34643 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/cloudvolume/microviewer/datacube.js
+-rw-r--r--   0 wms        (501) staff       (20)     1911 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/microviewer/favicon.ico
+-rw-r--r--   0 wms        (501) staff       (20)    17074 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/cloudvolume/microviewer/index.html
+-rw-r--r--   0 wms        (501) staff       (20)    86926 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/microviewer/jquery-3.3.1.js
+-rw-r--r--   0 wms        (501) staff       (20)     5640 2022-08-04 21:34:36.000000 cloud-volume-8.9.2/cloudvolume/paths.py
+-rw-r--r--   0 wms        (501) staff       (20)     3799 2021-02-11 23:00:42.000000 cloud-volume-8.9.2/cloudvolume/provenance.py
+-rw-r--r--   0 wms        (501) staff       (20)    10721 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/py_compressed_segmentation.py
+-rw-r--r--   0 wms        (501) staff       (20)     2639 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/scheduler.py
+-rw-r--r--   0 wms        (501) staff       (20)     6070 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/secrets.py
+-rw-r--r--   0 wms        (501) staff       (20)     2463 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/server.py
+-rw-r--r--   0 wms        (501) staff       (20)     6708 2021-07-21 05:29:44.000000 cloud-volume-8.9.2/cloudvolume/sharedmemory.py
+-rw-r--r--   0 wms        (501) staff       (20)    33156 2022-08-18 21:49:59.000000 cloud-volume-8.9.2/cloudvolume/skeleton.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.985992 cloud-volume-8.9.2/cloudvolume/storage/
+-rw-r--r--   0 wms        (501) staff       (20)      908 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/cloudvolume/storage/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    20968 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/cloudvolume/storage/storage.py
+-rw-r--r--   0 wms        (501) staff       (20)    15097 2021-07-21 05:29:44.000000 cloud-volume-8.9.2/cloudvolume/storage/storage_interfaces.py
+-rw-r--r--   0 wms        (501) staff       (20)     7173 2022-02-11 05:36:41.000000 cloud-volume-8.9.2/cloudvolume/threaded_queue.py
+-rw-r--r--   0 wms        (501) staff       (20)      175 2022-03-01 22:13:19.000000 cloud-volume-8.9.2/cloudvolume/types.py
+-rw-r--r--   0 wms        (501) staff       (20)     3349 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/cloudvolume/volumecutout.py
+-rw-r--r--   0 wms        (501) staff       (20)      499 2022-09-06 21:59:17.000000 cloud-volume-8.9.2/requirements.txt
+-rw-r--r--   0 wms        (501) staff       (20)       38 2022-09-06 22:03:19.991414 cloud-volume-8.9.2/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     2408 2022-09-06 22:03:00.000000 cloud-volume-8.9.2/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2022-09-06 22:03:19.990721 cloud-volume-8.9.2/test/
+-rw-r--r--   0 wms        (501) staff       (20)     4805 2022-05-10 21:12:56.000000 cloud-volume-8.9.2/test/test_chunks.py
+-rw-r--r--   0 wms        (501) staff       (20)    49288 2022-08-04 21:34:38.000000 cloud-volume-8.9.2/test/test_cloudvolume.py
+-rw-r--r--   0 wms        (501) staff       (20)     1759 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/test/test_connectionpools.py
+-rw-r--r--   0 wms        (501) staff       (20)     3441 2021-08-19 18:41:54.000000 cloud-volume-8.9.2/test/test_dask.py
+-rw-r--r--   0 wms        (501) staff       (20)    15455 2022-05-10 21:12:57.000000 cloud-volume-8.9.2/test/test_graphene.py
+-rw-r--r--   0 wms        (501) staff       (20)     7466 2022-09-06 21:58:34.000000 cloud-volume-8.9.2/test/test_lib.py
+-rw-r--r--   0 wms        (501) staff       (20)     1500 2022-05-10 21:12:57.000000 cloud-volume-8.9.2/test/test_lru.py
+-rw-r--r--   0 wms        (501) staff       (20)     5811 2022-03-02 05:51:29.000000 cloud-volume-8.9.2/test/test_meshing.py
+-rw-r--r--   0 wms        (501) staff       (20)     5777 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/test/test_paths.py
+-rw-r--r--   0 wms        (501) staff       (20)     1674 2021-07-01 19:28:07.000000 cloud-volume-8.9.2/test/test_precomputed_multilod.py
+-rw-r--r--   0 wms        (501) staff       (20)     3204 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/test/test_provenance.py
+-rw-r--r--   0 wms        (501) staff       (20)     6214 2021-07-01 19:28:05.000000 cloud-volume-8.9.2/test/test_sharding.py
+-rw-r--r--   0 wms        (501) staff       (20)     3099 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/test/test_sharedmemory.py
+-rw-r--r--   0 wms        (501) staff       (20)    19866 2021-12-27 22:30:59.000000 cloud-volume-8.9.2/test/test_skeletons.py
+-rw-r--r--   0 wms        (501) staff       (20)     9576 2021-06-11 02:56:35.000000 cloud-volume-8.9.2/test/test_storage.py
+-rw-r--r--   0 wms        (501) staff       (20)     2092 2021-01-11 02:21:16.000000 cloud-volume-8.9.2/test/test_threadedqueue.py
```

### Comparing `cloud-volume-8.9.1/LICENSE` & `cloud-volume-8.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/PKG-INFO` & `cloud-volume-8.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-volume
-Version: 8.9.1
+Version: 8.9.2
 Summary: A serverless client for reading and writing Neuroglancer Precomputed volumes both locally and on cloud services.
 Home-page: https://github.com/seung-lab/cloud-volume/
 Author: William Silversmith, Nico Kemnitz, Ignacio Tartavull, and others
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Description: [![Build Status](https://travis-ci.org/seung-lab/cloud-volume.svg?branch=master)](https://travis-ci.org/seung-lab/cloud-volume) [![PyPI version](https://badge.fury.io/py/cloud-volume.svg)](https://badge.fury.io/py/cloud-volume) [![SfN 2018 Poster](https://img.shields.io/badge/poster-SfN%202018-blue.svg)](https://drive.google.com/open?id=1RKtaAGV2f7F13opnkQfbp6YBqmoD3fZi) [![codecov](https://img.shields.io/badge/codecov-link-%23d819a6)](https://codecov.io/gh/seung-lab/cloud-volume) [![DOI](https://zenodo.org/badge/98333149.svg)](https://zenodo.org/badge/latestdoi/98333149)
```

### Comparing `cloud-volume-8.9.1/README.md` & `cloud-volume-8.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloud_volume.egg-info/PKG-INFO` & `cloud-volume-8.9.2/cloud_volume.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-volume
-Version: 8.9.1
+Version: 8.9.2
 Summary: A serverless client for reading and writing Neuroglancer Precomputed volumes both locally and on cloud services.
 Home-page: https://github.com/seung-lab/cloud-volume/
 Author: William Silversmith, Nico Kemnitz, Ignacio Tartavull, and others
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: BSD License
 Description: [![Build Status](https://travis-ci.org/seung-lab/cloud-volume.svg?branch=master)](https://travis-ci.org/seung-lab/cloud-volume) [![PyPI version](https://badge.fury.io/py/cloud-volume.svg)](https://badge.fury.io/py/cloud-volume) [![SfN 2018 Poster](https://img.shields.io/badge/poster-SfN%202018-blue.svg)](https://drive.google.com/open?id=1RKtaAGV2f7F13opnkQfbp6YBqmoD3fZi) [![codecov](https://img.shields.io/badge/codecov-link-%23d819a6)](https://codecov.io/gh/seung-lab/cloud-volume) [![DOI](https://zenodo.org/badge/98333149.svg)](https://zenodo.org/badge/latestdoi/98333149)
```

### Comparing `cloud-volume-8.9.1/cloud_volume.egg-info/SOURCES.txt` & `cloud-volume-8.9.2/cloud_volume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloud_volume.egg-info/requires.txt` & `cloud-volume-8.9.2/cloud_volume.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 python-dateutil
 requests>=2.22.0
 pysimdjson>=3.1.1
 simplejpeg
 six>=1.10.0
 tenacity>=4.10.0
 tqdm
-urllib3[brotli,secure]>=1.25.7
+urllib3[brotli]>=1.25.7
 zfpc
 
 [:sys_platform!="win32"]
 posix_ipc>=1.0.4
 psutil>=5.4.3
 
 [all_viewers]
```

### Comparing `cloud-volume-8.9.1/cloudvolume/__init__.py` & `cloud-volume-8.9.2/cloudvolume/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 from . import exceptions
 from . import secrets
 
 from . import microviewer
 from .microviewer import view, hyperview
 
-__version__ = '8.9.1'
+__version__ = '8.9.2'
 
 # Register plugins
 from .datasource.precomputed import register as register_precomputed
 from .datasource.graphene import register as register_graphene
 
 register_precomputed()
 register_graphene()
```

### Comparing `cloud-volume-8.9.1/cloudvolume/cacheservice.py` & `cloud-volume-8.9.2/cloudvolume/cacheservice.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/chunks.py` & `cloud-volume-8.9.2/cloudvolume/chunks.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/cloudvolume.py` & `cloud-volume-8.9.2/cloudvolume/cloudvolume.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/connectionpools.py` & `cloud-volume-8.9.2/cloudvolume/connectionpools.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/dask.py` & `cloud-volume-8.9.2/cloudvolume/dask.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/boss/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/boss/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/boss/image.py` & `cloud-volume-8.9.2/cloudvolume/datasource/boss/image.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/boss/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/boss/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/graphene/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/graphene/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/sharded.py` & `cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/sharded.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/graphene/mesh/unsharded.py` & `cloud-volume-8.9.2/cloudvolume/datasource/graphene/mesh/unsharded.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/graphene/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/graphene/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/n5/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/n5/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/n5/image.py` & `cloud-volume-8.9.2/cloudvolume/datasource/n5/image.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/n5/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/n5/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/common.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/common.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/common.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/common.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/rx.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/rx.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/image/tx.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/image/tx.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/multilod.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/multilod.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mesh/unsharded.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mesh/unsharded.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/mmh3.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/mmh3.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/sharding.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/sharding.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/__init__.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/metadata.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/metadata.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/sharded.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/sharded.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/skeleton/unsharded.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/skeleton/unsharded.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/datasource/precomputed/spatial_index.py` & `cloud-volume-8.9.2/cloudvolume/datasource/precomputed/spatial_index.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/exceptions.py` & `cloud-volume-8.9.2/cloudvolume/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/frontends/graphene.py` & `cloud-volume-8.9.2/cloudvolume/frontends/graphene.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/frontends/precomputed.py` & `cloud-volume-8.9.2/cloudvolume/frontends/precomputed.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/lib.py` & `cloud-volume-8.9.2/cloudvolume/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,16 @@
 Vec.g = Vec.y
 Vec.b = Vec.z
 Vec.a = Vec.w
 
 def floating(lst):
   return any(( isinstance(x, float) for x in lst ))
 
-FILENAME_RE = re.compile(r'(-?\d+)-(-?\d+)_(-?\d+)-(-?\d+)_(-?\d+)-(-?\d+)(?:\.gz|\.br)?$')
+FLT_RE = r'(-?\d+(?:\.\d+)?)' # floating point regexp
+FILENAME_RE = re.compile(fr'{FLT_RE}-{FLT_RE}_{FLT_RE}-{FLT_RE}_{FLT_RE}-{FLT_RE}(?:\.gz|\.br|\.zstd)?$')
 
 class Bbox(object):
   __slots__ = [ 'minpt', 'maxpt', '_dtype' ]
 
   """Represents a three dimensional cuboid in space."""
   def __init__(self, a, b, dtype=None):
     if dtype is None:
@@ -428,22 +429,26 @@
 
   @classmethod
   def from_vec(cls, vec, dtype=int):
     return Bbox( (0,0,0), vec, dtype=dtype)
 
   @classmethod
   def from_filename(cls, filename, dtype=int):
-    match = FILENAME_RE.search(os.path.basename(filename))
+    fname = os.path.basename(filename)
+    match = FILENAME_RE.search(fname)
 
     if match is None:
       raise ValueError("Unable to decode bounding box from: " + str(filename))
 
+    root, ext = os.path.splitext(fname)
+    parse_type = float if '.' in root else int
+
     (xmin, xmax,
      ymin, ymax,
-     zmin, zmax) = map(int, match.groups())
+     zmin, zmax) = map(parse_type, match.groups())
 
     return Bbox( (xmin, ymin, zmin), (xmax, ymax, zmax), dtype=dtype)
 
   @classmethod
   def from_slices(cls, slices, context=None, bounded=False, autocrop=False):
     if context:
       slices = context.reify_slices(
```

### Comparing `cloud-volume-8.9.1/cloudvolume/lru.py` & `cloud-volume-8.9.2/cloudvolume/lru.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/mesh.py` & `cloud-volume-8.9.2/cloudvolume/mesh.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/microviewer/__init__.py` & `cloud-volume-8.9.2/cloudvolume/microviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/microviewer/datacube.js` & `cloud-volume-8.9.2/cloudvolume/microviewer/datacube.js`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/microviewer/favicon.ico` & `cloud-volume-8.9.2/cloudvolume/microviewer/favicon.ico`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/microviewer/index.html` & `cloud-volume-8.9.2/cloudvolume/microviewer/index.html`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/microviewer/jquery-3.3.1.js` & `cloud-volume-8.9.2/cloudvolume/microviewer/jquery-3.3.1.js`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/paths.py` & `cloud-volume-8.9.2/cloudvolume/paths.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/provenance.py` & `cloud-volume-8.9.2/cloudvolume/provenance.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/py_compressed_segmentation.py` & `cloud-volume-8.9.2/cloudvolume/py_compressed_segmentation.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/scheduler.py` & `cloud-volume-8.9.2/cloudvolume/scheduler.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/secrets.py` & `cloud-volume-8.9.2/cloudvolume/secrets.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/server.py` & `cloud-volume-8.9.2/cloudvolume/server.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/sharedmemory.py` & `cloud-volume-8.9.2/cloudvolume/sharedmemory.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/skeleton.py` & `cloud-volume-8.9.2/cloudvolume/skeleton.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/storage/__init__.py` & `cloud-volume-8.9.2/cloudvolume/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/storage/storage.py` & `cloud-volume-8.9.2/cloudvolume/storage/storage.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/storage/storage_interfaces.py` & `cloud-volume-8.9.2/cloudvolume/storage/storage_interfaces.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/threaded_queue.py` & `cloud-volume-8.9.2/cloudvolume/threaded_queue.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/cloudvolume/volumecutout.py` & `cloud-volume-8.9.2/cloudvolume/volumecutout.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/setup.py` & `cloud-volume-8.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def requirements():
   with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), 'rt') as f:
     return f.readlines()
 
 setuptools.setup(
   name="cloud-volume",
-  version="8.9.1",
+  version="8.9.2",
   setup_requires=[
     'numpy<1.17; python_version<"3.5"',
     'numpy; python_version>="3.5"',
   ],
   python_requires="~=3.6", # >= 3.6 < 4.0
   install_requires=requirements(),
   # Environment Marker Examples:
```

### Comparing `cloud-volume-8.9.1/test/test_chunks.py` & `cloud-volume-8.9.2/test/test_chunks.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_cloudvolume.py` & `cloud-volume-8.9.2/test/test_cloudvolume.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_connectionpools.py` & `cloud-volume-8.9.2/test/test_connectionpools.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_dask.py` & `cloud-volume-8.9.2/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_graphene.py` & `cloud-volume-8.9.2/test/test_graphene.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_lib.py` & `cloud-volume-8.9.2/test/test_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -247,14 +247,19 @@
 
 
 def test_bbox_from_filename():
   filenames = [
     "0-512_0-512_0-16",
     "0-512_0-512_0-16.gz",
     "0-512_0-512_0-16.br",
+    "0-512_0-512_0-16.zstd",
+    "0.0-512.0_0.0-512.0_0.0-16.0",
+    "0.0-512.0_0.0-512.0_0.0-16.0.gz",
+    "0.0-512.0_0.0-512.0_0.0-16.0.br",
+    "0.0-512.0_0.0-512.0_0.0-16.0.zstd",
   ]
 
   for fn in filenames:
     bbox = Bbox.from_filename(fn)
     assert np.array_equal(bbox.minpt, [0, 0, 0])
     assert np.array_equal(bbox.maxpt, [512, 512, 16])
```

### Comparing `cloud-volume-8.9.1/test/test_lru.py` & `cloud-volume-8.9.2/test/test_lru.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_meshing.py` & `cloud-volume-8.9.2/test/test_meshing.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_paths.py` & `cloud-volume-8.9.2/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_precomputed_multilod.py` & `cloud-volume-8.9.2/test/test_precomputed_multilod.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_provenance.py` & `cloud-volume-8.9.2/test/test_provenance.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_sharding.py` & `cloud-volume-8.9.2/test/test_sharding.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_sharedmemory.py` & `cloud-volume-8.9.2/test/test_sharedmemory.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_skeletons.py` & `cloud-volume-8.9.2/test/test_skeletons.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_storage.py` & `cloud-volume-8.9.2/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `cloud-volume-8.9.1/test/test_threadedqueue.py` & `cloud-volume-8.9.2/test/test_threadedqueue.py`

 * *Files identical despite different names*

