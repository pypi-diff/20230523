# Comparing `tmp/tiledbsoma-1.2.3.tar.gz` & `tmp/tiledbsoma-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.3.tar", last modified: Wed May  3 20:56:22 2023, max compression
+gzip compressed data, was "tiledbsoma-1.2.4.tar", last modified: Mon May 22 22:52:31 2023, max compression
```

## Comparing `tiledbsoma-1.2.3.tar` & `tiledbsoma-1.2.4.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-03 20:56:20.000000 tiledbsoma-1.2.3/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-03 20:56:18.000000 tiledbsoma-1.2.3/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     9403 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     6296 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)    10856 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6700 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (122)     7122 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10172 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    14657 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15129 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.098111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7864 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_soma_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10346 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.102111 tiledbsoma-1.2.3/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2811 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.094111 tiledbsoma-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    26933 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7045 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33607 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11735 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    53795 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7781 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 20:56:22.106112 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-03 20:56:22.000000 tiledbsoma-1.2.3/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-03 20:56:19.000000 tiledbsoma-1.2.3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 22:52:30.000000 tiledbsoma-1.2.4/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27087 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7131 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33740 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55729 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/version.py
```

### Comparing `tiledbsoma-1.2.3/PKG-INFO` & `tiledbsoma-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.3/README.md` & `tiledbsoma-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # CMakeLists.txt
 #
 #
 # The MIT License
 #
-# Copyright (c) 2022 TileDB, Inc.
+# Copyright (c) 2022-2023 TileDB, Inc.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -38,15 +38,14 @@
 set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_CURRENT_SOURCE_DIR}/cmake/Modules/")
 
 set(TILEDBSOMA_CMAKE_INPUTS_DIR "${CMAKE_CURRENT_SOURCE_DIR}/cmake/inputs")
 
 # TileDB-SOMA Options
 option(TILEDBSOMA_BUILD_PYTHON "Build Python API bindings" ON)
 option(TILEDBSOMA_BUILD_CLI "Build tiledbsoma CLI tool" ON)
-option(TILEDBSOMA_BUILD_R "Build a static library (only) for R" OFF)
 option(TILEDBSOMA_BUILD_STATIC "Build a static library; otherwise, shared library" OFF)
 option(TILEDBSOMA_ENABLE_TESTING "Enable tests" ON)
 option(TILEDBSOMA_ENABLE_WERROR "Enables the -Werror flag during compilation." ON)
 
 # Superbuild option must be on by default.
 option(SUPERBUILD "If true, perform a superbuild (builds all missing dependencies)." ON)
 option(CMAKE_IDE "(Used for CLion builds). Disables superbuild and sets the EP install dir." OFF)
@@ -63,24 +62,14 @@
 option(TILEDB_WERROR "Enables the -Werror flag during compilation." OFF)
 option(TILEDB_SERIALIZATION "If true, enables building with support for query serialization" ON)
 option(TILEDB_VERBOSE "If true, sets default logging to verbose for TileDB" OFF)
 option(OVERRIDE_INSTALL_PREFIX "Ignores the setting of CMAKE_INSTALL_PREFIX and sets a default prefix" ON)
 option(ENABLE_ARROW_EXPORT "Installs an extra header for exporting in-memory results with Apache Arrow" ON)
 option(TILEDB_LOG_OUTPUT_ON_FAILURE "If true, print error logs if dependency sub-project build fails" ON)
 
-# NOTE: TILEDBSOMA_BUILD_R is added to INHERITED_CMAKE_ARGS in Superbuild.cmake
-# so the option is forwarded to the non-superbuild
-if(TILEDBSOMA_BUILD_R)
-  # Disable build targets when building for R
-  set(TILEDBSOMA_BUILD_PYTHON OFF)
-  set(TILEDBSOMA_BUILD_CLI OFF)
-  set(TILEDBSOMA_ENABLE_TESTING OFF)
-  set(TILEDBSOMA_BUILD_STATIC ON)
-endif()
-
 # Enable compiler cache to speed up recompilation
 find_program(CCACHE_FOUND ccache)
 
 if(CCACHE_FOUND)
   set_property(GLOBAL PROPERTY RULE_LAUNCH_COMPILE ccache)
   set_property(GLOBAL PROPERTY RULE_LAUNCH_LINK ccache)
 endif()
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files 13% similar despite different names*

