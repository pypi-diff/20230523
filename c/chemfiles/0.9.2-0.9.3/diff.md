# Comparing `tmp/chemfiles-0.9.2.tar.gz` & `tmp/chemfiles-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chemfiles-0.9.2.tar", last modified: Wed Jan  8 12:37:56 2020, max compression
+gzip compressed data, was "dist/chemfiles-0.9.3.tar", last modified: Thu Feb  6 21:29:39 2020, max compression
```

## Comparing `chemfiles-0.9.2.tar` & `chemfiles-0.9.3.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/
--rw-r--r--   0 guillaume   (501) staff       (20)     3661 2020-01-08 12:37:56.000000 chemfiles-0.9.2/PKG-INFO
--rw-r--r--   0 guillaume   (501) staff       (20)     1884 2019-12-17 11:23:00.000000 chemfiles-0.9.2/CMakeLists.txt
--rw-r--r--   0 guillaume   (501) staff       (20)     1478 2018-01-16 16:10:32.000000 chemfiles-0.9.2/LICENSE
--rw-r--r--   0 guillaume   (501) staff       (20)       13 2018-01-16 16:10:32.000000 chemfiles-0.9.2/requirements.txt
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/chemfiles/
--rw-r--r--   0 guillaume   (501) staff       (20)     2251 2019-03-13 21:38:39.000000 chemfiles-0.9.2/chemfiles/misc.py
--rw-r--r--   0 guillaume   (501) staff       (20)     2594 2019-12-17 11:22:55.000000 chemfiles-0.9.2/chemfiles/property.py
--rw-r--r--   0 guillaume   (501) staff       (20)     5285 2019-12-17 11:22:55.000000 chemfiles-0.9.2/chemfiles/cell.py
--rw-r--r--   0 guillaume   (501) staff       (20)      451 2020-01-08 12:24:44.000000 chemfiles-0.9.2/chemfiles/__init__.py
--rw-r--r--   0 guillaume   (501) staff       (20)     4921 2019-12-17 11:23:00.000000 chemfiles-0.9.2/chemfiles/trajectory.py
--rw-r--r--   0 guillaume   (501) staff       (20)     5109 2019-12-17 11:22:55.000000 chemfiles-0.9.2/chemfiles/residue.py
--rw-r--r--   0 guillaume   (501) staff       (20)       26 2018-01-16 16:10:32.000000 chemfiles-0.9.2/chemfiles/.gitignore
--rw-r--r--   0 guillaume   (501) staff       (20)     3310 2019-07-09 21:43:23.000000 chemfiles-0.9.2/chemfiles/utils.py
--rw-r--r--   0 guillaume   (501) staff       (20)     2872 2019-03-13 21:38:39.000000 chemfiles-0.9.2/chemfiles/clib.py
--rw-r--r--   0 guillaume   (501) staff       (20)    12449 2019-12-17 11:22:55.000000 chemfiles-0.9.2/chemfiles/frame.py
--rw-r--r--   0 guillaume   (501) staff       (20)    10281 2019-07-09 21:43:23.000000 chemfiles-0.9.2/chemfiles/topology.py
--rw-r--r--   0 guillaume   (501) staff       (20)     2981 2019-07-09 21:43:23.000000 chemfiles-0.9.2/chemfiles/selection.py
--rw-r--r--   0 guillaume   (501) staff       (20)     6126 2019-12-17 11:22:55.000000 chemfiles-0.9.2/chemfiles/atom.py
--rw-r--r--   0 guillaume   (501) staff       (20)    33798 2019-07-09 21:43:23.000000 chemfiles-0.9.2/chemfiles/ffi.py
--rw-r--r--   0 guillaume   (501) staff       (20)     2657 2019-03-20 22:18:37.000000 chemfiles-0.9.2/README.md
--rw-r--r--   0 guillaume   (501) staff       (20)     2054 2020-01-08 12:30:32.000000 chemfiles-0.9.2/setup.py
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/
--rw-r--r--   0 guillaume   (501) staff       (20)     8439 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/CMakeLists.txt
--rw-r--r--   0 guillaume   (501) staff       (20)      146 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/.codecov.yml
--rw-r--r--   0 guillaume   (501) staff       (20)     1535 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/LICENSE
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/cmake/
--rw-r--r--   0 guillaume   (501) staff       (20)       94 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/thread_local.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1066 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/uninstall.in.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)    10848 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/cmake/CompilerFlags.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)     1892 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/cmake/chemfiles-iwyu.imp
--rw-r--r--   0 guillaume   (501) staff       (20)     1798 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/ParseArguments.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)     2142 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/cmake/IncludeWhatYouUse.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)     1173 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/chemfiles-config-version.cmake.in
--rw-r--r--   0 guillaume   (501) staff       (20)     8741 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/FindPythonLibsNew.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)      121 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/cmake/chemfiles-config.cmake.in
--rw-r--r--   0 guillaume   (501) staff       (20)      364 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/InitRules.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)     3513 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/FindNetCDF.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)     4283 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/cmake/FindSphinx.cmake
--rw-r--r--   0 guillaume   (501) staff       (20)    16315 2020-01-08 12:24:06.000000 chemfiles-0.9.2/lib/CHANGELOG.md
--rw-r--r--   0 guillaume   (501) staff       (20)      355 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/AUTHORS
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/
--rw-r--r--   0 guillaume   (501) staff       (20)      611 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles.h
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/
--rw-r--r--   0 guillaume   (501) staff       (20)     1455 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/include/chemfiles/periodic_table.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     9315 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Trajectory.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3032 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/pdb_connectivity.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    10280 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Topology.hpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/
--rw-r--r--   0 guillaume   (501) staff       (20)     8220 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/LAMMPSData.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      913 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/TRR.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1013 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/GRO.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      845 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/XYZ.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1385 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/CML.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      884 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/XTC.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3218 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/Molfile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      898 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/SDF.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2790 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/MMTF.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1631 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/TNG.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      941 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/CSSR.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1297 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/MOL2.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3021 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/SMI.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3175 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/PDB.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1815 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/mmCIF.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1766 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/AmberNetCDF.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1160 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/formats/Tinker.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     4462 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Selection.hpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/selections/
--rw-r--r--   0 guillaume   (501) staff       (20)     2558 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/selections/parser.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    19300 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/selections/expr.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6316 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/selections/lexer.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6632 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/UnitCell.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      902 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/unreachable.hpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/
--rw-r--r--   0 guillaume   (501) staff       (20)     6253 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/types.h
--rw-r--r--   0 guillaume   (501) staff       (20)     2239 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/misc.h
--rw-r--r--   0 guillaume   (501) staff       (20)     6671 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/shared_allocator.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6442 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/cell.h
--rw-r--r--   0 guillaume   (501) staff       (20)    13990 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/frame.h
--rw-r--r--   0 guillaume   (501) staff       (20)     5906 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/trajectory.h
--rw-r--r--   0 guillaume   (501) staff       (20)    10379 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/atom.h
--rw-r--r--   0 guillaume   (501) staff       (20)     8774 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/residue.h
--rw-r--r--   0 guillaume   (501) staff       (20)     4759 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/property.h
--rw-r--r--   0 guillaume   (501) staff       (20)    11327 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/topology.h
--rw-r--r--   0 guillaume   (501) staff       (20)     6220 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/utils.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     4078 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/capi/selection.h
--rw-r--r--   0 guillaume   (501) staff       (20)     7228 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/File.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    11551 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/Connectivity.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3412 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/Configuration.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2519 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/error_fmt.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1597 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/Error.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2201 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/FormatFactory.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     9194 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/Property.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3171 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/sorted_set.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8052 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Atom.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2321 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/string_view.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5282 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Residue.hpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/files/
--rw-r--r--   0 guillaume   (501) staff       (20)      847 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/PlainFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6878 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/NcFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1058 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/files/TNGFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1289 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/Bz2File.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      995 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/GzFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1953 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/XDRFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1447 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/files/XzFile.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      892 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/config.in.h
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/include/chemfiles/external/
--rw-r--r--   0 guillaume   (501) staff       (20)     7149 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/include/chemfiles/external/span.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    28694 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/include/chemfiles/external/optional.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    41172 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/external/string_view.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1982 2019-12-17 11:23:03.000000 chemfiles-0.9.2/lib/include/chemfiles/mutex.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2407 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/utils.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    14259 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/types.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)    13552 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Frame.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      785 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles/warnings.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5883 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/Format.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6540 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/parse.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1813 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/include/chemfiles/misc.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)      597 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/include/chemfiles.hpp
--rw-r--r--   0 guillaume   (501) staff       (20)   105958 2019-03-13 21:26:44.000000 chemfiles-0.9.2/lib/Doxyfile.in
--rw-r--r--   0 guillaume   (501) staff       (20)     8085 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/README.md
--rw-r--r--   0 guillaume   (501) staff       (20)     1466 2019-12-17 11:23:03.000000 chemfiles-0.9.2/lib/appveyor.yml
--rw-r--r--   0 guillaume   (501) staff       (20)       22 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/.gitignore
--rw-r--r--   0 guillaume   (501) staff       (20)        6 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/VERSION
--rw-r--r--   0 guillaume   (501) staff       (20)     3200 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/Contributing.md
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/examples/
--rw-r--r--   0 guillaume   (501) staff       (20)      986 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/examples/CMakeLists.txt
--rw-r--r--   0 guillaume   (501) staff       (20)      685 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/examples/README.md
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/examples/cpp/
--rw-r--r--   0 guillaume   (501) staff       (20)      705 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/examples/cpp/indexes.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)      751 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/examples/cpp/select.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)      591 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/examples/cpp/generate.cpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/examples/c/
--rw-r--r--   0 guillaume   (501) staff       (20)      967 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/examples/c/generate.c
--rw-r--r--   0 guillaume   (501) staff       (20)     1758 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/examples/c/select.c
--rw-r--r--   0 guillaume   (501) staff       (20)      991 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/examples/c/indexes.c
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/scripts/
--rwxr-xr-x   0 guillaume   (501) staff       (20)     1791 2019-12-17 11:23:03.000000 chemfiles-0.9.2/lib/scripts/tidy.sh
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/scripts/ci/
--rwxr-xr-x   0 guillaume   (501) staff       (20)     2880 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/scripts/ci/check-public-headers.py
--rwxr-xr-x   0 guillaume   (501) staff       (20)     3141 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/scripts/ci/lint-code.py
--rwxr-xr-x   0 guillaume   (501) staff       (20)     3794 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/scripts/ci/check-capi-docs.py
--rw-r--r--   0 guillaume   (501) staff       (20)     2891 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/scripts/ci/setup-travis.sh
--rwxr-xr-x   0 guillaume   (501) staff       (20)     1155 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/scripts/ci/check-exported-symbols.py
--rw-r--r--   0 guillaume   (501) staff       (20)      860 2019-12-17 11:23:03.000000 chemfiles-0.9.2/lib/scripts/ci/setup-appveyor.ps1
--rwxr-xr-x   0 guillaume   (501) staff       (20)     1064 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/scripts/ci/build-docs.sh
--rw-r--r--   0 guillaume   (501) staff       (20)      311 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/scripts/ci/filter-textcoal-warnings.py
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/scripts/generate/
--rwxr-xr-x   0 guillaume   (501) staff       (20)     2674 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/scripts/generate/periodic_table.py
--rwxr-xr-x   0 guillaume   (501) staff       (20)     4050 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/scripts/generate/pdb_connectivity.py
--rwxr-xr-x   0 guillaume   (501) staff       (20)     1831 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/scripts/boost.sh
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/external/
--rw-r--r--   0 guillaume   (501) staff       (20)   255856 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/lzma.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   451385 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/mmtf-cpp.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)     7624 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/CMakeLists.txt
--rw-r--r--   0 guillaume   (501) staff       (20)   329575 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/tng.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   162586 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/zlib.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   487169 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/molfiles.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   513021 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/netcdf.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)    14644 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/README.md
--rw-r--r--   0 guillaume   (501) staff       (20)    70868 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/toml11.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)  1079347 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/xdrfile.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   364541 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/external/bzip2.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   374387 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/pugixml.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)   689394 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/external/fmt.tar.gz
--rw-r--r--   0 guillaume   (501) staff       (20)       36 2017-12-10 15:59:10.000000 chemfiles-0.9.2/lib/.git
--rw-r--r--   0 guillaume   (501) staff       (20)     3305 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/.travis.yml
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/src/
--rw-r--r--   0 guillaume   (501) staff       (20)     1878 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/utils.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6326 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Frame.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)      813 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/warnings.cpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/src/formats/
--rw-r--r--   0 guillaume   (501) staff       (20)    23938 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/SMI.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    27025 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/PDB.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8295 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/AmberNetCDF.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    15034 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/mmCIF.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5608 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/Tinker.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5936 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/XTC.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    12006 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/Molfile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    11322 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/SDF.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    18572 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/MMTF.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     9335 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/TNG.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5891 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/CSSR.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    10194 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/MOL2.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2524 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/XYZ.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    21787 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/CML.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    34103 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/LAMMPSData.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8182 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/TRR.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     9336 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/formats/GRO.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3183 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Format.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5985 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/parse.cpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/src/selections/
--rw-r--r--   0 guillaume   (501) staff       (20)    20576 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/selections/expr.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8482 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/selections/lexer.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    21685 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/selections/parser.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6646 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/FormatFactory.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3035 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Property.cpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/src/capi/
--rw-r--r--   0 guillaume   (501) staff       (20)     8735 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/capi/frame.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     1423 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/misc.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3090 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/property.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6920 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/capi/atom.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     4416 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/cell.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5950 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/capi/residue.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)      303 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/shared_allocator.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3340 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/trajectory.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8740 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/topology.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3003 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/capi/selection.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2918 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/Atom.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)      772 2019-12-17 11:25:26.000000 chemfiles-0.9.2/lib/src/Residue.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6191 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/File.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     6875 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Connectivity.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     7008 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Configuration.cpp
-drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-01-08 12:37:56.000000 chemfiles-0.9.2/lib/src/files/
--rw-r--r--   0 guillaume   (501) staff       (20)     2596 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/GzFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     3087 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/XDRFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5287 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/XzFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     7052 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/NcFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2192 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/TNGFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     5278 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/Bz2File.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     2478 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/files/PlainFile.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     8966 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/src/periodic_table.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     7042 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Trajectory.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)    17470 2019-01-26 13:01:21.000000 chemfiles-0.9.2/lib/src/pdb_connectivity.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     4522 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Topology.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     9200 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/Selection.cpp
--rw-r--r--   0 guillaume   (501) staff       (20)     7638 2019-12-17 11:25:29.000000 chemfiles-0.9.2/lib/src/UnitCell.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/
+-rw-r--r--   0 guillaume   (501) staff       (20)     3661 2020-02-06 21:29:39.000000 chemfiles-0.9.3/PKG-INFO
+-rw-r--r--   0 guillaume   (501) staff       (20)     1884 2019-12-17 11:23:00.000000 chemfiles-0.9.3/CMakeLists.txt
+-rw-r--r--   0 guillaume   (501) staff       (20)     1478 2018-01-16 16:10:32.000000 chemfiles-0.9.3/LICENSE
+-rw-r--r--   0 guillaume   (501) staff       (20)       13 2018-01-16 16:10:32.000000 chemfiles-0.9.3/requirements.txt
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/chemfiles/
+-rw-r--r--   0 guillaume   (501) staff       (20)     2251 2019-03-13 21:38:39.000000 chemfiles-0.9.3/chemfiles/misc.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     2594 2019-12-17 11:22:55.000000 chemfiles-0.9.3/chemfiles/property.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     5285 2019-12-17 11:22:55.000000 chemfiles-0.9.3/chemfiles/cell.py
+-rw-r--r--   0 guillaume   (501) staff       (20)      451 2020-02-06 21:28:35.000000 chemfiles-0.9.3/chemfiles/__init__.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     4921 2019-12-17 11:23:00.000000 chemfiles-0.9.3/chemfiles/trajectory.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     5109 2019-12-17 11:22:55.000000 chemfiles-0.9.3/chemfiles/residue.py
+-rw-r--r--   0 guillaume   (501) staff       (20)       26 2018-01-16 16:10:32.000000 chemfiles-0.9.3/chemfiles/.gitignore
+-rw-r--r--   0 guillaume   (501) staff       (20)     3310 2019-07-09 21:43:23.000000 chemfiles-0.9.3/chemfiles/utils.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     2872 2019-03-13 21:38:39.000000 chemfiles-0.9.3/chemfiles/clib.py
+-rw-r--r--   0 guillaume   (501) staff       (20)    12449 2019-12-17 11:22:55.000000 chemfiles-0.9.3/chemfiles/frame.py
+-rw-r--r--   0 guillaume   (501) staff       (20)    10281 2019-07-09 21:43:23.000000 chemfiles-0.9.3/chemfiles/topology.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     2981 2019-07-09 21:43:23.000000 chemfiles-0.9.3/chemfiles/selection.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     6126 2019-12-17 11:22:55.000000 chemfiles-0.9.3/chemfiles/atom.py
+-rw-r--r--   0 guillaume   (501) staff       (20)    33798 2019-07-09 21:43:23.000000 chemfiles-0.9.3/chemfiles/ffi.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     2657 2019-03-20 22:18:37.000000 chemfiles-0.9.3/README.md
+-rw-r--r--   0 guillaume   (501) staff       (20)     2054 2020-01-08 12:30:32.000000 chemfiles-0.9.3/setup.py
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/
+-rw-r--r--   0 guillaume   (501) staff       (20)     8674 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/CMakeLists.txt
+-rw-r--r--   0 guillaume   (501) staff       (20)      146 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/.codecov.yml
+-rw-r--r--   0 guillaume   (501) staff       (20)     1535 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/LICENSE
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/cmake/
+-rw-r--r--   0 guillaume   (501) staff       (20)       94 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/thread_local.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1066 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/uninstall.in.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)    10848 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/cmake/CompilerFlags.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)     1892 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/cmake/chemfiles-iwyu.imp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1798 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/ParseArguments.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)     2142 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/cmake/IncludeWhatYouUse.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)     1173 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/chemfiles-config-version.cmake.in
+-rw-r--r--   0 guillaume   (501) staff       (20)     8741 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/FindPythonLibsNew.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)      121 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/cmake/chemfiles-config.cmake.in
+-rw-r--r--   0 guillaume   (501) staff       (20)      364 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/InitRules.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)     3513 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/FindNetCDF.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)     4283 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/cmake/FindSphinx.cmake
+-rw-r--r--   0 guillaume   (501) staff       (20)    16517 2020-02-05 20:53:56.000000 chemfiles-0.9.3/lib/CHANGELOG.md
+-rw-r--r--   0 guillaume   (501) staff       (20)      355 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/AUTHORS
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/
+-rw-r--r--   0 guillaume   (501) staff       (20)      611 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles.h
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/
+-rw-r--r--   0 guillaume   (501) staff       (20)     1455 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/include/chemfiles/periodic_table.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     9315 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Trajectory.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3032 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/pdb_connectivity.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    10280 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Topology.hpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/
+-rw-r--r--   0 guillaume   (501) staff       (20)     8220 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/LAMMPSData.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      913 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/TRR.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1013 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/GRO.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      845 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/XYZ.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1385 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/CML.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      884 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/XTC.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3218 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/Molfile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      898 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/SDF.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2790 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/MMTF.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1631 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/TNG.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      941 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/CSSR.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1297 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/MOL2.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3021 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/SMI.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3175 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/PDB.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1815 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/mmCIF.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1766 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/AmberNetCDF.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1160 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/formats/Tinker.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     4462 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Selection.hpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/selections/
+-rw-r--r--   0 guillaume   (501) staff       (20)     2558 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/selections/parser.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    19300 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/selections/expr.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6316 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/selections/lexer.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6632 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/UnitCell.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      902 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/unreachable.hpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/
+-rw-r--r--   0 guillaume   (501) staff       (20)     6253 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/types.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     2239 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/misc.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     6671 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/shared_allocator.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6442 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/cell.h
+-rw-r--r--   0 guillaume   (501) staff       (20)    13990 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/frame.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     5906 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/trajectory.h
+-rw-r--r--   0 guillaume   (501) staff       (20)    10379 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/atom.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     8774 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/residue.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     4759 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/property.h
+-rw-r--r--   0 guillaume   (501) staff       (20)    11327 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/topology.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     6706 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/utils.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     4078 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/capi/selection.h
+-rw-r--r--   0 guillaume   (501) staff       (20)     7228 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/File.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    11551 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/Connectivity.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3412 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/Configuration.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2519 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/error_fmt.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1597 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/Error.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2201 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/FormatFactory.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     9194 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/Property.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3171 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/sorted_set.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8052 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Atom.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2321 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/string_view.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5282 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Residue.hpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/files/
+-rw-r--r--   0 guillaume   (501) staff       (20)      847 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/PlainFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6878 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/NcFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1058 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/files/TNGFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1289 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/Bz2File.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      995 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/GzFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1953 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/XDRFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1447 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/files/XzFile.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      892 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/config.in.h
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/include/chemfiles/external/
+-rw-r--r--   0 guillaume   (501) staff       (20)     7149 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/include/chemfiles/external/span.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    28694 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/include/chemfiles/external/optional.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    41172 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/external/string_view.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1982 2019-12-17 11:23:03.000000 chemfiles-0.9.3/lib/include/chemfiles/mutex.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2407 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/utils.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    14259 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/types.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    13552 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Frame.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      785 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles/warnings.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5883 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/Format.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6540 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/parse.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1813 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/include/chemfiles/misc.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      597 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/include/chemfiles.hpp
+-rw-r--r--   0 guillaume   (501) staff       (20)   105958 2019-03-13 21:26:44.000000 chemfiles-0.9.3/lib/Doxyfile.in
+-rw-r--r--   0 guillaume   (501) staff       (20)     8085 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/README.md
+-rw-r--r--   0 guillaume   (501) staff       (20)     1466 2019-12-17 11:23:03.000000 chemfiles-0.9.3/lib/appveyor.yml
+-rw-r--r--   0 guillaume   (501) staff       (20)       22 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/.gitignore
+-rw-r--r--   0 guillaume   (501) staff       (20)        6 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/VERSION
+-rw-r--r--   0 guillaume   (501) staff       (20)     3200 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/Contributing.md
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/examples/
+-rw-r--r--   0 guillaume   (501) staff       (20)      986 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/examples/CMakeLists.txt
+-rw-r--r--   0 guillaume   (501) staff       (20)      685 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/examples/README.md
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/examples/cpp/
+-rw-r--r--   0 guillaume   (501) staff       (20)      705 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/examples/cpp/indexes.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      751 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/examples/cpp/select.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      591 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/examples/cpp/generate.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/examples/c/
+-rw-r--r--   0 guillaume   (501) staff       (20)      967 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/examples/c/generate.c
+-rw-r--r--   0 guillaume   (501) staff       (20)     1758 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/examples/c/select.c
+-rw-r--r--   0 guillaume   (501) staff       (20)      991 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/examples/c/indexes.c
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/scripts/
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     1791 2019-12-17 11:23:03.000000 chemfiles-0.9.3/lib/scripts/tidy.sh
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/scripts/ci/
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     2880 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/scripts/ci/check-public-headers.py
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     3141 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/scripts/ci/lint-code.py
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     3794 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/scripts/ci/check-capi-docs.py
+-rw-r--r--   0 guillaume   (501) staff       (20)     2891 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/scripts/ci/setup-travis.sh
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     1155 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/scripts/ci/check-exported-symbols.py
+-rw-r--r--   0 guillaume   (501) staff       (20)      860 2019-12-17 11:23:03.000000 chemfiles-0.9.3/lib/scripts/ci/setup-appveyor.ps1
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     1064 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/scripts/ci/build-docs.sh
+-rw-r--r--   0 guillaume   (501) staff       (20)      311 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/scripts/ci/filter-textcoal-warnings.py
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/scripts/generate/
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     2674 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/scripts/generate/periodic_table.py
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     4050 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/scripts/generate/pdb_connectivity.py
+-rwxr-xr-x   0 guillaume   (501) staff       (20)     1831 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/scripts/boost.sh
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/external/
+-rw-r--r--   0 guillaume   (501) staff       (20)   255856 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/external/lzma.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   451385 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/external/mmtf-cpp.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)     8102 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/external/CMakeLists.txt
+-rw-r--r--   0 guillaume   (501) staff       (20)   329575 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/external/tng.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   162586 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/external/zlib.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   487169 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/external/molfiles.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   506362 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/external/netcdf.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)    14644 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/external/README.md
+-rw-r--r--   0 guillaume   (501) staff       (20)    70868 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/external/toml11.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)    42657 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/external/xdrfile.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   364541 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/external/bzip2.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   374387 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/external/pugixml.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)   717887 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/external/fmt.tar.gz
+-rw-r--r--   0 guillaume   (501) staff       (20)       36 2017-12-10 15:59:10.000000 chemfiles-0.9.3/lib/.git
+-rw-r--r--   0 guillaume   (501) staff       (20)     3305 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/.travis.yml
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/src/
+-rw-r--r--   0 guillaume   (501) staff       (20)     1878 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/utils.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6326 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Frame.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      813 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/warnings.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/src/formats/
+-rw-r--r--   0 guillaume   (501) staff       (20)    23938 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/SMI.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    27032 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/src/formats/PDB.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8295 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/AmberNetCDF.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    15034 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/mmCIF.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5608 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/Tinker.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5936 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/XTC.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    12006 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/Molfile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    11322 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/SDF.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    18614 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/src/formats/MMTF.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     9335 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/TNG.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5891 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/CSSR.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    10194 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/MOL2.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2530 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/src/formats/XYZ.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    21787 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/CML.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    34103 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/LAMMPSData.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8182 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/TRR.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     9336 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/formats/GRO.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3183 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Format.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5985 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/parse.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/src/selections/
+-rw-r--r--   0 guillaume   (501) staff       (20)    20576 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/selections/expr.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8482 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/selections/lexer.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    21685 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/selections/parser.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6646 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/FormatFactory.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3035 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Property.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/src/capi/
+-rw-r--r--   0 guillaume   (501) staff       (20)     8735 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/capi/frame.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     1423 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/misc.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3090 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/property.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6920 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/capi/atom.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     4416 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/cell.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5950 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/capi/residue.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      303 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/shared_allocator.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3340 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/trajectory.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8740 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/topology.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3003 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/capi/selection.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2918 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/Atom.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)      772 2019-12-17 11:25:26.000000 chemfiles-0.9.3/lib/src/Residue.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6191 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/File.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     6875 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Connectivity.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     7008 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Configuration.cpp
+drwxr-xr-x   0 guillaume   (501) staff       (20)        0 2020-02-06 21:29:39.000000 chemfiles-0.9.3/lib/src/files/
+-rw-r--r--   0 guillaume   (501) staff       (20)     2596 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/GzFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     3087 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/XDRFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5287 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/XzFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     7052 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/NcFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2192 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/TNGFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     5278 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/Bz2File.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     2478 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/files/PlainFile.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     8966 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/src/periodic_table.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     7042 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Trajectory.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)    17470 2019-01-26 13:01:21.000000 chemfiles-0.9.3/lib/src/pdb_connectivity.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     4522 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Topology.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     9200 2019-12-17 11:25:29.000000 chemfiles-0.9.3/lib/src/Selection.cpp
+-rw-r--r--   0 guillaume   (501) staff       (20)     7977 2020-02-05 20:00:28.000000 chemfiles-0.9.3/lib/src/UnitCell.cpp
```

### Comparing `chemfiles-0.9.2/PKG-INFO` & `chemfiles-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemfiles
-Version: 0.9.2
+Version: 0.9.3
 Summary: Read and write chemistry trajectory files
 Home-page: http://github.com/chemfiles/chemfiles.py
 Author: Guillaume Fraux
 Author-email: luthaf@luthaf.fr
 License: UNKNOWN
 Description: # Python binding for the chemfiles library
