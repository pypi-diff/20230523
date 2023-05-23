# Comparing `tmp/flashy-0.0.0.tar.gz` & `tmp/flashy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashy-0.0.0.tar", last modified: Tue Jul 26 12:37:41 2022, max compression
+gzip compressed data, was "flashy-0.0.1.tar", last modified: Tue May 23 14:40:50 2023, max compression
```

## Comparing `flashy-0.0.0.tar` & `flashy-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,40 @@
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-07-26 12:37:41.128136 flashy-0.0.0/
--rw-r--r--   0 defossez   (501) staff       (20)      469 2022-07-26 12:37:41.127794 flashy-0.0.0/PKG-INFO
-drwxr-xr-x   0 defossez   (501) staff       (20)        0 2022-07-26 12:37:41.127219 flashy-0.0.0/flashy.egg-info/
--rw-r--r--   0 defossez   (501) staff       (20)      469 2022-07-26 12:37:40.000000 flashy-0.0.0/flashy.egg-info/PKG-INFO
--rw-r--r--   0 defossez   (501) staff       (20)      138 2022-07-26 12:37:40.000000 flashy-0.0.0/flashy.egg-info/SOURCES.txt
--rw-r--r--   0 defossez   (501) staff       (20)        1 2022-07-26 12:37:40.000000 flashy-0.0.0/flashy.egg-info/dependency_links.txt
--rw-r--r--   0 defossez   (501) staff       (20)        7 2022-07-26 12:37:40.000000 flashy-0.0.0/flashy.egg-info/top_level.txt
--rw-r--r--   0 defossez   (501) staff       (20)       21 2021-04-27 20:49:32.000000 flashy-0.0.0/flashy.py
--rw-r--r--   0 defossez   (501) staff       (20)       38 2022-07-26 12:37:41.128233 flashy-0.0.0/setup.cfg
--rw-r--r--   0 defossez   (501) staff       (20)     1236 2022-07-26 12:37:18.000000 flashy-0.0.0/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.628027 flashy-0.0.1/
+-rw-r--r--   0 defossez   (501) staff       (20)     1087 2023-01-26 18:22:48.000000 flashy-0.0.1/LICENSE
+-rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-23 14:40:50.628492 flashy-0.0.1/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)     6011 2023-01-26 18:22:52.000000 flashy-0.0.1/README.md
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.589435 flashy-0.0.1/flashy/
+-rw-r--r--   0 defossez   (501) staff       (20)      436 2023-05-23 14:38:02.000000 flashy-0.0.1/flashy/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3690 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/adversarial.py
+-rw-r--r--   0 defossez   (501) staff       (20)     9899 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3531 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/formatter.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.617684 flashy-0.0.1/flashy/loggers/
+-rw-r--r--   0 defossez   (501) staff       (20)      322 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3692 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/base.py
+-rw-r--r--   0 defossez   (501) staff       (20)     6836 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/localfs.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8183 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/tensorboard.py
+-rw-r--r--   0 defossez   (501) staff       (20)     4667 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/utils.py
+-rw-r--r--   0 defossez   (501) staff       (20)     8616 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/loggers/wandb.py
+-rw-r--r--   0 defossez   (501) staff       (20)    11939 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/logging.py
+-rw-r--r--   0 defossez   (501) staff       (20)        0 2022-06-20 16:51:50.000000 flashy-0.0.1/flashy/py.typed
+-rw-r--r--   0 defossez   (501) staff       (20)     8336 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2633 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/state.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2159 2023-01-26 18:22:48.000000 flashy-0.0.1/flashy/utils.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.612441 flashy-0.0.1/flashy.egg-info/
+-rw-r--r--   0 defossez   (501) staff       (20)     7824 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/PKG-INFO
+-rw-r--r--   0 defossez   (501) staff       (20)      686 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/SOURCES.txt
+-rw-r--r--   0 defossez   (501) staff       (20)        1 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/dependency_links.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       85 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/requires.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       13 2023-05-23 14:40:50.000000 flashy-0.0.1/flashy.egg-info/top_level.txt
+-rw-r--r--   0 defossez   (501) staff       (20)       50 2023-01-03 13:51:29.000000 flashy-0.0.1/pyproject.toml
+-rw-r--r--   0 defossez   (501) staff       (20)      100 2023-05-23 14:40:50.630323 flashy-0.0.1/setup.cfg
+-rw-r--r--   0 defossez   (501) staff       (20)     1769 2023-01-26 18:22:48.000000 flashy-0.0.1/setup.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.624652 flashy-0.0.1/tests/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/__init__.py
+drwxr-xr-x   0 defossez   (501) staff       (20)        0 2023-05-23 14:40:50.627197 flashy-0.0.1/tests/dummy/
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/dummy/__init__.py
+-rw-r--r--   0 defossez   (501) staff       (20)     3733 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/dummy/train.py
+-rw-r--r--   0 defossez   (501) staff       (20)     2708 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_distrib.py
+-rw-r--r--   0 defossez   (501) staff       (20)      198 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_formatter.py
+-rw-r--r--   0 defossez   (501) staff       (20)      879 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_integ.py
+-rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_solver.py
+-rw-r--r--   0 defossez   (501) staff       (20)      197 2023-01-26 18:22:48.000000 flashy-0.0.1/tests/test_state.py
```