```diff
@@ -58,21 +58,41 @@
     # NB When updating the pinned URLs here, please also update in file apis/r/tools/get_tarball.R
     if(DOWNLOAD_TILEDB_PREBUILT)
         if (WIN32) # Windows
           SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-windows-x86_64-2.15.2-90f30eb.zip")
           SET(DOWNLOAD_SHA1 "1adc1ffa3c6c0f637bcb68d3cd278b0bee597b9c")
         elseif(APPLE) # OSX
 
-          if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
+          # Status quo as of 2023-05-18:
+          # * GitHub Actions does not have MacOS arm64 hardware available -- tracked at
+          #   https://github.com/github/roadmap/issues/528
+          # * The best we can do is cross-compile for arm64 while actually running on x86_64
+          # * When we're invoked from python setup.py:
+          #   o CMAKE_OSX_ARCHITECTURES is x86_64 or arm64
+          #   o CMAKE_SYSTEM_PROCESSOR is x86_64 in either case
+          #   o We must download the tiledb artifacts for the cross-compile architecture (x86_64 or arm64)
+          #   o Therefore we must respect CMAKE_OSX_ARCHITECTURES not CMAKE_SYSTEM_PROCESSOR
+          # * When we're invoked from R configure and src/Makevars.in:
+          #   o CMAKE_OSX_ARCHITECTURES is unset
+          #   o CMAKE_SYSTEM_PROCESSOR is x86_64
+
+          if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64)
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-x86_64-2.15.2-90f30eb.tar.gz")
+            SET(DOWNLOAD_SHA1 "616b9ab508d1233d3bc3d6a2a7b1c42c8098f38a")
+          elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64)
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-arm64-2.15.2-90f30eb.tar.gz")
+            SET(DOWNLOAD_SHA1 "882eadcc256f95a5c91094407770799a8bd4e759")
+          elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
             SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-x86_64-2.15.2-90f30eb.tar.gz")
             SET(DOWNLOAD_SHA1 "616b9ab508d1233d3bc3d6a2a7b1c42c8098f38a")
-          elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
+          elseif (CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
             SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-macos-arm64-2.15.2-90f30eb.tar.gz")
             SET(DOWNLOAD_SHA1 "882eadcc256f95a5c91094407770799a8bd4e759")
           endif()
+
         else() # Linux
           SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.2/tiledb-linux-x86_64-2.15.2-90f30eb.tar.gz")
           SET(DOWNLOAD_SHA1 "33ae11d507dc7bec82fbdfbd8e2b2e13cff16b89")
         endif()
 
         ExternalProject_Add(ep_tiledb
                 PREFIX "externals"
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 # ###########################################################
 # Common object library
 # ###########################################################
 add_library(TILEDB_SOMA_OBJECTS OBJECT
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.cc
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.cc
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.cc
 
   # TODO: uncomment when thread_pool is enabled
@@ -164,41 +165,42 @@
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_measurement.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_object.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/soma_sparse_ndarray.h
 #   ${CMAKE_CURRENT_SOURCE_DIR}/cpp_api/logger_public.h
 # )
 
 install(FILES 
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/logger_public.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/managed_query.h
   ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_array.h 
-  DESTINATION "include/soma"
+  ${CMAKE_CURRENT_SOURCE_DIR}/soma/soma_group.h 
+  DESTINATION "include/tiledbsoma/soma"
 )
 
 install(FILES 
-  ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/logger_public.h
   ${CMAKE_CURRENT_SOURCE_DIR}/tiledbsoma/tiledbsoma
   DESTINATION "include/tiledbsoma"
 )
 
 install(FILES
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/array_buffers.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/arrow_adapter.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/carrow.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/column_buffer.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/common.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/logger.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/stats.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/util.h  
   ${CMAKE_CURRENT_SOURCE_DIR}/utils/version.h
-  DESTINATION "include/utils"
+  DESTINATION "include/tiledbsoma/utils"
 )
 
 install(FILES 
   ${CMAKE_CURRENT_SOURCE_DIR}/external/include/span/span.hpp
-  DESTINATION "include/span"
+  DESTINATION "include/tiledbsoma/utils/span"
 )
 
 
 # ###########################################################
 # API symbol exports
 # ###########################################################
 include(GenerateExportHeader)
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 #include <mutex>
 #include <optional>
 #include <type_traits>
 
 #include <deque>
 #include <queue>
 
-#include "tiledbsoma/logger_public.h"
+#include "soma/logger_public.h"
 
 namespace tiledbsoma {
 
 template <class Item, class Container = std::deque<Item>>
 class ProducerConsumerQueue {
  public:
   ProducerConsumerQueue() = default;
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 #include "thread_pool/thread_pool.h"
 
 #include <cassert>
 #include <memory>
 #include <queue>
 #include <thread>
 
-#include "tiledbsoma/logger_public.h"
+#include "soma/logger_public.h"
 
 namespace tiledbsoma {
 
 // Constructor.  May throw an exception on error.  No logging is done as the
 // logger may not yet be initialized.
 ThreadPool::ThreadPool(size_t n)
     : concurrency_level_(n) {
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  * This file defines the performing TileDB queries.
  */
 
-#include "soma/managed_query.h"
-#include "tiledbsoma/logger_public.h"
+#include "managed_query.h"
+#include "logger_public.h"
 #include "utils/common.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 //===================================================================
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 #define MANAGED_QUERY_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 #include <unordered_set>
 
 #include <tiledb/tiledb>
 
-#include "utils/array_buffers.h"
-#include "utils/column_buffer.h"
-#include "utils/common.h"
+#include "../utils/array_buffers.h"
+#include "../utils/column_buffer.h"
+#include "../utils/common.h"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ManagedQuery {
    public:
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
  *
  * @section DESCRIPTION
  *
  *   This file defines the SOMAArray class.
  */
 
 #include "soma_array.h"
-#include "../tiledbsoma/logger_public.h"
 #include "../utils/util.h"
+#include "logger_public.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
 //===================================================================
 //= public static
 //===================================================================
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,14 @@
 #include <tiledb/tiledb>
 
 #include "managed_query.h"
 
 namespace tiledbsoma {
 using namespace tiledb;
 
-using MetadataValue =
-    std::tuple<std::string, tiledb_datatype_t, uint32_t, const void*>;
-enum MetadataInfo { key = 0, dtype, num, value };
-
 class SOMAArray {
    public:
     //===================================================================
     //= public static
     //===================================================================
 
     /**
@@ -128,21 +124,24 @@
     SOMAArray() = delete;
     SOMAArray(const SOMAArray&) = delete;
     SOMAArray(SOMAArray&&) = default;
     ~SOMAArray() = default;
 
     /**
      * Open the SOMAArray object.
+     *
+     * @param mode TILEDB_READ or TILEDB_WRITE
+     * @param timestamp Timestamp
      */
     void open(
         tiledb_query_type_t mode,
         std::optional<std::pair<uint64_t, uint64_t>> timestamp = std::nullopt);
 
     /**
-     * Closes the SOMAArray object.
+     * Close the SOMAArray object.
      */
     void close();
 
     /**
      * @brief Reset the state of this SOMAArray object to prepare for a
      * new query, while holding the array open.
      *
@@ -324,15 +323,15 @@
      * query
      */
     bool results_complete() {
         return mq_->results_complete();
     }
 
     /**
-     * @brief Returns the total number of cells read so far, including any
+     * @brief Return the total number of cells read so far, including any
      * previous incomplete queries.
      *
      * @return size_t Total number of cells read
      */
     size_t total_num_cells() {
         return mq_->total_num_cells();
     }
@@ -378,64 +377,77 @@
     void set_metadata(
         const std::string& key,
         tiledb_datatype_t value_type,
         uint32_t value_num,
         const void* value);
 
     /**
-     * Deletes a metadata key-value item from an open array. The array must
+     * Delete a metadata key-value item from an open array. The array must
      * be opened in WRITE mode, otherwise the function will error out.
      *
      * @param key The key of the metadata item to be deleted.
      *
      * @note The writes will take effect only upon closing the array.
      *
      * @note If the key does not exist, this will take no effect
      *     (i.e., the function will not error out).
      */
     void delete_metadata(const std::string& key);
 
     /**
-     * @brief Given a key, retrieve the associated value datatype, number of
+     * @brief Given a key, get the associated value datatype, number of
      * values, and value in binary form. The array must be opened in READ mode,
      * otherwise the function will error out.
      *
      * The value may consist of more than one items of the same datatype. Keys
      * that do not exist in the metadata will be return NULL for the value.
      *
+     * **Example:**
+     * @code{.cpp}
+     * // Open the array for reading
+     * tiledbsoma::SOMAArray soma_array = SOMAArray::open(TILEDB_READ,
+     "s3://bucket-name/group-name");
+     * tiledbsoma::MetadataValue meta_val = soma_array->get_metadata("key");
+     * std::string key = std::get<MetadataInfo::key>(meta_val);
+     * tiledb_datatype_t dtype = std::get<MetadataInfo::dtype>(meta_val);
+     * uint32_t num = std::get<MetadataInfo::num>(meta_val);
+     * const void* value = *((const
+     int32_t*)std::get<MetadataInfo::value>(meta_val));
+     * @endcode
+     *
      * @param key The key of the metadata item to be retrieved. UTF-8 encodings
      *     are acceptable.
      * @return MetadataValue (std::tuple<std::string, tiledb_datatype_t,
      * uint32_t, const void*>)
      */
     MetadataValue get_metadata(const std::string& key) const;
 
     /**
-     * @brief Given an index, retrieve the associated value datatype, number of
+     * @brief Given an index, get the associated value datatype, number of
      * values, and value in binary form. The array must be opened in READ mode,
      * otherwise the function will error out.
      *
      * @param index The index used to get the metadata.
      * @return MetadataValue (std::tuple<std::string, tiledb_datatype_t,
      * uint32_t, const void*>)
      */
     MetadataValue get_metadata(uint64_t index) const;
 
     /**
-     * Checks if key exists in metadata from an open array. The array must
+     * Check if the key exists in metadata from an open array. The array must
      * be opened in READ mode, otherwise the function will error out.
      *
      * @param key The key of the metadata item to be checked. UTF-8 encodings
      *     are acceptable.
      * @return true if the key exists, else false.
      */
     bool has_metadata(const std::string& key);
 
     /**
-     * Returns then number of metadata items in an open array. The array must
+     * Return then number of metadata items in an open array. The array must
      * be opened in READ mode, otherwise the function will error out.
      */
     uint64_t metadata_num() const;
 
    private:
     //===================================================================
     //= private non-static
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 // #include "soma_dataframe.h"
 // #include "soma_dense_ndarray.h"
 // #include "soma_experiment.h"
 // #include "soma_measurement.h"
 // #include "soma_object.h"
 // #include "soma_sparse_ndarray.h"
 
-#include <utils/arrow_adapter.h>
-#include <tiledbsoma/logger_public.h>
-#include <utils/array_buffers.h>
-#include <utils/column_buffer.h>
-#include <utils/common.h>
-#include <utils/stats.h>
-#include <utils/version.h>
-#include <soma/managed_query.h>
-#include <soma/soma_array.h>
+#include "utils/arrow_adapter.h"
+#include "utils/array_buffers.h"
+#include "utils/column_buffer.h"
+#include "utils/common.h"
+#include "utils/stats.h"
+#include "utils/version.h"
+#include "soma/logger_public.h"
+#include "soma/managed_query.h"
+#include "soma/soma_array.h"
+#include "soma/soma_group.h"
 
 #endif
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/array_buffers.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/array_buffers.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,20 @@
  */
 
 #ifndef ARRAY_BUFFERS_H
 #define ARRAY_BUFFERS_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
-#include <span/span.hpp>
 #include <tiledb/tiledb>
 
 #include "column_buffer.h"
 #include "common.h"
 #include "logger.h"
+#include "span/span.hpp"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 class ArrayBuffers {
    public:
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/column_buffer.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
  */
 
 #ifndef COLUMN_BUFFER_H
 #define COLUMN_BUFFER_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
-#include <span/span.hpp>
 #include <tiledb/tiledb>
 
 #include "common.h"
 #include "logger.h"
+#include "span/span.hpp"
 
 namespace tiledbsoma {
 
 using namespace tiledb;
 
 /**
  * @brief Class to store data for a TileDB dimension or attribute.
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   common.h
+ * @file   stats.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2022 TileDB, Inc.
+ * @copyright Copyright (c) 2023 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -26,32 +26,24 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  *   This declares the common functions in the API
  */
 
-#ifndef TILEDBSOMA_COMMON_H
-#define TILEDBSOMA_COMMON_H
+#ifndef TILEDBSOMA_STATS_H
+#define TILEDBSOMA_STATS_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <string>
 
-namespace tiledbsoma {
+namespace tiledbsoma::stats {
 
-class TileDBSOMAError : public std::runtime_error {
-   public:
-    explicit TileDBSOMAError(const char* m)
-        : std::runtime_error(m){};
-    explicit TileDBSOMAError(std::string m)
-        : std::runtime_error(m.c_str()){};
-
-   public:
-    virtual const char* what() const noexcept override {
-        return std::runtime_error::what();
-    };
-};
+void enable();
+void disable();
+void reset();
+std::string dump();
 
-};  // namespace tiledbsoma
+};  // namespace tiledbsoma::stats
 
-#endif  // TILEDBSOMA_COMMON_H
+#endif  // TILEDBSOMA_STATS_H
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files 0% similar despite different names*

```diff
@@ -240,10 +240,10 @@
 
 }  // namespace tiledbsoma
 
 /** Convert TileDB timestamp (in ms) to human readable timestamp. */
 std::string asc_timestamp(uint64_t timestamp_ms);
 
 // Also include the public logger functions here.
