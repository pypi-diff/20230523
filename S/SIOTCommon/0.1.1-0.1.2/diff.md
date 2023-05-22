# Comparing `tmp/SIOTCommon-0.1.1.tar.gz` & `tmp/SIOTCommon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.1.1.tar", last modified: Sun May 21 19:26:17 2023, max compression
+gzip compressed data, was "SIOTCommon-0.1.2.tar", last modified: Mon May 22 22:46:36 2023, max compression
```

## Comparing `SIOTCommon-0.1.1.tar` & `SIOTCommon-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.886474 SIOTCommon-0.1.1/
--rw-rw-rw-   0        0        0      339 2023-05-21 19:26:17.885475 SIOTCommon-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.874472 SIOTCommon-0.1.1/SIOTC/
--rw-rw-rw-   0        0        0     1843 2023-04-20 13:29:33.000000 SIOTCommon-0.1.1/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     7748 2023-05-21 19:25:53.000000 SIOTCommon-0.1.1/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.1/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.1/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-05-21 19:26:17.883489 SIOTCommon-0.1.1/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-21 19:26:17.000000 SIOTCommon-0.1.1/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 19:26:17.886474 SIOTCommon-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-05-21 19:26:09.000000 SIOTCommon-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.530639 SIOTCommon-0.1.2/
+-rw-rw-rw-   0        0        0      339 2023-05-22 22:46:36.530639 SIOTCommon-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.1.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.519639 SIOTCommon-0.1.2/SIOTC/
+-rw-rw-rw-   0        0        0     2080 2023-05-22 22:40:04.000000 SIOTCommon-0.1.2/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0    11682 2023-05-22 22:45:01.000000 SIOTCommon-0.1.2/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      484 2023-04-20 13:32:21.000000 SIOTCommon-0.1.2/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2738 2023-05-05 13:45:10.000000 SIOTCommon-0.1.2/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-05-22 22:46:36.528670 SIOTCommon-0.1.2/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 22:46:36.000000 SIOTCommon-0.1.2/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 22:46:36.531636 SIOTCommon-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-05-22 22:46:30.000000 SIOTCommon-0.1.2/setup.py
```

### Comparing `SIOTCommon-0.1.1/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.1.2/SIOTC/DatabaseLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,20 @@
 def GetModel(table_name):
     session, Base = GetSession()
     table_model = getattr(Base.classes, table_name, None)
     if table_model is None:
         raise ValueError(f"Table model not found for table name: {table_name}")
     return table_model
 
+def GetModel(table_name, session, Base):
+    table_model = getattr(Base.classes, table_name, None)
+    if table_model is None:
+        raise ValueError(f"Table model not found for table name: {table_name}")
+    return table_model
+
 # map models, unessecary
 def Users(Base):
     Users = Base.classes.users
     return Users
 
 def GetKeys(Base):
     Keys = Base.classes.rsakeys
```

### Comparing `SIOTCommon-0.1.1/SIOTC/Operations.py` & `SIOTCommon-0.1.2/SIOTC/Operations.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,14 +37,28 @@
             logger.error('Error: No table exists with provided values')
             return None
         # If no error, query the row that matches the provided value
         else:
             return str(result.__dict__[column])
     return executeQuery(queryFunc, value, column, table)
 
+def GetSpecificFromColumnInTable(session, base, value, column, table):
+    # Check if value is provided
+    assert value is not None, "Error: No value provided"
+    # Get all rows from the specified table and column
+    theTable = getattr(base.classes, table, None)
+    result = session.query(theTable).filter_by(id=value).first()
+    # Check if an error occurred during retrieval
+    if result is None:
+        print('Error: No table exists with provided values')
+        logger.error('Error: No table exists with provided values')
+        return None
+    # If no error, query the row that matches the provided value
+    else:
+        return str(result.__dict__[column])
 # Add to any table to the database. Currently checks if missing columns and database constraints
 def InsertToTable(table, values):
     def queryFunc(session, base, values):
         # Get table model and columns
         name = "public." + table
         tableModel = base.metadata.tables.get(name)
         # Check if table exists
@@ -70,14 +84,48 @@
         newObject = tableModel.insert().values(**newValues)
         session.execute(newObject)
         session.commit()
         # Return success
         return True
     return executeQuery(queryFunc, values)
 