```

### Comparing `chemfiles-0.9.2/CMakeLists.txt` & `chemfiles-0.9.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/LICENSE` & `chemfiles-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/misc.py` & `chemfiles-0.9.3/chemfiles/misc.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/property.py` & `chemfiles-0.9.3/chemfiles/property.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/cell.py` & `chemfiles-0.9.3/chemfiles/cell.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/trajectory.py` & `chemfiles-0.9.3/chemfiles/trajectory.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/residue.py` & `chemfiles-0.9.3/chemfiles/residue.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/utils.py` & `chemfiles-0.9.3/chemfiles/utils.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/clib.py` & `chemfiles-0.9.3/chemfiles/clib.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/frame.py` & `chemfiles-0.9.3/chemfiles/frame.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/topology.py` & `chemfiles-0.9.3/chemfiles/topology.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/selection.py` & `chemfiles-0.9.3/chemfiles/selection.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/atom.py` & `chemfiles-0.9.3/chemfiles/atom.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/chemfiles/ffi.py` & `chemfiles-0.9.3/chemfiles/ffi.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/README.md` & `chemfiles-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/setup.py` & `chemfiles-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/CMakeLists.txt` & `chemfiles-0.9.3/lib/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 cmake_minimum_required(VERSION 2.8.12)
 set(CMAKE_USER_MAKE_RULES_OVERRIDE "${CMAKE_CURRENT_SOURCE_DIR}/cmake/InitRules.cmake")
 