-#include "../tiledbsoma/logger_public.h"
+#include "../soma/logger_public.h"
 
 #endif  // TILEDB_LOGGER_H
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /**
- * @file   stats.h
+ * @file   version.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
  * @copyright Copyright (c) 2023 TileDB, Inc.
  *
@@ -23,27 +23,25 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- *   This declares the common functions in the API
+ * This exposes the version of the TileDB Embedded library in use.
  */
 
-#ifndef TILEDBSOMA_STATS_H
-#define TILEDBSOMA_STATS_H
+#ifndef TILEDBSOMA_VERSION_H
+#define TILEDBSOMA_VERSION_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <string>
 
-namespace tiledbsoma::stats {
+namespace tiledbsoma::version {
 
-void enable();
-void disable();
-void reset();
-std::string dump();
+std::string as_string();
+std::tuple<int, int, int> embedded_version_triple();
 
-};  // namespace tiledbsoma::stats
+};  // namespace tiledbsoma::version
 
-#endif  // TILEDBSOMA_STATS_H
+#endif  // TILEDBSOMA_VERSION_H
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,18 @@
  * This file defines the utility functions
  */
 
 #ifndef UTIL_H
 #define UTIL_H
 
 #include <regex>
-#include <span/span.hpp>
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
+#include "span/span.hpp"
+
 namespace tiledbsoma::util {
 
 using VarlenBufferPair =
     std::pair<std::vector<std::byte>, std::vector<uint64_t>>;
 
 template <typename T>
 VarlenBufferPair to_varlen_buffers(std::vector<T> data, bool arrow = true);
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 /**
- * @file   version.h
+ * @file   common.h
  *
  * @section LICENSE
  *
  * The MIT License
  *
- * @copyright Copyright (c) 2023 TileDB, Inc.
+ * @copyright Copyright (c) 2022 TileDB, Inc.
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
@@ -23,25 +23,39 @@
  * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
- * This exposes the version of the TileDB Embedded library in use.
+ *   This declares the common functions in the API
  */
 
-#ifndef TILEDBSOMA_VERSION_H
-#define TILEDBSOMA_VERSION_H
+#ifndef TILEDBSOMA_COMMON_H
+#define TILEDBSOMA_COMMON_H
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <string>
 
-namespace tiledbsoma::version {
+namespace tiledbsoma {
 
-std::string as_string();
-std::tuple<int, int, int> embedded_version_triple();
+using MetadataValue =
+    std::tuple<std::string, tiledb_datatype_t, uint32_t, const void*>;
+enum MetadataInfo { key = 0, dtype, num, value };
+
+class TileDBSOMAError : public std::runtime_error {
+   public:
+    explicit TileDBSOMAError(const char* m)
+        : std::runtime_error(m){};
+    explicit TileDBSOMAError(std::string m)
+        : std::runtime_error(m.c_str()){};
+
+   public:
+    virtual const char* what() const noexcept override {
+        return std::runtime_error::what();
+    };
+};
 
-};  // namespace tiledbsoma::version
+};  // namespace tiledbsoma
 
-#endif  // TILEDBSOMA_VERSION_H
+#endif  // TILEDBSOMA_COMMON_H
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 find_package(Catch_EP REQUIRED)
 
 add_executable(unit_soma EXCLUDE_FROM_ALL
     $<TARGET_OBJECTS:TILEDB_SOMA_OBJECTS>
     unit_column_buffer.cc
     unit_managed_query.cc
     unit_soma_array.cc
+    unit_soma_group.cc
 # TODO: uncomment when thread_pool is enabled
 #    unit_thread_pool.cc
 )
 
 target_link_libraries(unit_soma
   PRIVATE
     Catch2::Catch2WithMain
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/test_soma_array.py` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files 22% similar despite different names*

```diff
@@ -170,20 +170,20 @@
             num_cells_per_fragment,
             num_fragments,
             overlap,
             allow_duplicates,
             10);
 
         // Get total cell num
-        auto sr = SOMAArray::open(TILEDB_READ, ctx, uri);
+        auto soma_array = SOMAArray::open(TILEDB_READ, ctx, uri);
 
-        uint64_t nnz = sr->nnz();
+        uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
 
-        std::vector<int64_t> shape = sr->shape();
+        std::vector<int64_t> shape = soma_array->shape();
         REQUIRE(shape.size() == 1);
         REQUIRE(shape[0] == std::numeric_limits<int64_t>::max());
     }
 }
 
 TEST_CASE("SOMAArray: nnz with timestamp") {
     auto num_fragments = GENERATE(1, 10);
@@ -219,18 +219,18 @@
             overlap,
             allow_duplicates,
             20,
             true);
 
         // Get total cell num at timestamp (0, 15)
         std::pair<uint64_t, uint64_t> timestamp{0, 15};
