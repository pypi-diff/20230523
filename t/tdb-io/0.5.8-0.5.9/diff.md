# Comparing `tmp/tdb_io-0.5.8.tar.gz` & `tmp/tdb_io-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdb_io-0.5.8.tar", last modified: Fri Feb 17 16:29:31 2023, max compression
+gzip compressed data, was "tdb_io-0.5.9.tar", last modified: Tue May 23 12:30:23 2023, max compression
```

## Comparing `tdb_io-0.5.8.tar` & `tdb_io-0.5.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-02-17 16:29:31.038693 tdb_io-0.5.8/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     8429 2023-02-17 16:29:31.038693 tdb_io-0.5.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     6098 2023-02-17 16:29:29.000000 tdb_io-0.5.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-02-17 16:29:31.038693 tdb_io-0.5.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11288 2023-01-28 21:39:28.000000 tdb_io-0.5.8/bin/tdb_io
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-02-17 16:29:31.038693 tdb_io-0.5.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1630 2023-01-28 21:41:18.000000 tdb_io-0.5.8/setup.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-02-17 16:29:31.038693 tdb_io-0.5.8/tdb_io/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19469 2021-09-03 09:09:09.000000 tdb_io-0.5.8/tdb_io/h5t.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6199 2023-01-28 21:38:31.000000 tdb_io-0.5.8/tdb_io/h5toinfl.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17494 2023-02-17 16:28:41.000000 tdb_io-0.5.8/tdb_io/influx.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13587 2021-09-03 09:09:09.000000 tdb_io-0.5.8/tdb_io/mongo.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1474 2021-09-03 09:09:09.000000 tdb_io-0.5.8/tdb_io/org2h5.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       20 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-02-17 16:29:31.038693 tdb_io-0.5.8/tdb_io.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     8429 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      279 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       64 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2023-02-17 16:29:30.000000 tdb_io-0.5.8/tdb_io.egg-info/top_level.txt
+drwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)        0 2023-05-23 12:30:23.406855 tdb_io-0.5.9/
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)     8429 2023-05-23 12:30:23.406855 tdb_io-0.5.9/PKG-INFO
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)     6098 2023-05-23 12:12:19.000000 tdb_io-0.5.9/README.md
+drwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)        0 2023-05-23 12:30:23.402855 tdb_io-0.5.9/bin/
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)    11716 2023-05-23 12:27:10.000000 tdb_io-0.5.9/bin/tdb_io
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)       38 2023-05-23 12:30:23.406855 tdb_io-0.5.9/setup.cfg
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)     1639 2023-05-23 12:12:19.000000 tdb_io-0.5.9/setup.py
+drwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)        0 2023-05-23 12:30:23.402855 tdb_io-0.5.9/tdb_io/
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)    19469 2023-05-23 12:12:19.000000 tdb_io-0.5.9/tdb_io/h5t.py
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)     6199 2023-05-23 12:12:19.000000 tdb_io-0.5.9/tdb_io/h5toinfl.py
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)    19679 2023-05-23 12:12:19.000000 tdb_io-0.5.9/tdb_io/influx.py
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)    13587 2023-05-23 12:12:19.000000 tdb_io-0.5.9/tdb_io/mongo.py
+-rwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)     1474 2023-05-23 12:12:19.000000 tdb_io-0.5.9/tdb_io/org2h5.py
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)       20 2023-05-23 12:30:22.000000 tdb_io-0.5.9/tdb_io/version.py
+drwxrwxr-x   0 mitja-admin  (1000) mitja-admin  (1000)        0 2023-05-23 12:30:23.406855 tdb_io-0.5.9/tdb_io.egg-info/
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)     8429 2023-05-23 12:30:23.000000 tdb_io-0.5.9/tdb_io.egg-info/PKG-INFO
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)      279 2023-05-23 12:30:23.000000 tdb_io-0.5.9/tdb_io.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)        1 2023-05-23 12:30:23.000000 tdb_io-0.5.9/tdb_io.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)       71 2023-05-23 12:30:23.000000 tdb_io-0.5.9/tdb_io.egg-info/requires.txt
+-rw-rw-r--   0 mitja-admin  (1000) mitja-admin  (1000)        7 2023-05-23 12:30:23.000000 tdb_io-0.5.9/tdb_io.egg-info/top_level.txt
```

### Comparing `tdb_io-0.5.8/PKG-INFO` & `tdb_io-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdb_io
-Version: 0.5.8
+Version: 0.5.9
 Summary: Automatically created environment for python package
 Home-page: UNKNOWN
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: Project: tdb~io~
         ================
