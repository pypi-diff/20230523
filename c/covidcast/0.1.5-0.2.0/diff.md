# Comparing `tmp/covidcast-0.1.5.tar.gz` & `tmp/covidcast-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/covidcast-0.1.5.tar", last modified: Mon May 10 17:40:04 2021, max compression
+gzip compressed data, was "covidcast-0.2.0.tar", last modified: Tue May 23 16:52:19 2023, max compression
```

## Comparing `covidcast-0.1.5.tar` & `covidcast-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/
--rw-r--r--   0 alexreinhart   (501) staff       (20)     1277 2021-05-10 17:40:04.000000 covidcast-0.1.5/PKG-INFO
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast.egg-info/
--rw-r--r--   0 alexreinhart   (501) staff       (20)     1277 2021-05-10 17:40:03.000000 covidcast-0.1.5/covidcast.egg-info/PKG-INFO
--rw-r--r--   0 alexreinhart   (501) staff       (20)     1840 2021-05-10 17:40:03.000000 covidcast-0.1.5/covidcast.egg-info/SOURCES.txt
--rw-r--r--   0 alexreinhart   (501) staff       (20)      113 2021-05-10 17:40:03.000000 covidcast-0.1.5/covidcast.egg-info/requires.txt
--rw-r--r--   0 alexreinhart   (501) staff       (20)       10 2021-05-10 17:40:03.000000 covidcast-0.1.5/covidcast.egg-info/top_level.txt
--rw-r--r--   0 alexreinhart   (501) staff       (20)        1 2021-05-10 17:40:03.000000 covidcast-0.1.5/covidcast.egg-info/dependency_links.txt
--rw-r--r--   0 alexreinhart   (501) staff       (20)      680 2020-08-30 19:28:25.000000 covidcast-0.1.5/README.md
--rw-r--r--   0 alexreinhart   (501) staff       (20)     1054 2021-05-10 15:09:14.000000 covidcast-0.1.5/setup.py
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/geo_mappings/
--rw-r--r--   0 alexreinhart   (501) staff       (20)     2854 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/geo_mappings/state_census.csv
--rw-r--r--   0 alexreinhart   (501) staff       (20)  3674419 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/geo_mappings/county_census.csv
--rw-r--r--   0 alexreinhart   (501) staff       (20)  1299191 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/geo_mappings/msa_census.csv
--rw-r--r--   0 alexreinhart   (501) staff       (20)    17755 2021-01-13 22:07:33.000000 covidcast-0.1.5/covidcast/geography.py
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/shapefiles/
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/shapefiles/hrr/
--rw-r--r--   0 alexreinhart   (501) staff       (20)   236891 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf
--rw-r--r--   0 alexreinhart   (501) staff       (20)     2548 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx
--rw-r--r--   0 alexreinhart   (501) staff       (20)  1734200 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp
--rw-r--r--   0 alexreinhart   (501) staff       (20)      212 2020-10-06 20:41:58.000000 covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.prj
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/shapefiles/msa/
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    32493 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml
--rw-r--r--   0 alexreinhart   (501) staff       (20)  1494264 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp
--rw-r--r--   0 alexreinhart   (501) staff       (20)        5 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.cpg
--rw-r--r--   0 alexreinhart   (501) staff       (20)     7604 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx
--rw-r--r--   0 alexreinhart   (501) staff       (20)   148494 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf
--rw-r--r--   0 alexreinhart   (501) staff       (20)      165 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.prj
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    16594 2020-09-20 00:43:06.000000 covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/shapefiles/state/
--rw-r--r--   0 alexreinhart   (501) staff       (20)      165 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.prj
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    17903 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml
--rw-r--r--   0 alexreinhart   (501) staff       (20)  1394376 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp
--rw-r--r--   0 alexreinhart   (501) staff       (20)        5 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.cpg
--rw-r--r--   0 alexreinhart   (501) staff       (20)      548 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shx
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    31536 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml
--rw-r--r--   0 alexreinhart   (501) staff       (20)     9058 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf
-drwxr-xr-x   0 alexreinhart   (501) staff       (20)        0 2021-05-10 17:40:04.000000 covidcast-0.1.5/covidcast/shapefiles/county/
--rw-r--r--   0 alexreinhart   (501) staff       (20)      165 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.prj
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    21754 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml
--rw-r--r--   0 alexreinhart   (501) staff       (20)   527301 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf
--rwxr-xr-x   0 alexreinhart   (501) staff       (20)    34190 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml
--rw-r--r--   0 alexreinhart   (501) staff       (20)    25964 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shx
--rw-r--r--   0 alexreinhart   (501) staff       (20)  3662752 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp
--rw-r--r--   0 alexreinhart   (501) staff       (20)        5 2020-08-29 01:43:19.000000 covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.cpg
--rw-r--r--   0 alexreinhart   (501) staff       (20)    26652 2020-11-01 17:27:43.000000 covidcast-0.1.5/covidcast/plotting.py
--rw-r--r--   0 alexreinhart   (501) staff       (20)      726 2020-11-05 22:38:16.000000 covidcast-0.1.5/covidcast/__init__.py
--rw-r--r--   0 alexreinhart   (501) staff       (20)      182 2020-10-29 20:27:28.000000 covidcast-0.1.5/covidcast/errors.py
--rw-r--r--   0 alexreinhart   (501) staff       (20)    24249 2021-05-10 15:20:15.000000 covidcast-0.1.5/covidcast/covidcast.py
--rw-r--r--   0 alexreinhart   (501) staff       (20)       38 2021-05-10 17:40:04.000000 covidcast-0.1.5/setup.cfg
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/
+-rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-05-23 16:52:19.300094 covidcast-0.2.0/PKG-INFO
+-rw-r--r--   0 krivard  (12134) users      (100)      680 2020-12-16 14:58:59.000000 covidcast-0.2.0/README.md
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast/
+-rw-r--r--   0 krivard  (12134) users      (100)      739 2023-05-22 19:15:07.000000 covidcast-0.2.0/covidcast/__init__.py
+-rw-r--r--   0 krivard  (12134) users      (100)    24797 2023-05-22 19:15:07.000000 covidcast-0.2.0/covidcast/covidcast.py
+-rw-r--r--   0 krivard  (12134) users      (100)      182 2020-12-16 14:58:59.000000 covidcast-0.2.0/covidcast/errors.py
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.292094 covidcast-0.2.0/covidcast/geo_mappings/
+-rw-r--r--   0 krivard  (12134) users      (100)  3674419 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/county_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)  1299191 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/msa_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)     2854 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geo_mappings/state_census.csv
+-rw-r--r--   0 krivard  (12134) users      (100)    17755 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/geography.py
+-rw-r--r--   0 krivard  (12134) users      (100)     3426 2023-03-27 18:00:04.000000 covidcast-0.2.0/covidcast/make_reference_plots.py
+-rw-r--r--   0 krivard  (12134) users      (100)    26627 2023-03-29 14:35:17.000000 covidcast-0.2.0/covidcast/plotting.py
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast/shapefiles/
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.296094 covidcast-0.2.0/covidcast/shapefiles/county/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)   527301 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  3662752 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    21754 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    34190 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)    25964 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.296094 covidcast-0.2.0/covidcast/shapefiles/hrr/
+-rw-r--r--   0 krivard  (12134) users      (100)   236891 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      212 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1734200 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp
+-rw-r--r--   0 krivard  (12134) users      (100)     2548 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/covidcast/shapefiles/msa/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)   148494 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1494264 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    16594 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    32493 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)     7604 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.300094 covidcast-0.2.0/covidcast/shapefiles/state/
+-rw-r--r--   0 krivard  (12134) users      (100)        5 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.cpg
+-rw-r--r--   0 krivard  (12134) users      (100)     9058 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf
+-rw-r--r--   0 krivard  (12134) users      (100)      165 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.prj
+-rw-r--r--   0 krivard  (12134) users      (100)  1394376 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp
+-rwxr-xr-x   0 krivard  (12134) users      (100)    17903 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml
+-rwxr-xr-x   0 krivard  (12134) users      (100)    31536 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml
+-rw-r--r--   0 krivard  (12134) users      (100)      548 2020-12-16 14:59:00.000000 covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shx
+drwxr-xr-x   0 krivard  (12134) users      (100)        0 2023-05-23 16:52:19.288094 covidcast-0.2.0/covidcast.egg-info/
+-rw-r--r--   0 krivard  (12134) users      (100)     1277 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/PKG-INFO
+-rw-r--r--   0 krivard  (12134) users      (100)     1874 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/SOURCES.txt
+-rw-r--r--   0 krivard  (12134) users      (100)        1 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/dependency_links.txt
+-rw-r--r--   0 krivard  (12134) users      (100)      115 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/requires.txt
+-rw-r--r--   0 krivard  (12134) users      (100)       10 2023-05-23 16:52:19.000000 covidcast-0.2.0/covidcast.egg-info/top_level.txt
+-rw-r--r--   0 krivard  (12134) users      (100)       38 2023-05-23 16:52:19.300094 covidcast-0.2.0/setup.cfg
+-rw-r--r--   0 krivard  (12134) users      (100)     1056 2023-05-22 19:17:23.000000 covidcast-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `covidcast-0.1.5/PKG-INFO` & `covidcast-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covidcast
-Version: 0.1.5
+Version: 0.2.0
 Summary: Access COVID-19 data through the Delphi COVIDcast API
 Home-page: https://cmu-delphi.github.io/covidcast/covidcast-py/html/
 Author: Alex Reinhart
 Author-email: areinhar@stat.cmu.edu
 License: UNKNOWN
 Description: # COVIDcast API client
```