+if(NOT "${LAST_CMAKE_VERSION}" VERSION_EQUAL ${CMAKE_VERSION})
+    set(LAST_CMAKE_VERSION ${CMAKE_VERSION} CACHE INTERNAL "Last version of cmake used to configure")
+    message(STATUS "Running CMake version ${CMAKE_VERSION}")
+endif()
+
 project(chemfiles C CXX)
 
 set(CMAKE_MODULE_PATH "${CMAKE_MODULE_PATH};${PROJECT_SOURCE_DIR}/cmake")
 if (POLICY CMP0042)
     cmake_policy(SET CMP0042 NEW) # OSX RPATH handling
 endif()
 if (POLICY CMP0063)
```

### Comparing `chemfiles-0.9.2/lib/LICENSE` & `chemfiles-0.9.3/lib/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/uninstall.in.cmake` & `chemfiles-0.9.3/lib/cmake/uninstall.in.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/CompilerFlags.cmake` & `chemfiles-0.9.3/lib/cmake/CompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/chemfiles-iwyu.imp` & `chemfiles-0.9.3/lib/cmake/chemfiles-iwyu.imp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/ParseArguments.cmake` & `chemfiles-0.9.3/lib/cmake/ParseArguments.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/IncludeWhatYouUse.cmake` & `chemfiles-0.9.3/lib/cmake/IncludeWhatYouUse.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/chemfiles-config-version.cmake.in` & `chemfiles-0.9.3/lib/cmake/chemfiles-config-version.cmake.in`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/FindPythonLibsNew.cmake` & `chemfiles-0.9.3/lib/cmake/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/FindNetCDF.cmake` & `chemfiles-0.9.3/lib/cmake/FindNetCDF.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/cmake/FindSphinx.cmake` & `chemfiles-0.9.3/lib/cmake/FindSphinx.cmake`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/CHANGELOG.md` & `chemfiles-0.9.3/lib/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Next Release (current master)
 
