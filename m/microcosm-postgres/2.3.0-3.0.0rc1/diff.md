# Comparing `tmp/microcosm-postgres-2.3.0.tar.gz` & `tmp/microcosm-postgres-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-postgres-2.3.0.tar", last modified: Fri Mar  4 13:31:06 2022, max compression
+gzip compressed data, was "dist/microcosm-postgres-3.0.0rc1.tar", last modified: Tue May 23 16:48:26 2023, max compression
```

## Comparing `microcosm-postgres-2.3.0.tar` & `microcosm-postgres-3.0.0rc1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3566 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/cloning.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2224 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/createall.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/diff.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3874 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/encryptor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6253 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/providers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/encryption/store.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/errors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres/factories/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/factories/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4859 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/factories/engine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/factories/engine_routing_strategy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/factories/sessionmaker.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      740 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/identifiers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7659 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/migrate.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4867 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2246 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/operations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/store.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1164 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/copy.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/factories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1796 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/temporary/methods.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/toposort.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/microcosm_postgres/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      427 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      305 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/microcosm_postgres.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2022-03-04 13:31:06.000000 microcosm-postgres-2.3.0/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2144 2022-03-04 13:28:51.000000 microcosm-postgres-2.3.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11357 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4030 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/cloning.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      531 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/createall.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4357 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/dag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1026 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/diff.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3874 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/encryptor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      420 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6331 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3194 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/providers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3310 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3607 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/store.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1613 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/errors.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4859 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1605 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine_routing_strategy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      901 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/sessionmaker.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      802 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/identifiers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7786 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/migrate.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5042 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2425 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9517 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/store.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       73 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1164 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/copy.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1880 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/factories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/methods.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1096 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/toposort.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1907 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      430 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1493 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      770 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      304 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       19 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2023-05-23 16:48:26.000000 microcosm-postgres-3.0.0rc1/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2146 2023-05-23 16:46:02.000000 microcosm-postgres-3.0.0rc1/setup.py
```

### Comparing `microcosm-postgres-2.3.0/LICENSE` & `microcosm-postgres-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/README.md` & `microcosm-postgres-3.0.0rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 To change the database password:
 
     config.postgres.password = "mysecretpassword"
 
 
 ## Test Setup
 
-Tests (and automated builds) act as the "example" microservice and need a cooresponding database
+Tests (and automated builds) act as the "example" microservice and need a corresponding database
 and user:
 
     createuser example
     createdb -O example example_test_db
 
 Note that production usage should always create the user with a password. For example:
 
@@ -99,7 +99,15 @@
          key_ids="key1a;key1b,key2a;key2b",
          partitions="aws,aws-cn",
          account_ids="account-id1a;account-id1b,account-id2",
     )
 
 For more information, see the "Discovery Mode" section in:
 https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/migrate-mkps-v2.html