```

### Comparing `tdb_io-0.5.8/README.md` & `tdb_io-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tdb_io-0.5.8/bin/tdb_io` & `tdb_io-0.5.9/bin/tdb_io`

 * *Files 8% similar despite different names*

```diff
@@ -186,17 +186,17 @@
             delete = False
             dbpr = False
             if len(args)>1:
                 dbcheck = args[1]
                 print("D... args  = ",args)
                 print("D... kwargs=",kwargs)
             if len(args)>2:
-                sercheck = args[2]
+                sercheck = args[2]  # which series
             if len(args)>3:
-                qlimit = args[3]
+                qlimit = args[3]   # how many
             if len(args)>4:
                 IP = args[4]
             if len(kwargs)>0:
                 if 'delete' in kwargs.keys():
                     delete = kwargs["delete"]
                 if 'ip' in kwargs.keys():
                     IP = kwargs["ip"]
@@ -298,7 +298,12 @@
 
 def test_launch():
     assert launch('A')==0
 
 if __name__=="__main__":
     print("D...        tdb_io: version:",__version__)
     Fire( launch )
+    print("    ...  use  'column -s, -t < somefile.csv | less -#2 -N -S'  to view")
+    print("    ...    or with : cargo install csvlens; csvlens")
+    print('    ...    or with pip install visidata;  vd file.csv;  ')
+    print('                 shift-f [sort ]sort shift-s  "copy  |regex  shift-cd delcol   q')
+    print('    ...          #int %floa @date !defx-axe .plot  g.allplot   zz zoom  ')
```

### Comparing `tdb_io-0.5.8/setup.py` & `tdb_io-0.5.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     version=get_version("tdb_io/version.py"),
     #packages=find_packages(),
     packages=['tdb_io'],
     package_data={'tdb_io': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/tdb_io'],
-    install_requires = ['pymongo','matplotlib','argparse','pandas','numpy','datetime','fire','influxdb'],
+    install_requires = ['pymongo','matplotlib','argparse','pandas','numpy','datetime','fire','influxdb','tables'],
 )
 #
 #   To RECOVER AND ACCESS THE Data later in module: :
 #  X DATA_PATH = pkg_resources.resource_filename('tdb_io', 'data/')
 #  X DB_FILE =   pkg_resources.resource_filename('tdb_io', 'data/file')
 #   DB_FILE = pkg_resources.resource_filename(
 #       pkg_resources.Requirement.parse('nuphy2'),
```

### Comparing `tdb_io-0.5.8/tdb_io/h5t.py` & `tdb_io-0.5.9/tdb_io/h5t.py`

 * *Files identical despite different names*

### Comparing `tdb_io-0.5.8/tdb_io/h5toinfl.py` & `tdb_io-0.5.9/tdb_io/h5toinfl.py`

 * *Files identical despite different names*

### Comparing `tdb_io-0.5.8/tdb_io/influx.py` & `tdb_io-0.5.9/tdb_io/influx.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tdb_io.version import __version__
 
 import pandas as pd
 
 from influxdb import InfluxDBClient
 #from pymongo import MongoClient
 #import pymongo # to get ASCENDING
-import datetime
+import datetime as dt
 import time
 import os
 import json
 import sys
 
 import socket
 import sys