+## 0.9.3 (5 Feb 2020)
+
+* Fix a bug in the PDB format where no atomic name/type was read from short
+  ATOM/HETATM records.
+* Fix a few bugs related to UnitCell Matrix and infinite UnitCell construction
+
 ## 0.9.2 (18 Dec 2019)
 
 * When compiling chemfiles as a shared library, the dependencies symbols are
   now hidden. This should prevent clashes between say chemfiles's zlib and the
   system zlib.
 * Cache sub-selection (the 'name O' in 'is_bonded(#1, name O)'), reducing
   selection evaluation time by a huge margin.
```

### Comparing `chemfiles-0.9.2/lib/include/chemfiles.h` & `chemfiles-0.9.3/lib/include/chemfiles.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/periodic_table.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/periodic_table.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Trajectory.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Trajectory.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/pdb_connectivity.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/pdb_connectivity.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Topology.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Topology.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/LAMMPSData.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/LAMMPSData.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/TRR.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/TRR.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/GRO.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/GRO.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/XYZ.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/XYZ.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/CML.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/CML.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/XTC.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/XTC.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/Molfile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/Molfile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/SDF.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/SDF.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/MMTF.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/MMTF.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/TNG.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/TNG.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/CSSR.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/CSSR.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/MOL2.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/MOL2.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/SMI.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/SMI.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/PDB.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/PDB.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/mmCIF.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/mmCIF.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/AmberNetCDF.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/AmberNetCDF.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/formats/Tinker.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/formats/Tinker.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Selection.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Selection.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/selections/parser.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/selections/parser.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/selections/expr.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/selections/expr.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/selections/lexer.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/selections/lexer.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/UnitCell.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/UnitCell.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/unreachable.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/unreachable.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/types.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/types.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/misc.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/misc.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/shared_allocator.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/capi/shared_allocator.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/cell.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/cell.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/frame.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/frame.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/trajectory.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/trajectory.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/atom.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/atom.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/residue.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/residue.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/property.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/property.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/topology.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/topology.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/utils.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/capi/utils.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -87,14 +87,17 @@
     CATCH_AND_RETURN(ConfigurationError, CHFL_CONFIGURATION_ERROR)             \
     CATCH_AND_RETURN(OutOfBounds, CHFL_OUT_OF_BOUNDS)                          \
     CATCH_AND_RETURN(PropertyError, CHFL_PROPERTY_ERROR)                       \
     CATCH_AND_RETURN(Error, CHFL_GENERIC_ERROR)                                \
     catch (const std::exception& e) {                                          \
         set_last_error(e.what());                                              \
         return CHFL_CXX_ERROR;                                                 \
+    } catch (...) {                                                            \
+        set_last_error("UNKNOWN ERROR");                                       \
+        return CHFL_CXX_ERROR;                                                 \
     }                                                                          \
     return CHFL_SUCCESS;
 
 /// Wrap `instructions` in a try/catch bloc automatically, and goto the
 /// `error` label in case of error.
 #define CHFL_ERROR_GOTO(instructions)                                          \
     try {                                                                      \
@@ -106,13 +109,16 @@
     CATCH_AND_GOTO_ERROR(SelectionError)                                       \
     CATCH_AND_GOTO_ERROR(ConfigurationError)                                   \
     CATCH_AND_GOTO_ERROR(OutOfBounds)                                          \
     CATCH_AND_GOTO_ERROR(PropertyError)                                        \
     CATCH_AND_GOTO_ERROR(Error)                                                \
     catch (const std::exception& e) {                                          \
         set_last_error(e.what());                                              \
-        goto error;                                                            \
+        goto error;  /* NOLINT: goto is OK here */                             \
+    } catch (...) {                                                            \
+        set_last_error("UNKNOWN ERROR");                                       \
+        goto error;  /* NOLINT: goto is OK here */                             \
     }
 
 }
 
 #endif