### Comparing `covidcast-0.1.5/covidcast.egg-info/PKG-INFO` & `covidcast-0.2.0/covidcast.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covidcast
-Version: 0.1.5
+Version: 0.2.0
 Summary: Access COVID-19 data through the Delphi COVIDcast API
 Home-page: https://cmu-delphi.github.io/covidcast/covidcast-py/html/
 Author: Alex Reinhart
 Author-email: areinhar@stat.cmu.edu
 License: UNKNOWN
 Description: # COVIDcast API client
```

### Comparing `covidcast-0.1.5/covidcast.egg-info/SOURCES.txt` & `covidcast-0.2.0/covidcast.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 covidcast/__init__.py
 covidcast/covidcast.py
 covidcast/errors.py
 covidcast/geography.py
+covidcast/make_reference_plots.py
 covidcast/plotting.py
 covidcast.egg-info/PKG-INFO
 covidcast.egg-info/SOURCES.txt
 covidcast.egg-info/dependency_links.txt
 covidcast.egg-info/requires.txt
 covidcast.egg-info/top_level.txt
 covidcast/geo_mappings/county_census.csv
```

### Comparing `covidcast-0.1.5/README.md` & `covidcast-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/setup.py` & `covidcast-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="covidcast",
-    version="0.1.5",  # also update in docs/conf.py
+    version="0.2.0",  # also update in docs/conf.py
     author="Alex Reinhart",
     author_email="areinhar@stat.cmu.edu",
     description="Access COVID-19 data through the Delphi COVIDcast API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://cmu-delphi.github.io/covidcast/covidcast-py/html/",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     install_requires=[
-        "pandas",
+        "pandas<2",
         "requests",
         "delphi-epidata>=0.0.11",
         "geopandas",
         "matplotlib",
         "numpy",
         "descartes",
         "imageio-ffmpeg",
```

### Comparing `covidcast-0.1.5/covidcast/geo_mappings/state_census.csv` & `covidcast-0.2.0/covidcast/geo_mappings/state_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/geo_mappings/county_census.csv` & `covidcast-0.2.0/covidcast/geo_mappings/county_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/geo_mappings/msa_census.csv` & `covidcast-0.2.0/covidcast/geo_mappings/msa_census.csv`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/geography.py` & `covidcast-0.2.0/covidcast/geography.py`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf` & `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx` & `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp` & `covidcast-0.2.0/covidcast/shapefiles/hrr/geo_export_ad86cff5-e5ed-432e-9ec2-2ce8732099ee.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp` & `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx` & `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf` & `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/msa/cb_2019_us_cbsa_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp` & `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shx` & `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf` & `covidcast-0.2.0/covidcast/shapefiles/state/cb_2019_us_state_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.ea.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf` & `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.dbf`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml` & `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp.iso.xml`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shx` & `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shx`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/shapefiles/county/cb_2019_us_county_5m.shp` & `covidcast-0.2.0/covidcast/shapefiles/county/cb_2019_us_county_5m.shp`

 * *Files identical despite different names*

### Comparing `covidcast-0.1.5/covidcast/plotting.py` & `covidcast-0.2.0/covidcast/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
     cont = data.loc[[i in CONTIGUOUS_FIPS for i in data[state_col]], :].to_crs("ESRI:102003")
     alaska = data.loc[data[state_col] == "02", :].to_crs("ESRI:102006")
     pr = data.loc[data[state_col] == "72", :].to_crs("ESRI:102003")
     hawaii = data.loc[data[state_col] == "15", :].to_crs("ESRI:102007")
 
     alaska.geometry = alaska.geometry.scale(0.35, 0.35, origin=(0, 0)).translate(-1.8e6, -1.6e6)
     hawaii.geometry = hawaii.geometry.translate(-1e6, -2e6)
-    pr.geometry = pr.geometry.translate(-0.9e6, 1e6).rotate(-16, origin=(0, 0))
+    pr.geometry = pr.geometry.translate(-1.2e6, 0.5e6)
     return cont, alaska, pr, hawaii
 
 
 def _join_state_geo_df(data: pd.DataFrame,
                        state_col: str,
                        geo_info: gpd.GeoDataFrame,
                        join_type: str = "right") -> gpd.GeoDataFrame:
```

### Comparing `covidcast-0.1.5/covidcast/__init__.py` & `covidcast-0.2.0/covidcast/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 Functions:
 
 * signal - Fetch a Pandas data frame for one signal.
 * metadata - Fetch metadata for all available signals.
 
 """
 
-from .covidcast import signal, metadata, aggregate_signals
+from .covidcast import signal, metadata, aggregate_signals, use_api_key
 from .plotting import plot, plot_choropleth, get_geo_df, animate
 from .geography import (fips_to_name, cbsa_to_name, abbr_to_name,
                         name_to_abbr, name_to_cbsa, name_to_fips,
                         fips_to_abbr, abbr_to_fips)
```

### Comparing `covidcast-0.1.5/covidcast/covidcast.py` & `covidcast-0.2.0/covidcast/covidcast.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,38 @@
 import pandas as pd
 import numpy as np
 from delphi_epidata import Epidata
 from epiweeks import Week
 
 from .errors import NoDataWarning
 
-# Point API requests to the AWS endpoint
+# Point API requests to the default endpoint
 Epidata.BASE_URL = "https://api.covidcast.cmu.edu/epidata/api.php"
 
 VALID_GEO_TYPES = {"county", "hrr", "msa", "dma", "state",  "hhs", "nation"}
 
 _ASYNC_CALL = False
 
+def use_api_key(key):
+    """Set the API key to use for all subsequent queries.
+
+    :param key: String containing the API key for you and/or your group.
+
+    Anyone may access the Epidata API anonymously without providing an API key.
+    Anonymous API access is currently rate-limited and with a maximum of two of
+    the requested parameters having multiple selections (signals, dates, issues,
+    regions, etc). To be exempt from these limits, use this function to apply an
+    API key to all subsequent queries. You can register for an API key at
+    <https://forms.gle/hkBr5SfQgxguAfEt7>.
+
+    Consult the `API documentation
+    <https://cmu-delphi.github.io/delphi-epidata/api/api_keys.html>`_
+    for details on our API key policies.
+    """
+    Epidata.auth = key
 
 def signal(data_source: str,
            signal: str,  # pylint: disable=W0621
            start_day: date = None,
            end_day: date = None,
            geo_type: str = "county",
            geo_values: Union[str, Iterable[str]] = "*",
@@ -179,16 +196,15 @@
         if start_day is None else start_day
 
     end_day = signal_meta["max_time"].to_pydatetime().date() \
         if end_day is None else end_day
 
     if start_day > end_day:
         raise ValueError("end_day must be on or after start_day, but "
-                         "start_day = '{start}', end_day = '{end}'".format(
-                             start=start_day, end=end_day))
+                         f"start_day = '{start_day}', end_day = '{end_day}'")
     if _ASYNC_CALL:
         dfs = _async_fetch_epidata(
             data_source, signal, start_day, end_day, geo_type,
             geo_values, as_of, issues, lag, time_type
         )
     else:
         dfs = _fetch_epidata(
@@ -499,20 +515,16 @@
             (meta.signal == signal) &
             (meta.time_type == "day") &
             (meta.geo_type == geo_type))
 
     matches = meta[mask]
 
     if matches.shape[0] == 0:
-        raise ValueError("Unable to find metadata for source '{source}', "
-                         "signal '{signal}', at '{geo_type}' "
-                         "resolution.".format(
-                             source=data_source,
-                             signal=signal,
-                             geo_type=geo_type))
+        raise ValueError(f"Unable to find metadata for source '{data_source}', "
+                         f"signal '{signal}', at '{geo_type}' resolution.")
 
     assert matches.shape[0] == 1, "it should be impossible to have two identical signals"
     output: dict = matches.to_dict("records")[0]
     return output
 
 
 def _date_to_api_string(date: date, time_type: str = "day") -> str:  # pylint: disable=W0621
```

