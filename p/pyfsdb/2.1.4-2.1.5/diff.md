# Comparing `tmp/pyfsdb-2.1.4.tar.gz` & `tmp/pyfsdb-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-2.1.4.tar", last modified: Tue May 16 17:45:43 2023, max compression
+gzip compressed data, was "pyfsdb-2.1.5.tar", last modified: Tue May 23 21:00:24 2023, max compression
```

## Comparing `pyfsdb-2.1.4.tar` & `pyfsdb-2.1.5.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.790657 pyfsdb-2.1.4/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-03-18 13:10:45.000000 pyfsdb-2.1.4/LICENSE
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-16 17:45:43.789657 pyfsdb-2.1.4/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-17 14:56:42.000000 pyfsdb-2.1.4/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.604657 pyfsdb-2.1.4/pyfsdb/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/__init__.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35086 2023-01-25 14:19:32.000000 pyfsdb-2.1.4/pyfsdb/fsdb.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.609657 pyfsdb-2.1.4/pyfsdb/obsolete/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.4/pyfsdb/obsolete/__init__.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/db2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbensure.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbformat.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbfullpivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbheatmap.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbnormalize.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbreescape.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbsplitter.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbtopn.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/obsolete/dbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.788657 pyfsdb-2.1.4/pyfsdb/tools/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2021-04-11 14:12:46.000000 pyfsdb-2.1.4/pyfsdb/tools/__init__.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/bro2fsdb.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/fsdb2json.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/fsdb2many.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/json2fsdb.py
--rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-11-12 21:47:13.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2sql.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-05 01:36:03.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2tex.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdb2to1.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbaddtypes.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2023-01-06 15:32:58.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbaugment.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbcdf.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3430 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbcoluniq.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbdatetoepoch.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-05 01:16:54.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbensure.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbepochtodate.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbformat.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbfullpivot.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbheatmap.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-21 22:46:03.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbjinja.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbkeyedsort.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbnormalize.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbreescape.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbreversepivot.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-21 13:26:37.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbroc.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3230 2023-05-13 04:31:26.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbrow.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3524 2023-05-11 20:36:19.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbroweval.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbsplitter.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbsum.py
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-08-02 01:33:45.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbtopn.py
--rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-02-06 19:45:06.000000 pyfsdb-2.1.4/pyfsdb/tools/pdbzerofill.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-16 17:45:43.605657 pyfsdb-2.1.4/pyfsdb.egg-info/
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/PKG-INFO
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1505 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/SOURCES.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/dependency_links.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/entry_points.txt
--rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        7 2023-05-16 17:45:43.000000 pyfsdb-2.1.4/pyfsdb.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-16 17:45:43.790657 pyfsdb-2.1.4/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-16 17:45:09.000000 pyfsdb-2.1.4/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1127 2021-04-12 16:27:12.000000 pyfsdb-2.1.5/LICENSE
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     5649 2023-01-11 15:10:15.000000 pyfsdb-2.1.5/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.815670 pyfsdb-2.1.5/mod/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2020-10-09 02:50:07.000000 pyfsdb-2.1.5/mod/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       21 2020-10-09 02:49:47.000000 pyfsdb-2.1.5/mod/ick.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.815670 pyfsdb-2.1.5/pyfsdb/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      167 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/__init__.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)    35299 2023-05-23 20:58:56.000000 pyfsdb-2.1.5/pyfsdb/fsdb.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.817669 pyfsdb-2.1.5/pyfsdb/obsolete/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/__init__.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/db2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      226 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbdatetoepoch.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbensure.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      206 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbformat.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbfullpivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      210 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbheatmap.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      218 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbnormalize.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbreescape.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      230 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbreversepivot.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbsplitter.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      194 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      198 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbtopn.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)      214 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/obsolete/dbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/pyfsdb/tools/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        0 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/__init__.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1989 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/bro2fsdb.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3355 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/fsdb2json.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1868 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/fsdb2many.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2360 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/json2fsdb.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10589 2022-10-25 20:28:42.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2sql.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2845 2023-01-10 17:33:49.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2tex.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1133 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdb2to1.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     2665 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbaddtypes.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     7015 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbaugment.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3510 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbcdf.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     3430 2023-01-10 19:40:21.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbcoluniq.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1866 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbdatetoepoch.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     2134 2023-01-10 17:33:49.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbensure.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1900 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbepochtodate.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1398 2023-01-11 16:18:55.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbformat.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3022 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbfullpivot.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)    10044 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbheatmap.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2373 2023-01-23 22:31:04.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbjinja.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3707 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbkeyedsort.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1570 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbnormalize.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     1426 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbreescape.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     2663 2023-01-27 16:33:47.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbreversepivot.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3585 2022-08-15 21:23:13.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbroc.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3230 2023-05-23 20:59:33.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbrow.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3524 2023-05-23 20:59:33.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbroweval.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3513 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbsplitter.py
+-rwxrwxr-x   0 hardaker  (2174) hardaker  (2174)     3075 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbsum.py
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     3357 2022-07-13 23:54:39.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbtopn.py
+-rwxr-xr-x   0 hardaker  (2174) hardaker  (2174)     2297 2023-05-03 15:01:57.000000 pyfsdb-2.1.5/pyfsdb/tools/pdbzerofill.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 21:00:24.816670 pyfsdb-2.1.5/pyfsdb.egg-info/
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     6054 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/PKG-INFO
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1532 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)     1861 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/entry_points.txt
+-rw-rw-r--   0 hardaker  (2174) hardaker  (2174)       11 2023-05-23 21:00:24.000000 pyfsdb-2.1.5/pyfsdb.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-23 21:00:24.822670 pyfsdb-2.1.5/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     3323 2023-05-23 20:59:58.000000 pyfsdb-2.1.5/setup.py
```

### Comparing `pyfsdb-2.1.4/LICENSE` & `pyfsdb-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/PKG-INFO` & `pyfsdb-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.4
+Version: 2.1.5
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.4/README.md` & `pyfsdb-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/fsdb.py` & `pyfsdb-2.1.5/pyfsdb/fsdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,19 @@
 
         This must be set prior to writing the first row, and modifies
         the internal output_header_line too."""
         if len(self._out_column_names) == 0:
             self._out_column_names = self.column_names
         return self._out_column_names
 
+    @property
+    def comments(self):
+        """Returns a list of comments seen in the document"""
+        return self._comments
+
     @out_column_names.setter
     def out_column_names(self, values):
         mapping = self.__create_column_name_mapping__(values)
 
     # support functions
 
     def create_header_line(self, columns=None, separator_token=None, init_row=None):
@@ -660,14 +665,17 @@
 
                 self._write_header_line()
 
             if self._pass_comments == "y":
                 self._out_file_handle.write(line)
             else:
                 self._comments.append(line)
+        elif self._save_command_history:
+            self._comments.append(line)
+
         return next(self.fileh)
 
     def _convert_array_values(self, row):
         for (n, converter) in enumerate(self._converters):
             if row[n] == "-" or row[n] == "":
                 row[n] = None
             elif converter is not None and row[n] is not None:
```

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/bro2fsdb.py` & `pyfsdb-2.1.5/pyfsdb/tools/bro2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/fsdb2json.py` & `pyfsdb-2.1.5/pyfsdb/tools/fsdb2json.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/fsdb2many.py` & `pyfsdb-2.1.5/pyfsdb/tools/fsdb2many.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/json2fsdb.py` & `pyfsdb-2.1.5/pyfsdb/tools/json2fsdb.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdb2sql.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdb2sql.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdb2tex.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdb2tex.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdb2to1.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdb2to1.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbaddtypes.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbaddtypes.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbaugment.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbaugment.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbcdf.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbcdf.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbcoluniq.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbcoluniq.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbdatetoepoch.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbdatetoepoch.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbensure.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbensure.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbepochtodate.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbepochtodate.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbformat.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbformat.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbfullpivot.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbfullpivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbheatmap.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbheatmap.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbjinja.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbjinja.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbkeyedsort.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbkeyedsort.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbnormalize.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbnormalize.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbreescape.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbreescape.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbreversepivot.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbreversepivot.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbroc.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbroc.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbrow.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbrow.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbroweval.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbroweval.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbsplitter.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbsplitter.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbsum.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbsum.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbtopn.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbtopn.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb/tools/pdbzerofill.py` & `pyfsdb-2.1.5/pyfsdb/tools/pdbzerofill.py`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/pyfsdb.egg-info/PKG-INFO` & `pyfsdb-2.1.5/pyfsdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb
-Version: 2.1.4
+Version: 2.1.5
 Summary: A python implementation of the flat-file streaming database
 Home-page: https://github.com/gawseed/pyfsdb
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-2.1.4/pyfsdb.egg-info/SOURCES.txt` & `pyfsdb-2.1.5/pyfsdb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
 README.md
 setup.py
+mod/__init__.py
+mod/ick.py
 pyfsdb/__init__.py
 pyfsdb/fsdb.py
 pyfsdb.egg-info/PKG-INFO
 pyfsdb.egg-info/SOURCES.txt
 pyfsdb.egg-info/dependency_links.txt
 pyfsdb.egg-info/entry_points.txt
 pyfsdb.egg-info/top_level.txt
```

### Comparing `pyfsdb-2.1.4/pyfsdb.egg-info/entry_points.txt` & `pyfsdb-2.1.5/pyfsdb.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pyfsdb-2.1.4/setup.py` & `pyfsdb-2.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb",
-    version="2.1.4",
+    version="2.1.5",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A python implementation of the flat-file streaming database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb",
     packages=setuptools.find_packages(),
```