-        auto sr = SOMAArray::open(
+        auto soma_array = SOMAArray::open(
             TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto", timestamp);
 
-        uint64_t nnz = sr->nnz();
+        uint64_t nnz = soma_array->nnz();
         REQUIRE(nnz == expected_nnz);
     }
 }
 
 TEST_CASE("SOMAArray: nnz with consolidation") {
     auto num_fragments = GENERATE(1, 10);
     auto overlap = GENERATE(false, true);
@@ -273,18 +273,18 @@
         // Consolidate and optionally vacuum
         Array::consolidate(*ctx, uri);
         if (vacuum) {
             Array::vacuum(*ctx, uri);
         }
 
         // Get total cell num
-        auto sr = SOMAArray::open(
+        auto soma_array = SOMAArray::open(
             TILEDB_READ, ctx, uri, "nnz", {}, "auto", "auto");
 
-        uint64_t nnz = sr->nnz();
+        uint64_t nnz = soma_array->nnz();
         if (allow_duplicates) {
             // Since we wrote twice
             REQUIRE(nnz == 2 * expected_nnz);
         } else {
             REQUIRE(nnz == expected_nnz);
         }
     }
@@ -292,46 +292,46 @@
 
 TEST_CASE("SOMAArray: metadata") {
     auto ctx = std::make_shared<Context>();
 
     std::string base_uri = "mem://unit-test-array";
     const auto& [uri, expected_nnz] = create_array(base_uri, *ctx);
 
-    auto sr = SOMAArray::open(
+    auto soma_array = SOMAArray::open(
         TILEDB_WRITE,
         ctx,
         uri,
         "metadata_test",
         {},
         "auto",
         "auto",
         std::pair<uint64_t, uint64_t>(1, 1));
     int32_t val = 100;
-    sr->set_metadata("md", TILEDB_INT32, 1, &val);
-    sr->close();
+    soma_array->set_metadata("md", TILEDB_INT32, 1, &val);
+    soma_array->close();
 
-    sr->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(1, 1));
-    REQUIRE(sr->has_metadata("md") == true);
-    REQUIRE(sr->metadata_num() == 1);
+    soma_array->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(1, 1));
+    REQUIRE(soma_array->has_metadata("md") == true);
+    REQUIRE(soma_array->metadata_num() == 1);
 
-    auto mdval = sr->get_metadata(0);
+    auto mdval = soma_array->get_metadata(0);
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
     REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
 
-    mdval = sr->get_metadata("md");
+    mdval = soma_array->get_metadata("md");
     REQUIRE(std::get<MetadataInfo::key>(mdval) == "md");
     REQUIRE(std::get<MetadataInfo::dtype>(mdval) == TILEDB_INT32);
     REQUIRE(std::get<MetadataInfo::num>(mdval) == 1);
     REQUIRE(*((const int32_t*)std::get<MetadataInfo::value>(mdval)) == 100);
-    sr->close();
+    soma_array->close();
 
-    sr->open(TILEDB_WRITE, std::pair<uint64_t, uint64_t>(2, 2));
-    sr->delete_metadata("md");
-    sr->close();
-
-    sr->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(3, 3));
-    REQUIRE(sr->has_metadata("md") == false);
-    REQUIRE(sr->metadata_num() == 0);
-    sr->close();
+    soma_array->open(TILEDB_WRITE, std::pair<uint64_t, uint64_t>(2, 2));
+    soma_array->delete_metadata("md");
+    soma_array->close();
+
+    soma_array->open(TILEDB_READ, std::pair<uint64_t, uint64_t>(3, 3));
+    REQUIRE(soma_array->has_metadata("md") == false);
+    REQUIRE(soma_array->metadata_num() == 0);
+    soma_array->close();
 }
