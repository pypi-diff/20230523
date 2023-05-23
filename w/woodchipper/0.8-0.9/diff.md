# Comparing `tmp/woodchipper-0.8.tar.gz` & `tmp/woodchipper-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woodchipper-0.8.tar", last modified: Thu Nov  3 14:07:21 2022, max compression
+gzip compressed data, was "woodchipper-0.9.tar", last modified: Fri Dec  2 20:30:22 2022, max compression
```

## Comparing `woodchipper-0.8.tar` & `woodchipper-0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-11-03 14:07:21.813215 woodchipper-0.8/
--rw-r--r--   0 ian.mangan   (502) staff       (20)      116 2022-10-31 19:17:19.000000 woodchipper-0.8/CONTRIBUTORS
--rw-r--r--   0 ian.mangan   (502) staff       (20)     1060 2022-10-31 19:17:19.000000 woodchipper-0.8/COPYING
--rw-r--r--   0 ian.mangan   (502) staff       (20)       37 2022-10-31 19:17:19.000000 woodchipper-0.8/MANIFEST.in
--rw-r--r--   0 ian.mangan   (502) staff       (20)      475 2022-11-03 14:07:21.813294 woodchipper-0.8/PKG-INFO
--rw-r--r--   0 ian.mangan   (502) staff       (20)     1072 2022-10-31 19:17:19.000000 woodchipper-0.8/README.md
--rw-r--r--   0 ian.mangan   (502) staff       (20)      172 2022-10-31 19:17:19.000000 woodchipper-0.8/pyproject.toml
--rw-r--r--   0 ian.mangan   (502) staff       (20)      589 2022-11-03 14:07:21.813608 woodchipper-0.8/setup.cfg
-drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-11-03 14:07:21.811260 woodchipper-0.8/woodchipper/
--rw-r--r--   0 ian.mangan   (502) staff       (20)     2295 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/__init__.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     3242 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/configs.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     8465 2022-11-03 14:02:42.000000 woodchipper-0.8/woodchipper/context.py
-drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-11-03 14:07:21.812723 woodchipper-0.8/woodchipper/http/
--rw-r--r--   0 ian.mangan   (502) staff       (20)        0 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/http/__init__.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)      842 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/http/awslambda.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     3447 2022-11-03 14:02:42.000000 woodchipper-0.8/woodchipper/http/fastapi.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     2336 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/http/flask.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     1448 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/logger.py
-drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-11-03 14:07:21.813060 woodchipper-0.8/woodchipper/monitors/
--rw-r--r--   0 ian.mangan   (502) staff       (20)      297 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/monitors/__init__.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)     1533 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/monitors/sqlalchemy.py
--rw-r--r--   0 ian.mangan   (502) staff       (20)      974 2022-10-31 19:17:19.000000 woodchipper-0.8/woodchipper/processors.py
-drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-11-03 14:07:21.812126 woodchipper-0.8/woodchipper.egg-info/
--rw-r--r--   0 ian.mangan   (502) staff       (20)      475 2022-11-03 14:07:21.000000 woodchipper-0.8/woodchipper.egg-info/PKG-INFO
--rw-r--r--   0 ian.mangan   (502) staff       (20)      540 2022-11-03 14:07:21.000000 woodchipper-0.8/woodchipper.egg-info/SOURCES.txt
--rw-r--r--   0 ian.mangan   (502) staff       (20)        1 2022-11-03 14:07:21.000000 woodchipper-0.8/woodchipper.egg-info/dependency_links.txt
--rw-r--r--   0 ian.mangan   (502) staff       (20)       51 2022-11-03 14:07:21.000000 woodchipper-0.8/woodchipper.egg-info/requires.txt
--rw-r--r--   0 ian.mangan   (502) staff       (20)       12 2022-11-03 14:07:21.000000 woodchipper-0.8/woodchipper.egg-info/top_level.txt
+drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-12-02 20:30:22.746596 woodchipper-0.9/
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      116 2022-07-08 13:01:07.000000 woodchipper-0.9/CONTRIBUTORS
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     1060 2022-07-08 13:01:07.000000 woodchipper-0.9/COPYING
+-rw-r--r--   0 ian.mangan   (502) staff       (20)       37 2022-07-08 13:01:07.000000 woodchipper-0.9/MANIFEST.in
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      475 2022-12-02 20:30:22.746663 woodchipper-0.9/PKG-INFO
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     1072 2022-07-08 13:01:07.000000 woodchipper-0.9/README.md
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      172 2022-07-08 13:01:07.000000 woodchipper-0.9/pyproject.toml
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      589 2022-12-02 20:30:22.746965 woodchipper-0.9/setup.cfg
+drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-12-02 20:30:22.744405 woodchipper-0.9/woodchipper/
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     2295 2022-10-25 12:34:08.000000 woodchipper-0.9/woodchipper/__init__.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     3298 2022-12-02 20:21:39.000000 woodchipper-0.9/woodchipper/configs.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     8465 2022-12-02 20:21:39.000000 woodchipper-0.9/woodchipper/context.py
+drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-12-02 20:30:22.745969 woodchipper-0.9/woodchipper/http/
+-rw-r--r--   0 ian.mangan   (502) staff       (20)        0 2022-07-08 13:01:07.000000 woodchipper-0.9/woodchipper/http/__init__.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      842 2022-07-08 13:01:07.000000 woodchipper-0.9/woodchipper/http/awslambda.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     3447 2022-12-02 20:21:39.000000 woodchipper-0.9/woodchipper/http/fastapi.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     2336 2022-07-08 13:01:07.000000 woodchipper-0.9/woodchipper/http/flask.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     1448 2022-07-08 13:01:07.000000 woodchipper-0.9/woodchipper/logger.py
+drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-12-02 20:30:22.746346 woodchipper-0.9/woodchipper/monitors/
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      297 2022-07-08 13:01:07.000000 woodchipper-0.9/woodchipper/monitors/__init__.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     1533 2022-10-31 19:15:16.000000 woodchipper-0.9/woodchipper/monitors/sqlalchemy.py
+-rw-r--r--   0 ian.mangan   (502) staff       (20)     2332 2022-12-02 20:21:39.000000 woodchipper-0.9/woodchipper/processors.py
+drwxr-xr-x   0 ian.mangan   (502) staff       (20)        0 2022-12-02 20:30:22.745241 woodchipper-0.9/woodchipper.egg-info/
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      475 2022-12-02 20:30:22.000000 woodchipper-0.9/woodchipper.egg-info/PKG-INFO
+-rw-r--r--   0 ian.mangan   (502) staff       (20)      540 2022-12-02 20:30:22.000000 woodchipper-0.9/woodchipper.egg-info/SOURCES.txt
+-rw-r--r--   0 ian.mangan   (502) staff       (20)        1 2022-12-02 20:30:22.000000 woodchipper-0.9/woodchipper.egg-info/dependency_links.txt
+-rw-r--r--   0 ian.mangan   (502) staff       (20)       51 2022-12-02 20:30:22.000000 woodchipper-0.9/woodchipper.egg-info/requires.txt
+-rw-r--r--   0 ian.mangan   (502) staff       (20)       12 2022-12-02 20:30:22.000000 woodchipper-0.9/woodchipper.egg-info/top_level.txt
```

### Comparing `woodchipper-0.8/COPYING` & `woodchipper-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/README.md` & `woodchipper-0.9/README.md`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/setup.cfg` & `woodchipper-0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = woodchipper
-version = 0.8
+version = 0.9
 description = Woodchipper is a support library for plugging structured logging into a Python project.
 author = Tackle.io, Inc.
 url = https://github.com/tackle-io/woodchipper
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
```

