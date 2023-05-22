# Comparing `tmp/estela-0.2.1.tar.gz` & `tmp/estela-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estela-0.2.1.tar", last modified: Fri May  5 22:08:45 2023, max compression
+gzip compressed data, was "estela-0.2.2.tar", last modified: Mon May 22 23:27:12 2023, max compression
```

## Comparing `estela-0.2.1.tar` & `estela-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287894 estela-0.2.1/
--rw-r--r--   0 mgonnav    (501) staff       (20)      259 2023-05-05 22:08:45.287777 estela-0.2.1/PKG-INFO
--rw-r--r--   0 mgonnav    (501) staff       (20)     1548 2023-01-09 17:55:22.000000 estela-0.2.1/README.md
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.282647 estela-0.2.1/estela.egg-info/
--rw-r--r--   0 mgonnav    (501) staff       (20)      259 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/PKG-INFO
--rw-r--r--   0 mgonnav    (501) staff       (20)      910 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/SOURCES.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)        1 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/dependency_links.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       51 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/entry_points.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/requires.txt
--rw-r--r--   0 mgonnav    (501) staff       (20)       11 2023-05-05 22:08:45.000000 estela-0.2.1/estela.egg-info/top_level.txt
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.284757 estela-0.2.1/estela_cli/
--rw-r--r--   0 mgonnav    (501) staff       (20)       49 2023-05-05 21:57:11.000000 estela-0.2.1/estela_cli/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      543 2023-05-05 21:55:52.000000 estela-0.2.1/estela_cli/__main__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2357 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/context.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.285517 estela-0.2.1/estela_cli/create/
--rw-r--r--   0 mgonnav    (501) staff       (20)      332 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/create/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2040 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/create/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1792 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/create/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      629 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/create/project.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.285841 estela-0.2.1/estela_cli/data/
--rw-r--r--   0 mgonnav    (501) staff       (20)      333 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/data/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2734 2023-05-05 20:34:19.000000 estela-0.2.1/estela_cli/data/job.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.286193 estela-0.2.1/estela_cli/delete/
--rw-r--r--   0 mgonnav    (501) staff       (20)      306 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/delete/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      562 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/delete/project.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     3280 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/deploy.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     8738 2023-05-05 21:55:16.000000 estela-0.2.1/estela_cli/estela_client.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     2950 2023-01-09 17:55:22.000000 estela-0.2.1/estela_cli/init.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.286884 estela-0.2.1/estela_cli/list/
--rw-r--r--   0 mgonnav    (501) staff       (20)      358 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1888 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/list/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1835 2023-01-26 21:18:07.000000 estela-0.2.1/estela_cli/list/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      448 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/project.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1151 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/list/spider.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     3577 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/login.py
--rw-r--r--   0 mgonnav    (501) staff       (20)      517 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/logout.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287168 estela-0.2.1/estela_cli/stop/
--rw-r--r--   0 mgonnav    (501) staff       (20)      312 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/stop/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1110 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/stop/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1027 2023-04-19 22:49:34.000000 estela-0.2.1/estela_cli/templates.py
-drwxr-xr-x   0 mgonnav    (501) staff       (20)        0 2023-05-05 22:08:45.287601 estela-0.2.1/estela_cli/update/
--rw-r--r--   0 mgonnav    (501) staff       (20)      317 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/__init__.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1977 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/cronjob.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     1590 2022-07-18 19:23:21.000000 estela-0.2.1/estela_cli/update/job.py
--rw-r--r--   0 mgonnav    (501) staff       (20)     4179 2023-05-05 21:38:05.000000 estela-0.2.1/estela_cli/utils.py
--rw-r--r--   0 mgonnav    (501) staff       (20)       38 2023-05-05 22:08:45.287928 estela-0.2.1/setup.cfg
--rw-r--r--   0 mgonnav    (501) staff       (20)      601 2023-05-05 21:57:11.000000 estela-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 23:27:12.439841 estela-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-22 23:27:05.000000 estela-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-22 23:27:12.000000 estela-0.2.2/estela.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/create/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/create/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/data/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/delete/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8738 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/estela_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.435840 estela-0.2.2/estela_cli/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/list/spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/estela_cli/stop/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/stop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/stop/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 23:27:12.439841 estela-0.2.2/estela_cli/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/cronjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/update/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-22 23:27:05.000000 estela-0.2.2/estela_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 23:27:12.439841 estela-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-22 23:27:05.000000 estela-0.2.2/setup.py
```

### Comparing `estela-0.2.1/README.md` & `estela-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center"> estela CLI </h1>
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![version](https://img.shields.io/badge/version-0.1-blue)](https://github.com/bitmakerla/estela-cli)
+[![version](https://img.shields.io/badge/version-0.2.2-blue)](https://github.com/bitmakerla/estela-cli)
 [![python-version](https://img.shields.io/badge/python-v3.10-orange)](https://www.python.org)
 
 
 estela CLI is a command line client to interact with the estela API. It allows the user to perform the following actions:
 - Link a Scrapy project with a project in estela.
 - Create projects, jobs, and cronjobs in estela.
 - Get the data of a job.
```

### Comparing `estela-0.2.1/estela.egg-info/SOURCES.txt` & `estela-0.2.2/estela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/__main__.py` & `estela-0.2.2/estela_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/context.py` & `estela-0.2.2/estela_cli/context.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/create/cronjob.py` & `estela-0.2.2/estela_cli/create/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/create/job.py` & `estela-0.2.2/estela_cli/create/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/create/project.py` & `estela-0.2.2/estela_cli/create/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/data/job.py` & `estela-0.2.2/estela_cli/data/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from estela_cli.login import login
 from estela_cli.templates import BAD_EMOJI, CLOCK_EMOJI, OK_EMOJI
 from estela_cli.utils import get_estela_settings, save_chunk_data, save_data
 
 SHORT_HELP = "Retrieve data from a job"
 ALLOWED_DATA_TYPES = ["items", "requests", "logs", "stats"]
-ALLOWED_DATA_FORMATS = ["json", "csv"]
+ALLOWED_DATA_FORMATS = ["json", "csv", "tsv"]
 
 
 @click.command(short_help=SHORT_HELP)
 @click.argument("jid", required=True)
 @click.argument("sid", required=True)
 @click.argument("pid", required=False)
 @click.option(
@@ -63,15 +63,17 @@
             label="{} Downloading job data".format(CLOCK_EMOJI),
             show_eta=True,
             show_percent=True,
             show_pos=True,
         ) as progress_bar:
             next_chunk = None
             while True:
-                response = estela_client.get_spider_job_data(pid, sid, jid, datatype, next_chunk)
+                response = estela_client.get_spider_job_data(
+                    pid, sid, jid, datatype, next_chunk
+                )
                 chunk = response.get("results")
                 save_chunk_data(tmp_filename, chunk)
                 progress_bar.update(len(chunk))
                 next_chunk = response.get("next_chunk")
                 if next_chunk is None:
                     break
         click.echo("{} Data downloaded succesfully.".format(OK_EMOJI))
```

### Comparing `estela-0.2.1/estela_cli/delete/project.py` & `estela-0.2.2/estela_cli/delete/project.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/deploy.py` & `estela-0.2.2/estela_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/estela_client.py` & `estela-0.2.2/estela_cli/estela_client.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/init.py` & `estela-0.2.2/estela_cli/init.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/list/cronjob.py` & `estela-0.2.2/estela_cli/list/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/list/job.py` & `estela-0.2.2/estela_cli/list/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/list/spider.py` & `estela-0.2.2/estela_cli/list/spider.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/login.py` & `estela-0.2.2/estela_cli/login.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/logout.py` & `estela-0.2.2/estela_cli/logout.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/stop/job.py` & `estela-0.2.2/estela_cli/stop/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/templates.py` & `estela-0.2.2/estela_cli/templates.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/update/cronjob.py` & `estela-0.2.2/estela_cli/update/cronjob.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/update/job.py` & `estela-0.2.2/estela_cli/update/job.py`

 * *Files identical despite different names*

### Comparing `estela-0.2.1/estela_cli/utils.py` & `estela-0.2.2/estela_cli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -116,20 +116,21 @@
     with open(tmp_filename, "rb+") as F:
         F.seek(-1, 2)
         F.truncate()
         F.write(b"]\n")
 
     if format == "json":
         os.rename(tmp_filename, filename)
-    elif format == "csv":
+    elif format == "csv" or format == "tsv":
+        delimiter = "," if format == "csv" else "\t"
         with open(tmp_filename, "r", encoding="utf-8") as F:
             data = json.load(F)
         with open(filename, "w", encoding="utf-8") as F:
             keys = data[0].keys()
-            writer = csv.DictWriter(F, fieldnames=keys)
+            writer = csv.DictWriter(F, delimiter=delimiter, fieldnames=keys)
             writer.writeheader()
             for row in data:
                 writer.writerow({k: v for k, v in row.items() if k in keys})
             os.remove(tmp_filename)
 
 
 def validate_key_value_format(ctx, param, value):
```

### Comparing `estela-0.2.1/setup.py` & `estela-0.2.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="estela",
-    version="0.2.1",
+    version="0.2.2",
     description="Estela Command Line Interface",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "estela = estela_cli.__main__:cli",
         ],
     },
```