```

### Comparing `tiledbsoma-1.2.3/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/scripts/bld` & `tiledbsoma-1.2.4/dist_links/scripts/bld`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,20 @@
 
 # parse arguments
 # -------------------------------------------------------------------
 arg() { echo "$1" | sed "s/^${2-[^=]*=}//" | sed "s/:/;/g"; }
 
 build="Release"
 prefix=""
-r_build="OFF"
 tiledb=""
 
 while test $# != 0; do
   case "$1" in
   --build=*) build=$(arg "$1");;
   --prefix=*) prefix=$(arg "$1");;
-  --r-build) r_build="ON";;
   --tiledb=*) tiledb=$(arg "$1");;
   esac
   shift
 done
 
 # find number of cpus
 # -------------------------------------------------------------------
@@ -62,40 +60,29 @@
 fi
 
 # set installation path
 if [ -n "${prefix}"  ]; then 
   extra_opts+=" -DCMAKE_INSTALL_PREFIX=${prefix} -DOVERRIDE_INSTALL_PREFIX=OFF"
 fi
 
-# build for R only
-if [ "${r_build}" == "ON" ]; then 
-  extra_opts+=" -DTILEDBSOMA_BUILD_R=${r_build}"
-fi
-
 # build with custom tiledb
 if [ -n "${tiledb}"  ]; then
   printf "Build with TileDB: ${tiledb}\n"
   extra_opts+=" -DFORCE_BUILD_TILEDB=OFF"
   export TileDB_DIR="${tiledb}"
   export LD_LIBRARY_PATH="${tiledb}"
   export DYLD_LIBRARY_PATH="${tiledb}"
 fi
 
 # run cmake
 # -------------------------------------------------------------------
 printf "Building ${build} build\n"
 
 # cd to the top level directory of the repo
-if [ "${r_build}" == "OFF" ]; then 
-  cd "$(dirname "$0")/.."
-fi
+cd "$(dirname "$0")/.."
 
 rm -rf build
 mkdir -p build
 cmake -B build -S libtiledbsoma -DCMAKE_BUILD_TYPE=${build} ${extra_opts}
 cmake --build build -j ${nproc}
 cmake --build build --target install-libtiledbsoma
-
-# Skip unit test build when building for R
-if [ "${r_build}" == "OFF" ]; then
-  cmake --build build/libtiledbsoma --target build_tests -j ${nproc}
-fi
+cmake --build build/libtiledbsoma --target build_tests -j ${nproc}
```

### Comparing `tiledbsoma-1.2.3/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.2.4/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/scripts/show-versions.py` & `tiledbsoma-1.2.4/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.2.4/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/setup.py` & `tiledbsoma-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/__init__.py` & `tiledbsoma-1.2.4/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_collection.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,20 @@
 from ._common_nd_array import NDArray
 from ._dataframe import DataFrame
 from ._dense_nd_array import DenseNDArray
 from ._exception import SOMAError, is_does_not_exist_error
 from ._sparse_nd_array import SparseNDArray
 from ._tiledb_object import AnyTileDBObject, TileDBObject
 from ._types import OpenTimestamp
-from ._util import is_relative_uri, make_relative_path, uri_joinpath
+from ._util import (
+    is_relative_uri,
+    make_relative_path,
+    uri_joinpath,
+    validate_platform_config,
+)
 from .options import SOMATileDBContext
 from .options._soma_tiledb_context import _validate_soma_tiledb_context
 
 # A collection can hold any sub-type of TileDBObject
 CollectionElementType = TypeVar("CollectionElementType", bound=AnyTileDBObject)
 _TDBO = TypeVar("_TDBO", bound=AnyTileDBObject)
 _Coll = TypeVar("_Coll", bound="CollectionBase[AnyTileDBObject]")
@@ -87,16 +92,16 @@
         This creates a new SOMA collection of the current type in storage and
         returns it opened for writing.
 
         Args:
             uri:
                 The location to create this SOMA collection at.
             platform_config:
-                Optional call-specific options to use when
-                creating this collection. (Currently unused.)
+                Platform-specific options used to create this collection, provided in the form
+                ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}``.
             context:
                 If provided, the :class:`SOMATileDBContext` to use when creating and
                 opening this collection.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
@@ -105,14 +110,15 @@
             TileDBError:
                 If unable to create the underlying object.
 
         Lifecycle:
             Experimental.
         """
         context = _validate_soma_tiledb_context(context)
+        validate_platform_config(platform_config)
         tiledb.group_create(uri=uri, ctx=context.tiledb_ctx)
         handle = cls._wrapper_type.open(uri, "w", context, tiledb_timestamp)
         cls._set_create_metadata(handle)
         return cls(
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_common_nd_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
                 None)``, as the sequence length determines the number of dimensions
                 N in the N-dimensional array.
 
                 For :class:`SparseNDArray` only, if a slot is None, then the maximum
                 possible int64 will be used.  This makes a :class:`SparseNDArray`
                 growable.
             platform_config:
-                Platform-specific options used to create this Array,
-                provided via ``{"tiledb": {"create": ...}}`` nested keys.
+                Platform-specific options used to create this array, provided in the form
+                ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}``.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
 
         Returns:
             The created NDArray.
@@ -84,14 +84,15 @@
         # reason that the latter, while temptingly simple, is actually untrue is that tiledb core
         # requires that the capacity, when rounded up to an exact multiple of the extent, needs to
         # be representable as a signed 64-bit integer.  So in particular when a unit test (or anyone
         # else) sets extent to a not-power-of-two number like 999 or 1000 then the create fails if
         # the upper limit is exactly 2**63-1.
 
         context = _validate_soma_tiledb_context(context)
+        _util.validate_platform_config(platform_config)
         schema = cls._build_tiledb_schema(
             type,
             shape,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
             is_sparse=cls.is_sparse,
         )
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,16 +156,16 @@
                 stored in that column.  If provided, this sequence must have the same
                 length as ``index_column_names``, and the index-column domain will be as
                 specified.  If omitted entirely, or if ``None`` in a given dimension,
                 the corresponding index-column domain will use the minimum and maximum
                 possible values for the column's datatype.  This makes a
                 :class:`DataFrame` growable.
             platform_config:
-                Platform-specific options used to create this
-                DataFrame, provided via ``{"tiledb": {"create": ...}}`` nested keys.
+                Platform-specific options used to create this array, provided in the form
+                ``{"tiledb": {"create": {"dataframe_dim_zstd_level": 7}}}``.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
 
         Returns:
             The DataFrame.
@@ -197,14 +197,15 @@
             0            0    a
             1            1    b
 
         Lifecycle:
             Experimental.
         """
         context = _validate_soma_tiledb_context(context)