@@ -28,14 +28,26 @@
 
 
 # if DEBUG:print("D...  project/module:  tdb_io/influx :", __version__ )
 
 
 #OK
 #===============================================================
+def is_int(n):
+    print(f"/{n}/")
+    try:
+        float_n = float(n)
+        print(f"/{float_n}/")
+        int_n = int(float_n)
+        print(f"/{int_n}/")
+    except ValueError:
+        return False
+    else:
+        return float_n == int_n
+
 
 def check_port(IP="127.0.0.1"):
     """
 Checks if influx runs on IP
     """
     ok = False
     client = InfluxDBClient(host=IP, port=8086)
@@ -55,15 +67,15 @@
 
 def check_databases(IP="127.0.0.1", user="", password=""):
     """
 Checks if influx runs on IP AND shows databases
 r=client.query('SELECT "temp" FROM "autogen"."idx232"')
 
     """
-    if DEBUG:print("D... checkd: ",IP,user)
+    #if DEBUG:print("D... checkd: ",IP,user)
     ok = False
     autho = False
     dbs = []
     if user=="":
         client = InfluxDBClient(host=IP, port=8086)
     else:
         client = InfluxDBClient(host=IP, port=8086, username=user, password=password)
@@ -76,29 +88,29 @@
             print("X... NO DATABASE ON ",IP)
         if  type(ex).__name__.find("InfluxDBClientError")==0:
             print("i... database exists, authorization needed")
             ok = False
             autho = True
     if autho and user=="":
         print("I... trying with credentials from CONFIG")
-        creds,ips = read_infl_credentials( DEBUG = DEBUG)
+        creds,ips = read_infl_credentials( DEBUG = 0)
 
         # NO SSL
         gotit = False
         try:
-            if DEBUG:print("D... chkd:  getting client NO SSL")
+            #if DEBUG:print("D... chkd:  getting client NO SSL")
             client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=False, timeout=3)
             client.get_list_database() # this checks error
             gotit = True
         except:
             print("X... exception without SSL, trying with SSL")
 
         if not gotit:
             try:
-                if DEBUG:print("D... chkd: getting client WITH SSL")
+                #if DEBUG:print("D... chkd: getting client WITH SSL")
                 client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=True, timeout=3)
                 client.get_list_database() # this checks error
             except:
                 print("X... ",IP, 8086,creds[0],creds[1],creds[2] )
 
         dbs = client.get_list_database()
     return dbs
@@ -113,15 +125,15 @@
                  user="", password="",
                  delete=False):
     """
 Checks if influx runs on IP, fir each DATABASE it shows ALL SERIES
 r=client.query('SELECT "temp" FROM "autogen"."idx232"')
 
     """
-    if DEBUG:print("D... checks: ",IP,user)
+    #if DEBUG:print("D... checks: ",IP,user)
 
     ok = False
     autho = False
     dbs = []
     liseries = []
     if user=="":
         client = InfluxDBClient(host=IP, port=8086)
@@ -136,48 +148,68 @@
             print("X... NO DATABASE ON ",IP)
         if  type(ex).__name__.find("InfluxDBClientError")==0:
             print("i... database exists, authorization needed")
             ok = False
             autho = True
     if autho and user=="":
         print("I... trying with credentials from CONFIG")
-        creds,ips = read_infl_credentials( DEBUG=DEBUG)
+        creds,ips = read_infl_credentials( DEBUG=0)
 
         # NO SSL
         gotit = False