+def InsertMultipleToTable(table, values):
+    def queryFunc(session, base, values):
+        # Get table model and columns
+        name = "public." + table
+        tableModel = base.metadata.tables.get(name)
+        # Check if table exists
+        if tableModel is None:
+            return False, 'Error: Table not found'
+        columnsModel = tableModel.columns.keys()
+        newValues = []
+        # Ensure that values are provided
+        assert values is not None, "Error: No values provided"
+        # Loop through the columns in the table and create a list of dictionaries
+        # representing the rows to be inserted
+        for value in values:
+            tempValues = {}
+            for column in columnsModel:
+                if column in value:
+                    tempValues[column] = value[column]
+                elif column == 'id':
+                    # Generate a new id value using the default sequence
+                    query = f"SELECT nextval('{table}_id_seq')"
+                    result = session.execute(query)
+                    tempValues[column] = result.scalar()
+                else:
+                    tempValues[column] = None  # Use default value for missing columns
+            newValues.append(tempValues)
+        # Insert the new rows into the table
+        session.execute(tableModel.insert().values(newValues))
+        session.commit()
+        # Return success
+        return True
+    return executeQuery(queryFunc, values)
+
 def GetFromTable(table, id):
     def queryFunc(session, base, table, id):
         # Get the table model from the metadata based on the provided table name
         name = "public." + table
         tableModel = base.metadata.tables.get(name)
         # Check if the table exists in the metadata
         if tableModel is None:
@@ -106,24 +154,42 @@
         query = delete(tableModel).where(tableModel.c.id == id)
         # Execute the query and commit the transaction
         session.execute(query)
         session.commit()
         return True
     return executeQuery(queryFunc, table, id)
 
+def RemoveMultipleFromTable(table, ids):
+    def queryFunc(session, base, table, ids):
+        # Get the table model from the metadata based on the provided table name
+        name = "public." + table
+        tableModel = base.metadata.tables.get(name)
+        # Check if the table exists in the metadata
+        if tableModel is None:
+            return False, 'Error: Table not found'
+        # Ensure that an ID is provided
+        assert ids is not None, "Error: No ID provided"
+        # Create a query to remove a row with the given ID from the table
+        query = delete(tableModel).where(tableModel.c.id.in_(ids))
+        # Execute the query and commit the transaction
+        session.execute(query)
+        session.commit()
+        return True
+    return executeQuery(queryFunc, table, ids)
+
 def GetAllObjectsInModel(modelName):
     # Connect to database
     session, base = dl.GetSession()
     # If session or base is None, return error message
     if session is None or base is None:
         logger.error('Unable to connect to the database')
         return None
     try:
         # Retrieve all rows from the specified database model
-        rows = session.query(dl.GetModel(modelName)).all()
+        rows = session.query(dl.GetModel(modelName, session=session, Base=base)).all()
         # If there are no rows, return error message
         if not rows:
             logger.error('The list is empty')
             return None
         # Return the rows
         return rows
     except (SQLAlchemyError, IntegrityError, ValueError, AssertionError, TypeError) as e:
@@ -132,14 +198,36 @@
         print("Error:", e)
         logger.error(e)
         return None
     finally:
         # Close the session
         session.close()
 
+def GetAllObjectsInModel(modelName, session, base):
+    # Connect to database
+    # If session or base is None, return error message
+    if session is None or base is None:
+        logger.error('Unable to connect to the database')
+        return None
+    try:
+        # Retrieve all rows from the specified database model
+        rows = session.query(dl.GetModel(modelName, session=session, Base=base)).all()
+        # If there are no rows, return error message
+        if not rows:
+            logger.error('The list is empty')
+            return None
+        # Return the rows
+        return rows
+    except (SQLAlchemyError, IntegrityError, ValueError, AssertionError, TypeError) as e:
+        # If there is an error, rollback the session, print the error, and return it
+        session.rollback()
+        print("Error:", e)
+        logger.error(e)
+        return None
+
 def GetAllFromTable(tableName):
     def queryFunc(session, base, tableName):
         # Construct the full table name
         realName = "public." + tableName
         # Get the table object for the specified table name
         tableObject = base.metadata.tables.get(realName)
         # Check if the table object exists
```

### Comparing `SIOTCommon-0.1.1/SIOTC/helperhttps.py` & `SIOTCommon-0.1.2/SIOTC/helperhttps.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.1/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.1.2/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.1.1/setup.py` & `SIOTCommon-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```