+        _util.validate_platform_config(platform_config)
         schema = _canonicalize_schema(schema, index_column_names)
         tdb_schema = _build_tiledb_schema(
             schema,
             index_column_names,
             domain,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
@@ -397,14 +398,15 @@
         # the Arrow schema has two index columns in the order "burger" and "meister", and suppose
         # the user set index_column_names = ["meister", "burger"] when creating the TileDB schema.
         # Then the above for-loop over the Arrow schema will find the former ordering, but for the
         # ``writer[dims] = attrs`` below we must have dims with the latter ordering.
         dim_cols_list = [dim_cols_map[name] for name in self.index_column_names]
         dim_cols_tuple = tuple(dim_cols_list)
         self._handle.writer[dim_cols_tuple] = attr_cols_map
+        self._consolidate_and_vacuum_fragment_metadata()
 
         return self
 
     def _set_reader_coord(
         self, sr: clib.SOMAArray, dim_idx: int, dim: tiledb.Dim, coord: object
     ) -> bool:
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_dense_nd_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,15 @@
         Lifecycle:
             Experimental.
         """
         _util.check_type("values", values, (pa.Tensor,))
 
         del platform_config  # Currently unused.
         self._handle.writer[coords] = values.to_numpy()
+        self._consolidate_and_vacuum_fragment_metadata()
         return self
 
     @classmethod
     def _dim_capacity_and_extent(
         cls,
         dim_name: str,
         dim_shape: Optional[int],
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_exception.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_factory.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_sparse_nd_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,34 +185,37 @@
         del platform_config  # Currently unused.
 
         arr = self._handle.writer
 
         if isinstance(values, pa.SparseCOOTensor):
             data, coords = values.to_numpy()
             arr[tuple(c for c in coords.T)] = data
+            self._consolidate_and_vacuum_fragment_metadata()
             return self
 
         if isinstance(values, (pa.SparseCSCMatrix, pa.SparseCSRMatrix)):
             if self.ndim != 2:
                 raise ValueError(
                     f"Unable to write 2D Arrow sparse matrix to {self.ndim}D SparseNDArray"
                 )
             # TODO: the ``to_scipy`` function is not zero copy. Need to explore zero-copy options.
             sp = values.to_scipy().tocoo()
             arr[sp.row, sp.col] = sp.data
+            self._consolidate_and_vacuum_fragment_metadata()
             return self
 
         if isinstance(values, pa.Table):
             data = values.column("soma_data").to_numpy()
             coord_tbl = values.drop(["soma_data"])
             coords = tuple(
                 coord_tbl.column(f"soma_dim_{n}").to_numpy()
                 for n in range(coord_tbl.num_columns)
             )
             arr[coords] = data
+            self._consolidate_and_vacuum_fragment_metadata()
             return self
 
         raise TypeError(
             f"Unsupported Arrow type or non-arrow type for values argument: {type(values)}"
         )
 
     def _set_reader_coord(
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -184,7 +184,25 @@
         at the given URI, sets the necessary metadata, and returns a handle to
         the newly-created array, open for writing.
         """
         tiledb.Array.create(uri, schema, ctx=context.tiledb_ctx)
         handle = cls._wrapper_type.open(uri, "w", context, tiledb_timestamp)
         cls._set_create_metadata(handle)
         return handle
+
+    def _consolidate_and_vacuum_fragment_metadata(self) -> None:
+        """
+        This post-ingestion helper consolidates and vacuums fragment metadata and commit files --
+        this is quick to do, and positively impacts query performance.  It does _not_ consolidate
+        bulk array data, which is more time-consuming and should be done at the user's opt-in
+        discretion.
+        """
+
+        for mode in ["fragment_meta", "commits"]:
+
+            cfg = self._ctx.config()
+            cfg["sm.consolidation.mode"] = mode
+            cfg["sm.vacuum.mode"] = mode
+            ctx = tiledb.Ctx(cfg)
+
+            tiledb.consolidate(self.uri, ctx=ctx)
+            tiledb.vacuum(self.uri, ctx=ctx)
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_types.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/_util.py` & `tiledbsoma-1.2.4/src/tiledbsoma/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from itertools import zip_longest
 from typing import Any, Optional, Tuple, Type, TypeVar
 
 import somacore
 from somacore import options
 
 from ._types import OpenTimestamp, Slice, is_slice_of
+from .options._tiledb_create_options import TileDBCreateOptions
 
 
 def get_start_stamp() -> float:
     """Returns information about start time of an event.
 
     Nominally float seconds since the epoch, but articulated here
     as being compatible with the format_elapsed function.
@@ -256,7 +257,16 @@
 
     This may raise an exception, since millis may be outside the representable
     range for a Python datetime.
     """
     secs, millis = divmod(millis, 1000)
     dt = datetime.datetime.fromtimestamp(secs, tz=datetime.timezone.utc)
     return dt.replace(microsecond=millis * 1000)
+
+
+def validate_platform_config(platform_config: Any) -> None:
+    """Offers a run-time type check on this ingestion/creation argument, which is easy to miskey."""
+    if platform_config is not None:
+        if isinstance(platform_config, TileDBCreateOptions):
+            raise TypeError(
+                """platform_config argument is of type TileDBCreateOptions -- please wrap it in `{"tiledb": {"create": argument}}`."""
+            )
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/eta.py` & `tiledbsoma-1.2.4/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.2.4/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.2.4/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.2.4/src/tiledbsoma/io/ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,19 @@
     Args:
         experiment_uri: The experiment to create or update.
 
         input_path: A path to an input H5AD file.
 
         measurement_name: The name of the measurement to store data in.
 
+        context: Optional :class:`SOMATileDBContext` containing storage parameters, etc.
+
+        platform_config: Platform-specific options used to create this array, provided in the form
+        ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}`` nested keys.
+
         ingest_mode: The ingestion type to perform:
             - ``write``: Writes all data, creating new layers if the SOMA already exists.
             - ``resume``: Adds data to an existing SOMA, skipping writing data
               that was previously written. Useful for continuing after a partial
               or interrupted ingestion operation.
             - ``schema_only``: Creates groups and the array schema, without
               writing any data to the array. Useful to prepare for appending
@@ -173,14 +178,20 @@
     Args:
         experiment_uri: The experiment to create or update.
 
         input_path: A path to an input H5AD file.
 
         measurement_name: The name of the measurement to store data in.
 
+        context: Optional :class:`SOMATileDBContext` containing storage parameters, etc.
+
+        platform_config:
+            Platform-specific options used to create this array, provided in the form
+            ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}``.
+
         ingest_mode: The ingestion type to perform:
             - ``write``: Writes all data, creating new layers if the SOMA already exists.
             - ``resume``: Adds data to an existing SOMA, skipping writing data
               that was previously written. Useful for continuing after a partial
               or interrupted ingestion operation.
             - ``schema_only``: Creates groups and the array schema, without
               writing any data to the array. Useful to prepare for appending
@@ -201,14 +212,16 @@
         )
 
     if not isinstance(anndata, ad.AnnData):
         raise TypeError(
             "Second argument is not an AnnData object -- did you want from_h5ad?"
         )
 
+    _util.validate_platform_config(platform_config)
+
     context = _validate_soma_tiledb_context(context)
 
     # Without _at least_ an index, there is nothing to indicate the dimension indices.
     if anndata.obs.index.empty or anndata.var.index.empty:
         raise NotImplementedError("Empty AnnData.obs or AnnData.var unsupported.")
 
     s = _util.get_start_stamp()
