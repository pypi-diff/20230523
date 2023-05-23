# Comparing `tmp/nice-sql-0.0.7.tar.gz` & `tmp/nice-sql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice-sql-0.0.7.tar", last modified: Wed Sep  7 11:30:29 2022, max compression
+gzip compressed data, was "nice-sql-1.0.0.tar", last modified: Tue May 23 13:26:04 2023, max compression
```

## Comparing `nice-sql-0.0.7.tar` & `nice-sql-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2022-09-07 11:30:29.928101 nice-sql-0.0.7/
--rw-r--r--   0 lichengming   (502) staff       (20)     2585 2022-09-07 11:30:29.927845 nice-sql-0.0.7/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)     2282 2022-09-07 11:29:17.000000 nice-sql-0.0.7/README.md
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2022-09-07 11:30:29.917884 nice-sql-0.0.7/nice_sql.egg-info/
--rw-r--r--   0 lichengming   (502) staff       (20)     2585 2022-09-07 11:30:29.000000 nice-sql-0.0.7/nice_sql.egg-info/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)      387 2022-09-07 11:30:29.000000 nice-sql-0.0.7/nice_sql.egg-info/SOURCES.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        1 2022-09-07 11:30:29.000000 nice-sql-0.0.7/nice_sql.egg-info/dependency_links.txt
--rw-r--r--   0 lichengming   (502) staff       (20)       23 2022-09-07 11:30:29.000000 nice-sql-0.0.7/nice_sql.egg-info/requires.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        8 2022-09-07 11:30:29.000000 nice-sql-0.0.7/nice_sql.egg-info/top_level.txt
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2022-09-07 11:30:29.924423 nice-sql-0.0.7/nicesql/
--rw-r--r--   0 lichengming   (502) staff       (20)      122 2022-09-07 10:17:32.000000 nice-sql-0.0.7/nicesql/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     2337 2022-09-07 11:25:14.000000 nice-sql-0.0.7/nicesql/shortcuts.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2022-09-07 11:30:29.927480 nice-sql-0.0.7/nicesql/sqlengine/
--rw-r--r--   0 lichengming   (502) staff       (20)      496 2022-09-07 09:58:41.000000 nice-sql-0.0.7/nicesql/sqlengine/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      291 2022-09-07 09:58:41.000000 nice-sql-0.0.7/nicesql/sqlengine/base.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1144 2022-09-07 11:26:23.000000 nice-sql-0.0.7/nicesql/sqlengine/mysql.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1039 2022-09-07 10:14:01.000000 nice-sql-0.0.7/nicesql/sqlengine/sqlite.py
--rw-r--r--   0 lichengming   (502) staff       (20)      379 2022-09-01 01:18:46.000000 nice-sql-0.0.7/nicesql/sqlmodel.py
--rw-r--r--   0 lichengming   (502) staff       (20)      844 2022-09-07 10:13:50.000000 nice-sql-0.0.7/nicesql/sqlresult.py
--rw-r--r--   0 lichengming   (502) staff       (20)      678 2022-09-07 07:15:28.000000 nice-sql-0.0.7/nicesql/utils.py
--rw-r--r--   0 lichengming   (502) staff       (20)       38 2022-09-07 11:30:29.928185 nice-sql-0.0.7/setup.cfg
--rw-r--r--   0 lichengming   (502) staff       (20)      718 2022-09-07 11:26:34.000000 nice-sql-0.0.7/setup.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.956797 nice-sql-1.0.0/
+-rw-r--r--   0 lichengming   (502) staff       (20)     3143 2023-05-23 13:26:04.956393 nice-sql-1.0.0/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)     2840 2023-05-23 13:22:52.000000 nice-sql-1.0.0/README.md
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.945513 nice-sql-1.0.0/nice_sql.egg-info/
+-rw-r--r--   0 lichengming   (502) staff       (20)     3143 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)      603 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)       23 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/requires.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-05-23 13:26:04.000000 nice-sql-1.0.0/nice_sql.egg-info/top_level.txt
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.945945 nice-sql-1.0.0/nicesql/
+-rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/__init__.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.950543 nice-sql-1.0.0/nicesql/engine/
+-rw-r--r--   0 lichengming   (502) staff       (20)       54 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1002 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/base.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      330 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/engine/impl_dummy.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1561 2023-05-23 13:15:25.000000 nice-sql-1.0.0/nicesql/engine/impl_mysql.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1439 2023-05-23 13:17:53.000000 nice-sql-1.0.0/nicesql/engine/impl_sqlite.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1089 2023-05-23 10:12:03.000000 nice-sql-1.0.0/nicesql/engine/reg.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1104 2023-05-23 13:14:48.000000 nice-sql-1.0.0/nicesql/engine/sqlformat.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.952829 nice-sql-1.0.0/nicesql/shortcut/
+-rw-r--r--   0 lichengming   (502) staff       (20)      116 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/shortcut/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      727 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/shortcut/annotate.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1208 2023-05-23 12:55:23.000000 nice-sql-1.0.0/nicesql/shortcut/core.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-05-23 13:26:04.955779 nice-sql-1.0.0/nicesql/utils/
+-rw-r--r--   0 lichengming   (502) staff       (20)      148 2023-05-23 13:11:34.000000 nice-sql-1.0.0/nicesql/utils/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      326 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/error.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      386 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/fill_model.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      556 2023-05-23 10:10:49.000000 nice-sql-1.0.0/nicesql/utils/parse_db_url.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1947 2023-05-23 12:48:20.000000 nice-sql-1.0.0/nicesql/utils/pick_value.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-05-23 13:26:04.956928 nice-sql-1.0.0/setup.cfg
+-rw-r--r--   0 lichengming   (502) staff       (20)      718 2023-05-23 10:12:03.000000 nice-sql-1.0.0/setup.py
```

### Comparing `nice-sql-0.0.7/PKG-INFO` & `nice-sql-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 0.0.7
+Version: 1.0.0
 Summary: easy nice sql: decorator with sql
 Home-page: https://github.com/657143946/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -24,85 +24,108 @@
 丨     person        丨
  --------------------
 丨 id        int     丨
 丨 name      string  丨
  --------------------
 """
 
-import nicesql
-from nicesql.sqlmodel import SqlModel
-from nicesql.sqlengine.sqlite import Sqlite
 from typing import List
 
-nicesql.register(Sqlite(":memory:"))
+from nicesql.engine import reg_engine
+from nicesql.shortcut.annotate import insert, delete, update, select, ddl
 
 
-class Person(SqlModel):
+class Person:
     def __init__(self):
         self.id = None
         self.name = None
 
 
-@nicesql.bind("""
-    create table if not exists person(
-        id      integer not null primary key,
-        name    varchar(127)
-    )
-""")
-def create_person_table():
-    pass
-
-
-@nicesql.insert("insert into person(name) values ({name})")
-def insert(name) -> int:
-    pass
-
-
-@nicesql.select("select * from person where id={id}", model=Person, first=True)
-def get(id) -> Person:
-    pass
-
-
-@nicesql.select("select * from person where name like {name}", model=Person)
-def find(name) -> List[Person]:
-    pass
-
-
-@nicesql.update("update person set name={name} where id={id}")
-def update_name(id: int, name: str) -> int:
-    pass
-
-
-@nicesql.delete("delete from person where name={name}")
-def delete(name: str) -> int:
-    pass
-
-
-if __name__ == '__main__':
-    create_person_table()  # create person table
-
-    id = insert("name001")  # id=1
-    person = get(id)  # person=Person(id=1, name=name001)
-
-    rowcount = update_name(id, "name002")  # rowcount=1
-    person = get(id)  # person=Person(id=1, name=name002)
-
-    rowcount = delete("name002")  # rowcount=1
-    person = get(id)  # person=None
-
-    insert("name003")
-    insert("name004")
-    persons = find("name%")  # persons=[Person(id=2, name=name003), Person(id=3, name=name004)]
-
-    # #############################
-    # also you can use execute api
-    # #############################
-    persons = nicesql.execute("select * from person where name like {name}", name="name%").all(model=Person)  # persons=[Person(id=2, name=name003), Person(id=3, name=name004)]
-
-    new_id = nicesql.execute("insert into person(name) values({name})", name="name005").insertid()  # new_id = 4
-
-    rowcount = nicesql.execute(
-        "update person set name={name} where id = {id}", name="name006", id=new_id
-    )  # rowcount = 1
+def setup_module():
+    reg_engine("mysql://localhost/test?user=test&password=test", alias="mysql")
+    create_table()
+
+
+def teardown_module():
+    drop_table()
+
+
+@ddl("""
+create table if not exists person(
+    id      integer not null primary key AUTO_INCREMENT,
+    name    varchar(127)
+)
+""", engine="mysql")
+def create_table():
+    pass
+
+
+@ddl("drop table if exists person", engine="mysql")
+def drop_table():
+    pass
+
+
+# noinspection DuplicatedCode, PyMethodMayBeStatic, PyShadowingBuiltins
+class TestMysql:
+    @insert("insert into person(name) values({name})", engine="mysql")
+    def insert(self, name: str) -> int | str:
+        pass
+
+    @delete("delete from person where id={id}", engine="mysql")
+    def delete(self, id: int) -> int:
+        pass
+
+    @update("update person set name={name} where id={id}", engine="mysql")
+    def update(self, id: int, name: str) -> int:
+        pass
+
+    @select("select * from person where id={ id }", model=Person, first=True, engine="mysql")
+    def get(self, id: int) -> Person:
+        pass
+
+    @select("select * from person where id in ({ ids })", model=Person, engine="mysql")
+    def gets(self, *ids: int) -> List[Person]:
+        pass
+
+    @select("select * from person where name like { name }", model=Person, engine="mysql")
+    def find(self, name: str) -> List[Person]:
+        pass
+
+    def test_insert(self):
+        name = "insert001"
+        new_id = self.insert(name)
+
+        person = self.get(new_id)
+        assert person
+        assert person.name == name
+
+    def test_delete(self):
+        name = "delete001"
+        new_id = self.insert(name)
+        assert self.delete(new_id) == 1
+
+        person = self.get(new_id)
+        assert person is None
+
+    def test_update(self):
+        name = "update001"
+        update_name = "update002"
+        new_id = self.insert(name)
+        assert self.update(new_id, update_name) == 1
+        person = self.get(new_id)
+        assert person
+        assert person.name == update_name
+
+    def test_gets(self):
+        name1 = "gets001"
+        name2 = "gets002"
+        id1 = self.insert(name1)
+        id2 = self.insert(name2)
+        persons = self.gets(id1, id2)
+        assert len(persons) == 2
+        assert persons[0].id == id1
+        assert persons[1].id == id2
+        assert persons[0].name == name1
+        assert persons[1].name == name2
 ```
```

### Comparing `nice-sql-0.0.7/nice_sql.egg-info/PKG-INFO` & `nice-sql-1.0.0/nice_sql.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 0.0.7
+Version: 1.0.0
 Summary: easy nice sql: decorator with sql
 Home-page: https://github.com/657143946/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -24,85 +24,108 @@
 丨     person        丨
  --------------------
 丨 id        int     丨
 丨 name      string  丨
  --------------------
 """
 