+
+
+## Migration guide: 2.x => 3.x
+Version 3.x uses sqlalchemy 2.x, any breaking changes are introduced by sqlalchemy 2.
+
+The official [sqlalchemy 2 migration guide](https://docs.sqlalchemy.org/en/20/changelog/migration_20.html) contains step to ensure your application is compatible with sqlalchemy 2.
+
+Additionally, follow https://docs.sqlalchemy.org/en/20/changelog/whatsnew_20.html#orm-declarative-models to update your models to use the new declarative styles.
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/cloning.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/cloning.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/context.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 """
 Session context management.
 
 """
 from contextlib import contextmanager
 from functools import wraps
 
+from sqlalchemy.orm import scoped_session
+
 from microcosm_postgres.operations import new_session, recreate_all
 
 
 class SessionContext:
     """
     Save current session in well-known location and provide context management.
 
+    New in version 3.0.0:
+        Now thread safe using a `scoped_session`.
     """
     session = None
 
     def __init__(self, graph, expire_on_commit=False):
         self.graph = graph
         self.expire_on_commit = expire_on_commit
+        self.session_cls = scoped_session(
+            lambda: new_session(self.graph, self.expire_on_commit)
+        )
 
     def open(self):
-        SessionContext.session = new_session(self.graph, self.expire_on_commit)
+        SessionContext.session = self.session_cls()
         return self
 
     def close(self):
         if SessionContext.session:
-            SessionContext.session.close()
+            self.session_cls.remove()
             SessionContext.session = None
 
     def recreate_all(self):
         """
         Recreate all database tables, but only in a testing context.
         """
         if self.graph.metadata.testing:
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/createall.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/createall.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/dag.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/dag.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/diff.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/diff.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/encryption/encryptor.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/encryptor.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/encryption/models.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 """
 Encryption-related models.
 
 """
-from typing import Optional, Sequence, Tuple
+from typing import (
+    Callable,
+    Dict,
+    Optional,
+    Sequence,
+    Tuple,
+)
 
 from sqlalchemy import Column, LargeBinary, String
 from sqlalchemy.dialects.postgresql import ARRAY
 from sqlalchemy.event import contains, listen, remove
 
 from microcosm_postgres.encryption.encryptor import Encryptor
 
@@ -145,15 +151,15 @@
         """
         # save the current encryptor statically
         cls.__encryptor__ = encryptor
 
         # NB: we cannot use the before_insert listener in conjunction with a foreign key relationship
         # for encrypted data; SQLAlchemy will warn about using 'related attribute set' operation so
         # late in its insert/flush process.
-        listeners = dict(
+        listeners: Dict[str, Callable] = dict(
             init=on_init,
             load=on_load,
         )
 
         for name, func in listeners.items():
             # If we initialize the graph multiple times (as in many unit testing scenarios),
             # we will accumulate listener functions -- with unpredictable results. As protection,
@@ -171,8 +177,8 @@
     """
     A mixin that in include ciphertext and an array of key ids.
 
     """
     # save the encrypted data as unindexed binary
     ciphertext = Column(LargeBinary, nullable=False)
     # save the encryption key ids in an indexed column for future re-keying
-    key_ids = Column(ARRAY(String), nullable=False, index=True)
+    key_ids = Column(ARRAY(String), nullable=False, index=True)  # type: ignore
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/encryption/providers.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/providers.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/encryption/registry.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/encryption/store.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/encryption/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/errors.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/factories/engine.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/factories/engine_routing_strategy.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/engine_routing_strategy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/factories/sessionmaker.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/factories/sessionmaker.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/health.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/health.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """
 Simple Postgres health check.
 
 """
 from alembic.script import ScriptDirectory
+from sqlalchemy import text
 
 from microcosm_postgres.context import SessionContext
 
 
 def check_health(graph):
     """
     Basic database health check.
 
     """
-    SessionContext.session.execute("SELECT 1;")
+    SessionContext.session.execute(text("SELECT 1;"))
 
 
 def check_alembic(graph):
     """
     Check connectivity to an alembic database.
 
     Returns the current migration.
 
     """
     return SessionContext.session.execute(
-        "SELECT version_num FROM alembic_version LIMIT 1;",
+        text(
+            "SELECT version_num FROM alembic_version LIMIT 1;",
+        )
     ).scalar()
 
 
 def get_current_head_version(graph):
     """
     Returns the current head version.
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/metrics.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/metrics.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/migrate.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/migrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,28 +91,28 @@
 def get_alembic_environment_options(graph):
     try:
         return graph.config.alembic.environment_options
     except (AttributeError, LockedGraphError, NotBoundError):
         return dict()
 
 
-def run_online_migration(self):
+def run_online_migration(self, model_cls=Model):
     """
     Run an online migration using microcosm configuration.
 
     This function takes the place of the `env.py` file in the Alembic migration.
 
     """
     connectable = self.graph.postgres
 
     with connectable.connect() as connection:
         context.configure(
             connection=connection,
             # assumes that all models extend our base
-            target_metadata=Model.metadata,
+            target_metadata=model_cls.metadata,
             **get_alembic_environment_options(self.graph),
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
@@ -149,15 +149,15 @@
 
     def downgrade():
         ${downgrades if downgrades else "pass"}
     ''')
 
 
 @contextmanager
-def patch_script_directory(graph):
+def patch_script_directory(graph, model_cls=Model):
     """
     Monkey patch the `ScriptDirectory` class, working around configuration assumptions.
 
     Changes include:
       - Using a generated, temporary directory (with a generated, temporary `script.py.mako`)
         instead of the assumed script directory.
       - Using our `make_script_directory` function instead of the default `ScriptDirectory.from_config`.
@@ -171,15 +171,19 @@
     # use a temporary directory for the revision template
     with open(join(temporary_dir, "script.py.mako"), "w") as file_:
         file_.write(make_script_py_mako())
         file_.flush()
 
     # monkey patch our script directory and migration logic
     setattr(ScriptDirectory, "from_config", classmethod(make_script_directory))
-    setattr(ScriptDirectory, "run_env", run_online_migration)
+    setattr(
+        ScriptDirectory,
+        "run_env",
+        lambda self: run_online_migration(self, model_cls),
+    )
     setattr(ScriptDirectory, "graph", graph)
     try:
         yield temporary_dir
     finally:
         # cleanup
         delattr(ScriptDirectory, "graph")
         setattr(ScriptDirectory, "run_env", run_env_original)
@@ -201,15 +205,15 @@
         migrations_dir = graph.metadata.get_path("migrations")
 
     if not isdir(migrations_dir):
         raise Exception("Migrations dir must exist: {}".format(migrations_dir))
     return migrations_dir
 
 
-def main(graph, *args):
+def main(graph, *args, model_cls=Model):
     """
     Entry point for invoking Alembic's `CommandLine`.
 
     Alembic's CLI defines its own argument parsing and command invocation; we want
     to use these directly but define configuration our own way. This function takes
     the behavior of `CommandLine.main()` and reinterprets it with our patching.
 
@@ -222,10 +226,10 @@
     cli = CommandLine()
     options = cli.parser.parse_args(args if args else argv[1:])
     if not hasattr(options, "cmd"):
         cli.parser.error("too few arguments")
     if options.cmd[0].__name__ == "init":
         cli.parser.error("Alembic 'init' command should not be used in the microcosm!")
 
-    with patch_script_directory(graph) as temporary_dir:
+    with patch_script_directory(graph, model_cls) as temporary_dir:
         config = make_alembic_config(temporary_dir, migrations_dir)
         cli.run_cmd(config, options)
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/models.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
 Support for building models.
 
 Every model must inherit from `Model` and should inherit from the `EntityMixin`.
 
 """
 from datetime import datetime
+from enum import Enum
 from time import time
 from uuid import uuid4
 
+import sqlalchemy
 from dateutil.tz import tzutc
 from pytz import utc
 from sqlalchemy import Column, Float, types
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import DeclarativeBase
 from sqlalchemy_utils import UUIDType
 
 
 EPOCH = datetime(1970, 1, 1)
 
-Model = declarative_base()
+
+class Model(DeclarativeBase):
+    type_annotation_map = {
+        Enum: sqlalchemy.Enum(Enum, native_enum=False, length=255),
+    }
 
 
 def utcnow():
     """
     Create a non-naive UTC datetime for the current time.
 
     Needed when *updating* UTCDateTime values because result values are currently
@@ -61,15 +67,15 @@
 
 
 class PrimaryKeyMixin:
     """
     Define a model with a randomized UUID primary key and tracking created/updated times.
 
     """
-    id = Column(UUIDType(), primary_key=True, default=uuid4)
+    id = Column(UUIDType(), primary_key=True, default=uuid4)  # type: ignore
     created_at = Column(UTCDateTime, default=utcnow, nullable=False)
     updated_at = Column(UTCDateTime, default=utcnow, onupdate=utcnow, nullable=False)
 
     def new_timestamp(self):
         return utcnow()
 
     @property
@@ -82,15 +88,15 @@
 
 
 class UnixTimestampPrimaryKeyMixin:
     """
     Define a model with a randomized UUID primary key and tracking created/updated times.
 
     """
-    id = Column(UUIDType(), primary_key=True, default=uuid4)
+    id = Column(UUIDType(), primary_key=True, default=uuid4)  # type: ignore
     created_at = Column(Float, default=time, nullable=False)
     updated_at = Column(Float, default=time, onupdate=time, nullable=False)
 
     def new_timestamp(self):
         return time()
 
     @property
@@ -115,15 +121,15 @@
         Return a dict of non-private members.
 
         """
         return {
             key: value
             for key, value in self.__dict__.items()
             # NB: ignore internal SQLAlchemy state and nested relationships
-            if not key.startswith("_") and not isinstance(value, Model)
+            if not key.startswith("_") and not isinstance(value, DeclarativeBase)
         }
 
     def __eq__(self, other):
         return type(other) is type(self) and self._members() == other._members()
 
     def __ne__(self, other):
         return not self.__eq__(other)
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/operations.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Common database operations.
 
 """
-from sqlalchemy import MetaData
+from sqlalchemy import MetaData, text
 from sqlalchemy.exc import ProgrammingError
 
 from microcosm_postgres.migrate import main
 from microcosm_postgres.models import Model
 
 
 def stamp_head(graph):
@@ -20,77 +20,80 @@
 def get_current_head(graph):
     """
     Get the current database head revision, if any.
 
     """
     session = new_session(graph)
     try:
-        result = session.execute("SELECT version_num FROM alembic_version")
+        result = session.execute(text("SELECT version_num FROM alembic_version"))
     except ProgrammingError:
         return None
     else:
         return result.scalar()
     finally:
         session.close()
 
 
-def create_all(graph):
+def create_all(graph, model_cls=Model):
     """
     Create all database tables.
 
     """
     head = get_current_head(graph)
     if head is None:
-        Model.metadata.create_all(graph.postgres)
+        model_cls.metadata.create_all(graph.postgres)
         stamp_head(graph)
 
 
-def drop_all(graph):
+def drop_all(graph, model_cls=Model):
     """
     Drop all database tables.
 
     """
-    Model.metadata.drop_all(graph.postgres)
+    model_cls.metadata.drop_all(graph.postgres)
     drop_alembic_table(graph)
 
 
 def drop_alembic_table(graph):
     """
     Drop the alembic version table.
 
     """
     try:
-        graph.postgres.execute("DROP TABLE alembic_version;")
+        with graph.postgres.connect() as connection:
+            connection.execute(text("DROP TABLE alembic_version"))
+            connection.commit()
+
     except ProgrammingError:
         return False
     else:
         return True
 
 
 # Cached database metadata instance
 _metadata = None
 
 
-def recreate_all(graph):
+def recreate_all(graph, model_cls=Model):
     """
     Drop and add back all database tables, or reset all data associated with a database.
     Intended mainly for testing, where a test database may either need to be re-initialized
     or cleared out between tests
 
     """
 
     global _metadata
 
     if _metadata is None:
         # First-run, the test database/metadata needs to be initialized
-        drop_all(graph)
-        create_all(graph)
+        drop_all(graph, model_cls)
+        create_all(graph, model_cls)
+        _metadata = MetaData()
+        _metadata.reflect(graph.postgres)
 
-        _metadata = MetaData(bind=graph.postgres)
-        _metadata.reflect()
         return
 
     # Otherwise, truncate all existing tables
     connection = graph.postgres.connect()
     transaction = connection.begin()
     for table in reversed(_metadata.sorted_tables):
         connection.execute(table.delete())
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/store.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/store.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/temporary/context.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/temporary/copy.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/copy.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/temporary/factories.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/factories.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/temporary/methods.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/temporary/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def insert_many(self, items):
     """
     Insert many items at once into a temporary table.
 
     """
     return SessionContext.session.execute(
-        self.insert(values=[
+        self.insert().values([
             to_dict(item, self.c)
             for item in items
         ]),
     ).rowcount
 
 
 def upsert_into(self, table):
```

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/toposort.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/toposort.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres/types.py` & `microcosm-postgres-3.0.0rc1/microcosm_postgres/types.py`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres.egg-info/SOURCES.txt` & `microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/microcosm_postgres.egg-info/entry_points.txt` & `microcosm-postgres-3.0.0rc1/microcosm_postgres.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/setup.cfg` & `microcosm-postgres-3.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `microcosm-postgres-2.3.0/setup.py` & `microcosm-postgres-3.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-postgres"
-version = "2.3.0"
+version = "3.0.0rc1"
 
 setup(
     name=project,
     version=version,
     description="Opinionated persistence with PostgreSQL",
     author="Globality Engineering",
     author_email="engineering@globality.com",
@@ -20,15 +20,15 @@
     install_requires=[
         "alembic>=1.0.0",
         "microcosm>=2.12.0",
         "microcosm-logging>=1.5.0",
         "psycopg2-binary>=2.7.5",
         "python-dateutil>=2.7.3",
         "pytz>=2018.5",
-        "SQLAlchemy>=1.4.10",
+        "SQLAlchemy>=2.0.0",
         "SQLAlchemy-Utils>=0.37.0",
     ],
     setup_requires=[
         "nose>=1.3.6",
     ],
     dependency_links=[
     ],
```