@@ -225,40 +238,49 @@
     # Must be done first, to create the parent directory.
     experiment = _create_or_open_coll(
         Experiment, experiment_uri, ingest_mode, context=context
     )
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # OBS
-    df_uri = _util.uri_joinpath(experiment.uri, "obs")
+    df_uri = _util.uri_joinpath(experiment_uri, "obs")
     with _write_dataframe(
         df_uri,
         conversions.decategoricalize_obs_or_var(anndata.obs),
         id_column_name="obs_id",
         platform_config=platform_config,
         context=context,
         ingest_mode=ingest_mode,
     ) as obs:
         _maybe_set(experiment, "obs", obs, use_relative_uri=use_relative_uri)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # MS
+
+    # For local disk and S3, this is the same as experiment.ms.uri.
+    # For ingest_mode="resume" on TileDB Cloud, experiment_uri will be of the form
+    # tiledb://namespace/s3://bucket/path/to/exp whereas experiment.ms.uri will
+    # be of the form tiledb://namespace/uuid. Only for the former is it suitable
+    # to append "/ms" so that is what we do here.
+    experiment_ms_uri = f"{experiment_uri}/ms"
+
     with _create_or_open_coll(
         Collection[Measurement],
-        _util.uri_joinpath(experiment.uri, "ms"),
+        experiment_ms_uri,
         ingest_mode,
         context=context,
     ) as ms:
         _maybe_set(experiment, "ms", ms, use_relative_uri=use_relative_uri)
 
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         # MS/meas
+        measurement_uri = _util.uri_joinpath(experiment_ms_uri, measurement_name)
         with _create_or_open_coll(
             Measurement,
-            f"{experiment.ms.uri}/{measurement_name}",
+            measurement_uri,
             ingest_mode,
             context=context,
         ) as measurement:
             _maybe_set(
                 ms, measurement_name, measurement, use_relative_uri=use_relative_uri
             )
 
@@ -272,83 +294,86 @@
                 ingest_mode,
                 use_relative_uri=use_relative_uri,
             )
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/VAR
             with _write_dataframe(
-                _util.uri_joinpath(measurement.uri, "var"),
+                _util.uri_joinpath(measurement_uri, "var"),
                 conversions.decategoricalize_obs_or_var(anndata.var),
                 id_column_name="var_id",
                 platform_config=platform_config,
                 context=context,
                 ingest_mode=ingest_mode,
             ) as var:
                 _maybe_set(measurement, "var", var, use_relative_uri=use_relative_uri)
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/X/DATA
 
+            measurement_X_uri = _util.uri_joinpath(measurement_uri, "X")
             with _create_or_open_coll(
                 Collection,
-                _util.uri_joinpath(measurement.uri, "X"),
+                measurement_X_uri,
                 ingest_mode,
                 context=context,
             ) as x:
                 _maybe_set(measurement, "X", x, use_relative_uri=use_relative_uri)
 
                 # Since we did ``anndata = ad.read_h5ad(path_to_h5ad, "r")`` with the "r":
                 # * If we do ``anndata.X[:]`` we're loading all of a CSR/CSC/etc into memory.
                 # * If we do ``anndata.X`` we're getting a pageable object which can be loaded
                 #   chunkwise into memory.
                 # Using the latter allows us to ingest larger .h5ad files without OOMing.
 
                 with create_from_matrix(
                     X_kind,
-                    _util.uri_joinpath(measurement.X.uri, "data"),
+                    _util.uri_joinpath(measurement_X_uri, "data"),
                     anndata.X,
                     platform_config,
                     ingest_mode,
                     context,
                 ) as data:
                     _maybe_set(x, "data", data, use_relative_uri=use_relative_uri)
 
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/meas/OBSM,VARM,OBSP,VARP
                 if len(anndata.obsm.keys()) > 0:  # do not create an empty collection
