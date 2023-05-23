# Comparing `tmp/pfstools-0.2.3.tar.gz` & `tmp/pfstools-0.2.4.tar.gz`

## Comparing `pfstools-0.2.3.tar` & `pfstools-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pfstools-0.2.3/requirements.txt
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pfstools-0.2.3/testing.ipynb
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/__init__.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/output.py
--rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/sql.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pfstools-0.2.3/pfstools/tools.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pfstools-0.2.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pfstools-0.2.3/LICENSE
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pfstools-0.2.3/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pfstools-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 pfstools-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pfstools-0.2.4/requirements.txt
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pfstools-0.2.4/testing.ipynb
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pfstools-0.2.4/pfstools/__init__.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 pfstools-0.2.4/pfstools/output.py
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 pfstools-0.2.4/pfstools/sql.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 pfstools-0.2.4/pfstools/tools.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pfstools-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pfstools-0.2.4/LICENSE
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pfstools-0.2.4/README.md
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pfstools-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 pfstools-0.2.4/PKG-INFO
```

### Comparing `pfstools-0.2.3/testing.ipynb` & `pfstools-0.2.4/testing.ipynb`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.3/pfstools/output.py` & `pfstools-0.2.4/pfstools/output.py`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.3/pfstools/sql.py` & `pfstools-0.2.4/pfstools/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
 
 
         with self.connection() as con:
             if isinstance(sql, str):
                 sql = [sql]
             for q in list(sql):
                 con.execute(text(q))
- 
+            con.commit()
+            
     def __exit__(self):
         if not self.cnx is None:
             self.cnx.close()
 
 
     def to_sql(self,
         df,
```

### Comparing `pfstools-0.2.3/pfstools/tools.py` & `pfstools-0.2.4/pfstools/tools.py`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.3/.gitignore` & `pfstools-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.3/LICENSE` & `pfstools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pfstools-0.2.3/pyproject.toml` & `pfstools-0.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pfstools"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="Jake Bridge", email="bridge.jake@gmail.com" },
 ]
 description = "Tools for my regular use. Particular to my work environment: SQL Server with Windows authentication"
 readme = "README.md"
 requires-python = ">=3.7"
+dependencies = [
+  "pyodbc",
+  "pandas",
+  "sqlalchemy",
+  "python-dotenv",
+  "xlsxwriter",
+  "openpyxl"
+]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