-        mytimeout =3
-        if qlimit > 10000:
-            mytimeout = 10
-        if qlimit > 60000:
-            mytimeout = 20
-        if qlimit > 120000:
-            mytimeout = 30
+        limit_int = True
+        mytimeout =3 # below 10000 events
+
+        # ------------ make time possible  1h 1d 1w
+        #  > SELECT "water_level" FROM "h2o_feet" WHERE time > now() - 1h
+        if type(qlimit) is str:
+            limit_int = False
+            if not qlimit[-1] in ["s","m","h","d","w"]:
+                print("X...   limit is string but it is not 1s 1m 1h 1d 1w:", qlimit)
+                print("X.... exit")
+                sys.exit(1)
+            intnum = "".join(qlimit[:-1])
+            if  not is_int(intnum):
+                print("X...   limit is string but it is not  integer s m h d w:", qlimit, intnum)
+                print("X.... exit")
+                sys.exit(1)
+            mytimeout = 30 # worst case scenario
+        #-------------
+        if limit_int:
+            if qlimit > 10000:
+                mytimeout = 10
+            if qlimit > 60000:
+                mytimeout = 20
+            if qlimit > 120000:
+                mytimeout = 30
+
+
         try:
             client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=False, timeout=mytimeout)
             dbs = client.get_list_database() # generates exception
             gotit = True
         except:
             print("X... chks: exception without SSL")
 
         if not gotit:
-            if DEBUG:print("D... chks: trying with SSL")
+            #if DEBUG:print("D... chks: trying with SSL")
             client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=True, timeout=mytimeout)
             dbs = client.get_list_database() # generates excep
 
-        if DEBUG:print("D... client obtained - nossl")
+        #if DEBUG:print("D... client obtained - nossl")
         dbs = client.get_list_database()
     #print("D... list of databases obtained", dbs)
 
 
     TERMW = 55
     TERMW, rows = os.get_terminal_size(0)
     #TERMW-=1
     #-------------------------------- if series not given, list them
     if series == "":
-        if DEBUG:print("D... stage check....")
+        #if DEBUG:print("D... stage check....")
         for i in dbs:
             if i["name"].find("_")==0:
                 continue
             if (database!="")and(database!=i["name"]):
                 continue
             print("\n",i['name'],"_"*(TERMW-len(i['name'])-2) )
             sers = client.get_list_series( i['name'] )
@@ -200,15 +232,15 @@
                 if k % one == 0:
                     print()
             print()
         print()
         return liseries
 
     #-----series given....we go to "read" option
-    if DEBUG:print("D... stage read....")
+    #if DEBUG:print("D... stage read....")
     dbs = [i['name'] for i in dbs]
     if not database in dbs:
         print("X ... no such database - exit", database,"in", dbs)
         sys.exit(1)# quit()
     i = database
     print(i,"_"*(TERMW-len(i)-2) )
 
@@ -218,39 +250,54 @@
         sys.exit(1)# quit()
 
     client.switch_database(i)
     #
     # i must find columns:
 
     #r = client.query('SELECT "temp" FROM "autogen"."'+series+'" ')
-    print("i... quering with limit ", qlimit)
 