-import nicesql
-from nicesql.sqlmodel import SqlModel
-from nicesql.sqlengine.sqlite import Sqlite
 from typing import List
 
-nicesql.register(Sqlite(":memory:"))
+from nicesql.engine import reg_engine
+from nicesql.shortcut.annotate import insert, delete, update, select, ddl
 
 
-class Person(SqlModel):
+class Person:
     def __init__(self):
         self.id = None
         self.name = None
 
 
-@nicesql.bind("""
-    create table if not exists person(
-        id      integer not null primary key,
-        name    varchar(127)
-    )
-""")
-def create_person_table():
-    pass
-
-
-@nicesql.insert("insert into person(name) values ({name})")
-def insert(name) -> int:
-    pass
-
-
-@nicesql.select("select * from person where id={id}", model=Person, first=True)
-def get(id) -> Person:
-    pass
-
-
-@nicesql.select("select * from person where name like {name}", model=Person)
-def find(name) -> List[Person]:
-    pass
-
-
-@nicesql.update("update person set name={name} where id={id}")
-def update_name(id: int, name: str) -> int:
-    pass
-
-
-@nicesql.delete("delete from person where name={name}")
-def delete(name: str) -> int:
-    pass
-
-
-if __name__ == '__main__':
-    create_person_table()  # create person table
-
-    id = insert("name001")  # id=1
-    person = get(id)  # person=Person(id=1, name=name001)
-
-    rowcount = update_name(id, "name002")  # rowcount=1
-    person = get(id)  # person=Person(id=1, name=name002)
-
-    rowcount = delete("name002")  # rowcount=1
-    person = get(id)  # person=None
-
-    insert("name003")
-    insert("name004")
-    persons = find("name%")  # persons=[Person(id=2, name=name003), Person(id=3, name=name004)]
-
-    # #############################
-    # also you can use execute api
-    # #############################
-    persons = nicesql.execute("select * from person where name like {name}", name="name%").all(model=Person)  # persons=[Person(id=2, name=name003), Person(id=3, name=name004)]
-
-    new_id = nicesql.execute("insert into person(name) values({name})", name="name005").insertid()  # new_id = 4
-
-    rowcount = nicesql.execute(
-        "update person set name={name} where id = {id}", name="name006", id=new_id
-    )  # rowcount = 1
+def setup_module():
+    reg_engine("mysql://localhost/test?user=test&password=test", alias="mysql")
+    create_table()
+
+
+def teardown_module():
+    drop_table()
+
+
+@ddl("""
+create table if not exists person(
+    id      integer not null primary key AUTO_INCREMENT,
+    name    varchar(127)
+)
+""", engine="mysql")
+def create_table():
+    pass
+
+
+@ddl("drop table if exists person", engine="mysql")
+def drop_table():
+    pass
+
+
+# noinspection DuplicatedCode, PyMethodMayBeStatic, PyShadowingBuiltins
+class TestMysql:
+    @insert("insert into person(name) values({name})", engine="mysql")
+    def insert(self, name: str) -> int | str:
+        pass
+
+    @delete("delete from person where id={id}", engine="mysql")
+    def delete(self, id: int) -> int:
+        pass
+
+    @update("update person set name={name} where id={id}", engine="mysql")
+    def update(self, id: int, name: str) -> int:
+        pass
+
+    @select("select * from person where id={ id }", model=Person, first=True, engine="mysql")
+    def get(self, id: int) -> Person:
+        pass
+
+    @select("select * from person where id in ({ ids })", model=Person, engine="mysql")
+    def gets(self, *ids: int) -> List[Person]:
+        pass
+
+    @select("select * from person where name like { name }", model=Person, engine="mysql")
+    def find(self, name: str) -> List[Person]:
+        pass
+
+    def test_insert(self):
+        name = "insert001"
+        new_id = self.insert(name)
+
+        person = self.get(new_id)
+        assert person
+        assert person.name == name
+
+    def test_delete(self):
+        name = "delete001"
+        new_id = self.insert(name)
+        assert self.delete(new_id) == 1
+
+        person = self.get(new_id)
+        assert person is None
+
+    def test_update(self):
+        name = "update001"
+        update_name = "update002"
+        new_id = self.insert(name)
+        assert self.update(new_id, update_name) == 1
+        person = self.get(new_id)
+        assert person
+        assert person.name == update_name
+
+    def test_gets(self):
+        name1 = "gets001"
+        name2 = "gets002"
+        id1 = self.insert(name1)
+        id2 = self.insert(name2)
+        persons = self.gets(id1, id2)
+        assert len(persons) == 2
+        assert persons[0].id == id1
+        assert persons[1].id == id2
+        assert persons[0].name == name1
+        assert persons[1].name == name2
 ```
```

### Comparing `nice-sql-0.0.7/setup.py` & `nice-sql-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # upload pypi
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 setup(
     name='nice-sql',
-    version='0.0.7',
+    version='1.0.0',
     author='minusli',
     author_email='minusli@foxmail.com',
     url='https://github.com/657143946/nicesql',
     description='easy nice sql: decorator with sql',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