+                    obsm_uri = _util.uri_joinpath(measurement_uri, "obsm")
                     with _create_or_open_coll(
                         Collection,
-                        _util.uri_joinpath(measurement.uri, "obsm"),
+                        obsm_uri,
                         ingest_mode,
                         context=context,
                     ) as obsm:
                         _maybe_set(
                             measurement, "obsm", obsm, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsm.keys():
                             with create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
-                                _util.uri_joinpath(measurement.obsm.uri, key),
+                                _util.uri_joinpath(obsm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsm[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
                                 context=context,
                             ) as arr:
                                 _maybe_set(
                                     obsm, key, arr, use_relative_uri=use_relative_uri
                                 )
                             arr.close()
                     measurement.obsm.close()
 
                 if len(anndata.varm.keys()) > 0:  # do not create an empty collection
+                    _util.uri_joinpath(measurement_uri, "varm")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varm"),
                         ingest_mode,
                         context=context,
                     ) as varm:
                         _maybe_set(
@@ -356,15 +381,15 @@
                         )
                         for key in anndata.varm.keys():
                             with create_from_matrix(
                                 # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
                                 # consider a use-dense flag at the tiledbsoma.io API
                                 # DenseNDArray,
                                 SparseNDArray,
-                                _util.uri_joinpath(measurement.varm.uri, key),
+                                _util.uri_joinpath(varm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varm[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
                                 context=context,
                             ) as darr:
@@ -372,27 +397,28 @@
                                     varm,
                                     key,
                                     darr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.obsp.keys()) > 0:  # do not create an empty collection
+                    _util.uri_joinpath(measurement_uri, "obsp")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "obsp"),
                         ingest_mode,
                         context=context,
                     ) as obsp:
                         _maybe_set(
                             measurement, "obsp", obsp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsp.keys():
                             with create_from_matrix(
                                 SparseNDArray,
-                                _util.uri_joinpath(measurement.obsp.uri, key),
+                                _util.uri_joinpath(obsp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsp[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
                                 context=context,
                             ) as sarr:
@@ -400,27 +426,28 @@
                                     obsp,
                                     key,
                                     sarr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.varp.keys()) > 0:  # do not create an empty collection
+                    _util.uri_joinpath(measurement_uri, "obsp")
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varp"),
                         ingest_mode,
                         context=context,
                     ) as varp:
                         _maybe_set(
                             measurement, "varp", varp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varp.keys():
                             with create_from_matrix(
                                 SparseNDArray,
-                                _util.uri_joinpath(measurement.varp.uri, key),
+                                _util.uri_joinpath(varp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varp[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
                                 context=context,
                             ) as sarr:
@@ -430,58 +457,60 @@
                                     sarr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/RAW
                 if anndata.raw is not None:
+                    raw_uri = _util.uri_joinpath(experiment_ms_uri, "raw")
                     with _create_or_open_coll(
                         Measurement,
-                        _util.uri_joinpath(experiment.ms.uri, "raw"),
+                        raw_uri,
                         ingest_mode,
                         context=context,
                     ) as raw_measurement:
                         _maybe_set(
                             ms,
                             "raw",
                             raw_measurement,
                             use_relative_uri=use_relative_uri,
                         )
 
                         with _write_dataframe(
-                            _util.uri_joinpath(raw_measurement.uri, "var"),
+                            _util.uri_joinpath(raw_uri, "var"),
                             conversions.decategoricalize_obs_or_var(anndata.raw.var),
                             id_column_name="var_id",
                             platform_config=platform_config,
                             context=context,
                             ingest_mode=ingest_mode,
                         ) as var:
                             _maybe_set(
                                 raw_measurement,
                                 "var",
                                 var,
                                 use_relative_uri=use_relative_uri,
                             )
 
+                        raw_X_uri = _util.uri_joinpath(raw_uri, "X")
                         with _create_or_open_coll(
                             Collection,
-                            _util.uri_joinpath(raw_measurement.uri, "X"),
+                            raw_X_uri,
                             ingest_mode,
                             context=context,
                         ) as rm_x:
                             _maybe_set(
                                 raw_measurement,
                                 "X",
                                 rm_x,
                                 use_relative_uri=use_relative_uri,
                             )
 
                             with create_from_matrix(
                                 SparseNDArray,
-                                _util.uri_joinpath(raw_measurement.X.uri, "data"),
+                                _util.uri_joinpath(raw_X_uri, "data"),
                                 anndata.raw.X,
                                 platform_config,
                                 ingest_mode,
                                 context=context,
                             ) as rm_x_data:
                                 _maybe_set(
                                     rm_x,
@@ -646,14 +675,16 @@
 ) -> _NDArr:
     """
     Create and populate the ``soma_matrix`` from the contents of ``matrix``.
 
     Lifecycle:
         Experimental.
     """
+    _util.validate_platform_config(platform_config)
+
     # SparseDataset has no ndim but it has a shape
     if len(matrix.shape) != 2:
         raise ValueError(f"expected matrix.shape == 2; got {matrix.shape}")
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {uri}")
 
@@ -1029,15 +1060,25 @@
     coords = [slice(None), slice(None)]
     i = 0
     while i < dim_max_size:
         t1 = time.time()
 
         # Chunk size on the stride axis
         if isinstance(matrix, (np.ndarray, h5py.Dataset)):
-            chunk_size = int(math.ceil(goal_chunk_nnz / matrix.shape[stride_axis]))
+            # These are dense, being ingested as sparse.
+            # Example:
+            # * goal_chunk_nnz = 100M
+            # * An obsm element has shape (32458, 2)
+            # * stride_axis = 0 (ingest row-wise)
+            # * We want ceiling of 100M / 2 to obtain chunk_size = 50M rows
+            # * This attains goal_chunk_nnz = 100_000_000 since we have 50M rows
+            #   with 2 elements each
+            # * Result: we divide by the shape, slotted by the non-stride axis
+            non_stride_axis = 1 - stride_axis
+            chunk_size = int(math.ceil(goal_chunk_nnz / matrix.shape[non_stride_axis]))
         else:
             chunk_size = _find_sparse_chunk_size(  # type: ignore [unreachable]
                 matrix, i, stride_axis, goal_chunk_nnz
             )
 
         i2 = i + chunk_size
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/logging.py` & `tiledbsoma-1.2.4/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.2.4/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.2.4/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from somacore import options
 
 DEFAULT_TILE_ORDER = "row-major"
 DEFAULT_CELL_ORDER = "row-major"
 DEFAULT_DATAFRAME_DIM_ZSTD_LEVEL = 3
 DEFAULT_SPARSE_ND_ARRAY_DIM_ZSTD_LEVEL = 3
 DEFAULT_WRITE_X_CHUNKED = True
-DEFAULT_GOAL_CHUNK_NNZ = 200_000_000
+DEFAULT_GOAL_CHUNK_NNZ = 100_000_000
 DEFAULT_OFFSET_FILTERS = (
     "DoubleDeltaFilter",
     "BitWidthReductionFilter",
     "ZstdFilter",
 )
 DEFAULT_VALIDITY_FILTERS = None
 DEFAULT_TILE_EXTENT = 2048
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.2.4/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.2.4/src/tiledbsoma/query_condition.cc`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 #include <exception>
 
 // #define TILEDB_DEPRECATED
 // #define TILEDB_DEPRECATED_EXPORT
 
 // #include "util.h"
 #include <tiledb/tiledb> // C++
+#include <tiledbsoma/tiledbsoma>
 
-#include "tiledbsoma/logger_public.h"
 #define TPY_ERROR_LOC(m) throw tiledbsoma::TileDBSOMAError(m);
 
 #if TILEDB_VERSION_MAJOR == 2 && TILEDB_VERSION_MINOR >= 2
 
 #if !defined(NDEBUG)
 //#include "debug.cc"
 #endif
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.2.4/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.3/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.2.4/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 dist_links/libtiledbsoma/src/external/.clang-format
 dist_links/libtiledbsoma/src/external/include/span/span.hpp
 dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
 dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
 dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
 dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
 dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+dist_links/libtiledbsoma/src/soma/logger_public.h
 dist_links/libtiledbsoma/src/soma/managed_query.cc
 dist_links/libtiledbsoma/src/soma/managed_query.h
 dist_links/libtiledbsoma/src/soma/soma_array.cc
 dist_links/libtiledbsoma/src/soma/soma_array.h
-dist_links/libtiledbsoma/src/tiledbsoma/logger_public.h
+dist_links/libtiledbsoma/src/soma/soma_group.cc
+dist_links/libtiledbsoma/src/soma/soma_group.h
 dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
 dist_links/libtiledbsoma/src/utils/array_buffers.h
 dist_links/libtiledbsoma/src/utils/arrow_adapter.h
 dist_links/libtiledbsoma/src/utils/carrow.h
 dist_links/libtiledbsoma/src/utils/column_buffer.cc
 dist_links/libtiledbsoma/src/utils/column_buffer.h
 dist_links/libtiledbsoma/src/utils/common.h
@@ -52,14 +54,15 @@
 dist_links/libtiledbsoma/test/CMakeLists.txt
 dist_links/libtiledbsoma/test/test_query_condition.py
 dist_links/libtiledbsoma/test/test_simple.py
 dist_links/libtiledbsoma/test/test_soma_array.py
 dist_links/libtiledbsoma/test/unit_column_buffer.cc
 dist_links/libtiledbsoma/test/unit_managed_query.cc
 dist_links/libtiledbsoma/test/unit_soma_array.cc
+dist_links/libtiledbsoma/test/unit_soma_group.cc
 dist_links/libtiledbsoma/test/unit_thread_pool.cc
 dist_links/scripts/README.md
 dist_links/scripts/bld
 dist_links/scripts/run-clang-format.sh
 dist_links/scripts/show-versions.py
 dist_links/scripts/update-tiledb-version.py
 src/tiledbsoma/__init__.py
```

### Comparing `tiledbsoma-1.2.3/version.py` & `tiledbsoma-1.2.4/version.py`

 * *Files identical despite different names*

