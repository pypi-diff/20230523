# Comparing `tmp/SIOTCommon-0.1.3.tar.gz` & `tmp/SIOTCommon-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.1.3.tar", last modified: Mon May 22 23:18:59 2023, max compression
+gzip compressed data, was "SIOTCommon-0.1.4.tar", last modified: Tue May 23 17:38:55 2023, max compression
```

## Comparing `SIOTCommon-0.1.3.tar` & `SIOTCommon-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.698311 SIOTCommon-0.1.3/
--rw-rw-rw-   0        0        0      339 2023-05-22 23:18:59.697311 SIOTCommon-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.3/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.688308 SIOTCommon-0.1.3/SIOTC/
--rw-rw-rw-   0        0        0     2374 2023-05-22 23:17:55.000000 SIOTCommon-0.1.3/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0    11682 2023-05-22 22:45:01.000000 SIOTCommon-0.1.3/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.3/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.3/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-05-22 23:18:59.696308 SIOTCommon-0.1.3/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 23:18:59.000000 SIOTCommon-0.1.3/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 23:18:59.699329 SIOTCommon-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-05-22 23:18:50.000000 SIOTCommon-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:38:55.628134 SIOTCommon-0.1.4/
+-rw-rw-rw-   0        0        0      339 2023-05-23 17:38:55.628134 SIOTCommon-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.4/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 17:38:55.618140 SIOTCommon-0.1.4/SIOTC/
+-rw-rw-rw-   0        0        0     2419 2023-05-23 17:35:47.000000 SIOTCommon-0.1.4/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0    11693 2023-05-23 17:36:08.000000 SIOTCommon-0.1.4/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.4/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2860 2023-05-23 17:38:07.000000 SIOTCommon-0.1.4/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:38:55.626136 SIOTCommon-0.1.4/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-23 17:38:55.000000 SIOTCommon-0.1.4/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-23 17:38:55.000000 SIOTCommon-0.1.4/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:38:55.000000 SIOTCommon-0.1.4/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-05-23 17:38:55.000000 SIOTCommon-0.1.4/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-23 17:38:55.000000 SIOTCommon-0.1.4/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:38:55.629133 SIOTCommon-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-05-23 17:38:52.000000 SIOTCommon-0.1.4/setup.py
```

### Comparing `SIOTCommon-0.1.3/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.1.4/SIOTC/DatabaseLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     # Check if a session already exists
     if global_session is not None:
         return global_session
 
     # Create a new session if it doesn't exist
     Base = automap_base()
-    engine = create_engine(first_line, echo=True)
+    engine = create_engine('postgresql://postgres:3485780@localhost:5432/sweiotdb', echo=True)
     Base.prepare(engine, reflect=True, schema='public')
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
 
     # Store the session in the global variable
     global_session = session
```

### Comparing `SIOTCommon-0.1.3/SIOTC/Operations.py` & `SIOTCommon-0.1.4/SIOTC/Operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         session.rollback()
         logger.error(str(e))
         return None
     finally:
         # Close the session
         session.close()
 
-def GetSpecificFromColumnInTable(value, column, table):
+def GetSpecificFromColumnInTableWithSession(value, column, table):
     def queryFunc(session, base, value, column, table):
         # Check if value is provided
         assert value is not None, "Error: No value provided"
         # Get all rows from the specified table and column
         theTable = getattr(base.classes, table, None)
         result = session.query(theTable).filter_by(id=value).first()
         # Check if an error occurred during retrieval
```

### Comparing `SIOTCommon-0.1.3/SIOTC/helperhttps.py` & `SIOTCommon-0.1.4/SIOTC/helperhttps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from flask import request, jsonify 
 from functools import wraps
 from flask_jwt_extended import get_jwt_identity, verify_jwt_in_request
 from enum import Enum
 import SIOTC.Operations as op
+import SIOTC.DatabaseLayer as db
 import re
 
 # Checks what type of data is being sent and returns correct object
 def CheckContentType():
     content_type = request.headers.get('Content-Type')
     if content_type == 'application/json':
         print('Json Message received')
@@ -49,29 +50,30 @@
         # Get the id from the JWT
         jwt_id = get_jwt_identity()
 
         user = jwt_id
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
 
-        user_role = op.GetSpecificFromColumnInTable(user, 'role_id', 'users')
+        user_role = op.GetSpecificFromColumnInTableWithSession(user, 'role_id', 'users')
 
         if user_role != 'System Administrator':
             return jsonify({'message': 'You do not have permission to access this endpoint.'}), 403
         return fn(*args, **kwargs)
     return wrapper
 
 
 def device_ownership_required(f):
     @wraps(f)
     def wrapper(*args, **kwargs):
         verify_jwt_in_request()
         user = get_jwt_identity()
         if not user:
             return jsonify({'message': 'Current user not provided.'}), 401
-        customerID = op.GetSpecificFromColumnInTable(user, 'customer_id', 'users')
-        customerFK = op.GetSpecificFromColumnInTable(user, 'customer_id', 'devices')
+        dbsession, Base = db.GetSession()
+        customerID = op.GetSpecificFromColumnInTable(dbsession, Base, user, 'customer_id', 'users')
+        customerFK = op.GetSpecificFromColumnInTable(dbsession, Base, user, 'customer_id', 'devices')
 
         if customerID != customerFK:
             return jsonify({'message': 'User does not own device.'}), 403
         return f(*args, **kwargs)
     return wrapper
```

### Comparing `SIOTCommon-0.1.3/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.1.4/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.3/setup.py` & `SIOTCommon-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