-    r = client.query('SELECT * FROM "autogen"."'+series+'" ORDER BY time ASC LIMIT '+str(qlimit)  )
-    #print(r.raw)
-    cols = r.raw['series'][0]['columns']
-    points = r.get_points()
-    print(cols)
-    print()
-    ppoints=0
-    dfdict = {}
-    divme = 1000
-    #h5 = h5py.File("savetest.h5")
-    for p in points:
-        #print(p, type(p))
-        dfdict[ppoints] = p
-        ppoints+=1
-        if (ppoints % divme)==0:
-            print("{:9.0f} * {}  ".format(ppoints/ divme, divme ), end="\r" )
-    print("\nCOLUMNS:",cols)
-    print("TOTAL: {} points printed, the demanded number was {}".format( ppoints, qlimit ) )
-    df = pd.DataFrame.from_dict(dfdict, "index")
-    print(df.head() )
-    print(df.tail() )
+    # print("________________________________")
+    # if limit_int:
+    #     print("i... quering INC with limit: ", qlimit)
+    #     r = client.query('SELECT * FROM "autogen"."'+series+'" ORDER BY time ASC LIMIT '+str(qlimit)  )
+    # else:
+    #     print("i... quering INC with time: ", qlimit)
+    #     r = client.query('SELECT * FROM "autogen"."'+series+'" WHERE TIME > now() - '+str(qlimit) +" ORDER BY time ASC " )
+
+    # #print(r.raw)
+    # cols = r.raw['series'][0]['columns']
+    # points = r.get_points()
+    # print(cols)
+    # print()
+    # ppoints=0
+    # dfdict = {}
+    # divme = 1000
+    # #h5 = h5py.File("savetest.h5")
+    # for p in points:
+    #     #print(p, type(p))
+    #     dfdict[ppoints] = p
+    #     ppoints+=1
+    #     if (ppoints % divme)==0:
+    #         print("{:9.0f} * {}  ".format(ppoints/ divme, divme ), end="\r" )
+    # print("\nCOLUMNS:",cols)
+    # print("TOTAL: {} points printed, the demanded number was {}".format( ppoints, qlimit ) )
+    # df = pd.DataFrame.from_dict(dfdict, "index")
+    # print(df.head() )
+    # print(df.tail() )
+
+    print("________________________________")
+    if limit_int:
+        print("i... quering DESC with limit: ", qlimit)
+        r = client.query('SELECT * FROM "autogen"."'+series+'" ORDER BY time DESC LIMIT '+str(qlimit)  )
+    else:
+        print("i... quering DESC with time: ", qlimit)
+        r = client.query('SELECT * FROM "autogen"."'+series+'" WHERE TIME > now() - '+str(qlimit) +" ORDER BY time DESC " )
+
+    # r = client.query('SELECT * FROM "autogen"."'+series+'" ORDER BY time DESC LIMIT '+str(qlimit)  )
 
-    r = client.query('SELECT * FROM "autogen"."'+series+'" ORDER BY time DESC LIMIT '+str(qlimit)  )
     #print(r.raw)
     cols = r.raw['series'][0]['columns']
     points = r.get_points()
     print(cols)
     print()
     ppoints=0
     dfdict = {}
@@ -266,16 +313,25 @@
     print("TOTAL: {} points printed, the demanded number was {}".format( ppoints, qlimit ) )
 
     df = pd.DataFrame.from_dict(dfdict, "index")
     print(df.head() )
     print(df.tail() )
 
     #hdf = HDFStore("influx_{}_{}.h5".format(series,ppoints) )
-    fname = "influx_{}_{}.h5".format(series,ppoints)
-    df.to_hdf( fname, series ,format ="table", mode = 'a' )
+    now = dt.datetime.now().strftime("%Y%m%d_%H%M%S")
+    fname = "influx_{}_{}_{}".format(series,now,ppoints)
+    fnameh5 = "{}.h5".format(fname)
+    fnamecsv = "{}.csv".format(fname)
+    fnameparq = "{}.parquet".format(fname)
+    print("i... saving h5", fnameh5)
+    df.to_hdf( fnameh5, series ,format ="table", mode = 'a' ) # this was ment as incremental .... sorry
+    print("i... saving csv", fnamecsv)
+    df.to_csv( fnamecsv )
+    print("i... saving parquet", fnameparq)
+    df.to_parquet( fnameparq )
 
     if delete:
         DELETE = 'DELETE  FROM "'+series+'" '
         print( DELETE )
         res = input("REALLY DELETE? y/n")
         if res == "y":
             r = client.query( DELETE)
@@ -310,21 +366,21 @@
             print("X... NO DATABASE ON ",IP)
         if  type(ex).__name__.find("InfluxDBClientError")==0:
             print("i... database exists, authorization needed")
             ok = False
             autho = True
     if autho and user=="":
         print("I... trying with credentials from CONFIG")
-        creds,ips = read_infl_credentials( DEBUG=DEBUG)
+        creds,ips = read_infl_credentials( DEBUG=0)
         # NO SSL
         client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=False, timeout=3)
-        if DEBUG:print("D... client obtained - empty")
+        #if DEBUG:print("D... client obtained - empty")
         dbs = client.get_list_database()
     dbs = [i['name'] for i in dbs]