```

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/capi/selection.h` & `chemfiles-0.9.3/lib/include/chemfiles/capi/selection.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/File.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/File.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Connectivity.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Connectivity.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Configuration.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Configuration.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/error_fmt.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/error_fmt.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Error.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Error.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/FormatFactory.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/FormatFactory.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Property.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Property.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/sorted_set.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/sorted_set.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Atom.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Atom.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/string_view.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/string_view.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Residue.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Residue.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/PlainFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/PlainFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/NcFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/NcFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/TNGFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/TNGFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/Bz2File.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/Bz2File.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/GzFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/GzFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/XDRFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/XDRFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/files/XzFile.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/files/XzFile.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/config.in.h` & `chemfiles-0.9.3/lib/include/chemfiles/config.in.h`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/external/span.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/external/span.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/external/optional.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/external/optional.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/external/string_view.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/external/string_view.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/mutex.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/mutex.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/utils.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/utils.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/types.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/types.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Frame.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Frame.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/warnings.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/warnings.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/Format.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/Format.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/parse.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/parse.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles/misc.hpp` & `chemfiles-0.9.3/lib/include/chemfiles/misc.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/include/chemfiles.hpp` & `chemfiles-0.9.3/lib/include/chemfiles.hpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/Doxyfile.in` & `chemfiles-0.9.3/lib/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/README.md` & `chemfiles-0.9.3/lib/README.md`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/appveyor.yml` & `chemfiles-0.9.3/lib/appveyor.yml`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/Contributing.md` & `chemfiles-0.9.3/lib/Contributing.md`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/CMakeLists.txt` & `chemfiles-0.9.3/lib/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/README.md` & `chemfiles-0.9.3/lib/examples/README.md`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/cpp/indexes.cpp` & `chemfiles-0.9.3/lib/examples/cpp/indexes.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/cpp/select.cpp` & `chemfiles-0.9.3/lib/examples/cpp/select.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/cpp/generate.cpp` & `chemfiles-0.9.3/lib/examples/cpp/generate.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/c/generate.c` & `chemfiles-0.9.3/lib/examples/c/generate.c`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/c/select.c` & `chemfiles-0.9.3/lib/examples/c/select.c`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/examples/c/indexes.c` & `chemfiles-0.9.3/lib/examples/c/indexes.c`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/tidy.sh` & `chemfiles-0.9.3/lib/scripts/tidy.sh`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/check-public-headers.py` & `chemfiles-0.9.3/lib/scripts/ci/check-public-headers.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/lint-code.py` & `chemfiles-0.9.3/lib/scripts/ci/lint-code.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/check-capi-docs.py` & `chemfiles-0.9.3/lib/scripts/ci/check-capi-docs.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/setup-travis.sh` & `chemfiles-0.9.3/lib/scripts/ci/setup-travis.sh`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/check-exported-symbols.py` & `chemfiles-0.9.3/lib/scripts/ci/check-exported-symbols.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/setup-appveyor.ps1` & `chemfiles-0.9.3/lib/scripts/ci/setup-appveyor.ps1`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/ci/build-docs.sh` & `chemfiles-0.9.3/lib/scripts/ci/build-docs.sh`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/generate/periodic_table.py` & `chemfiles-0.9.3/lib/scripts/generate/periodic_table.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/generate/pdb_connectivity.py` & `chemfiles-0.9.3/lib/scripts/generate/pdb_connectivity.py`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/scripts/boost.sh` & `chemfiles-0.9.3/lib/scripts/boost.sh`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/lzma.tar.gz` & `chemfiles-0.9.3/lib/external/lzma.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/mmtf-cpp.tar.gz` & `chemfiles-0.9.3/lib/external/mmtf-cpp.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/CMakeLists.txt` & `chemfiles-0.9.3/lib/external/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,19 @@
             WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
         )
         execute_process(
             COMMAND ${CMAKE_COMMAND} -E touch ${_name_}/${_shasum_}
             WORKING_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}
         )
     endif()
+
+    if(EXISTS "${CMAKE_CURRENT_BINARY_DIR}/${_name_}/.git")
+        # .git directories can get huge and increase the size of this repository
+        message(FATAL_ERROR "${_name_} archive contains a .git directory, please remove it")
+    endif()
 endfunction()
 
 function(external_library _name_)
     unpack_library(${_name_})
     add_subdirectory(
         ${CMAKE_CURRENT_BINARY_DIR}/${_name_}
         ${CMAKE_CURRENT_BINARY_DIR}/${_name_}
@@ -112,20 +117,29 @@
     set(BZIP2_INCLUDE_DIR ${BZIP2_INCLUDE_DIR} PARENT_SCOPE)
 endif()
 list(APPEND EXTERNAL_INCLUDES ${BZIP2_INCLUDE_DIR})
 
 # ==========
 # fmtlib: https://github.com/chemfiles/fmt
 # ==========
+if (${CMAKE_VERSION} VERSION_LESS "3.1")
+    # fmt uses target_compile_features, which is not available on older cmake
+    # versions.
+    function(target_compile_features)
+    endfunction()
+endif()
+
 external_library(fmt)
 list(APPEND EXTERNAL_INCLUDES ${CMAKE_CURRENT_BINARY_DIR}/fmt/include/)
 
 # Hide FMT variables from CMake GUI
 mark_as_advanced(FORCE
+    FMT_CUDA_TEST
     FMT_DOC
+    FMT_FUZZ
     FMT_INSTALL
     FMT_PEDANTIC
     FMT_TEST
     FMT_WERROR
 )
 
 # ==========
```