### Comparing `woodchipper-0.8/woodchipper/__init__.py` & `woodchipper-0.9/woodchipper/__init__.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/configs.py` & `woodchipper-0.9/woodchipper/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     processors = [
         structlog.stdlib.add_log_level,
         structlog.stdlib.add_logger_name,
         structlog.stdlib.ExtraAdder(),
         structlog.stdlib.PositionalArgumentsFormatter(),
         structlog.processors.StackInfoRenderer(),
         woodchipper.processors.GitVersionProcessor(),
+        woodchipper.processors.DatadogTraceProcessor(),
         structlog.processors.TimeStamper(fmt="%Y-%m-%d %H:%M.%S", utc=False),
         structlog.processors.CallsiteParameterAdder(
             parameters=callsite_parameters, additional_ignores=["woodchipper"]
         ),
         SentryJsonProcessor(level=logging.ERROR, as_extra=True, active=not os.getenv("WOODCHIPPER_DISABLE_SENTRY")),
         structlog.processors.format_exc_info,
         structlog.processors.UnicodeDecoder(),
```

### Comparing `woodchipper-0.8/woodchipper/context.py` & `woodchipper-0.9/woodchipper/context.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/http/awslambda.py` & `woodchipper-0.9/woodchipper/http/awslambda.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/http/fastapi.py` & `woodchipper-0.9/woodchipper/http/fastapi.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/http/flask.py` & `woodchipper-0.9/woodchipper/http/flask.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/logger.py` & `woodchipper-0.9/woodchipper/logger.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper/monitors/sqlalchemy.py` & `woodchipper-0.9/woodchipper/monitors/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `woodchipper-0.8/woodchipper.egg-info/SOURCES.txt` & `woodchipper-0.9/woodchipper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