-    if DEBUG:print("D... list of databases obtained", dbs)
+    #if DEBUG:print("D... list of databases obtained", dbs)
 
 
     TERMW = 55
     TERMW, rows = os.get_terminal_size(0)
 
     if not database in dbs:
         print("X ... no such database - exit", database,"in", dbs)
@@ -368,15 +424,15 @@
 def checkout_hostname_database(database="test", series='idx0', IP="127.0.0.1", user="", password="", delete = False):
     """
     Check Hostname in the LOCAL influx DATABASES --- IF DIFFER: DROP;
     """
 
     MYHOSTNAME = socket.gethostname()
     NEWDB = "i_am_" + MYHOSTNAME
-    if DEBUG:print("D... gethostname:", MYHOSTNAME, NEWDB )
+    #if DEBUG:print("D... gethostname:", MYHOSTNAME, NEWDB )
 
     IP = "127.0.0.1"
     ok = False
     autho = False
     dbs = []
 
     if user=="":
@@ -391,40 +447,40 @@
             print("X... NO DATABASE ON ",IP)
         if  type(ex).__name__.find("InfluxDBClientError")==0:
             print("i... database exists, authorization needed")
             ok = False
             autho = True
     if autho and user=="":
         print("I... trying with credentials from CONFIG")
-        creds,ips = read_infl_credentials(DEBUG=DEBUG)
+        creds,ips = read_infl_credentials(DEBUG=0)
 
         # NO SSL
         gotit = False
         try:
             client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=False, timeout=3)
             dbs = client.get_list_database()
             gotit = True
-            if DEBUG:print("D... client obtained with NO SSL")
+            #if DEBUG:print("D... client obtained with NO SSL")
         except:
             print("X... NO SSL - didnt work, I try SSL")
 
         if not gotit:
             try:
-                if DEBUG:print("D... client trying with  SSL")
+                #if DEBUG:print("D... client trying with  SSL")
                 client = InfluxDBClient(IP, 8086,creds[0],creds[1],creds[2],ssl=True, timeout=3)
                 dbs = client.get_list_database()
-                if DEBUG:print("D... client obtained with WITH SSL")
+                #if DEBUG:print("D... client obtained with WITH SSL")
             except:
                 print("X... WITH SSL - didnt work", IP, 8086,creds[0],creds[1],creds[2])
 
 
         dbs = client.get_list_database()
     dbs = [i['name'] for i in dbs]
 
-    if DEBUG:print("D... list of databases obtained", dbs)
+    #if DEBUG:print("D... list of databases obtained", dbs)
 
     host_present = False
     ohost_present = False
     ohost_name = "x"
     for i in dbs:
         if i == NEWDB:
             host_present = True
@@ -432,15 +488,15 @@
             ohost_present = True
             ohost_name = i
     if ohost_present:
         print("!... other host present:",ohost_name," - DROP it:", ohost_present)
         client.drop_database(ohost_name)
         #return
     if host_present:
-        if DEBUG:print("D... all ok, my hostname is there with i_am_...")
+        #if DEBUG:print("D... all ok, my hostname is there with i_am_...")
         return
     print("!... CREATE DATABASE myself:", NEWDB)
     client.create_database(NEWDB)
 
 
 #def drop_measurement():
```

### Comparing `tdb_io-0.5.8/tdb_io/mongo.py` & `tdb_io-0.5.9/tdb_io/mongo.py`

 * *Files identical despite different names*

### Comparing `tdb_io-0.5.8/tdb_io/org2h5.py` & `tdb_io-0.5.9/tdb_io/org2h5.py`

 * *Files identical despite different names*

### Comparing `tdb_io-0.5.8/tdb_io.egg-info/PKG-INFO` & `tdb_io-0.5.9/tdb_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdb-io
-Version: 0.5.8
+Version: 0.5.9
 Summary: Automatically created environment for python package
 Home-page: UNKNOWN
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: Project: tdb~io~
         ================
```