### Comparing `chemfiles-0.9.2/lib/external/tng.tar.gz` & `chemfiles-0.9.3/lib/external/tng.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/zlib.tar.gz` & `chemfiles-0.9.3/lib/external/zlib.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/molfiles.tar.gz` & `chemfiles-0.9.3/lib/external/molfiles.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/README.md` & `chemfiles-0.9.3/lib/external/README.md`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/toml11.tar.gz` & `chemfiles-0.9.3/lib/external/toml11.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/bzip2.tar.gz` & `chemfiles-0.9.3/lib/external/bzip2.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/external/pugixml.tar.gz` & `chemfiles-0.9.3/lib/external/pugixml.tar.gz`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/.travis.yml` & `chemfiles-0.9.3/lib/.travis.yml`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/utils.cpp` & `chemfiles-0.9.3/lib/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Frame.cpp` & `chemfiles-0.9.3/lib/src/Frame.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/warnings.cpp` & `chemfiles-0.9.3/lib/src/warnings.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/SMI.cpp` & `chemfiles-0.9.3/lib/src/formats/SMI.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/PDB.cpp` & `chemfiles-0.9.3/lib/src/formats/PDB.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
     auto name = line.substr(12, 4);
     if (line.length() >= 78) {
         auto type = line.substr(76, 2);
         // Read both atom name and atom type
         atom = Atom(trim(name).to_string(), trim(type).to_string());
     } else {
         // Read just the atom name and hope for the best.
-        Atom(trim(name).to_string());
+        atom = Atom(trim(name).to_string());
     }
 
     auto altloc = line.substr(16, 1);
     if (altloc != " ") {
         atom.set("altloc", altloc.to_string());
     }
```

### Comparing `chemfiles-0.9.2/lib/src/formats/AmberNetCDF.cpp` & `chemfiles-0.9.3/lib/src/formats/AmberNetCDF.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/mmCIF.cpp` & `chemfiles-0.9.3/lib/src/formats/mmCIF.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/Tinker.cpp` & `chemfiles-0.9.3/lib/src/formats/Tinker.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/XTC.cpp` & `chemfiles-0.9.3/lib/src/formats/XTC.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/Molfile.cpp` & `chemfiles-0.9.3/lib/src/formats/Molfile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/SDF.cpp` & `chemfiles-0.9.3/lib/src/formats/SDF.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/MMTF.cpp` & `chemfiles-0.9.3/lib/src/formats/MMTF.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,16 @@
     if (!mmtf::isDefaultValue(structure_.depositionDate)) {
         frame.set("deposition_date", structure_.depositionDate);
     }
 
     auto inter_residue_bond_count = structure_.bondAtomList.size() / 2;
     size_t bond_index = 0;
     while (bond_index < inter_residue_bond_count) {
-        auto atom1 = structure_.bondAtomList[bond_index * 2 + 0];
-        auto atom2 = structure_.bondAtomList[bond_index * 2 + 1];
+        auto atom1 = static_cast<size_t>(structure_.bondAtomList[bond_index * 2 + 0]);
+        auto atom2 = static_cast<size_t>(structure_.bondAtomList[bond_index * 2 + 1]);
 
         // We are below the atoms we care about
         if ((atom1 < atomSkip_) || (atom2 < atomSkip_)) {
             bond_index++;
             continue;
         }
```

### Comparing `chemfiles-0.9.2/lib/src/formats/TNG.cpp` & `chemfiles-0.9.3/lib/src/formats/TNG.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/CSSR.cpp` & `chemfiles-0.9.3/lib/src/formats/CSSR.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/MOL2.cpp` & `chemfiles-0.9.3/lib/src/formats/MOL2.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/XYZ.cpp` & `chemfiles-0.9.3/lib/src/formats/XYZ.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     file_.print("Written by the chemfiles library\n", frame.size());
 
     for (size_t i = 0; i < frame.size(); i++) {
         auto name = topology[i].name();
         if (name.empty()) {
             name = "X";
         }
-        file_.print("{} {} {} {}\n",
+        file_.print("{} {:g} {:g} {:g}\n",
             name, positions[i][0], positions[i][1], positions[i][2]
         );
     }
 }
 
 optional<uint64_t> XYZFormat::forward() {
     auto position = file_.tellpos();
```

### Comparing `chemfiles-0.9.2/lib/src/formats/CML.cpp` & `chemfiles-0.9.3/lib/src/formats/CML.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/LAMMPSData.cpp` & `chemfiles-0.9.3/lib/src/formats/LAMMPSData.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/TRR.cpp` & `chemfiles-0.9.3/lib/src/formats/TRR.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/formats/GRO.cpp` & `chemfiles-0.9.3/lib/src/formats/GRO.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Format.cpp` & `chemfiles-0.9.3/lib/src/Format.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/parse.cpp` & `chemfiles-0.9.3/lib/src/parse.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/selections/expr.cpp` & `chemfiles-0.9.3/lib/src/selections/expr.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/selections/lexer.cpp` & `chemfiles-0.9.3/lib/src/selections/lexer.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/selections/parser.cpp` & `chemfiles-0.9.3/lib/src/selections/parser.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/FormatFactory.cpp` & `chemfiles-0.9.3/lib/src/FormatFactory.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Property.cpp` & `chemfiles-0.9.3/lib/src/Property.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/frame.cpp` & `chemfiles-0.9.3/lib/src/capi/frame.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/misc.cpp` & `chemfiles-0.9.3/lib/src/capi/misc.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/property.cpp` & `chemfiles-0.9.3/lib/src/capi/property.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/atom.cpp` & `chemfiles-0.9.3/lib/src/capi/atom.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/cell.cpp` & `chemfiles-0.9.3/lib/src/capi/cell.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/residue.cpp` & `chemfiles-0.9.3/lib/src/capi/residue.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/trajectory.cpp` & `chemfiles-0.9.3/lib/src/capi/trajectory.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/topology.cpp` & `chemfiles-0.9.3/lib/src/capi/topology.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/capi/selection.cpp` & `chemfiles-0.9.3/lib/src/capi/selection.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Atom.cpp` & `chemfiles-0.9.3/lib/src/Atom.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Residue.cpp` & `chemfiles-0.9.3/lib/src/Residue.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/File.cpp` & `chemfiles-0.9.3/lib/src/File.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Connectivity.cpp` & `chemfiles-0.9.3/lib/src/Connectivity.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Configuration.cpp` & `chemfiles-0.9.3/lib/src/Configuration.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/GzFile.cpp` & `chemfiles-0.9.3/lib/src/files/GzFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/XDRFile.cpp` & `chemfiles-0.9.3/lib/src/files/XDRFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/XzFile.cpp` & `chemfiles-0.9.3/lib/src/files/XzFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/NcFile.cpp` & `chemfiles-0.9.3/lib/src/files/NcFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/TNGFile.cpp` & `chemfiles-0.9.3/lib/src/files/TNGFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/Bz2File.cpp` & `chemfiles-0.9.3/lib/src/files/Bz2File.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/files/PlainFile.cpp` & `chemfiles-0.9.3/lib/src/files/PlainFile.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/periodic_table.cpp` & `chemfiles-0.9.3/lib/src/periodic_table.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Trajectory.cpp` & `chemfiles-0.9.3/lib/src/Trajectory.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/pdb_connectivity.cpp` & `chemfiles-0.9.3/lib/src/pdb_connectivity.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Topology.cpp` & `chemfiles-0.9.3/lib/src/Topology.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/Selection.cpp` & `chemfiles-0.9.3/lib/src/Selection.cpp`

 * *Files identical despite different names*

### Comparing `chemfiles-0.9.2/lib/src/UnitCell.cpp` & `chemfiles-0.9.3/lib/src/UnitCell.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,27 @@
     a_(a),
     b_(b),
     c_(c),
     alpha_(alpha),
     beta_(beta),
     gamma_(gamma)
 {
+    auto is_zero = [](double length) {
+        // We think that 0.00001 is close enough to 0
+        return fabs(length) < 1e-5;
+    };
     auto is_90 = [](double angle) {
         // We think that 89.999° is close enough to 90°
         return fabs(angle - 90.0) < 1e-3;
     };
-    if (is_90(alpha_) && is_90(beta_) && is_90(gamma_)) {
+    if (is_zero(a_) && is_zero(b_) && is_zero(c_)) {
+        shape_ = INFINITE;
+        a_ = b_ = c_ = 0;
+        alpha_ = beta_ = gamma_ = 90;
+    } else if (is_90(alpha_) && is_90(beta_) && is_90(gamma_)) {
         shape_ = ORTHORHOMBIC;
         // Make sure alpha/beta/gamma are actually 90°, so that the matrix
         // update below does not create a non diagonal matrix.
         alpha_ = 90;
         beta_ = 90;
         gamma_ = 90;
     } else {
@@ -73,26 +81,30 @@
     if (matrix[0][0] == 0 && matrix[1][1] == 0 && matrix[2][2] == 0 &&
         matrix[0][1] == 0 && matrix[0][2] == 0 && matrix[1][2] == 0) {
 
         shape_ = INFINITE;
         a_ = b_ = c_ = 0;
         alpha_ = beta_ = gamma_ = 90.0;
 
+        update_matrix();
+
         return;
     }
 
     if (matrix[0][1] == 0 && matrix[0][2] == 0 && matrix[1][2] == 0) {
         shape_ = ORTHORHOMBIC;
 
         a_ = matrix[0][0];
         b_ = matrix[1][1];
         c_ = matrix[2][2];
 
         alpha_ = beta_ = gamma_ = 90.0;
 
+        update_matrix();
+
         return;
     }
 
     shape_ = TRICLINIC;
 
     Vector3D v1 = {matrix[0][0], matrix[1][0], matrix[2][0]};
     Vector3D v2 = {matrix[0][1], matrix[1][1], matrix[2][1]};
```

