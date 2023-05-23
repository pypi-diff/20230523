# Comparing `tmp/the_new_hotness-1.2.3.tar.gz` & `tmp/the_new_hotness-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "the_new_hotness-1.2.3.tar", max compression
+gzip compressed data, was "the_new_hotness-1.2.4.tar", max compression
```

## Comparing `the_new_hotness-1.2.3.tar` & `the_new_hotness-1.2.4.tar`

### file list

```diff
@@ -1,304 +1,58 @@
--rw-r--r--   0        0        0    26530 2021-01-25 12:20:24.199782 the_new_hotness-1.2.3/LICENSE
--rw-r--r--   0        0        0     1369 2023-04-21 13:07:13.379253 the_new_hotness-1.2.3/README.rst
--rw-r--r--   0        0        0     5389 2023-04-21 13:07:13.379253 the_new_hotness-1.2.3/config/config.toml.example
--rw-r--r--   0        0        0      288 2023-04-21 13:07:13.383253 the_new_hotness-1.2.3/hotness/__init__.py
--rw-r--r--   0        0        0      849 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/builders/__init__.py
--rw-r--r--   0        0        0      230 2022-06-02 10:01:53.714952 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      188 2021-10-06 15:16:54.694389 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      192 2021-10-06 15:19:39.044410 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      228 2022-06-02 10:11:44.818772 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      228 2022-06-02 10:11:58.409806 the_new_hotness-1.2.3/hotness/builders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1093 2022-06-02 10:01:53.714952 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-310.pyc
--rw-r--r--   0        0        0     1044 2021-10-06 15:16:54.695389 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-36.pyc
--rw-r--r--   0        0        0     1048 2021-10-06 15:19:39.046410 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-37.pyc
--rw-r--r--   0        0        0     1092 2022-06-02 10:11:44.819772 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-38.pyc
--rw-r--r--   0        0        0     1092 2022-06-02 10:11:58.416806 the_new_hotness-1.2.3/hotness/builders/__pycache__/builder.cpython-39.pyc
--rw-r--r--   0        0        0    11853 2023-04-21 13:39:35.515484 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-310.pyc
--rw-r--r--   0        0        0    11623 2021-12-07 12:17:58.425775 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-36.pyc
--rw-r--r--   0        0        0    11607 2021-12-07 12:18:07.200803 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-37.pyc
--rw-r--r--   0        0        0    11754 2023-03-08 14:49:46.320328 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-38.pyc
--rw-r--r--   0        0        0    11822 2023-03-08 14:49:56.474381 the_new_hotness-1.2.3/hotness/builders/__pycache__/koji.cpython-39.pyc
--rw-r--r--   0        0        0     1467 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/builders/builder.py
--rw-r--r--   0        0        0    18241 2023-04-24 10:44:45.364657 the_new_hotness-1.2.3/hotness/builders/koji.py
--rw-r--r--   0        0        0      804 2022-06-02 08:11:44.409651 the_new_hotness-1.2.3/hotness/common/__init__.py
--rw-r--r--   0        0        0      187 2022-06-02 10:01:54.135952 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      145 2021-10-06 15:16:55.442389 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      149 2021-10-06 15:19:39.934411 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      185 2022-06-02 10:11:45.270773 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      185 2022-06-02 10:11:58.925807 the_new_hotness-1.2.3/hotness/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3220 2023-04-21 13:39:35.949486 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-310.pyc
--rw-r--r--   0        0        0     3229 2021-10-06 15:16:55.443389 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-36.pyc
--rw-r--r--   0        0        0     3213 2021-10-06 15:19:39.935411 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-37.pyc
--rw-r--r--   0        0        0     3207 2022-06-02 10:11:45.272773 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2022-06-02 10:11:58.926807 the_new_hotness-1.2.3/hotness/common/__pycache__/rpm.cpython-39.pyc
--rw-r--r--   0        0        0     5876 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/common/rpm.py
--rw-r--r--   0        0        0     6329 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/config.py
--rw-r--r--   0        0        0      897 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/databases/__init__.py
--rw-r--r--   0        0        0      270 2023-04-21 13:39:35.596484 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      193 2021-10-06 15:16:54.828389 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      197 2021-10-06 15:19:39.254410 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      268 2022-06-02 10:11:44.921772 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      268 2022-06-02 10:11:58.533806 the_new_hotness-1.2.3/hotness/databases/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2221 2023-04-21 13:39:35.598484 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-310.pyc
--rw-r--r--   0        0        0     2141 2021-10-06 15:16:54.830389 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-36.pyc
--rw-r--r--   0        0        0     2145 2021-10-06 15:19:39.257410 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-37.pyc
--rw-r--r--   0        0        0     2228 2022-06-02 10:11:44.922772 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-38.pyc
--rw-r--r--   0        0        0     2228 2022-06-02 10:11:58.534806 the_new_hotness-1.2.3/hotness/databases/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0        0        0     1464 2022-06-02 10:01:53.814952 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-310.pyc
--rw-r--r--   0        0        0     1434 2021-10-06 15:16:54.829389 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-36.pyc
--rw-r--r--   0        0        0     1438 2021-10-06 15:19:39.255411 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-37.pyc
--rw-r--r--   0        0        0     1484 2022-06-02 10:11:44.922772 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-38.pyc
--rw-r--r--   0        0        0     1484 2022-06-02 10:11:58.533806 the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0     2828 2023-04-21 13:39:35.601484 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-310.pyc
--rw-r--r--   0        0        0     2821 2022-10-05 13:45:56.825878 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-38.pyc
--rw-r--r--   0        0        0     2815 2022-10-05 13:47:00.536070 the_new_hotness-1.2.3/hotness/databases/__pycache__/redis.cpython-39.pyc
--rw-r--r--   0        0        0     2511 2023-04-21 13:07:13.384253 the_new_hotness-1.2.3/hotness/databases/cache.py
--rw-r--r--   0        0        0     1803 2022-06-02 08:11:44.411651 the_new_hotness-1.2.3/hotness/databases/database.py
--rw-r--r--   0        0        0     3609 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/databases/redis.py
--rw-r--r--   0        0        0      812 2022-06-02 08:11:44.411651 the_new_hotness-1.2.3/hotness/domain/__init__.py
--rw-r--r--   0        0        0      195 2022-06-02 10:01:53.713952 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2021-10-06 15:16:54.691389 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      157 2021-10-06 15:19:39.038411 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      193 2022-06-02 10:11:44.817772 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      193 2022-06-02 10:11:58.408806 the_new_hotness-1.2.3/hotness/domain/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1775 2023-04-21 13:39:35.512484 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-310.pyc
--rw-r--r--   0        0        0     1760 2021-10-06 15:16:54.693389 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-36.pyc
--rw-r--r--   0        0        0     1764 2021-10-06 15:19:39.041411 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-37.pyc
--rw-r--r--   0        0        0     1784 2022-06-02 10:11:44.817772 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-38.pyc
--rw-r--r--   0        0        0     1784 2022-06-02 10:11:58.409806 the_new_hotness-1.2.3/hotness/domain/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0     2181 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/domain/package.py
--rw-r--r--   0        0        0     1140 2023-04-21 13:07:13.385253 the_new_hotness-1.2.3/hotness/exceptions/__init__.py
--rw-r--r--   0        0        0      507 2023-04-21 13:39:35.592484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      497 2021-12-07 12:17:58.506775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      501 2021-12-07 12:18:07.281803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      505 2022-06-02 10:11:44.917772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      505 2022-06-02 10:11:58.527806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1299 2023-04-21 13:39:35.592484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-310.pyc
--rw-r--r--   0        0        0     1268 2021-12-07 12:17:58.507775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-36.pyc
--rw-r--r--   0        0        0     1272 2021-12-07 12:18:07.282803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-37.pyc
--rw-r--r--   0        0        0     1294 2022-06-02 10:11:44.918772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-38.pyc
--rw-r--r--   0        0        0     1294 2022-06-02 10:11:58.528806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/base_exception.cpython-39.pyc
--rw-r--r--   0        0        0     1788 2023-04-21 13:39:35.593484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-310.pyc
--rw-r--r--   0        0        0     1736 2021-12-07 12:17:58.507775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-36.pyc
--rw-r--r--   0        0        0     1740 2021-12-07 12:18:07.283804 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-37.pyc
--rw-r--r--   0        0        0     1779 2022-06-02 10:11:44.919772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-38.pyc
--rw-r--r--   0        0        0     1779 2022-06-02 10:11:58.529806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/builder_exception.cpython-39.pyc
--rw-r--r--   0        0        0      841 2023-04-21 13:39:35.594484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-310.pyc
--rw-r--r--   0        0        0      825 2021-12-07 12:17:58.508775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-36.pyc
--rw-r--r--   0        0        0      829 2021-12-07 12:18:07.283804 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-37.pyc
--rw-r--r--   0        0        0      839 2022-06-02 10:11:44.919772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-38.pyc
--rw-r--r--   0        0        0      839 2022-06-02 10:11:58.530806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/download_exception.cpython-39.pyc
--rw-r--r--   0        0        0     1122 2021-04-12 11:42:23.041453 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/html_exception.cpython-39.pyc
--rw-r--r--   0        0        0     1168 2023-04-21 13:39:35.595484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-310.pyc
--rw-r--r--   0        0        0     1146 2021-12-07 12:17:58.508775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-36.pyc
--rw-r--r--   0        0        0     1150 2021-12-07 12:18:07.284803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-37.pyc
--rw-r--r--   0        0        0     1157 2022-06-02 10:11:44.920772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-38.pyc
--rw-r--r--   0        0        0     1157 2022-06-02 10:11:58.531806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/http_exception.cpython-39.pyc
--rw-r--r--   0        0        0      876 2023-04-21 13:39:35.595484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-310.pyc
--rw-r--r--   0        0        0      858 2021-12-07 12:17:58.509775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-36.pyc
--rw-r--r--   0        0        0      862 2021-12-07 12:18:07.284803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-37.pyc
--rw-r--r--   0        0        0      872 2022-06-02 10:11:44.920772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-38.pyc
--rw-r--r--   0        0        0      872 2022-06-02 10:11:58.531806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/notifier_exception.cpython-39.pyc
--rw-r--r--   0        0        0      841 2023-04-21 13:39:35.596484 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-310.pyc
--rw-r--r--   0        0        0      823 2021-12-07 12:17:58.509775 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-36.pyc
--rw-r--r--   0        0        0      827 2021-12-07 12:18:07.285803 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-37.pyc
--rw-r--r--   0        0        0      837 2022-06-02 10:11:44.921772 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-38.pyc
--rw-r--r--   0        0        0      837 2022-06-02 10:11:58.532806 the_new_hotness-1.2.3/hotness/exceptions/__pycache__/patcher_exception.cpython-39.pyc
--rw-r--r--   0        0        0     1602 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/base_exception.py
--rw-r--r--   0        0        0     2438 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/builder_exception.py
--rw-r--r--   0        0        0     1223 2023-04-21 13:07:13.386253 the_new_hotness-1.2.3/hotness/exceptions/download_exception.py
--rw-r--r--   0        0        0     1513 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/http_exception.py
--rw-r--r--   0        0        0     1253 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/notifier_exception.py
--rw-r--r--   0        0        0     1219 2023-04-21 13:07:13.387253 the_new_hotness-1.2.3/hotness/exceptions/patcher_exception.py
--rw-r--r--   0        0        0    28765 2023-04-24 10:44:45.366658 the_new_hotness-1.2.3/hotness/hotness_consumer.py
--rw-r--r--   0        0        0      919 2022-06-02 08:11:44.414651 the_new_hotness-1.2.3/hotness/notifiers/__init__.py
--rw-r--r--   0        0        0      297 2022-06-02 10:01:53.841952 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      255 2021-10-06 15:16:54.831389 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      259 2021-10-06 15:19:39.259410 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      295 2022-06-02 10:11:44.949772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      295 2022-06-02 10:11:58.570806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7855 2023-04-21 13:39:35.637484 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-310.pyc
--rw-r--r--   0        0        0     8123 2021-11-23 15:45:23.344454 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-36.pyc
--rw-r--r--   0        0        0     7802 2022-02-10 13:19:26.228272 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-37.pyc
--rw-r--r--   0        0        0     7872 2022-06-02 10:11:44.951772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-38.pyc
--rw-r--r--   0        0        0     7842 2022-06-02 10:11:58.572806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/bugzilla.cpython-39.pyc
--rw-r--r--   0        0        0     2995 2023-04-21 13:39:35.645484 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-310.pyc
--rw-r--r--   0        0        0     2972 2021-11-23 15:45:23.352454 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-36.pyc
--rw-r--r--   0        0        0     2976 2021-11-23 15:45:33.176491 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-37.pyc
--rw-r--r--   0        0        0     2994 2022-06-02 10:11:44.960772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-38.pyc
--rw-r--r--   0        0        0     3008 2022-06-02 10:11:58.585806 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/fedora_messaging.cpython-39.pyc
--rw-r--r--   0        0        0     1302 2022-06-02 10:01:53.841952 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2021-10-06 15:16:54.832389 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-36.pyc
--rw-r--r--   0        0        0     1255 2021-10-06 15:19:39.261411 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-37.pyc
--rw-r--r--   0        0        0     1299 2022-06-02 10:11:44.949772 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-38.pyc
--rw-r--r--   0        0        0     1299 2022-06-02 10:11:58.571807 the_new_hotness-1.2.3/hotness/notifiers/__pycache__/notifier.cpython-39.pyc
--rw-r--r--   0        0        0    10095 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/notifiers/bugzilla.py
--rw-r--r--   0        0        0     3552 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/notifiers/fedora_messaging.py
--rw-r--r--   0        0        0     1663 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/notifiers/notifier.py
--rw-r--r--   0        0        0      857 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/patchers/__init__.py
--rw-r--r--   0        0        0      238 2022-06-02 10:01:54.130952 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      196 2021-10-06 15:16:55.434389 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      200 2021-10-06 15:19:39.925411 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      236 2022-06-02 10:11:45.261773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      236 2022-06-02 10:11:58.921807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3249 2023-04-21 13:39:35.946486 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-310.pyc
--rw-r--r--   0        0        0     3480 2021-11-23 15:45:23.640455 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-36.pyc
--rw-r--r--   0        0        0     3176 2022-02-10 13:25:53.423747 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-37.pyc
--rw-r--r--   0        0        0     3199 2022-06-02 10:11:45.265773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-38.pyc
--rw-r--r--   0        0        0     3234 2022-06-02 10:11:58.922807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-39.pyc
--rw-r--r--   0        0        0     5239 2022-04-14 10:12:40.509773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/pagure.cpython-38.pyc
--rw-r--r--   0        0        0     5451 2021-07-22 11:18:54.809605 the_new_hotness-1.2.3/hotness/patchers/__pycache__/pagure.cpython-39.pyc
--rw-r--r--   0        0        0     1249 2022-06-02 10:01:54.131952 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-310.pyc
--rw-r--r--   0        0        0     1198 2021-10-06 15:16:55.435389 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-36.pyc
--rw-r--r--   0        0        0     1202 2021-10-06 15:19:39.926411 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-37.pyc
--rw-r--r--   0        0        0     1246 2022-06-02 10:11:45.263773 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-38.pyc
--rw-r--r--   0        0        0     1246 2022-06-02 10:11:58.921807 the_new_hotness-1.2.3/hotness/patchers/__pycache__/patcher.cpython-39.pyc
--rw-r--r--   0        0        0     4008 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/patchers/bugzilla.py
--rw-r--r--   0        0        0     1607 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/patchers/patcher.py
--rw-r--r--   0        0        0     1181 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/__init__.py
--rw-r--r--   0        0        0      542 2022-06-02 10:01:54.142952 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      500 2021-10-06 15:16:55.450389 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      504 2021-10-06 15:19:39.944411 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      540 2022-06-02 10:11:45.283773 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      540 2022-06-02 10:11:58.932807 the_new_hotness-1.2.3/hotness/requests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      939 2022-06-02 10:01:54.143952 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-310.pyc
--rw-r--r--   0        0        0      887 2021-10-06 15:16:55.452389 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-36.pyc
--rw-r--r--   0        0        0      891 2021-10-06 15:19:39.950410 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-37.pyc
--rw-r--r--   0        0        0      933 2022-06-02 10:11:45.286773 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-38.pyc
--rw-r--r--   0        0        0      933 2022-06-02 10:11:58.934807 the_new_hotness-1.2.3/hotness/requests/__pycache__/build_request.cpython-39.pyc
--rw-r--r--   0        0        0      897 2022-06-02 10:01:54.145952 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-310.pyc
--rw-r--r--   0        0        0      845 2021-10-06 15:16:55.456389 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-36.pyc
--rw-r--r--   0        0        0      849 2021-10-06 15:19:39.954411 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-37.pyc
--rw-r--r--   0        0        0      891 2022-06-02 10:11:45.289773 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-38.pyc
--rw-r--r--   0        0        0      891 2022-06-02 10:11:58.935807 the_new_hotness-1.2.3/hotness/requests/__pycache__/insert_data_request.cpython-39.pyc
--rw-r--r--   0        0        0     1041 2022-06-02 10:01:54.144952 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-310.pyc
--rw-r--r--   0        0        0      987 2021-10-06 15:16:55.453389 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-36.pyc
--rw-r--r--   0        0        0      991 2021-10-06 15:19:39.951411 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-37.pyc
--rw-r--r--   0        0        0     1033 2022-06-02 10:11:45.287773 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-38.pyc
--rw-r--r--   0        0        0     1033 2022-06-02 10:11:58.934807 the_new_hotness-1.2.3/hotness/requests/__pycache__/notify_request.cpython-39.pyc
--rw-r--r--   0        0        0      885 2022-06-02 10:01:54.143952 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-310.pyc
--rw-r--r--   0        0        0      835 2021-10-06 15:16:55.452389 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-36.pyc
--rw-r--r--   0        0        0      839 2021-10-06 15:19:39.949411 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-37.pyc
--rw-r--r--   0        0        0      881 2022-06-02 10:11:45.285773 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-38.pyc
--rw-r--r--   0        0        0      881 2022-06-02 10:11:58.933807 the_new_hotness-1.2.3/hotness/requests/__pycache__/package_request.cpython-39.pyc
--rw-r--r--   0        0        0     1632 2023-04-21 13:39:35.955486 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-310.pyc
--rw-r--r--   0        0        0     1537 2021-10-06 15:16:55.451389 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-36.pyc
--rw-r--r--   0        0        0     1541 2021-10-06 15:19:39.947410 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-37.pyc
--rw-r--r--   0        0        0     1629 2022-06-02 10:11:45.284773 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-38.pyc
--rw-r--r--   0        0        0     1629 2022-06-02 10:11:58.933807 the_new_hotness-1.2.3/hotness/requests/__pycache__/request.cpython-39.pyc
--rw-r--r--   0        0        0      805 2022-06-02 10:01:54.145952 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-310.pyc
--rw-r--r--   0        0        0      755 2021-10-06 15:16:55.457389 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-36.pyc
--rw-r--r--   0        0        0      759 2021-10-06 15:19:39.956411 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-37.pyc
--rw-r--r--   0        0        0      801 2022-06-02 10:11:45.290773 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-38.pyc
--rw-r--r--   0        0        0      801 2022-06-02 10:11:58.936807 the_new_hotness-1.2.3/hotness/requests/__pycache__/retrieve_data_request.cpython-39.pyc
--rw-r--r--   0        0        0     1046 2022-06-02 10:01:54.144952 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-310.pyc
--rw-r--r--   0        0        0      992 2021-10-06 15:16:55.454389 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-36.pyc
--rw-r--r--   0        0        0      996 2021-10-06 15:19:39.953410 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-37.pyc
--rw-r--r--   0        0        0     1038 2022-06-02 10:11:45.288773 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-38.pyc
--rw-r--r--   0        0        0     1038 2022-06-02 10:11:58.935807 the_new_hotness-1.2.3/hotness/requests/__pycache__/submit_patch_request.cpython-39.pyc
--rw-r--r--   0        0        0     1287 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/build_request.py
--rw-r--r--   0        0        0     1256 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/insert_data_request.py
--rw-r--r--   0        0        0     1394 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/notify_request.py
--rw-r--r--   0        0        0     1234 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/package_request.py
--rw-r--r--   0        0        0     1905 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/requests/request.py
--rw-r--r--   0        0        0     1152 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/retrieve_data_request.py
--rw-r--r--   0        0        0     1389 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/requests/submit_patch_request.py
--rw-r--r--   0        0        0      934 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/responses/__init__.py
--rw-r--r--   0        0        0      312 2022-06-02 10:01:54.139952 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      270 2021-10-06 15:16:55.461389 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      274 2021-10-06 15:19:39.960410 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      310 2022-06-02 10:11:45.278773 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      310 2022-06-02 10:11:58.929807 the_new_hotness-1.2.3/hotness/responses/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1204 2022-06-02 10:01:54.140952 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     1168 2021-10-06 15:16:55.463389 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-36.pyc
--rw-r--r--   0        0        0     1172 2021-10-06 15:19:39.962411 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-37.pyc
--rw-r--r--   0        0        0     1216 2022-06-02 10:11:45.279773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-38.pyc
--rw-r--r--   0        0        0     1216 2022-06-02 10:11:58.930807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response.cpython-39.pyc
--rw-r--r--   0        0        0     5684 2023-04-21 13:39:35.954486 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-310.pyc
--rw-r--r--   0        0        0     5749 2021-12-07 12:17:58.828776 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-36.pyc
--rw-r--r--   0        0        0     5753 2021-12-07 12:18:07.544804 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-37.pyc
--rw-r--r--   0        0        0     5774 2022-06-02 10:11:45.282773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-38.pyc
--rw-r--r--   0        0        0     5770 2022-06-02 10:11:58.932807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-39.pyc
--rw-r--r--   0        0        0     1389 2022-06-02 10:01:54.140952 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-310.pyc
--rw-r--r--   0        0        0     1338 2021-10-06 15:16:55.464389 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-36.pyc
--rw-r--r--   0        0        0     1342 2021-10-06 15:19:39.964411 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-37.pyc
--rw-r--r--   0        0        0     1392 2022-06-02 10:11:45.280773 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-38.pyc
--rw-r--r--   0        0        0     1392 2022-06-02 10:11:58.931807 the_new_hotness-1.2.3/hotness/responses/__pycache__/response_success.cpython-39.pyc
--rw-r--r--   0        0        0     1540 2022-06-02 08:11:44.416651 the_new_hotness-1.2.3/hotness/responses/response.py
--rw-r--r--   0        0        0     6212 2023-04-21 13:07:13.388253 the_new_hotness-1.2.3/hotness/responses/response_failure.py
--rw-r--r--   0        0        0     1623 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/responses/response_success.py
--rw-r--r--   0        0        0     1194 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/__init__.py
--rw-r--r--   0        0        0      560 2022-06-02 10:01:54.146952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      518 2021-10-06 15:16:55.458389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      522 2021-10-06 15:19:39.958411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      558 2022-06-02 10:11:45.291773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      558 2022-06-02 10:11:58.937807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2022-06-02 10:01:54.147952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1564 2021-10-06 15:16:55.460389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1570 2021-10-06 15:19:39.959411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1626 2022-06-02 10:11:45.292773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1624 2022-06-02 10:11:58.937807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/insert_data_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1643 2022-06-02 10:01:54.149952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1577 2021-10-06 15:16:55.472389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1583 2021-10-06 15:19:39.972411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1645 2022-06-02 10:11:45.296773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1639 2022-06-02 10:11:58.940807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/notify_user_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1656 2022-06-02 10:01:54.148952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1592 2021-10-06 15:16:55.469389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1598 2021-10-06 15:19:39.969411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1654 2022-06-02 10:11:45.294773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1652 2022-06-02 10:11:58.939808 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_check_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1655 2022-06-02 10:01:54.148952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1591 2021-10-06 15:16:55.471389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1597 2021-10-06 15:19:39.970410 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1653 2022-06-02 10:11:45.295773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1651 2022-06-02 10:11:58.939808 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1635 2022-06-02 10:01:54.147952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1571 2021-10-06 15:16:55.467389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1577 2021-10-06 15:19:39.968411 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1633 2022-06-02 10:11:45.293773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1631 2022-06-02 10:11:58.938807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1673 2022-06-02 10:01:54.149952 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-310.pyc
--rw-r--r--   0        0        0     1607 2021-10-06 15:16:55.474389 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-36.pyc
--rw-r--r--   0        0        0     1613 2021-10-06 15:19:39.973410 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-37.pyc
--rw-r--r--   0        0        0     1675 2022-06-02 10:11:45.297773 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-38.pyc
--rw-r--r--   0        0        0     1669 2022-06-02 10:11:58.941807 the_new_hotness-1.2.3/hotness/use_cases/__pycache__/submit_patch_use_case.cpython-39.pyc
--rw-r--r--   0        0        0     1992 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/insert_data_use_case.py
--rw-r--r--   0        0        0     2033 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/notify_user_use_case.py
--rw-r--r--   0        0        0     2011 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/package_check_use_case.py
--rw-r--r--   0        0        0     1982 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/package_scratch_build_use_case.py
--rw-r--r--   0        0        0     1991 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/retrieve_data_use_case.py
--rw-r--r--   0        0        0     2061 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/use_cases/submit_patch_use_case.py
--rw-r--r--   0        0        0      931 2022-06-02 08:11:44.418651 the_new_hotness-1.2.3/hotness/validators/__init__.py
--rw-r--r--   0        0        0      306 2022-06-02 10:01:54.133952 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      264 2021-10-06 15:16:55.438389 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0        0        0      268 2021-10-06 15:19:39.929411 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0      304 2022-06-02 10:11:45.266773 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      304 2022-06-02 10:11:58.923807 the_new_hotness-1.2.3/hotness/validators/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4391 2023-04-21 13:39:35.948486 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-310.pyc
--rw-r--r--   0        0        0     3518 2021-10-06 15:16:55.440389 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-36.pyc
--rw-r--r--   0        0        0     3517 2021-10-06 15:19:39.932411 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-37.pyc
--rw-r--r--   0        0        0     4391 2022-06-02 10:11:45.269773 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-38.pyc
--rw-r--r--   0        0        0     4391 2022-06-02 10:11:58.924807 the_new_hotness-1.2.3/hotness/validators/__pycache__/mdapi.cpython-39.pyc
--rw-r--r--   0        0        0     3522 2023-04-21 13:39:35.951486 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-310.pyc
--rw-r--r--   0        0        0     2787 2021-10-06 15:16:55.447389 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-36.pyc
--rw-r--r--   0        0        0     2791 2021-10-06 15:19:39.941411 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-37.pyc
--rw-r--r--   0        0        0     3526 2022-06-02 10:11:45.275773 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-38.pyc
--rw-r--r--   0        0        0     3511 2022-06-02 10:11:58.928807 the_new_hotness-1.2.3/hotness/validators/__pycache__/pagure.cpython-39.pyc
--rw-r--r--   0        0        0     2817 2023-04-21 13:39:35.952486 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-310.pyc
--rw-r--r--   0        0        0     2619 2021-10-06 15:16:55.449389 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-36.pyc
--rw-r--r--   0        0        0     2623 2021-10-06 15:19:39.942411 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-37.pyc
--rw-r--r--   0        0        0     2804 2022-06-02 10:11:45.276773 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-38.pyc
--rw-r--r--   0        0        0     2798 2022-06-02 10:11:58.929807 the_new_hotness-1.2.3/hotness/validators/__pycache__/pdc.cpython-39.pyc
--rw-r--r--   0        0        0      938 2022-06-02 10:01:54.133952 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-310.pyc
--rw-r--r--   0        0        0      891 2021-10-06 15:16:55.439389 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-36.pyc
--rw-r--r--   0        0        0      895 2021-10-06 15:19:39.930410 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-37.pyc
--rw-r--r--   0        0        0      939 2022-06-02 10:11:45.267773 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-38.pyc
--rw-r--r--   0        0        0      939 2022-06-02 10:11:58.923807 the_new_hotness-1.2.3/hotness/validators/__pycache__/validator.cpython-39.pyc
--rw-r--r--   0        0        0     5409 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/mdapi.py
--rw-r--r--   0        0        0     5768 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/pagure.py
--rw-r--r--   0        0        0     3597 2023-04-21 13:07:13.389253 the_new_hotness-1.2.3/hotness/validators/pdc.py
--rw-r--r--   0        0        0     1309 2022-06-02 08:11:44.419651 the_new_hotness-1.2.3/hotness/validators/validator.py
--rw-r--r--   0        0        0     2482 2023-04-24 14:30:13.547842 the_new_hotness-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 the_new_hotness-1.2.3/setup.py
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 the_new_hotness-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    26530 2021-01-25 12:20:24.199782 the_new_hotness-1.2.4/LICENSE
+-rw-r--r--   0        0        0     1369 2023-04-21 13:07:13.379253 the_new_hotness-1.2.4/README.rst
+-rw-r--r--   0        0        0     5389 2023-04-21 13:07:13.379253 the_new_hotness-1.2.4/config/config.toml.example
+-rw-r--r--   0        0        0      288 2023-04-21 13:07:13.383253 the_new_hotness-1.2.4/hotness/__init__.py
+-rw-r--r--   0        0        0      849 2022-06-02 08:11:44.409651 the_new_hotness-1.2.4/hotness/builders/__init__.py
+-rw-r--r--   0        0        0     1467 2022-06-02 08:11:44.409651 the_new_hotness-1.2.4/hotness/builders/builder.py
+-rw-r--r--   0        0        0    19346 2023-05-23 11:04:10.587254 the_new_hotness-1.2.4/hotness/builders/koji.py
+-rw-r--r--   0        0        0      804 2022-06-02 08:11:44.409651 the_new_hotness-1.2.4/hotness/common/__init__.py
+-rw-r--r--   0        0        0     5876 2023-04-21 13:07:13.384253 the_new_hotness-1.2.4/hotness/common/rpm.py
+-rw-r--r--   0        0        0     6329 2023-04-21 13:07:13.384253 the_new_hotness-1.2.4/hotness/config.py
+-rw-r--r--   0        0        0      897 2023-04-21 13:07:13.384253 the_new_hotness-1.2.4/hotness/databases/__init__.py
+-rw-r--r--   0        0        0     2511 2023-04-21 13:07:13.384253 the_new_hotness-1.2.4/hotness/databases/cache.py
+-rw-r--r--   0        0        0     1803 2022-06-02 08:11:44.411651 the_new_hotness-1.2.4/hotness/databases/database.py
+-rw-r--r--   0        0        0     3609 2023-04-21 13:07:13.385253 the_new_hotness-1.2.4/hotness/databases/redis.py
+-rw-r--r--   0        0        0      812 2022-06-02 08:11:44.411651 the_new_hotness-1.2.4/hotness/domain/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-21 13:07:13.385253 the_new_hotness-1.2.4/hotness/domain/package.py
+-rw-r--r--   0        0        0     1140 2023-04-21 13:07:13.385253 the_new_hotness-1.2.4/hotness/exceptions/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-21 13:07:13.386253 the_new_hotness-1.2.4/hotness/exceptions/base_exception.py
+-rw-r--r--   0        0        0     2438 2023-04-21 13:07:13.386253 the_new_hotness-1.2.4/hotness/exceptions/builder_exception.py
+-rw-r--r--   0        0        0     1223 2023-04-21 13:07:13.386253 the_new_hotness-1.2.4/hotness/exceptions/download_exception.py
+-rw-r--r--   0        0        0     1513 2023-04-21 13:07:13.387253 the_new_hotness-1.2.4/hotness/exceptions/http_exception.py
+-rw-r--r--   0        0        0     1253 2023-04-21 13:07:13.387253 the_new_hotness-1.2.4/hotness/exceptions/notifier_exception.py
+-rw-r--r--   0        0        0     1219 2023-04-21 13:07:13.387253 the_new_hotness-1.2.4/hotness/exceptions/patcher_exception.py
+-rw-r--r--   0        0        0    28765 2023-04-24 15:04:09.499603 the_new_hotness-1.2.4/hotness/hotness_consumer.py
+-rw-r--r--   0        0        0      919 2022-06-02 08:11:44.414651 the_new_hotness-1.2.4/hotness/notifiers/__init__.py
+-rw-r--r--   0        0        0    10095 2023-04-21 13:07:13.388253 the_new_hotness-1.2.4/hotness/notifiers/bugzilla.py
+-rw-r--r--   0        0        0     3552 2023-04-21 13:07:13.388253 the_new_hotness-1.2.4/hotness/notifiers/fedora_messaging.py
+-rw-r--r--   0        0        0     1663 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/notifiers/notifier.py
+-rw-r--r--   0        0        0      857 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/patchers/__init__.py
+-rw-r--r--   0        0        0     4008 2023-04-21 13:07:13.388253 the_new_hotness-1.2.4/hotness/patchers/bugzilla.py
+-rw-r--r--   0        0        0     1607 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/patchers/patcher.py
+-rw-r--r--   0        0        0     1181 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/__init__.py
+-rw-r--r--   0        0        0     1287 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/build_request.py
+-rw-r--r--   0        0        0     1256 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/insert_data_request.py
+-rw-r--r--   0        0        0     1394 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/notify_request.py
+-rw-r--r--   0        0        0     1234 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/package_request.py
+-rw-r--r--   0        0        0     1905 2023-04-21 13:07:13.388253 the_new_hotness-1.2.4/hotness/requests/request.py
+-rw-r--r--   0        0        0     1152 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/retrieve_data_request.py
+-rw-r--r--   0        0        0     1389 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/requests/submit_patch_request.py
+-rw-r--r--   0        0        0      934 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/responses/__init__.py
+-rw-r--r--   0        0        0     1540 2022-06-02 08:11:44.416651 the_new_hotness-1.2.4/hotness/responses/response.py
+-rw-r--r--   0        0        0     6212 2023-04-21 13:07:13.388253 the_new_hotness-1.2.4/hotness/responses/response_failure.py
+-rw-r--r--   0        0        0     1623 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/responses/response_success.py
+-rw-r--r--   0        0        0     1194 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/__init__.py
+-rw-r--r--   0        0        0     1992 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/insert_data_use_case.py
+-rw-r--r--   0        0        0     2033 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/notify_user_use_case.py
+-rw-r--r--   0        0        0     2011 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/package_check_use_case.py
+-rw-r--r--   0        0        0     1982 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/package_scratch_build_use_case.py
+-rw-r--r--   0        0        0     1991 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/retrieve_data_use_case.py
+-rw-r--r--   0        0        0     2061 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/use_cases/submit_patch_use_case.py
+-rw-r--r--   0        0        0      931 2022-06-02 08:11:44.418651 the_new_hotness-1.2.4/hotness/validators/__init__.py
+-rw-r--r--   0        0        0     5409 2023-04-21 13:07:13.389253 the_new_hotness-1.2.4/hotness/validators/mdapi.py
+-rw-r--r--   0        0        0     5768 2023-04-21 13:07:13.389253 the_new_hotness-1.2.4/hotness/validators/pagure.py
+-rw-r--r--   0        0        0     3597 2023-04-21 13:07:13.389253 the_new_hotness-1.2.4/hotness/validators/pdc.py
+-rw-r--r--   0        0        0     1309 2022-06-02 08:11:44.419651 the_new_hotness-1.2.4/hotness/validators/validator.py
+-rw-r--r--   0        0        0     2602 2023-05-23 11:43:11.612993 the_new_hotness-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 the_new_hotness-1.2.4/setup.py
+-rw-r--r--   0        0        0     2745 1970-01-01 00:00:00.000000 the_new_hotness-1.2.4/PKG-INFO
```

### Comparing `the_new_hotness-1.2.3/LICENSE` & `the_new_hotness-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/README.rst` & `the_new_hotness-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/config/config.toml.example` & `the_new_hotness-1.2.4/config/config.toml.example`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/builders/__init__.py` & `the_new_hotness-1.2.4/hotness/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/builders/builder.py` & `the_new_hotness-1.2.4/hotness/builders/builder.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/builders/koji.py` & `the_new_hotness-1.2.4/hotness/builders/koji.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,15 +194,19 @@
                 output["patch"] = f.read()
 
             # We compare the old sources to the new ones to make sure we download
             # new sources from bumping the specfile version. Some packages don't
             # use macros in the source URL(s). We want to detect these and notify
             # the packager on the bug we filed about the new version.
             old_sources = self._dist_git_sources(tmp)
-            new_sources = self._spec_sources(specfile, tmp)
+            try:
+                new_sources = self._spec_sources(specfile, tmp)
+            except DownloadException as exc:
+                # Attach the patch if DownloadException is thrown
+                raise BuilderException(str(exc), value=output)
             output["message"] = self._compare_sources(old_sources, new_sources)
 
             try:
                 cmd_output = sp.check_output(
                     [
                         "rpmbuild",
                         "-D",
@@ -222,15 +226,28 @@
                     std_out = exc.stdout.decode()
                 if exc.stderr:
                     std_err = exc.stderr.decode()
                 raise BuilderException(
                     str(exc), value=output, std_out=std_out, std_err=std_err
                 )
 
-            srpm = os.path.join(tmp, cmd_output.decode("utf-8").strip().split()[-1])
+            # The output from rpmbuild looks like this
+            # warning: source_date_epoch_from_changelog set but %changelog is missing
+            # Wrote: ./SRPMS/uncrustify-0.77.1-1.fc38.src.rpm
+            #
+            # RPM build warnings:
+            #     source_date_epoch_from_changelog set but %changelog is missing
+            #
+            # We need to separate just the source RPM
+            srpm = ""
+            for line in cmd_output.decode("utf-8").splitlines():
+                if line.startswith("Wrote"):
+                    srpm = os.path.join(tmp, line.split()[-1])
+                    break
+
             _logger.debug("Got srpm %r" % srpm)
 
             session = self._session_maker()
             if not session:
                 raise BuilderException("Can't authenticate with Koji!")
             output["build_id"] = self._scratch_build(session, package.name, srpm)
 
@@ -245,17 +262,14 @@
             ['/path/to/repo/source0.tar.gz', '/path/to/repo/source1.tar.gz']
 
         Params:
             dist_git_path: The filesystem path to the dist-git repository
 
         Returns:
             A list of absolute paths to source files downloaded
-
-        Raises:
-            subprocess.CalledProcessError: When downloading the sources fails.
         """
         files = []
         # The output format is:
         # Downloading requests-2.12.4.tar.gz
         # ####################################################################### 100.0%
         # Downloading requests-2.12.4-tests.tar.gz
         # ####################################################################### 100.0%
@@ -444,15 +458,27 @@
 
         Returns:
             Build id.
         """
         _logger.info("Uploading {source} to koji".format(source=source))
         suffix = "".join([random.choice(string.ascii_letters) for i in range(8)])
         serverdir = "%s/%r.%s" % ("cli-build", time.time(), suffix)
-        session.uploadWrapper(source, serverdir)
+        retry_counter = 0
+        upload_successful = False
+        while retry_counter < 3 and not upload_successful:
+            try:
+                session.uploadWrapper(source, serverdir)
+                upload_successful = True
+            except koji.GenericError:
+                # Wait for 5 seconds and retry the upload
+                time.sleep(5)
+                retry_counter += 1
+
+        if not upload_successful:
+            raise BuilderException("Couldn't upload source {} to koji.".format(source))
 
         remote = "%s/%s" % (serverdir, os.path.basename(source))
         _logger.info(
             "Intiating koji build for %r"
             % dict(name=name, target=self.target_tag, source=remote, opts=self.opts)
         )
         task_id = session.build(
```

### Comparing `the_new_hotness-1.2.3/hotness/common/__init__.py` & `the_new_hotness-1.2.4/hotness/common/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/common/rpm.py` & `the_new_hotness-1.2.4/hotness/common/rpm.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/config.py` & `the_new_hotness-1.2.4/hotness/config.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/databases/__init__.py` & `the_new_hotness-1.2.4/hotness/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/databases/__pycache__/database.cpython-36.pyc` & `the_new_hotness-1.2.4/hotness/databases/database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,113 @@
-00000000: 330d 0d0a 32ea 5a61 0b07 0000 e300 0000  3...2.Za........
-00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000020: 0073 1200 0000 4700 6400 6401 8400 6401  .s....G.d.d...d.
-00000030: 8302 5a00 6402 5300 2903 6300 0000 0000  ..Z.d.S.).c.....
-00000040: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000050: 3200 0000 6500 5a01 6400 5a02 6401 5a03  2...e.Z.d.Z.d.Z.
-00000060: 6504 6504 6505 6402 9c03 6403 6404 8404  e.e.e.d...d.d...
-00000070: 5a06 6504 6505 6405 9c02 6406 6407 8404  Z.e.e.d...d.d...
-00000080: 5a07 6408 5300 2909 da08 4461 7461 6261  Z.d.S.)...Databa
-00000090: 7365 7a95 0a20 2020 2041 6273 7472 6163  sez..    Abstrac
-000000a0: 7420 636c 6173 7320 666f 7220 6461 7461  t class for data
-000000b0: 6261 7365 7320 7573 6564 2062 7920 7468  bases used by th
-000000c0: 652d 6e65 772d 686f 746e 6573 7320 746f  e-new-hotness to
-000000d0: 2073 746f 7265 206b 6579 2f76 616c 7565   store key/value
-000000e0: 2070 6169 7273 2e0a 2020 2020 5468 6973   pairs..    This
-000000f0: 2063 6c61 7373 206d 7573 7420 6265 2069   class must be i
-00000100: 6e68 6572 6974 6564 2062 7920 6576 6572  nherited by ever
-00000110: 7920 6578 7465 726e 616c 2064 6174 6162  y external datab
-00000120: 6173 652e 0a20 2020 2029 03da 036b 6579  ase..    )...key
-00000130: da05 7661 6c75 65da 0672 6574 7572 6e63  ..value..returnc
-00000140: 0300 0000 0000 0000 0300 0000 0100 0000  ................
-00000150: 4300 0000 7308 0000 0074 0082 0164 0153  C...s....t...d.S
-00000160: 0029 0261 4901 0000 0a20 2020 2020 2020  .).aI....       
-00000170: 2049 6e73 6572 7420 6d65 7468 6f64 2074   Insert method t
-00000180: 6861 7420 7368 6f75 6c64 2062 6520 696d  hat should be im
-00000190: 706c 656d 656e 7465 6420 6279 2065 7665  plemented by eve
-000001a0: 7279 2063 6869 6c64 2063 6c61 7373 2e0a  ry child class..
-000001b0: 0a20 2020 2020 2020 2049 7420 7368 6f75  .        It shou
-000001c0: 6c64 2069 6e73 6572 7420 6b65 792f 7661  ld insert key/va
-000001d0: 6c75 6520 7061 6972 2074 6f20 6461 7461  lue pair to data
-000001e0: 6261 7365 2075 7369 6e67 2074 6865 2065  base using the e
-000001f0: 7874 6572 6e61 6c20 7379 7374 656d 2061  xternal system a
-00000200: 6e64 0a20 2020 2020 2020 2072 6574 7572  nd.        retur
-00000210: 6e20 6469 6374 696f 6e61 7279 2063 6f6e  n dictionary con
-00000220: 7461 696e 696e 6720 616e 7920 7265 6c61  taining any rela
-00000230: 7465 6420 696e 666f 2e0a 0a20 2020 2020  ted info...     
-00000240: 2020 2049 6e20 6361 7365 206f 6620 616e     In case of an
-00000250: 7920 6973 7375 6520 7468 6174 2077 6f75  y issue that wou
-00000260: 6c64 2070 7265 7665 6e74 2069 6e73 6572  ld prevent inser
-00000270: 7469 6e67 2074 6865 2064 6174 612c 206d  ting the data, m
-00000280: 6574 686f 6420 7368 6f75 6c64 0a20 2020  ethod should.   
-00000290: 2020 2020 2072 6169 7365 2061 6e20 6578       raise an ex
-000002a0: 6365 7074 696f 6e2e 0a20 2020 2020 2020  ception..       
-000002b0: 204e 2901 da13 4e6f 7449 6d70 6c65 6d65   N)...NotImpleme
-000002c0: 6e74 6564 4572 726f 7229 03da 0473 656c  ntedError)...sel
-000002d0: 6672 0200 0000 7203 0000 00a9 0072 0700  fr....r......r..
-000002e0: 0000 fa22 2f61 7070 2f68 6f74 6e65 7373  ..."/app/hotness
-000002f0: 2f64 6174 6162 6173 6573 2f64 6174 6162  /databases/datab
-00000300: 6173 652e 7079 da06 696e 7365 7274 1800  ase.py..insert..
-00000310: 0000 7302 0000 0000 0a7a 0f44 6174 6162  ..s......z.Datab
-00000320: 6173 652e 696e 7365 7274 2902 7202 0000  ase.insert).r...
-00000330: 0072 0400 0000 6302 0000 0000 0000 0002  .r....c.........
-00000340: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
-00000350: 7400 8201 6401 5300 2902 614f 0100 000a  t...d.S.).aO....
-00000360: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
-00000370: 206d 6574 686f 6420 7468 6174 2073 686f   method that sho
-00000380: 756c 6420 6265 2069 6d70 6c65 6d65 6e74  uld be implement
-00000390: 6564 2062 7920 6576 6572 7920 6368 696c  ed by every chil
-000003a0: 6420 636c 6173 732e 0a0a 2020 2020 2020  d class...      
-000003b0: 2020 4974 2073 686f 756c 6420 7265 7472    It should retr
-000003c0: 6965 7665 2076 616c 7565 2066 6f72 206b  ieve value for k
-000003d0: 6579 2066 726f 6d20 6461 7461 6261 7365  ey from database
-000003e0: 2075 7369 6e67 2074 6865 2065 7874 6572   using the exter
-000003f0: 6e61 6c20 7379 7374 656d 2061 6e64 0a20  nal system and. 
-00000400: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-00000410: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00000420: 696e 6720 616e 7920 7265 6c61 7465 6420  ing any related 
-00000430: 696e 666f 2e0a 0a20 2020 2020 2020 2049  info...        I
-00000440: 6e20 6361 7365 206f 6620 616e 7920 6973  n case of any is
-00000450: 7375 6520 7468 6174 2077 6f75 6c64 2070  sue that would p
-00000460: 7265 7665 6e74 2072 6574 7269 6576 696e  revent retrievin
-00000470: 6720 7468 6520 6461 7461 2c20 6d65 7468  g the data, meth
-00000480: 6f64 2073 686f 756c 640a 2020 2020 2020  od should.      
-00000490: 2020 7261 6973 6520 616e 2065 7863 6570    raise an excep
-000004a0: 7469 6f6e 2e0a 2020 2020 2020 2020 4e29  tion..        N)
-000004b0: 0172 0500 0000 2902 7206 0000 0072 0200  .r....).r....r..
-000004c0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000004d0: 00da 0872 6574 7269 6576 6524 0000 0073  ...retrieve$...s
-000004e0: 0200 0000 000a 7a11 4461 7461 6261 7365  ......z.Database
-000004f0: 2e72 6574 7269 6576 654e 2908 da08 5f5f  .retrieveN)...__
-00000500: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000510: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000520: da07 5f5f 646f 635f 5fda 0373 7472 da04  ..__doc__..str..
-00000530: 6469 6374 7209 0000 0072 0a00 0000 7207  dictr....r....r.
-00000540: 0000 0072 0700 0000 7207 0000 0072 0800  ...r....r....r..
-00000550: 0000 7201 0000 0012 0000 0073 0600 0000  ..r........s....
-00000560: 0804 0402 120c 7201 0000 004e 2901 7201  ......r....N).r.
-00000570: 0000 0072 0700 0000 7207 0000 0072 0700  ...r....r....r..
-00000580: 0000 7208 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000590: 3e12 0000 0073 0000 0000                 >....s....
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 436f 7079  f-8 -*-.#.# Copy
+00000020: 7269 6768 7420 2843 2920 3230 3231 2052  right (C) 2021 R
+00000030: 6564 2048 6174 2c20 496e 632e 0a23 0a23  ed Hat, Inc..#.#
+00000040: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000050: 2066 7265 6520 736f 6674 7761 7265 3b20   free software; 
+00000060: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000070: 6275 7465 2069 7420 616e 642f 6f72 0a23  bute it and/or.#
+00000080: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+00000090: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+000000a0: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+000000b0: 626c 6963 204c 6963 656e 7365 0a23 2061  blic License.# a
+000000c0: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
+000000d0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
+000000e0: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
+000000f0: 6865 7220 7665 7273 696f 6e20 320a 2320  her version 2.# 
+00000100: 6f66 2074 6865 204c 6963 656e 7365 2c20  of the License, 
+00000110: 6f72 2028 6174 2079 6f75 7220 6f70 7469  or (at your opti
+00000120: 6f6e 2920 616e 7920 6c61 7465 7220 7665  on) any later ve
+00000130: 7273 696f 6e2e 0a23 0a23 2054 6869 7320  rsion..#.# This 
+00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+00000170: 6265 2075 7365 6675 6c2c 0a23 2062 7574  be useful,.# but
+00000180: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+00000190: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+000001a0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+000001b0: 7761 7272 616e 7479 206f 660a 2320 4d45  warranty of.# ME
+000001c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000001d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000001e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000001f0: 452e 2020 5365 6520 7468 650a 2320 474e  E.  See the.# GN
+00000200: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000210: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
+00000220: 6520 6465 7461 696c 732e 0a23 0a23 2059  e details..#.# Y
+00000230: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000240: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+00000250: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 0a23 2061 6c6f 6e67 2077 6974 6820 7468  .# along with th
+00000280: 6973 2070 726f 6772 616d 3b20 6966 206e  is program; if n
+00000290: 6f74 2c20 7772 6974 6520 746f 2074 6865  ot, write to the
+000002a0: 2046 7265 6520 536f 6674 7761 7265 0a23   Free Software.#
+000002b0: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
+000002c0: 2e2c 2035 3120 4672 616e 6b6c 696e 2053  ., 51 Franklin S
+000002d0: 7472 6565 742c 2046 6966 7468 2046 6c6f  treet, Fifth Flo
+000002e0: 6f72 2c20 426f 7374 6f6e 2c20 4d41 2020  or, Boston, MA  
+000002f0: 3032 3131 302d 3133 3031 2c20 5553 412e  02110-1301, USA.
+00000300: 0a63 6c61 7373 2044 6174 6162 6173 653a  .class Database:
+00000310: 0a20 2020 2022 2222 0a20 2020 2041 6273  .    """.    Abs
+00000320: 7472 6163 7420 636c 6173 7320 666f 7220  tract class for 
+00000330: 6461 7461 6261 7365 7320 7573 6564 2062  databases used b
+00000340: 7920 7468 652d 6e65 772d 686f 746e 6573  y the-new-hotnes
+00000350: 7320 746f 2073 746f 7265 206b 6579 2f76  s to store key/v
+00000360: 616c 7565 2070 6169 7273 2e0a 2020 2020  alue pairs..    
+00000370: 5468 6973 2063 6c61 7373 206d 7573 7420  This class must 
+00000380: 6265 2069 6e68 6572 6974 6564 2062 7920  be inherited by 
+00000390: 6576 6572 7920 6578 7465 726e 616c 2064  every external d
+000003a0: 6174 6162 6173 652e 0a20 2020 2022 2222  atabase..    """
+000003b0: 0a0a 2020 2020 6465 6620 696e 7365 7274  ..    def insert
+000003c0: 2873 656c 662c 206b 6579 3a20 7374 722c  (self, key: str,
+000003d0: 2076 616c 7565 3a20 7374 7229 202d 3e20   value: str) -> 
+000003e0: 6469 6374 3a0a 2020 2020 2020 2020 2222  dict:.        ""
+000003f0: 220a 2020 2020 2020 2020 496e 7365 7274  ".        Insert
+00000400: 206d 6574 686f 6420 7468 6174 2073 686f   method that sho
+00000410: 756c 6420 6265 2069 6d70 6c65 6d65 6e74  uld be implement
+00000420: 6564 2062 7920 6576 6572 7920 6368 696c  ed by every chil
+00000430: 6420 636c 6173 732e 0a0a 2020 2020 2020  d class...      
+00000440: 2020 4974 2073 686f 756c 6420 696e 7365    It should inse
+00000450: 7274 206b 6579 2f76 616c 7565 2070 6169  rt key/value pai
+00000460: 7220 746f 2064 6174 6162 6173 6520 7573  r to database us
+00000470: 696e 6720 7468 6520 6578 7465 726e 616c  ing the external
+00000480: 2073 7973 7465 6d20 616e 640a 2020 2020   system and.    
+00000490: 2020 2020 7265 7475 726e 2064 6963 7469      return dicti
+000004a0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+000004b0: 2061 6e79 2072 656c 6174 6564 2069 6e66   any related inf
+000004c0: 6f2e 0a0a 2020 2020 2020 2020 496e 2063  o...        In c
+000004d0: 6173 6520 6f66 2061 6e79 2069 7373 7565  ase of any issue
+000004e0: 2074 6861 7420 776f 756c 6420 7072 6576   that would prev
+000004f0: 656e 7420 696e 7365 7274 696e 6720 7468  ent inserting th
+00000500: 6520 6461 7461 2c20 6d65 7468 6f64 2073  e data, method s
+00000510: 686f 756c 640a 2020 2020 2020 2020 7261  hould.        ra
+00000520: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+00000530: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00000540: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00000550: 6d70 6c65 6d65 6e74 6564 4572 726f 720a  mplementedError.
+00000560: 0a20 2020 2064 6566 2072 6574 7269 6576  .    def retriev
+00000570: 6528 7365 6c66 2c20 6b65 793a 2073 7472  e(self, key: str
+00000580: 2920 2d3e 2064 6963 743a 0a20 2020 2020  ) -> dict:.     
+00000590: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+000005a0: 6574 7269 6576 6520 6d65 7468 6f64 2074  etrieve method t
+000005b0: 6861 7420 7368 6f75 6c64 2062 6520 696d  hat should be im
+000005c0: 706c 656d 656e 7465 6420 6279 2065 7665  plemented by eve
+000005d0: 7279 2063 6869 6c64 2063 6c61 7373 2e0a  ry child class..
+000005e0: 0a20 2020 2020 2020 2049 7420 7368 6f75  .        It shou
+000005f0: 6c64 2072 6574 7269 6576 6520 7661 6c75  ld retrieve valu
+00000600: 6520 666f 7220 6b65 7920 6672 6f6d 2064  e for key from d
+00000610: 6174 6162 6173 6520 7573 696e 6720 7468  atabase using th
+00000620: 6520 6578 7465 726e 616c 2073 7973 7465  e external syste
+00000630: 6d20 616e 640a 2020 2020 2020 2020 7265  m and.        re
+00000640: 7475 726e 2064 6963 7469 6f6e 6172 7920  turn dictionary 
+00000650: 636f 6e74 6169 6e69 6e67 2061 6e79 2072  containing any r
+00000660: 656c 6174 6564 2069 6e66 6f2e 0a0a 2020  elated info...  
+00000670: 2020 2020 2020 496e 2063 6173 6520 6f66        In case of
+00000680: 2061 6e79 2069 7373 7565 2074 6861 7420   any issue that 
+00000690: 776f 756c 6420 7072 6576 656e 7420 7265  would prevent re
+000006a0: 7472 6965 7669 6e67 2074 6865 2064 6174  trieving the dat
+000006b0: 612c 206d 6574 686f 6420 7368 6f75 6c64  a, method should
+000006c0: 0a20 2020 2020 2020 2072 6169 7365 2061  .        raise a
+000006d0: 6e20 6578 6365 7074 696f 6e2e 0a20 2020  n exception..   
+000006e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000006f0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+00000700: 656e 7465 6445 7272 6f72 0a              entedError.
```

### Comparing `the_new_hotness-1.2.3/hotness/databases/cache.py` & `the_new_hotness-1.2.4/hotness/databases/cache.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/databases/database.py` & `the_new_hotness-1.2.4/hotness/patchers/patcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,36 +11,32 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-class Database:
+from hotness.domain.package import Package
+
+
+class Patcher:
     """
-    Abstract class for databases used by the-new-hotness to store key/value pairs.
-    This class must be inherited by every external database.
+    Abstract class for patchers used by the-new-hotness to submit a patch.
+    This class must be inherited by every external patcher.
     """
 
-    def insert(self, key: str, value: str) -> dict:
+    def submit_patch(self, package: Package, patch: str, opts: dict) -> dict:
         """
-        Insert method that should be implemented by every child class.
+        Submit patch method that should be implemented by every child class.
 
-        It should insert key/value pair to database using the external system and
-        return dictionary containing any related info.
+        It should submit patch for package to external system and
+        return dictionary containing additional info.
 
-        In case of any issue that would prevent inserting the data, method should
+        In case of any issue that would prevent submitting the patch, method should
         raise an exception.
-        """
-        raise NotImplementedError
 
-    def retrieve(self, key: str) -> dict:
-        """
-        Retrieve method that should be implemented by every child class.
-
-        It should retrieve value for key from database using the external system and
-        return dictionary containing any related info.
-
-        In case of any issue that would prevent retrieving the data, method should
-        raise an exception.
+        Params:
+            package: Package to attach patch for
+            patch: Patch to attach
+            opts: Optional arguments specific for the external patcher system
         """
         raise NotImplementedError
```

### Comparing `the_new_hotness-1.2.3/hotness/databases/redis.py` & `the_new_hotness-1.2.4/hotness/databases/redis.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/domain/__init__.py` & `the_new_hotness-1.2.4/hotness/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/domain/package.py` & `the_new_hotness-1.2.4/hotness/domain/package.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/__init__.py` & `the_new_hotness-1.2.4/hotness/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/base_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/base_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/builder_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/builder_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/download_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/download_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/http_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/http_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/notifier_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/notifier_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/exceptions/patcher_exception.py` & `the_new_hotness-1.2.4/hotness/exceptions/patcher_exception.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/hotness_consumer.py` & `the_new_hotness-1.2.4/hotness/hotness_consumer.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/notifiers/__init__.py` & `the_new_hotness-1.2.4/hotness/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/notifiers/bugzilla.py` & `the_new_hotness-1.2.4/hotness/notifiers/bugzilla.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/notifiers/fedora_messaging.py` & `the_new_hotness-1.2.4/hotness/notifiers/fedora_messaging.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/notifiers/notifier.py` & `the_new_hotness-1.2.4/hotness/notifiers/notifier.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/patchers/__init__.py` & `the_new_hotness-1.2.4/hotness/patchers/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/patchers/__pycache__/bugzilla.cpython-36.pyc` & `the_new_hotness-1.2.4/hotness/patchers/bugzilla.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,218 +1,251 @@
-00000000: 330d 0d0a 02ec 9c61 bd11 0000 e300 0000  3......a........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 6600 0000 6400 6401 6c00 5a00 6400  .sf...d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c04 5a04 6400 6403 6c05  ..d.d.l.Z.d.d.l.
-00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6406 6c09 6d0a 5a0a 0100 6500  ..d.d.l.m.Z...e.
-00000070: 6a0b 650c 8301 5a0d 4700 6407 6408 8400  j.e...Z.G.d.d...
-00000080: 6408 650a 8303 5a0e 6401 5300 2909 e900  d.e...Z.d.S.)...
-00000090: 0000 004e 2901 da12 5465 6d70 6f72 6172  ...N)...Temporar
-000000a0: 7944 6972 6563 746f 7279 2901 da10 5061  yDirectory)...Pa
-000000b0: 7463 6865 7245 7863 6570 7469 6f6e 2901  tcherException).
-000000c0: da07 5061 636b 6167 65e9 0100 0000 2901  ..Package.....).
-000000d0: da07 5061 7463 6865 7263 0000 0000 0000  ..Patcherc......
-000000e0: 0000 0000 0000 0600 0000 0000 0000 7342  ..............sB
-000000f0: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
-00000100: 0465 0465 0465 0464 0264 039c 0587 0066  .e.e.e.d.d.....f
-00000110: 0164 0464 0584 0c5a 0565 0665 0465 0765  .d.d...Z.e.e.e.e
-00000120: 0764 069c 0464 0764 0884 045a 0887 0004  .d...d.d...Z....
-00000130: 005a 0953 0029 09da 0842 7567 7a69 6c6c  .Z.S.)...Bugzill
-00000140: 617a ad0a 2020 2020 5468 6973 2063 6c61  az..    This cla
-00000150: 7373 2069 7320 6120 7772 6170 7065 7220  ss is a wrapper 
-00000160: 666f 7220 6874 7470 733a 2f2f 6275 677a  for https://bugz
-00000170: 696c 6c61 2e72 6564 6861 742e 636f 6d2f  illa.redhat.com/
-00000180: 0a20 2020 2049 7420 7375 626d 6974 2070  .    It submit p
-00000190: 6174 6368 6573 2074 6f20 4275 677a 696c  atches to Bugzil
-000001a0: 6c61 2e0a 0a20 2020 2041 7474 7269 6275  la...    Attribu
-000001b0: 7465 733a 0a20 2020 2020 2020 2062 7567  tes:.        bug
-000001c0: 7a69 6c6c 6120 2862 7567 7a69 6c6c 612e  zilla (bugzilla.
-000001d0: 4275 677a 696c 6c61 293a 2042 7567 7a69  Bugzilla): Bugzi
-000001e0: 6c6c 6120 7365 7373 696f 6e0a 2020 2020  lla session.    
-000001f0: 4e29 05da 0a73 6572 7665 725f 7572 6cda  N)...server_url.
-00000200: 0875 7365 726e 616d 65da 0870 6173 7377  .username..passw
-00000210: 6f72 64da 0761 7069 5f6b 6579 da06 7265  ord..api_key..re
-00000220: 7475 726e 6305 0000 0000 0000 0005 0000  turnc...........
-00000230: 0007 0000 0003 0000 0073 5c00 0000 7400  .........s\...t.
-00000240: 7401 7c00 8302 6a02 8300 0100 7c04 7228  t.|...j.....|.r(
-00000250: 7403 6a01 7c01 7c04 6401 6401 6402 8d04  t.j.|.|.d.d.d...
-00000260: 7c00 5f03 6e28 7c02 7248 7c03 7248 7403  |._.n(|.rH|.rHt.
-00000270: 6a01 7c01 7c02 7c03 6401 6401 6403 8d05  j.|.|.|.d.d.d...
-00000280: 7c00 5f03 6e08 7404 6404 8301 8201 6405  |._.n.t.d.....d.
-00000290: 7c00 6a03 5f05 6401 5300 2906 612e 0200  |.j._.d.S.).a...
-000002a0: 000a 2020 2020 2020 2020 436c 6173 7320  ..        Class 
-000002b0: 636f 6e73 7472 7563 746f 722e 0a0a 2020  constructor...  
-000002c0: 2020 2020 2020 4974 2069 6e69 7469 616c        It initial
-000002d0: 697a 6573 2062 7567 7a69 6c6c 6120 7365  izes bugzilla se
-000002e0: 7373 696f 6e20 7573 696e 6720 7468 6520  ssion using the 
-000002f0: 7072 6f76 6964 6564 2063 7265 6465 6e74  provided credent
-00000300: 6961 6c73 2e0a 2020 2020 2020 2020 4966  ials..        If
-00000310: 2074 6865 2060 6170 695f 6b65 7960 2069   the `api_key` i
-00000320: 7320 6e6f 7420 7072 6f76 6964 6564 2c20  s not provided, 
-00000330: 6974 2077 696c 6c20 7472 7920 746f 2065  it will try to e
-00000340: 7374 6162 6c69 7368 2061 2073 6573 7369  stablish a sessi
-00000350: 6f6e 0a20 2020 2020 2020 2075 7369 6e67  on.        using
-00000360: 2060 7573 6572 6e61 6d65 6020 616e 6420   `username` and 
-00000370: 6070 6173 7377 6f72 6460 2e0a 0a20 2020  `password`...   
-00000380: 2020 2020 2050 6172 616d 733a 0a20 2020       Params:.   
-00000390: 2020 2020 2020 2020 2073 6572 7665 725f           server_
-000003a0: 7572 6c3a 2055 524c 206f 6620 7468 6520  url: URL of the 
-000003b0: 6275 677a 696c 6c61 2073 6572 7665 720a  bugzilla server.
-000003c0: 2020 2020 2020 2020 2020 2020 7573 6572              user
-000003d0: 6e61 6d65 3a20 5573 6572 6e61 6d65 2074  name: Username t
-000003e0: 6f20 7573 6520 666f 7220 6175 7468 656e  o use for authen
-000003f0: 7469 6361 7469 6f6e 0a20 2020 2020 2020  tication.       
-00000400: 2020 2020 2070 6173 7377 6f72 643a 2050       password: P
-00000410: 6173 7377 6f72 6420 746f 2075 7365 2066  assword to use f
-00000420: 6f72 2061 7574 6865 6e74 6963 6174 696f  or authenticatio
-00000430: 6e0a 2020 2020 2020 2020 2020 2020 6170  n.            ap
-00000440: 695f 6b65 793a 2041 5049 206b 6579 2074  i_key: API key t
-00000450: 6f20 7573 6520 666f 7220 6175 7468 656e  o use for authen
-00000460: 7469 6361 7469 6f6e 0a0a 2020 2020 2020  tication..      
-00000470: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00000480: 2020 2020 2020 5061 7463 6865 7245 7863        PatcherExc
-00000490: 6570 7469 6f6e 3a20 5768 656e 2074 6865  eption: When the
-000004a0: 2062 7567 7a69 6c6c 6120 7365 7373 696f   bugzilla sessio
-000004b0: 6e20 6361 6e27 7420 6265 2065 7374 6162  n can't be estab
-000004c0: 6c69 7368 6564 0a20 2020 2020 2020 204e  lished.        N
-000004d0: 2904 da03 7572 6c72 0b00 0000 da0a 636f  )...urlr......co
-000004e0: 6f6b 6965 6669 6c65 da09 746f 6b65 6e66  okiefile..tokenf
-000004f0: 696c 6529 0572 0d00 0000 da04 7573 6572  ile).r......user
-00000500: 720a 0000 0072 0e00 0000 720f 0000 007a  r....r....r....z
-00000510: 5641 7574 6865 6e74 6963 6174 696f 6e20  VAuthentication 
-00000520: 696e 666f 206e 6f74 2070 726f 7669 6465  info not provide
-00000530: 6421 2050 726f 7669 6465 2065 6974 6865  d! Provide eithe
-00000540: 7220 2775 7365 726e 616d 6527 2061 6e64  r 'username' and
-00000550: 2027 7061 7373 776f 7264 2720 6f72 2041   'password' or A
-00000560: 5049 206b 6579 2e54 2906 da05 7375 7065  PI key.T)...supe
-00000570: 7272 0700 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
-00000580: da08 6275 677a 696c 6c61 7203 0000 00da  ..bugzillar.....
-00000590: 0f62 7567 5f61 7574 6f72 6566 7265 7368  .bug_autorefresh
-000005a0: 2905 da04 7365 6c66 7208 0000 0072 0900  )...selfr....r..
-000005b0: 0000 720a 0000 0072 0b00 0000 2901 da09  ..r....r....)...
-000005c0: 5f5f 636c 6173 735f 5fa9 00fa 412f 7661  __class__...A/va
-000005d0: 722f 686f 6d65 2f7a 6c6f 7065 7a2f 6769  r/home/zlopez/gi
-000005e0: 742f 7468 652d 6e65 772d 686f 746e 6573  t/the-new-hotnes
-000005f0: 732f 686f 746e 6573 732f 7061 7463 6865  s/hotness/patche
-00000600: 7273 2f62 7567 7a69 6c6c 612e 7079 7212  rs/bugzilla.pyr.
-00000610: 0000 0029 0000 0073 1c00 0000 0017 0e01  ...)...s........
-00000620: 0401 0401 1202 0801 0401 0201 0201 0201  ................
-00000630: 0201 0c03 0201 0603 7a11 4275 677a 696c  ........z.Bugzil
-00000640: 6c61 2e5f 5f69 6e69 745f 5f29 04da 0770  la.__init__)...p
-00000650: 6163 6b61 6765 da05 7061 7463 68da 046f  ackage..patch..o
-00000660: 7074 7372 0c00 0000 6304 0000 0000 0000  ptsr....c.......
-00000670: 000b 0000 0014 0000 0043 0000 0073 c200  .........C...s..
-00000680: 0000 6900 7d04 7c03 6a00 6401 6402 8302  ..i.}.|.j.d.d...
-00000690: 7d05 7c03 6a00 6403 6404 8302 7d06 7c05  }.|.j.d.d...}.|.
-000006a0: 6402 6b02 732a 7c06 0c00 7232 7401 6405  d.k.s*|...r2t.d.
-000006b0: 8301 8201 7402 6406 6407 6408 8d02 8f72  ....t.d.d.d....r
-000006c0: 7d07 7403 6a04 6a05 7c07 7c06 8302 7d08  }.t.j.j.|.|...}.
-000006d0: 7406 7c08 6409 8302 8f10 7d09 7c09 6a07  t.|.d.....}.|.j.
-000006e0: 7c02 8301 0100 5700 640a 5100 5200 5800  |.....W.d.Q.R.X.
-000006f0: 7408 6a09 640b 7c05 1600 8301 0100 640c  t.j.d.|.......d.
-00000700: 6a0a 7c01 6a0b 7c05 8302 7d0a 7c00 6a0c  j.|.j.|...}.|.j.
-00000710: 6a0d 7c05 7c08 7c0a 640d 640e 8d04 0100  j.|.|.|.d.d.....
-00000720: 7408 6a0e 640f 7c05 1600 8301 0100 5700  t.j.d.|.......W.
-00000730: 640a 5100 5200 5800 7c05 7c04 6401 3c00  d.Q.R.X.|.|.d.<.
-00000740: 7c04 5300 2910 610c 0300 000a 2020 2020  |.S.).a.....    
-00000750: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-00000760: 6973 2069 6e68 6572 6974 6564 2066 726f  is inherited fro
-00000770: 6d20 6068 6f74 6e65 7373 2e70 6174 6368  m `hotness.patch
-00000780: 6572 732e 5061 7463 6865 7260 2e0a 0a20  ers.Patcher`... 
-00000790: 2020 2020 2020 2049 7420 6174 7461 6368         It attach
-000007a0: 6573 2066 696c 6520 746f 2065 7869 7374  es file to exist
-000007b0: 696e 6720 7469 636b 6574 2069 6e20 6275  ing ticket in bu
-000007c0: 677a 696c 6c61 2e0a 0a20 2020 2020 2020  gzilla...       
-000007d0: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
-000007e0: 2020 2020 2070 6163 6b61 6765 3a20 5061       package: Pa
-000007f0: 636b 6167 6520 746f 2063 7265 6174 6520  ckage to create 
-00000800: 6e6f 7469 6669 6361 7469 6f6e 2066 6f72  notification for
-00000810: 0a20 2020 2020 2020 2020 2020 2070 6174  .            pat
-00000820: 6368 3a20 5061 7463 6820 746f 2061 7474  ch: Patch to att
-00000830: 6163 682c 2069 7420 6e65 6564 7320 746f  ach, it needs to
-00000840: 2062 6520 636f 6e76 6572 7465 6420 746f   be converted to
-00000850: 2066 696c 6520 6669 7273 740a 2020 2020   file first.    
-00000860: 2020 2020 2020 2020 6f70 7473 3a20 4164          opts: Ad
-00000870: 6469 7469 6f6e 616c 206f 7074 696f 6e73  ditional options
-00000880: 2066 6f72 2062 7567 7a69 6c6c 612e 2045   for bugzilla. E
-00000890: 7861 6d70 6c65 3a0a 2020 2020 2020 2020  xample:.        
-000008a0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2262                "b
-000008c0: 7a5f 6964 223a 2031 3030 2c20 2320 4275  z_id": 100, # Bu
-000008d0: 677a 696c 6c61 2074 6963 6b65 7420 6964  gzilla ticket id
-000008e0: 2c20 6966 2070 726f 7669 6465 6420 7468  , if provided th
-000008f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000910: 2020 2020 2320 6e65 7720 6d65 7373 6167      # new messag
-00000920: 6520 7769 6c6c 2062 6520 6164 6465 6420  e will be added 
-00000930: 6173 206e 6577 2063 6f6d 6d65 6e74 2074  as new comment t
-00000940: 6f20 7468 6973 2074 6963 6b65 740a 2020  o this ticket.  
-00000950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000960: 2020 2270 6174 6368 5f66 696c 656e 616d    "patch_filenam
-00000970: 6522 3a20 2270 6174 6368 2220 2320 4e61  e": "patch" # Na
-00000980: 6d65 206f 6620 7468 6520 6669 6c65 2c20  me of the file, 
-00000990: 7468 6174 2073 686f 756c 6420 6265 2061  that should be a
-000009a0: 7474 6163 6865 640a 2020 2020 2020 2020  ttached.        
-000009b0: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
-000009c0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000009d0: 2020 2020 2020 2020 4469 6374 696f 6e61          Dictiona
-000009e0: 7279 2063 6f6e 7461 696e 696e 6720 7469  ry containing ti
-000009f0: 636b 6574 2062 7567 7a69 6c6c 6120 6964  cket bugzilla id
-00000a00: 0a20 2020 2020 2020 2020 2020 2045 7861  .            Exa
-00000a10: 6d70 6c65 3a0a 2020 2020 2020 2020 2020  mple:.          
-00000a20: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00000a30: 2020 2020 2262 7a5f 6964 223a 2031 3030      "bz_id": 100
-00000a40: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-00000a50: 2020 2020 2020 20da 0562 7a5f 6964 7201         ..bz_idr.
-00000a60: 0000 00da 0e70 6174 6368 5f66 696c 656e  .....patch_filen
-00000a70: 616d 65da 007a 4f41 6464 6974 696f 6e61  ame..zOAdditiona
-00000a80: 6c20 7061 7261 6d65 7465 7273 2061 7265  l parameters are
-00000a90: 206d 6973 7369 6e67 2120 506c 6561 7365   missing! Please
-00000aa0: 2070 726f 7669 6465 2060 627a 5f69 6460   provide `bz_id`
-00000ab0: 2061 6e64 2060 7061 7463 685f 6669 6c65   and `patch_file
-00000ac0: 6e61 6d65 602e 7a04 7468 6e2d 7a08 2f76  name`.z.thn-z./v
-00000ad0: 6172 2f74 6d70 2902 da06 7072 6566 6978  ar/tmp)...prefix
-00000ae0: da03 6469 72da 0177 4e7a 1841 7474 6163  ..dir..wNz.Attac
-00000af0: 6869 6e67 2066 696c 6520 746f 2062 7567  hing file to bug
-00000b00: 2025 727a 1255 7064 6174 6520 746f 207b   %rz.Update to {
-00000b10: 7d20 2823 7b7d 2954 2901 da08 6973 5f70  } (#{})T)...is_p
-00000b20: 6174 6368 7a18 4174 7461 6368 6564 2066  atchz.Attached f
-00000b30: 696c 6520 746f 2062 7567 3a20 2572 290f  ile to bug: %r).
-00000b40: da03 6765 7472 0300 0000 7202 0000 00da  ..getr....r.....
-00000b50: 026f 73da 0470 6174 68da 046a 6f69 6eda  .os..path..join.
-00000b60: 046f 7065 6eda 0577 7269 7465 da07 5f6c  .open..write.._l
-00000b70: 6f67 6765 72da 0564 6562 7567 da06 666f  ogger..debug..fo
-00000b80: 726d 6174 da07 7665 7273 696f 6e72 1300  rmat..versionr..
-00000b90: 0000 da0a 6174 7461 6368 6669 6c65 da04  ....attachfile..
-00000ba0: 696e 666f 290b 7215 0000 0072 1900 0000  info).r....r....
-00000bb0: 721a 0000 0072 1b00 0000 da06 6f75 7470  r....r......outp
-00000bc0: 7574 da06 6275 675f 6964 da08 6669 6c65  ut..bug_id..file
-00000bd0: 6e61 6d65 da03 746d 70da 0866 696c 6570  name..tmp..filep
-00000be0: 6174 68da 0166 da0b 6465 7363 7269 7074  ath..f..descript
-00000bf0: 696f 6e72 1700 0000 7217 0000 0072 1800  ionr....r....r..
-00000c00: 0000 da0c 7375 626d 6974 5f70 6174 6368  ....submit_patch
-00000c10: 5400 0000 7320 0000 0000 1704 010c 010c  T...s ..........
-00000c20: 010e 0102 0106 070e 010e 010c 0114 020e  ................
-00000c30: 010e 0114 0118 0208 017a 1542 7567 7a69  .........z.Bugzi
-00000c40: 6c6c 612e 7375 626d 6974 5f70 6174 6368  lla.submit_patch
-00000c50: 290a da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000c60: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000c70: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fda  name__..__doc__.
-00000c80: 0373 7472 7212 0000 0072 0400 0000 da04  .strr....r......
-00000c90: 6469 6374 7236 0000 00da 0d5f 5f63 6c61  dictr6.....__cla
-00000ca0: 7373 6365 6c6c 5f5f 7217 0000 0072 1700  sscell__r....r..
-00000cb0: 0000 2901 7216 0000 0072 1800 0000 7207  ..).r....r....r.
-00000cc0: 0000 0020 0000 0073 0e00 0000 0807 0404  ... ...s........
-00000cd0: 0201 0201 0201 0201 1225 7207 0000 0029  .........%r....)
-00000ce0: 0fda 076c 6f67 6769 6e67 7224 0000 00da  ...loggingr$....
-00000cf0: 0874 656d 7066 696c 6572 0200 0000 7213  .tempfiler....r.
-00000d00: 0000 00da 1268 6f74 6e65 7373 2e65 7863  .....hotness.exc
-00000d10: 6570 7469 6f6e 7372 0300 0000 5a16 686f  eptionsr....Z.ho
-00000d20: 746e 6573 732e 646f 6d61 696e 2e70 6163  tness.domain.pac
-00000d30: 6b61 6765 7204 0000 00da 0770 6174 6368  kager......patch
-00000d40: 6572 7206 0000 00da 0967 6574 4c6f 6767  err......getLogg
-00000d50: 6572 7237 0000 0072 2900 0000 7207 0000  err7...r)...r...
-00000d60: 0072 1700 0000 7217 0000 0072 1700 0000  .r....r....r....
-00000d70: 7218 0000 00da 083c 6d6f 6475 6c65 3e12  r......<module>.
-00000d80: 0000 0073 1000 0000 0801 0801 0c02 0802  ...s............
-00000d90: 0c01 0c01 0c03 0a03                      ........
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 436f 7079  f-8 -*-.#.# Copy
+00000020: 7269 6768 7420 2843 2920 3230 3231 2052  right (C) 2021 R
+00000030: 6564 2048 6174 2c20 496e 632e 0a23 0a23  ed Hat, Inc..#.#
+00000040: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000050: 2066 7265 6520 736f 6674 7761 7265 3b20   free software; 
+00000060: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000070: 6275 7465 2069 7420 616e 642f 6f72 0a23  bute it and/or.#
+00000080: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+00000090: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+000000a0: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+000000b0: 626c 6963 204c 6963 656e 7365 0a23 2061  blic License.# a
+000000c0: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
+000000d0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
+000000e0: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
+000000f0: 6865 7220 7665 7273 696f 6e20 320a 2320  her version 2.# 
+00000100: 6f66 2074 6865 204c 6963 656e 7365 2c20  of the License, 
+00000110: 6f72 2028 6174 2079 6f75 7220 6f70 7469  or (at your opti
+00000120: 6f6e 2920 616e 7920 6c61 7465 7220 7665  on) any later ve
+00000130: 7273 696f 6e2e 0a23 0a23 2054 6869 7320  rsion..#.# This 
+00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+00000170: 6265 2075 7365 6675 6c2c 0a23 2062 7574  be useful,.# but
+00000180: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+00000190: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+000001a0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+000001b0: 7761 7272 616e 7479 206f 660a 2320 4d45  warranty of.# ME
+000001c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000001d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000001e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000001f0: 452e 2020 5365 6520 7468 650a 2320 474e  E.  See the.# GN
+00000200: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000210: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
+00000220: 6520 6465 7461 696c 732e 0a23 0a23 2059  e details..#.# Y
+00000230: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000240: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+00000250: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 0a23 2061 6c6f 6e67 2077 6974 6820 7468  .# along with th
+00000280: 6973 2070 726f 6772 616d 3b20 6966 206e  is program; if n
+00000290: 6f74 2c20 7772 6974 6520 746f 2074 6865  ot, write to the
+000002a0: 2046 7265 6520 536f 6674 7761 7265 0a23   Free Software.#
+000002b0: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
+000002c0: 2e2c 2035 3120 4672 616e 6b6c 696e 2053  ., 51 Franklin S
+000002d0: 7472 6565 742c 2046 6966 7468 2046 6c6f  treet, Fifth Flo
+000002e0: 6f72 2c20 426f 7374 6f6e 2c20 4d41 2020  or, Boston, MA  
+000002f0: 3032 3131 302d 3133 3031 2c20 5553 412e  02110-1301, USA.
+00000300: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
+00000310: 696d 706f 7274 206f 730a 6672 6f6d 2074  import os.from t
+00000320: 656d 7066 696c 6520 696d 706f 7274 2054  empfile import T
+00000330: 656d 706f 7261 7279 4469 7265 6374 6f72  emporaryDirector
+00000340: 790a 0a69 6d70 6f72 7420 6275 677a 696c  y..import bugzil
+00000350: 6c61 2020 2320 7479 7065 3a20 6967 6e6f  la  # type: igno
+00000360: 7265 0a0a 6672 6f6d 2068 6f74 6e65 7373  re..from hotness
+00000370: 2e65 7863 6570 7469 6f6e 7320 696d 706f  .exceptions impo
+00000380: 7274 2050 6174 6368 6572 4578 6365 7074  rt PatcherExcept
+00000390: 696f 6e0a 6672 6f6d 2068 6f74 6e65 7373  ion.from hotness
+000003a0: 2e64 6f6d 6169 6e2e 7061 636b 6167 6520  .domain.package 
+000003b0: 696d 706f 7274 2050 6163 6b61 6765 0a66  import Package.f
+000003c0: 726f 6d20 2e70 6174 6368 6572 2069 6d70  rom .patcher imp
+000003d0: 6f72 7420 5061 7463 6865 720a 0a0a 5f6c  ort Patcher..._l
+000003e0: 6f67 6765 7220 3d20 6c6f 6767 696e 672e  ogger = logging.
+000003f0: 6765 744c 6f67 6765 7228 5f5f 6e61 6d65  getLogger(__name
+00000400: 5f5f 290a 0a0a 636c 6173 7320 4275 677a  __)...class Bugz
+00000410: 696c 6c61 2850 6174 6368 6572 293a 0a20  illa(Patcher):. 
+00000420: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
+00000430: 636c 6173 7320 6973 2061 2077 7261 7070  class is a wrapp
+00000440: 6572 2066 6f72 2068 7474 7073 3a2f 2f62  er for https://b
+00000450: 7567 7a69 6c6c 612e 7265 6468 6174 2e63  ugzilla.redhat.c
+00000460: 6f6d 2f0a 2020 2020 4974 2073 7562 6d69  om/.    It submi
+00000470: 7420 7061 7463 6865 7320 746f 2042 7567  t patches to Bug
+00000480: 7a69 6c6c 612e 0a0a 2020 2020 4174 7472  zilla...    Attr
+00000490: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+000004a0: 6275 677a 696c 6c61 2028 6275 677a 696c  bugzilla (bugzil
+000004b0: 6c61 2e42 7567 7a69 6c6c 6129 3a20 4275  la.Bugzilla): Bu
+000004c0: 677a 696c 6c61 2073 6573 7369 6f6e 0a20  gzilla session. 
+000004d0: 2020 2022 2222 0a0a 2020 2020 6465 6620     """..    def 
+000004e0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+000004f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00000500: 7365 7276 6572 5f75 726c 3a20 7374 722c  server_url: str,
+00000510: 0a20 2020 2020 2020 2061 7069 5f6b 6579  .        api_key
+00000520: 3a20 7374 722c 0a20 2020 2029 202d 3e20  : str,.    ) -> 
+00000530: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00000540: 220a 2020 2020 2020 2020 436c 6173 7320  ".        Class 
+00000550: 636f 6e73 7472 7563 746f 722e 0a0a 2020  constructor...  
+00000560: 2020 2020 2020 4974 2069 6e69 7469 616c        It initial
+00000570: 697a 6573 2062 7567 7a69 6c6c 6120 7365  izes bugzilla se
+00000580: 7373 696f 6e20 7573 696e 6720 7468 6520  ssion using the 
+00000590: 7072 6f76 6964 6564 2063 7265 6465 6e74  provided credent
+000005a0: 6961 6c73 2e0a 2020 2020 2020 2020 4966  ials..        If
+000005b0: 2074 6865 2060 6170 695f 6b65 7960 2069   the `api_key` i
+000005c0: 7320 6e6f 7420 7072 6f76 6964 6564 2069  s not provided i
+000005d0: 7420 7261 6973 6573 2061 6e20 6050 6174  t raises an `Pat
+000005e0: 6368 6572 4578 6365 7074 696f 6e60 2e0a  cherException`..
+000005f0: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
+00000600: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00000610: 7665 725f 7572 6c3a 2055 524c 206f 6620  ver_url: URL of 
+00000620: 7468 6520 6275 677a 696c 6c61 2073 6572  the bugzilla ser
+00000630: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+00000640: 6170 695f 6b65 793a 2041 5049 206b 6579  api_key: API key
+00000650: 2074 6f20 7573 6520 666f 7220 6175 7468   to use for auth
+00000660: 656e 7469 6361 7469 6f6e 0a0a 2020 2020  entication..    
+00000670: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00000680: 2020 2020 2020 2020 5061 7463 6865 7245          PatcherE
+00000690: 7863 6570 7469 6f6e 3a20 5768 656e 2074  xception: When t
+000006a0: 6865 2062 7567 7a69 6c6c 6120 7365 7373  he bugzilla sess
+000006b0: 696f 6e20 6361 6e27 7420 6265 2065 7374  ion can't be est
+000006c0: 6162 6c69 7368 6564 0a20 2020 2020 2020  ablished.       
+000006d0: 2022 2222 0a20 2020 2020 2020 2073 7570   """.        sup
+000006e0: 6572 2842 7567 7a69 6c6c 612c 2073 656c  er(Bugzilla, sel
+000006f0: 6629 2e5f 5f69 6e69 745f 5f28 290a 2020  f).__init__().  
+00000700: 2020 2020 2020 6966 2061 7069 5f6b 6579        if api_key
+00000710: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00000720: 6c66 2e62 7567 7a69 6c6c 6120 3d20 6275  lf.bugzilla = bu
+00000730: 677a 696c 6c61 2e42 7567 7a69 6c6c 6128  gzilla.Bugzilla(
+00000740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000750: 2075 726c 3d73 6572 7665 725f 7572 6c2c   url=server_url,
+00000760: 2061 7069 5f6b 6579 3d61 7069 5f6b 6579   api_key=api_key
+00000770: 2c20 636f 6f6b 6965 6669 6c65 3d4e 6f6e  , cookiefile=Non
+00000780: 652c 2074 6f6b 656e 6669 6c65 3d4e 6f6e  e, tokenfile=Non
+00000790: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+000007a0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000007b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000007c0: 5061 7463 6865 7245 7863 6570 7469 6f6e  PatcherException
+000007d0: 2822 4175 7468 656e 7469 6361 7469 6f6e  ("Authentication
+000007e0: 2069 6e66 6f20 6e6f 7420 7072 6f76 6964   info not provid
+000007f0: 6564 2120 5072 6f76 6964 6520 4150 4920  ed! Provide API 
+00000800: 6b65 792e 2229 0a20 2020 2020 2020 2073  key.").        s
+00000810: 656c 662e 6275 677a 696c 6c61 2e62 7567  elf.bugzilla.bug
+00000820: 5f61 7574 6f72 6566 7265 7368 203d 2054  _autorefresh = T
+00000830: 7275 650a 0a20 2020 2064 6566 2073 7562  rue..    def sub
+00000840: 6d69 745f 7061 7463 6828 7365 6c66 2c20  mit_patch(self, 
+00000850: 7061 636b 6167 653a 2050 6163 6b61 6765  package: Package
+00000860: 2c20 7061 7463 683a 2073 7472 2c20 6f70  , patch: str, op
+00000870: 7473 3a20 6469 6374 2920 2d3e 2064 6963  ts: dict) -> dic
+00000880: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+00000890: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
+000008a0: 6f64 2069 7320 696e 6865 7269 7465 6420  od is inherited 
+000008b0: 6672 6f6d 2060 686f 746e 6573 732e 7061  from `hotness.pa
+000008c0: 7463 6865 7273 2e50 6174 6368 6572 602e  tchers.Patcher`.
+000008d0: 0a0a 2020 2020 2020 2020 4974 2061 7474  ..        It att
+000008e0: 6163 6865 7320 6669 6c65 2074 6f20 6578  aches file to ex
+000008f0: 6973 7469 6e67 2074 6963 6b65 7420 696e  isting ticket in
+00000900: 2062 7567 7a69 6c6c 612e 0a0a 2020 2020   bugzilla...    
+00000910: 2020 2020 5061 7261 6d73 3a0a 2020 2020      Params:.    
+00000920: 2020 2020 2020 2020 7061 636b 6167 653a          package:
+00000930: 2050 6163 6b61 6765 2074 6f20 6372 6561   Package to crea
+00000940: 7465 206e 6f74 6966 6963 6174 696f 6e20  te notification 
+00000950: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+00000960: 7061 7463 683a 2050 6174 6368 2074 6f20  patch: Patch to 
+00000970: 6174 7461 6368 2c20 6974 206e 6565 6473  attach, it needs
+00000980: 2074 6f20 6265 2063 6f6e 7665 7274 6564   to be converted
+00000990: 2074 6f20 6669 6c65 2066 6972 7374 0a20   to file first. 
+000009a0: 2020 2020 2020 2020 2020 206f 7074 733a             opts:
+000009b0: 2041 6464 6974 696f 6e61 6c20 6f70 7469   Additional opti
+000009c0: 6f6e 7320 666f 7220 6275 677a 696c 6c61  ons for bugzilla
+000009d0: 2e20 4578 616d 706c 653a 0a20 2020 2020  . Example:.     
+000009e0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a00: 2022 627a 5f69 6422 3a20 3130 302c 2023   "bz_id": 100, #
+00000a10: 2042 7567 7a69 6c6c 6120 7469 636b 6574   Bugzilla ticket
+00000a20: 2069 642c 2069 6620 7072 6f76 6964 6564   id, if provided
+00000a30: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00000a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a50: 2020 2020 2020 2023 206e 6577 206d 6573         # new mes
+00000a60: 7361 6765 2077 696c 6c20 6265 2061 6464  sage will be add
+00000a70: 6564 2061 7320 6e65 7720 636f 6d6d 656e  ed as new commen
+00000a80: 7420 746f 2074 6869 7320 7469 636b 6574  t to this ticket
+00000a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000aa0: 2020 2020 2022 7061 7463 685f 6669 6c65       "patch_file
+00000ab0: 6e61 6d65 223a 2022 7061 7463 6822 2023  name": "patch" #
+00000ac0: 204e 616d 6520 6f66 2074 6865 2066 696c   Name of the fil
+00000ad0: 652c 2074 6861 7420 7368 6f75 6c64 2062  e, that should b
+00000ae0: 6520 6174 7461 6368 6564 0a20 2020 2020  e attached.     
+00000af0: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
+00000b00: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00000b10: 2020 2020 2020 2020 2020 2044 6963 7469             Dicti
+00000b20: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00000b30: 2074 6963 6b65 7420 6275 677a 696c 6c61   ticket bugzilla
+00000b40: 2069 640a 2020 2020 2020 2020 2020 2020   id.            
+00000b50: 4578 616d 706c 653a 0a20 2020 2020 2020  Example:.       
+00000b60: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00000b70: 2020 2020 2020 2022 627a 5f69 6422 3a20         "bz_id": 
+00000b80: 3130 300a 2020 2020 2020 2020 2020 2020  100.            
+00000b90: 7d0a 2020 2020 2020 2020 2222 220a 2020  }.        """.  
+00000ba0: 2020 2020 2020 6f75 7470 7574 203d 207b        output = {
+00000bb0: 7d0a 2020 2020 2020 2020 6275 675f 6964  }.        bug_id
+00000bc0: 203d 206f 7074 732e 6765 7428 2262 7a5f   = opts.get("bz_
+00000bd0: 6964 222c 2030 290a 2020 2020 2020 2020  id", 0).        
+00000be0: 6669 6c65 6e61 6d65 203d 206f 7074 732e  filename = opts.
+00000bf0: 6765 7428 2270 6174 6368 5f66 696c 656e  get("patch_filen
+00000c00: 616d 6522 2c20 2222 290a 2020 2020 2020  ame", "").      
+00000c10: 2020 6966 2062 7567 5f69 6420 3d3d 2030    if bug_id == 0
+00000c20: 206f 7220 6e6f 7420 6669 6c65 6e61 6d65   or not filename
+00000c30: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00000c40: 6973 6520 5061 7463 6865 7245 7863 6570  ise PatcherExcep
+00000c50: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00000c60: 2020 2020 2020 2241 6464 6974 696f 6e61        "Additiona
+00000c70: 6c20 7061 7261 6d65 7465 7273 2061 7265  l parameters are
+00000c80: 206d 6973 7369 6e67 2120 220a 2020 2020   missing! ".    
+00000c90: 2020 2020 2020 2020 2020 2020 2250 6c65              "Ple
+00000ca0: 6173 6520 7072 6f76 6964 6520 6062 7a5f  ase provide `bz_
+00000cb0: 6964 6020 616e 6420 6070 6174 6368 5f66  id` and `patch_f
+00000cc0: 696c 656e 616d 6560 2e22 0a20 2020 2020  ilename`.".     
+00000cd0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00000ce0: 2020 2320 5772 6974 6520 6669 6c65 2074    # Write file t
+00000cf0: 6f20 7465 6d70 6f72 6172 7920 6469 7265  o temporary dire
+00000d00: 6374 6f72 790a 2020 2020 2020 2020 2320  ctory.        # 
+00000d10: 616e 6420 7374 6f70 2062 616e 6469 7420  and stop bandit 
+00000d20: 6672 6f6d 2063 6f6d 706c 6169 6e69 6e67  from complaining
+00000d30: 2061 626f 7574 2061 2068 6172 6463 6f64   about a hardcod
+00000d40: 6564 2074 656d 706f 7261 7279 2064 6972  ed temporary dir
+00000d50: 6563 746f 7279 0a20 2020 2020 2020 2023  ectory.        #
+00000d60: 2062 6563 6175 7365 2069 7427 7320 6e65   because it's ne
+00000d70: 6564 6564 2066 6f72 204f 7065 6e53 6869  eded for OpenShi
+00000d80: 6674 0a20 2020 2020 2020 2077 6974 6820  ft.        with 
+00000d90: 5465 6d70 6f72 6172 7944 6972 6563 746f  TemporaryDirecto
+00000da0: 7279 2870 7265 6669 783d 2274 686e 2d22  ry(prefix="thn-"
+00000db0: 2c20 6469 723d 222f 7661 722f 746d 7022  , dir="/var/tmp"
+00000dc0: 2920 6173 2074 6d70 3a20 2023 206e 6f73  ) as tmp:  # nos
+00000dd0: 6563 0a20 2020 2020 2020 2020 2020 2066  ec.            f
+00000de0: 696c 6570 6174 6820 3d20 6f73 2e70 6174  ilepath = os.pat
+00000df0: 682e 6a6f 696e 2874 6d70 2c20 6669 6c65  h.join(tmp, file
+00000e00: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
+00000e10: 2020 7769 7468 206f 7065 6e28 6669 6c65    with open(file
+00000e20: 7061 7468 2c20 2277 2229 2061 7320 663a  path, "w") as f:
+00000e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000e40: 2066 2e77 7269 7465 2870 6174 6368 290a   f.write(patch).
+00000e50: 0a20 2020 2020 2020 2020 2020 205f 6c6f  .            _lo
+00000e60: 6767 6572 2e64 6562 7567 2822 4174 7461  gger.debug("Atta
+00000e70: 6368 696e 6720 6669 6c65 2074 6f20 6275  ching file to bu
+00000e80: 6720 2572 2220 2520 6275 675f 6964 290a  g %r" % bug_id).
+00000e90: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00000ea0: 7269 7074 696f 6e20 3d20 2255 7064 6174  ription = "Updat
+00000eb0: 6520 746f 207b 7d20 2823 7b7d 2922 2e66  e to {} (#{})".f
+00000ec0: 6f72 6d61 7428 7061 636b 6167 652e 7665  ormat(package.ve
+00000ed0: 7273 696f 6e2c 2062 7567 5f69 6429 0a20  rsion, bug_id). 
+00000ee0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000ef0: 6275 677a 696c 6c61 2e61 7474 6163 6866  bugzilla.attachf
+00000f00: 696c 6528 6275 675f 6964 2c20 6669 6c65  ile(bug_id, file
+00000f10: 7061 7468 2c20 6465 7363 7269 7074 696f  path, descriptio
+00000f20: 6e2c 2069 735f 7061 7463 683d 5472 7565  n, is_patch=True
+00000f30: 290a 2020 2020 2020 2020 2020 2020 5f6c  ).            _l
+00000f40: 6f67 6765 722e 696e 666f 2822 4174 7461  ogger.info("Atta
+00000f50: 6368 6564 2066 696c 6520 746f 2062 7567  ched file to bug
+00000f60: 3a20 2572 2220 2520 6275 675f 6964 290a  : %r" % bug_id).
+00000f70: 0a20 2020 2020 2020 206f 7574 7075 745b  .        output[
+00000f80: 2262 7a5f 6964 225d 203d 2062 7567 5f69  "bz_id"] = bug_i
+00000f90: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00000fa0: 206f 7574 7075 740a                       output.
```

### Comparing `the_new_hotness-1.2.3/hotness/patchers/patcher.py` & `the_new_hotness-1.2.4/hotness/use_cases/submit_patch_use_case.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,32 +11,52 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-from hotness.domain.package import Package
+import logging
 
+from hotness.patchers import Patcher
+from hotness.requests import SubmitPatchRequest
+from hotness import responses
 
-class Patcher:
+
+logger = logging.getLogger(__name__)
+
+
+class SubmitPatchUseCase:
     """
-    Abstract class for patchers used by the-new-hotness to submit a patch.
-    This class must be inherited by every external patcher.
+    This class represents use case for submitting the patch to package with provided patcher.
+
+    Attributes:
+        patcher: Patcher to use.
     """
 
-    def submit_patch(self, package: Package, patch: str, opts: dict) -> dict:
+    def __init__(self, patcher: Patcher):
         """
-        Submit patch method that should be implemented by every child class.
-
-        It should submit patch for package to external system and
-        return dictionary containing additional info.
+        Class constructor.
+        """
+        self.patcher = patcher
 
-        In case of any issue that would prevent submitting the patch, method should
-        raise an exception.
+    def submit_patch(self, request: SubmitPatchRequest) -> responses.Response:
+        """
+        Call the submit_patch method on the patcher.
+        This method will handle any error that happens during submit of the patch.
 
         Params:
-            package: Package to attach patch for
-            patch: Patch to attach
-            opts: Optional arguments specific for the external patcher system
+            request: Request to handle.
+
+        Return:
+           Output of the build.
         """
-        raise NotImplementedError
+        if not request:
+            return responses.ResponseFailure.invalid_request_error(request)
+        try:
+            result = self.patcher.submit_patch(
+                request.package, request.patch, request.opts
+            )
+            return responses.ResponseSuccess(result)
+        except Exception as exc:
+            logger.exception("Submit patch use case failure", exc_info=True)
+            return responses.ResponseFailure.patcher_error(exc)
```

### Comparing `the_new_hotness-1.2.3/hotness/requests/__init__.py` & `the_new_hotness-1.2.4/hotness/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/build_request.py` & `the_new_hotness-1.2.4/hotness/requests/build_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/insert_data_request.py` & `the_new_hotness-1.2.4/hotness/requests/insert_data_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/notify_request.py` & `the_new_hotness-1.2.4/hotness/requests/notify_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/package_request.py` & `the_new_hotness-1.2.4/hotness/requests/package_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/request.py` & `the_new_hotness-1.2.4/hotness/requests/request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/retrieve_data_request.py` & `the_new_hotness-1.2.4/hotness/requests/retrieve_data_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/requests/submit_patch_request.py` & `the_new_hotness-1.2.4/hotness/requests/submit_patch_request.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/responses/__init__.py` & `the_new_hotness-1.2.4/hotness/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/responses/__pycache__/response_failure.cpython-36.pyc` & `the_new_hotness-1.2.4/hotness/responses/response_failure.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,360 +1,389 @@
-00000000: 330d 0d0a e503 9e61 2618 0000 e300 0000  3......a&.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 4c00 0000 6400 6401 6c00 5a00 6400  .sL...d.d.l.Z.d.
-00000030: 6402 6c01 6d02 5a02 0100 6400 6403 6c03  d.l.m.Z...d.d.l.
-00000040: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6405 6c07 6d08 5a08 0100 4700  ..d.d.l.m.Z...G.
-00000060: 6406 6407 8400 6407 6508 8303 5a09 6401  d.d...d.e...Z.d.
-00000070: 5300 2908 e900 0000 004e 2901 da03 416e  S.)......N)...An
-00000080: 7929 01da 1442 6173 6548 6f74 6e65 7373  y)...BaseHotness
-00000090: 4578 6365 7074 696f 6e29 01da 0752 6571  Exception)...Req
-000000a0: 7565 7374 2901 da08 5265 7370 6f6e 7365  uest)...Response
-000000b0: 6300 0000 0000 0000 0000 0000 0004 0000  c...............
-000000c0: 0040 0000 0073 fe00 0000 6500 5a01 6400  .@...s....e.Z.d.
-000000d0: 5a02 6401 5a03 6402 5a04 6403 5a05 6404  Z.d.Z.d.Z.d.Z.d.
-000000e0: 5a06 6405 5a07 6406 5a08 6407 5a09 650a  Z.d.Z.d.Z.d.Z.e.
-000000f0: 650b 6408 6409 9c03 640a 640b 8404 5a0c  e.d.d...d.d...Z.
-00000100: 650b 650d 640c 9c02 640d 640e 8404 5a0e  e.e.d...d.d...Z.
-00000110: 650b 650a 6701 640c 9c02 640f 6410 8404  e.e.g.d...d.d...
-00000120: 5a0f 650b 650b 640c 9c02 6411 6412 8404  Z.e.e.d...d.d...
-00000130: 5a10 6511 6413 6414 8400 8301 5a12 6513  Z.e.d.d.....Z.e.
-00000140: 6415 9c01 6416 6417 8404 5a14 6515 650b  d...d.d...Z.e.e.
-00000150: 6400 640c 9c02 6418 6419 8404 8301 5a16  d.d...d.d.....Z.
-00000160: 6515 650b 6400 640c 9c02 641a 641b 8404  e.e.d.d...d.d...
-00000170: 8301 5a17 6515 650b 6400 640c 9c02 641c  ..Z.e.e.d.d...d.
-00000180: 641d 8404 8301 5a18 6515 650b 6400 640c  d.....Z.e.e.d.d.
-00000190: 9c02 641e 641f 8404 8301 5a19 6515 650b  ..d.d.....Z.e.e.
-000001a0: 6400 640c 9c02 6420 6421 8404 8301 5a1a  d.d...d d!....Z.
-000001b0: 6515 651b 6400 6422 9c02 6423 6424 8404  e.e.d.d"..d#d$..
-000001c0: 8301 5a1c 6408 5300 2925 da0f 5265 7370  ..Z.d.S.)%..Resp
-000001d0: 6f6e 7365 4661 696c 7572 6561 8101 0000  onseFailurea....
-000001e0: 0a20 2020 2043 6c61 7373 2074 6861 7420  .    Class that 
-000001f0: 7265 7072 6573 656e 7473 2066 6169 6c75  represents failu
-00000200: 7265 2072 6573 706f 6e73 6520 7265 7475  re response retu
-00000210: 726e 6564 2066 726f 6d20 7573 6520 6361  rned from use ca
-00000220: 7365 2e0a 2020 2020 4974 2069 7320 7365  se..    It is se
-00000230: 6e64 2077 6865 6e20 736f 6d65 2065 7863  nd when some exc
-00000240: 6570 7469 6f6e 2068 6170 7065 6e20 6475  eption happen du
-00000250: 7269 6e67 2074 6865 2075 7365 2063 6173  ring the use cas
-00000260: 652e 0a20 2020 2044 6566 696e 6573 2063  e..    Defines c
-00000270: 6f6e 7374 616e 7473 2066 6f72 2065 7272  onstants for err
-00000280: 6f72 2074 7970 6573 2e0a 0a20 2020 2041  or types...    A
-00000290: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-000002a0: 2020 2074 7970 653a 2054 7970 6520 6f66     type: Type of
-000002b0: 2074 6865 2066 6169 6c75 7265 2e0a 2020   the failure..  
-000002c0: 2020 2020 2020 6d65 7373 6167 653a 2045        message: E
-000002d0: 7272 6f72 206d 6573 7361 6765 2e0a 2020  rror message..  
-000002e0: 2020 2020 2020 7472 6163 6562 6163 6b3a        traceback:
-000002f0: 2045 7863 6570 7469 6f6e 2074 7261 6365   Exception trace
-00000300: 6261 636b 2061 7320 7374 7269 6e67 2e0a  back as string..
-00000310: 2020 2020 2020 2020 7573 655f 6361 7365          use_case
-00000320: 5f76 616c 7565 3a20 5061 7274 6961 6c20  _value: Partial 
-00000330: 7573 6520 6361 7365 206f 7574 7075 7420  use case output 
-00000340: 6672 6f6d 2045 7863 6570 7469 6f6e 2c20  from Exception, 
-00000350: 6966 2070 726f 7669 6465 642e 0a20 2020  if provided..   
-00000360: 205a 0e56 616c 6964 6174 6f72 4572 726f   Z.ValidatorErro
-00000370: 725a 0c42 7569 6c64 6572 4572 726f 72da  rZ.BuilderError.
-00000380: 0d44 6174 6162 6173 6545 7272 6f72 5a0d  .DatabaseErrorZ.
-00000390: 4e6f 7469 6669 6572 4572 726f 725a 0c50  NotifierErrorZ.P
-000003a0: 6174 6368 6572 4572 726f 725a 1349 6e76  atcherErrorZ.Inv
-000003b0: 616c 6964 5265 7175 6573 7445 7272 6f72  alidRequestError
-000003c0: 4e29 03da 0474 7970 65da 076d 6573 7361  N)...type..messa
-000003d0: 6765 da06 7265 7475 726e 6303 0000 0000  ge..returnc.....
-000003e0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-000003f0: 2e00 0000 7c01 7c00 5f00 7c00 6a01 7c02  ....|.|._.|.j.|.
-00000400: 8301 7c00 5f02 7c00 6a03 7c02 8301 7c00  ..|._.|.j.|...|.
-00000410: 5f04 7c00 6a05 7c02 8301 7c00 5f06 6401  _.|.j.|...|._.d.
-00000420: 5300 2902 7a24 0a20 2020 2020 2020 2043  S.).z$.        C
-00000430: 6c61 7373 2063 6f6e 7374 7275 6374 6f72  lass constructor
-00000440: 2e0a 2020 2020 2020 2020 4e29 0772 0800  ..        N).r..
-00000450: 0000 da0f 5f66 6f72 6d61 745f 6d65 7373  ...._format_mess
-00000460: 6167 6572 0900 0000 da10 5f67 6574 5f73  ager......_get_s
-00000470: 7461 636b 5f74 7261 6365 da09 7472 6163  tack_trace..trac
-00000480: 6562 6163 6bda 0a5f 6765 745f 7661 6c75  eback.._get_valu
-00000490: 65da 0e75 7365 5f63 6173 655f 7661 6c75  e..use_case_valu
-000004a0: 6529 03da 0473 656c 6672 0800 0000 7209  e)...selfr....r.
-000004b0: 0000 00a9 0072 1100 0000 fa4a 2f76 6172  .....r.....J/var
-000004c0: 2f68 6f6d 652f 7a6c 6f70 657a 2f67 6974  /home/zlopez/git
-000004d0: 2f74 6865 2d6e 6577 2d68 6f74 6e65 7373  /the-new-hotness
-000004e0: 2f68 6f74 6e65 7373 2f72 6573 706f 6e73  /hotness/respons
-000004f0: 6573 2f72 6573 706f 6e73 655f 6661 696c  es/response_fail
-00000500: 7572 652e 7079 da08 5f5f 696e 6974 5f5f  ure.py..__init__
-00000510: 2e00 0000 7308 0000 0000 0406 010c 010c  ....s...........
-00000520: 017a 1852 6573 706f 6e73 6546 6169 6c75  .z.ResponseFailu
-00000530: 7265 2e5f 5f69 6e69 745f 5f29 0272 0900  re.__init__).r..
-00000540: 0000 720a 0000 0063 0200 0000 0000 0000  ..r....c........
-00000550: 0300 0000 0300 0000 4300 0000 7318 0000  ........C...s...
-00000560: 0064 017d 0274 007c 0174 0183 0272 147c  .d.}.t.|.t...r.|
-00000570: 016a 027d 027c 0253 0029 0261 0d01 0000  .j.}.|.S.).a....
-00000580: 0a20 2020 2020 2020 2052 6574 7269 6576  .        Retriev
-00000590: 6573 2074 6865 2075 7365 2063 6173 6520  es the use case 
-000005a0: 7661 6c75 6520 696e 666f 726d 6174 696f  value informatio
-000005b0: 6e20 6672 6f6d 2045 7863 6570 7469 6f6e  n from Exception
-000005c0: 2c0a 2020 2020 2020 2020 6f74 6865 7277  ,.        otherw
-000005d0: 6973 6520 6a75 7374 2072 6574 7572 6e73  ise just returns
-000005e0: 2065 6d70 7479 2064 6963 742e 0a0a 2020   empty dict...  
-000005f0: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
-00000600: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00000610: 653a 2049 6e70 7574 2074 6f20 7265 7472  e: Input to retr
-00000620: 6965 7665 2075 7365 2063 6173 6520 7661  ieve use case va
-00000630: 6c75 6520 6672 6f6d 0a0a 2020 2020 2020  lue from..      
-00000640: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00000650: 2020 2020 2020 2056 616c 7565 2069 6620         Value if 
-00000660: 6d65 7373 6167 6520 6973 2045 7863 6570  message is Excep
-00000670: 7469 6f6e 2c20 6f74 6865 7277 6973 6520  tion, otherwise 
-00000680: 4e6f 6e65 0a20 2020 2020 2020 204e 2903  None.        N).
-00000690: da0a 6973 696e 7374 616e 6365 7203 0000  ..isinstancer...
-000006a0: 00da 0576 616c 7565 2903 7210 0000 0072  ...value).r....r
-000006b0: 0900 0000 7215 0000 0072 1100 0000 7211  ....r....r....r.
-000006c0: 0000 0072 1200 0000 720e 0000 0037 0000  ...r....r....7..
-000006d0: 0073 0800 0000 000b 0402 0a01 0602 7a1a  .s............z.
-000006e0: 5265 7370 6f6e 7365 4661 696c 7572 652e  ResponseFailure.
-000006f0: 5f67 6574 5f76 616c 7565 6302 0000 0000  _get_valuec.....
-00000700: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00000710: 1e00 0000 6700 7d02 7400 7c01 7401 8302  ....g.}.t.|.t...
-00000720: 721a 7402 6a03 7c01 6a04 8301 7d02 7c02  r.t.j.|.j...}.|.
-00000730: 5300 2901 6115 0100 000a 2020 2020 2020  S.).a.....      
-00000740: 2020 5265 7472 6965 7665 7320 7468 6520    Retrieves the 
-00000750: 7374 6163 6b20 7472 6163 6520 696e 666f  stack trace info
-00000760: 726d 6174 696f 6e20 6672 6f6d 2045 7863  rmation from Exc
-00000770: 6570 7469 6f6e 2c0a 2020 2020 2020 2020  eption,.        
-00000780: 6f74 6865 7277 6973 6520 6a75 7374 2072  otherwise just r
-00000790: 6574 7572 6e73 2065 6d70 7479 206c 6973  eturns empty lis
-000007a0: 742e 0a0a 2020 2020 2020 2020 5061 7261  t...        Para
-000007b0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-000007c0: 6d65 7373 6167 653a 2049 6e70 7574 2074  message: Input t
-000007d0: 6f20 7265 7472 6965 7665 2073 7461 636b  o retrieve stack
-000007e0: 2074 7261 6365 2066 726f 6d0a 0a20 2020   trace from..   
-000007f0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00000800: 2020 2020 2020 2020 2020 5374 6163 6b20            Stack 
-00000810: 7472 6163 6520 6966 206d 6573 7361 6765  trace if message
-00000820: 2069 7320 4578 6365 7074 696f 6e2c 206f   is Exception, o
-00000830: 7468 6572 7769 7365 2065 6d70 7479 2073  therwise empty s
-00000840: 7472 696e 670a 2020 2020 2020 2020 2905  tring.        ).
-00000850: 7214 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00000860: 720d 0000 00da 0966 6f72 6d61 745f 7462  r......format_tb
-00000870: da0d 5f5f 7472 6163 6562 6163 6b5f 5f29  ..__traceback__)
-00000880: 0372 1000 0000 7209 0000 005a 0b73 7461  .r....r....Z.sta
-00000890: 636b 5f74 7261 6365 7211 0000 0072 1100  ck_tracer....r..
-000008a0: 0000 7212 0000 0072 0c00 0000 4900 0000  ..r....r....I...
-000008b0: 7308 0000 0000 0b04 020a 010c 027a 2052  s............z R
-000008c0: 6573 706f 6e73 6546 6169 6c75 7265 2e5f  esponseFailure._
-000008d0: 6765 745f 7374 6163 6b5f 7472 6163 6563  get_stack_tracec
-000008e0: 0200 0000 0000 0000 0200 0000 0400 0000  ................
-000008f0: 4300 0000 7324 0000 0074 007c 0174 0183  C...s$...t.|.t..
-00000900: 0272 2064 016a 027c 016a 036a 0464 026a  .r d.j.|.j.j.d.j
-00000910: 027c 0183 0183 0253 007c 0153 0029 0361  .|.....S.|.S.).a
-00000920: 1901 0000 0a20 2020 2020 2020 2046 6f72  .....        For
-00000930: 6d61 7473 2074 6865 2069 6e70 7574 206d  mats the input m
-00000940: 6573 7361 6765 2069 6620 7468 6520 6d65  essage if the me
-00000950: 7373 6167 6520 696e 6865 7269 7473 2066  ssage inherits f
-00000960: 726f 6d20 4578 6365 7074 696f 6e2c 0a20  rom Exception,. 
-00000970: 2020 2020 2020 206f 7468 6572 7769 7365         otherwise
-00000980: 206a 7573 7420 7265 7475 726e 2069 7420   just return it 
-00000990: 6261 636b 2e0a 0a20 2020 2020 2020 2050  back...        P
-000009a0: 6172 616d 733a 0a20 2020 2020 2020 2020  arams:.         
-000009b0: 2020 206d 6573 7361 6765 3a20 496e 7075     message: Inpu
-000009c0: 7420 6d65 7373 6167 6520 746f 2066 6f72  t message to for
-000009d0: 6d61 740a 0a20 2020 2020 2020 2052 6574  mat..        Ret
-000009e0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000009f0: 2020 5374 7269 6e67 2069 6620 6578 6365    String if exce
-00000a00: 7074 696f 6e2c 206f 7468 6572 7769 7365  ption, otherwise
-00000a10: 2072 6574 7572 6e20 7468 6520 7361 6d65   return the same
-00000a20: 206f 626a 6563 7420 7765 2072 6563 6569   object we recei
-00000a30: 7665 642e 0a20 2020 2020 2020 207a 067b  ved..        z.{
-00000a40: 7d3a 207b 7d7a 027b 7d29 0572 1400 0000  }: {}z.{}).r....
-00000a50: 7216 0000 00da 0666 6f72 6d61 74da 095f  r......format.._
-00000a60: 5f63 6c61 7373 5f5f da08 5f5f 6e61 6d65  _class__..__name
-00000a70: 5f5f 2902 7210 0000 0072 0900 0000 7211  __).r....r....r.
-00000a80: 0000 0072 1100 0000 7212 0000 0072 0b00  ...r....r....r..
-00000a90: 0000 5b00 0000 7306 0000 0000 0b0a 0116  ..[...s.........
-00000aa0: 027a 1f52 6573 706f 6e73 6546 6169 6c75  .z.ResponseFailu
-00000ab0: 7265 2e5f 666f 726d 6174 5f6d 6573 7361  re._format_messa
-00000ac0: 6765 6301 0000 0000 0000 0001 0000 0004  gec.............
-00000ad0: 0000 0043 0000 0073 1200 0000 7c00 6a00  ...C...s....|.j.
-00000ae0: 7c00 6a01 7c00 6a02 6401 9c03 5300 2902  |.j.|.j.d...S.).
-00000af0: 7a4a 0a20 2020 2020 2020 2052 6574 7572  zJ.        Retur
-00000b00: 6e73 2074 6865 2064 6963 7420 7265 7072  ns the dict repr
-00000b10: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00000b20: 6520 6661 696c 7572 6520 7265 7370 6f6e  e failure respon
-00000b30: 7365 2e0a 2020 2020 2020 2020 2903 7208  se..        ).r.
-00000b40: 0000 0072 0900 0000 720f 0000 0029 0372  ...r....r....).r
-00000b50: 0800 0000 7209 0000 0072 0f00 0000 2901  ....r....r....).
-00000b60: 7210 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000b70: 1200 0000 7215 0000 006b 0000 0073 0600  ....r....k...s..
-00000b80: 0000 0006 0401 0401 7a15 5265 7370 6f6e  ........z.Respon
-00000b90: 7365 4661 696c 7572 652e 7661 6c75 6529  seFailure.value)
-00000ba0: 0172 0a00 0000 6301 0000 0000 0000 0001  .r....c.........
-00000bb0: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00000bc0: 6401 5300 2902 7a35 0a20 2020 2020 2020  d.S.).z5.       
-00000bd0: 2042 6f6f 6c65 616e 2072 6570 7265 7365   Boolean represe
-00000be0: 6e74 6174 696f 6e20 6f66 2072 6573 706f  ntation of respo
-00000bf0: 6e73 652e 0a20 2020 2020 2020 2046 7211  nse..        Fr.
-00000c00: 0000 0029 0172 1000 0000 7211 0000 0072  ...).r....r....r
-00000c10: 1100 0000 7212 0000 00da 085f 5f62 6f6f  ....r......__boo
-00000c20: 6c5f 5f76 0000 0073 0200 0000 0004 7a18  l__v...s......z.
-00000c30: 5265 7370 6f6e 7365 4661 696c 7572 652e  ResponseFailure.
-00000c40: 5f5f 626f 6f6c 5f5f 6302 0000 0000 0000  __bool__c.......
-00000c50: 0003 0000 0004 0000 0043 0000 0073 1200  .........C...s..
-00000c60: 0000 7400 7400 6a01 7c01 6401 8d02 7d02  ..t.t.j.|.d...}.
-00000c70: 7c02 5300 2902 7ab1 0a20 2020 2020 2020  |.S.).z..       
-00000c80: 2043 7265 6174 6573 2072 6573 706f 6e73   Creates respons
-00000c90: 6520 666f 7220 7661 6c69 6461 746f 7220  e for validator 
-00000ca0: 6661 696c 7572 652e 0a0a 2020 2020 2020  failure...      
-00000cb0: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
-00000cc0: 2020 2020 2020 6d65 7373 6167 653a 204d        message: M
-00000cd0: 6573 7361 6765 2074 6f20 6164 6420 746f  essage to add to
-00000ce0: 2074 6869 7320 6572 726f 720a 0a20 2020   this error..   
-00000cf0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00000d00: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
-00000d10: 7365 4661 696c 7572 6520 6f62 6a65 6374  seFailure object
-00000d20: 0a20 2020 2020 2020 2029 0272 0800 0000  .        ).r....
-00000d30: 7209 0000 0029 0272 0600 0000 da0f 5641  r....).r......VA
-00000d40: 4c49 4441 544f 525f 4552 524f 5229 03da  LIDATOR_ERROR)..
-00000d50: 0363 6c73 7209 0000 00da 0872 6573 706f  .clsr......respo
-00000d60: 6e73 6572 1100 0000 7211 0000 0072 1200  nser....r....r..
-00000d70: 0000 da0f 7661 6c69 6461 746f 725f 6572  ....validator_er
-00000d80: 726f 727c 0000 0073 0600 0000 000b 0201  ror|...s........
-00000d90: 0c03 7a1f 5265 7370 6f6e 7365 4661 696c  ..z.ResponseFail
-00000da0: 7572 652e 7661 6c69 6461 746f 725f 6572  ure.validator_er
-00000db0: 726f 7263 0200 0000 0000 0000 0300 0000  rorc............
-00000dc0: 0400 0000 4300 0000 7312 0000 0074 0074  ....C...s....t.t
-00000dd0: 006a 017c 0164 018d 027d 027c 0253 0029  .j.|.d...}.|.S.)
-00000de0: 027a af0a 2020 2020 2020 2020 4372 6561  .z..        Crea
-00000df0: 7465 7320 7265 7370 6f6e 7365 2066 6f72  tes response for
-00000e00: 2062 7569 6c64 6572 2066 6169 6c75 7265   builder failure
-00000e10: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00000e20: 733a 0a20 2020 2020 2020 2020 2020 206d  s:.            m
-00000e30: 6573 7361 6765 3a20 4d65 7373 6167 6520  essage: Message 
-00000e40: 746f 2061 6464 2074 6f20 7468 6973 2065  to add to this e
-00000e50: 7272 6f72 0a0a 2020 2020 2020 2020 5265  rror..        Re
-00000e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00000e70: 2020 2052 6573 706f 6e73 6546 6169 6c75     ResponseFailu
-00000e80: 7265 206f 626a 6563 740a 2020 2020 2020  re object.      
-00000e90: 2020 2902 7208 0000 0072 0900 0000 2902    ).r....r....).
-00000ea0: 7206 0000 00da 0d42 5549 4c44 4552 5f45  r......BUILDER_E
-00000eb0: 5252 4f52 2903 721e 0000 0072 0900 0000  RROR).r....r....
-00000ec0: 721f 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000ed0: 1200 0000 da0d 6275 696c 6465 725f 6572  ......builder_er
-00000ee0: 726f 728d 0000 0073 0400 0000 000b 0e02  ror....s........
-00000ef0: 7a1d 5265 7370 6f6e 7365 4661 696c 7572  z.ResponseFailur
-00000f00: 652e 6275 696c 6465 725f 6572 726f 7263  e.builder_errorc
-00000f10: 0200 0000 0000 0000 0300 0000 0400 0000  ................
-00000f20: 4300 0000 7312 0000 0074 0074 006a 017c  C...s....t.t.j.|
-00000f30: 0164 018d 027d 027c 0253 0029 027a b00a  .d...}.|.S.).z..
-00000f40: 2020 2020 2020 2020 4372 6561 7465 7320          Creates 
-00000f50: 7265 7370 6f6e 7365 2066 6f72 2064 6174  response for dat
-00000f60: 6162 6173 6520 6661 696c 7572 652e 0a0a  abase failure...
-00000f70: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
-00000f80: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00000f90: 6167 653a 204d 6573 7361 6765 2074 6f20  age: Message to 
-00000fa0: 6164 6420 746f 2074 6869 7320 6572 726f  add to this erro
-00000fb0: 720a 0a20 2020 2020 2020 2052 6574 7572  r..        Retur
-00000fc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00000fd0: 5265 7370 6f6e 7365 4661 696c 7572 6520  ResponseFailure 
-00000fe0: 6f62 6a65 6374 0a20 2020 2020 2020 2029  object.        )
-00000ff0: 0272 0800 0000 7209 0000 0029 0272 0600  .r....r....).r..
-00001000: 0000 da0e 4441 5441 4241 5345 5f45 5252  ....DATABASE_ERR
-00001010: 4f52 2903 721e 0000 0072 0900 0000 721f  OR).r....r....r.
-00001020: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001030: 0000 da0e 6461 7461 6261 7365 5f65 7272  ....database_err
-00001040: 6f72 9c00 0000 7304 0000 0000 0b0e 027a  or....s........z
-00001050: 1e52 6573 706f 6e73 6546 6169 6c75 7265  .ResponseFailure
-00001060: 2e64 6174 6162 6173 655f 6572 726f 7263  .database_errorc
-00001070: 0200 0000 0000 0000 0300 0000 0400 0000  ................
-00001080: 4300 0000 7312 0000 0074 0074 006a 017c  C...s....t.t.j.|
-00001090: 0164 018d 027d 027c 0253 0029 027a b00a  .d...}.|.S.).z..
-000010a0: 2020 2020 2020 2020 4372 6561 7465 7320          Creates 
-000010b0: 7265 7370 6f6e 7365 2066 6f72 206e 6f74  response for not
-000010c0: 6966 6965 7220 6661 696c 7572 652e 0a0a  ifier failure...
-000010d0: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
-000010e0: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-000010f0: 6167 653a 204d 6573 7361 6765 2074 6f20  age: Message to 
-00001100: 6164 6420 746f 2074 6869 7320 6572 726f  add to this erro
-00001110: 720a 0a20 2020 2020 2020 2052 6574 7572  r..        Retur
-00001120: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00001130: 5265 7370 6f6e 7365 4661 696c 7572 6520  ResponseFailure 
-00001140: 6f62 6a65 6374 0a20 2020 2020 2020 2029  object.        )
-00001150: 0272 0800 0000 7209 0000 0029 0272 0600  .r....r....).r..
-00001160: 0000 da0e 4e4f 5449 4649 4552 5f45 5252  ....NOTIFIER_ERR
-00001170: 4f52 2903 721e 0000 0072 0900 0000 721f  OR).r....r....r.
-00001180: 0000 0072 1100 0000 7211 0000 0072 1200  ...r....r....r..
-00001190: 0000 da0e 6e6f 7469 6669 6572 5f65 7272  ....notifier_err
-000011a0: 6f72 ab00 0000 7304 0000 0000 0b0e 027a  or....s........z
-000011b0: 1e52 6573 706f 6e73 6546 6169 6c75 7265  .ResponseFailure
-000011c0: 2e6e 6f74 6966 6965 725f 6572 726f 7263  .notifier_errorc
-000011d0: 0200 0000 0000 0000 0300 0000 0400 0000  ................
-000011e0: 4300 0000 7312 0000 0074 0074 006a 017c  C...s....t.t.j.|
-000011f0: 0164 018d 027d 027c 0253 0029 027a af0a  .d...}.|.S.).z..
-00001200: 2020 2020 2020 2020 4372 6561 7465 7320          Creates 
-00001210: 7265 7370 6f6e 7365 2066 6f72 2070 6174  response for pat
-00001220: 6368 6572 2066 6169 6c75 7265 2e0a 0a20  cher failure... 
-00001230: 2020 2020 2020 2050 6172 616d 733a 0a20         Params:. 
-00001240: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00001250: 6765 3a20 4d65 7373 6167 6520 746f 2061  ge: Message to a
-00001260: 6464 2074 6f20 7468 6973 2065 7272 6f72  dd to this error
-00001270: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00001280: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00001290: 6573 706f 6e73 6546 6169 6c75 7265 206f  esponseFailure o
-000012a0: 626a 6563 740a 2020 2020 2020 2020 2902  bject.        ).
-000012b0: 7208 0000 0072 0900 0000 2902 7206 0000  r....r....).r...
-000012c0: 00da 0d50 4154 4348 4552 5f45 5252 4f52  ...PATCHER_ERROR
-000012d0: 2903 721e 0000 0072 0900 0000 721f 0000  ).r....r....r...
-000012e0: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-000012f0: da0d 7061 7463 6865 725f 6572 726f 72ba  ..patcher_error.
-00001300: 0000 0073 0400 0000 000b 0e02 7a1d 5265  ...s........z.Re
-00001310: 7370 6f6e 7365 4661 696c 7572 652e 7061  sponseFailure.pa
-00001320: 7463 6865 725f 6572 726f 7229 02da 0772  tcher_error)...r
-00001330: 6571 7565 7374 720a 0000 0063 0200 0000  equestr....c....
-00001340: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-00001350: 7318 0000 0074 0074 006a 0174 027c 016a  s....t.t.j.t.|.j
-00001360: 0383 0164 018d 027d 027c 0253 0029 027a  ...d...}.|.S.).z
-00001370: bf0a 2020 2020 2020 2020 4372 6561 7465  ..        Create
-00001380: 7320 7265 7370 6f6e 7365 2066 6f72 2069  s response for i
-00001390: 6e76 616c 6964 2072 6571 7565 7374 2066  nvalid request f
-000013a0: 6169 6c75 7265 2e0a 0a20 2020 2020 2020  ailure...       
-000013b0: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
-000013c0: 2020 2020 2072 6571 7565 7374 3a20 496e       request: In
-000013d0: 7661 6c69 6420 7265 7175 6573 7420 746f  valid request to
-000013e0: 2061 6464 2074 6f20 7468 6973 2065 7272   add to this err
-000013f0: 6f72 0a0a 2020 2020 2020 2020 5265 7475  or..        Retu
-00001400: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00001410: 2052 6573 706f 6e73 6546 6169 6c75 7265   ResponseFailure
-00001420: 206f 626a 6563 740a 2020 2020 2020 2020   object.        
-00001430: 2902 7208 0000 0072 0900 0000 2904 7206  ).r....r....).r.
-00001440: 0000 00da 1549 4e56 414c 4944 5f52 4551  .....INVALID_REQ
-00001450: 5545 5354 5f45 5252 4f52 da03 7374 72da  UEST_ERROR..str.
-00001460: 0665 7272 6f72 7329 0372 1e00 0000 7229  .errors).r....r)
-00001470: 0000 0072 1f00 0000 7211 0000 0072 1100  ...r....r....r..
-00001480: 0000 7212 0000 00da 1569 6e76 616c 6964  ..r......invalid
-00001490: 5f72 6571 7565 7374 5f65 7272 6f72 c900  _request_error..
-000014a0: 0000 7306 0000 0000 0b02 0112 037a 2552  ..s..........z%R
-000014b0: 6573 706f 6e73 6546 6169 6c75 7265 2e69  esponseFailure.i
-000014c0: 6e76 616c 6964 5f72 6571 7565 7374 5f65  nvalid_request_e
-000014d0: 7272 6f72 291d 721b 0000 00da 0a5f 5f6d  rror).r......__m
-000014e0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000014f0: 616d 655f 5fda 075f 5f64 6f63 5f5f 721d  ame__..__doc__r.
-00001500: 0000 0072 2100 0000 7223 0000 0072 2500  ...r!...r#...r%.
-00001510: 0000 7227 0000 0072 2a00 0000 722b 0000  ..r'...r*...r+..
-00001520: 0072 0200 0000 7213 0000 00da 0464 6963  .r....r......dic
-00001530: 7472 0e00 0000 720c 0000 0072 0b00 0000  tr....r....r....
-00001540: da08 7072 6f70 6572 7479 7215 0000 00da  ..propertyr.....
-00001550: 0462 6f6f 6c72 1c00 0000 da0b 636c 6173  .boolr......clas
-00001560: 736d 6574 686f 6472 2000 0000 7222 0000  smethodr ...r"..
-00001570: 0072 2400 0000 7226 0000 0072 2800 0000  .r$...r&...r(...
-00001580: 7204 0000 0072 2d00 0000 7211 0000 0072  r....r-...r....r
-00001590: 1100 0000 7211 0000 0072 1200 0000 7206  ....r....r....r.
-000015a0: 0000 001a 0000 0073 3200 0000 080b 0402  .......s2.......
-000015b0: 0401 0401 0401 0401 0401 0402 1209 1012  ................
-000015c0: 1212 1010 0c0b 0e06 0201 1210 0201 120e  ................
-000015d0: 0201 120e 0201 120e 0201 120e 0201 7206  ..............r.
-000015e0: 0000 0029 0a72 0d00 0000 da06 7479 7069  ...).r......typi
-000015f0: 6e67 7202 0000 00da 1268 6f74 6e65 7373  ngr......hotness
-00001600: 2e65 7863 6570 7469 6f6e 7372 0300 0000  .exceptionsr....
-00001610: da10 686f 746e 6573 732e 7265 7175 6573  ..hotness.reques
-00001620: 7473 7204 0000 005a 1168 6f74 6e65 7373  tsr....Z.hotness
-00001630: 2e72 6573 706f 6e73 6573 7205 0000 0072  .responsesr....r
-00001640: 0600 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00001650: 0000 0072 1200 0000 da08 3c6d 6f64 756c  ...r......<modul
-00001660: 653e 1200 0000 730a 0000 0008 010c 020c  e>....s.........
-00001670: 010c 010c 03                             .....
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 436f 7079  f-8 -*-.#.# Copy
+00000020: 7269 6768 7420 2843 2920 3230 3231 2052  right (C) 2021 R
+00000030: 6564 2048 6174 2c20 496e 632e 0a23 0a23  ed Hat, Inc..#.#
+00000040: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000050: 2066 7265 6520 736f 6674 7761 7265 3b20   free software; 
+00000060: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000070: 6275 7465 2069 7420 616e 642f 6f72 0a23  bute it and/or.#
+00000080: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+00000090: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+000000a0: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+000000b0: 626c 6963 204c 6963 656e 7365 0a23 2061  blic License.# a
+000000c0: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
+000000d0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
+000000e0: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
+000000f0: 6865 7220 7665 7273 696f 6e20 320a 2320  her version 2.# 
+00000100: 6f66 2074 6865 204c 6963 656e 7365 2c20  of the License, 
+00000110: 6f72 2028 6174 2079 6f75 7220 6f70 7469  or (at your opti
+00000120: 6f6e 2920 616e 7920 6c61 7465 7220 7665  on) any later ve
+00000130: 7273 696f 6e2e 0a23 0a23 2054 6869 7320  rsion..#.# This 
+00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+00000170: 6265 2075 7365 6675 6c2c 0a23 2062 7574  be useful,.# but
+00000180: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+00000190: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+000001a0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+000001b0: 7761 7272 616e 7479 206f 660a 2320 4d45  warranty of.# ME
+000001c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000001d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000001e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000001f0: 452e 2020 5365 6520 7468 650a 2320 474e  E.  See the.# GN
+00000200: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000210: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
+00000220: 6520 6465 7461 696c 732e 0a23 0a23 2059  e details..#.# Y
+00000230: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000240: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+00000250: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 0a23 2061 6c6f 6e67 2077 6974 6820 7468  .# along with th
+00000280: 6973 2070 726f 6772 616d 3b20 6966 206e  is program; if n
+00000290: 6f74 2c20 7772 6974 6520 746f 2074 6865  ot, write to the
+000002a0: 2046 7265 6520 536f 6674 7761 7265 0a23   Free Software.#
+000002b0: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
+000002c0: 2e2c 2035 3120 4672 616e 6b6c 696e 2053  ., 51 Franklin S
+000002d0: 7472 6565 742c 2046 6966 7468 2046 6c6f  treet, Fifth Flo
+000002e0: 6f72 2c20 426f 7374 6f6e 2c20 4d41 2020  or, Boston, MA  
+000002f0: 3032 3131 302d 3133 3031 2c20 5553 412e  02110-1301, USA.
+00000300: 0a69 6d70 6f72 7420 7472 6163 6562 6163  .import tracebac
+00000310: 6b0a 6672 6f6d 2074 7970 696e 6720 696d  k.from typing im
+00000320: 706f 7274 2041 6e79 2c20 4f70 7469 6f6e  port Any, Option
+00000330: 616c 2c20 4c69 7374 0a0a 6672 6f6d 2068  al, List..from h
+00000340: 6f74 6e65 7373 2e65 7863 6570 7469 6f6e  otness.exception
+00000350: 7320 696d 706f 7274 2042 6173 6548 6f74  s import BaseHot
+00000360: 6e65 7373 4578 6365 7074 696f 6e0a 6672  nessException.fr
+00000370: 6f6d 2068 6f74 6e65 7373 2e72 6571 7565  om hotness.reque
+00000380: 7374 7320 696d 706f 7274 2052 6571 7565  sts import Reque
+00000390: 7374 0a66 726f 6d20 686f 746e 6573 732e  st.from hotness.
+000003a0: 7265 7370 6f6e 7365 7320 696d 706f 7274  responses import
+000003b0: 2052 6573 706f 6e73 650a 0a0a 636c 6173   Response...clas
+000003c0: 7320 5265 7370 6f6e 7365 4661 696c 7572  s ResponseFailur
+000003d0: 6528 5265 7370 6f6e 7365 293a 0a20 2020  e(Response):.   
+000003e0: 2022 2222 0a20 2020 2043 6c61 7373 2074   """.    Class t
+000003f0: 6861 7420 7265 7072 6573 656e 7473 2066  hat represents f
+00000400: 6169 6c75 7265 2072 6573 706f 6e73 6520  ailure response 
+00000410: 7265 7475 726e 6564 2066 726f 6d20 7573  returned from us
+00000420: 6520 6361 7365 2e0a 2020 2020 4974 2069  e case..    It i
+00000430: 7320 7365 6e64 2077 6865 6e20 736f 6d65  s send when some
+00000440: 2065 7863 6570 7469 6f6e 2068 6170 7065   exception happe
+00000450: 6e20 6475 7269 6e67 2074 6865 2075 7365  n during the use
+00000460: 2063 6173 652e 0a20 2020 2044 6566 696e   case..    Defin
+00000470: 6573 2063 6f6e 7374 616e 7473 2066 6f72  es constants for
+00000480: 2065 7272 6f72 2074 7970 6573 2e0a 0a20   error types... 
+00000490: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+000004a0: 2020 2020 2020 2074 7970 653a 2054 7970         type: Typ
+000004b0: 6520 6f66 2074 6865 2066 6169 6c75 7265  e of the failure
+000004c0: 2e0a 2020 2020 2020 2020 6d65 7373 6167  ..        messag
+000004d0: 653a 2045 7272 6f72 206d 6573 7361 6765  e: Error message
+000004e0: 2e0a 2020 2020 2020 2020 7472 6163 6562  ..        traceb
+000004f0: 6163 6b3a 2045 7863 6570 7469 6f6e 2074  ack: Exception t
+00000500: 7261 6365 6261 636b 2061 7320 7374 7269  raceback as stri
+00000510: 6e67 2e0a 2020 2020 2020 2020 7573 655f  ng..        use_
+00000520: 6361 7365 5f76 616c 7565 3a20 5061 7274  case_value: Part
+00000530: 6961 6c20 7573 6520 6361 7365 206f 7574  ial use case out
+00000540: 7075 7420 6672 6f6d 2045 7863 6570 7469  put from Excepti
+00000550: 6f6e 2c20 6966 2070 726f 7669 6465 642e  on, if provided.
+00000560: 0a20 2020 2022 2222 0a0a 2020 2020 5641  .    """..    VA
+00000570: 4c49 4441 544f 525f 4552 524f 5220 3d20  LIDATOR_ERROR = 
+00000580: 2256 616c 6964 6174 6f72 4572 726f 7222  "ValidatorError"
+00000590: 0a20 2020 2042 5549 4c44 4552 5f45 5252  .    BUILDER_ERR
+000005a0: 4f52 203d 2022 4275 696c 6465 7245 7272  OR = "BuilderErr
+000005b0: 6f72 220a 2020 2020 4441 5441 4241 5345  or".    DATABASE
+000005c0: 5f45 5252 4f52 203d 2022 4461 7461 6261  _ERROR = "Databa
+000005d0: 7365 4572 726f 7222 0a20 2020 204e 4f54  seError".    NOT
+000005e0: 4946 4945 525f 4552 524f 5220 3d20 224e  IFIER_ERROR = "N
+000005f0: 6f74 6966 6965 7245 7272 6f72 220a 2020  otifierError".  
+00000600: 2020 5041 5443 4845 525f 4552 524f 5220    PATCHER_ERROR 
+00000610: 3d20 2250 6174 6368 6572 4572 726f 7222  = "PatcherError"
+00000620: 0a20 2020 2049 4e56 414c 4944 5f52 4551  .    INVALID_REQ
+00000630: 5545 5354 5f45 5252 4f52 203d 2022 496e  UEST_ERROR = "In
+00000640: 7661 6c69 6452 6571 7565 7374 4572 726f  validRequestErro
+00000650: 7222 0a0a 2020 2020 6465 6620 5f5f 696e  r"..    def __in
+00000660: 6974 5f5f 2873 656c 662c 2074 7970 653a  it__(self, type:
+00000670: 2073 7472 2c20 6d65 7373 6167 653a 2041   str, message: A
+00000680: 6e79 2920 2d3e 204e 6f6e 653a 0a20 2020  ny) -> None:.   
+00000690: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000006a0: 2043 6c61 7373 2063 6f6e 7374 7275 6374   Class construct
+000006b0: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
+000006c0: 2020 2020 2020 2020 7365 6c66 2e74 7970          self.typ
+000006d0: 6520 3d20 7479 7065 0a20 2020 2020 2020  e = type.       
+000006e0: 2073 656c 662e 6d65 7373 6167 6520 3d20   self.message = 
+000006f0: 7365 6c66 2e5f 666f 726d 6174 5f6d 6573  self._format_mes
+00000700: 7361 6765 286d 6573 7361 6765 290a 2020  sage(message).  
+00000710: 2020 2020 2020 7365 6c66 2e74 7261 6365        self.trace
+00000720: 6261 636b 203d 2073 656c 662e 5f67 6574  back = self._get
+00000730: 5f73 7461 636b 5f74 7261 6365 286d 6573  _stack_trace(mes
+00000740: 7361 6765 290a 2020 2020 2020 2020 7365  sage).        se
+00000750: 6c66 2e75 7365 5f63 6173 655f 7661 6c75  lf.use_case_valu
+00000760: 6520 3d20 7365 6c66 2e5f 6765 745f 7661  e = self._get_va
+00000770: 6c75 6528 6d65 7373 6167 6529 0a0a 2020  lue(message)..  
+00000780: 2020 6465 6620 5f67 6574 5f76 616c 7565    def _get_value
+00000790: 2873 656c 662c 206d 6573 7361 6765 3a20  (self, message: 
+000007a0: 416e 7929 202d 3e20 4f70 7469 6f6e 616c  Any) -> Optional
+000007b0: 5b64 6963 745d 3a0a 2020 2020 2020 2020  [dict]:.        
+000007c0: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
+000007d0: 6965 7665 7320 7468 6520 7573 6520 6361  ieves the use ca
+000007e0: 7365 2076 616c 7565 2069 6e66 6f72 6d61  se value informa
+000007f0: 7469 6f6e 2066 726f 6d20 4578 6365 7074  tion from Except
+00000800: 696f 6e2c 0a20 2020 2020 2020 206f 7468  ion,.        oth
+00000810: 6572 7769 7365 206a 7573 7420 7265 7475  erwise just retu
+00000820: 726e 7320 656d 7074 7920 6469 6374 2e0a  rns empty dict..
+00000830: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
+00000840: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+00000850: 7361 6765 3a20 496e 7075 7420 746f 2072  sage: Input to r
+00000860: 6574 7269 6576 6520 7573 6520 6361 7365  etrieve use case
+00000870: 2076 616c 7565 2066 726f 6d0a 0a20 2020   value from..   
+00000880: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00000890: 2020 2020 2020 2020 2020 5661 6c75 6520            Value 
+000008a0: 6966 206d 6573 7361 6765 2069 7320 4578  if message is Ex
+000008b0: 6365 7074 696f 6e2c 206f 7468 6572 7769  ception, otherwi
+000008c0: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
+000008d0: 2222 220a 2020 2020 2020 2020 7661 6c75  """.        valu
+000008e0: 6520 3d20 4e6f 6e65 0a0a 2020 2020 2020  e = None..      
+000008f0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00000900: 6d65 7373 6167 652c 2042 6173 6548 6f74  message, BaseHot
+00000910: 6e65 7373 4578 6365 7074 696f 6e29 3a0a  nessException):.
+00000920: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00000930: 6520 3d20 6d65 7373 6167 652e 7661 6c75  e = message.valu
+00000940: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+00000950: 6e20 7661 6c75 650a 0a20 2020 2064 6566  n value..    def
+00000960: 205f 6765 745f 7374 6163 6b5f 7472 6163   _get_stack_trac
+00000970: 6528 7365 6c66 2c20 6d65 7373 6167 653a  e(self, message:
+00000980: 2041 6e79 2920 2d3e 204c 6973 745b 7374   Any) -> List[st
+00000990: 725d 3a0a 2020 2020 2020 2020 2222 220a  r]:.        """.
+000009a0: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
+000009b0: 7320 7468 6520 7374 6163 6b20 7472 6163  s the stack trac
+000009c0: 6520 696e 666f 726d 6174 696f 6e20 6672  e information fr
+000009d0: 6f6d 2045 7863 6570 7469 6f6e 2c0a 2020  om Exception,.  
+000009e0: 2020 2020 2020 6f74 6865 7277 6973 6520        otherwise 
+000009f0: 6a75 7374 2072 6574 7572 6e73 2065 6d70  just returns emp
+00000a00: 7479 206c 6973 742e 0a0a 2020 2020 2020  ty list...      
+00000a10: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
+00000a20: 2020 2020 2020 6d65 7373 6167 653a 2049        message: I
+00000a30: 6e70 7574 2074 6f20 7265 7472 6965 7665  nput to retrieve
+00000a40: 2073 7461 636b 2074 7261 6365 2066 726f   stack trace fro
+00000a50: 6d0a 0a20 2020 2020 2020 2052 6574 7572  m..        Retur
+00000a60: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00000a70: 5374 6163 6b20 7472 6163 6520 6966 206d  Stack trace if m
+00000a80: 6573 7361 6765 2069 7320 4578 6365 7074  essage is Except
+00000a90: 696f 6e2c 206f 7468 6572 7769 7365 2065  ion, otherwise e
+00000aa0: 6d70 7479 2073 7472 696e 670a 2020 2020  mpty string.    
+00000ab0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00000ac0: 7374 6163 6b5f 7472 6163 6520 3d20 5b5d  stack_trace = []
+00000ad0: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
+00000ae0: 6e73 7461 6e63 6528 6d65 7373 6167 652c  nstance(message,
+00000af0: 2045 7863 6570 7469 6f6e 293a 0a20 2020   Exception):.   
+00000b00: 2020 2020 2020 2020 2073 7461 636b 5f74           stack_t
+00000b10: 7261 6365 203d 2074 7261 6365 6261 636b  race = traceback
+00000b20: 2e66 6f72 6d61 745f 7462 286d 6573 7361  .format_tb(messa
+00000b30: 6765 2e5f 5f74 7261 6365 6261 636b 5f5f  ge.__traceback__
+00000b40: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00000b50: 6e20 7374 6163 6b5f 7472 6163 650a 0a20  n stack_trace.. 
+00000b60: 2020 2064 6566 205f 666f 726d 6174 5f6d     def _format_m
+00000b70: 6573 7361 6765 2873 656c 662c 206d 6573  essage(self, mes
+00000b80: 7361 6765 3a20 416e 7929 202d 3e20 416e  sage: Any) -> An
+00000b90: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
+00000ba0: 2020 2020 2020 2046 6f72 6d61 7473 2074         Formats t
+00000bb0: 6865 2069 6e70 7574 206d 6573 7361 6765  he input message
+00000bc0: 2069 6620 7468 6520 6d65 7373 6167 6520   if the message 
+00000bd0: 696e 6865 7269 7473 2066 726f 6d20 4578  inherits from Ex
+00000be0: 6365 7074 696f 6e2c 0a20 2020 2020 2020  ception,.       
+00000bf0: 206f 7468 6572 7769 7365 206a 7573 7420   otherwise just 
+00000c00: 7265 7475 726e 2069 7420 6261 636b 2e0a  return it back..
+00000c10: 0a20 2020 2020 2020 2050 6172 616d 733a  .        Params:
+00000c20: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
+00000c30: 7361 6765 3a20 496e 7075 7420 6d65 7373  sage: Input mess
+00000c40: 6167 6520 746f 2066 6f72 6d61 740a 0a20  age to format.. 
+00000c50: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00000c60: 2020 2020 2020 2020 2020 2020 5374 7269              Stri
+00000c70: 6e67 2069 6620 6578 6365 7074 696f 6e2c  ng if exception,
+00000c80: 206f 7468 6572 7769 7365 2072 6574 7572   otherwise retur
+00000c90: 6e20 7468 6520 7361 6d65 206f 626a 6563  n the same objec
+00000ca0: 7420 7765 2072 6563 6569 7665 642e 0a20  t we received.. 
+00000cb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000cc0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00000cd0: 286d 6573 7361 6765 2c20 4578 6365 7074  (message, Except
+00000ce0: 696f 6e29 3a0a 2020 2020 2020 2020 2020  ion):.          
+00000cf0: 2020 7265 7475 726e 2022 7b7d 3a20 7b7d    return "{}: {}
+00000d00: 222e 666f 726d 6174 286d 6573 7361 6765  ".format(message
+00000d10: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+00000d20: 655f 5f2c 2022 7b7d 222e 666f 726d 6174  e__, "{}".format
+00000d30: 286d 6573 7361 6765 2929 0a0a 2020 2020  (message))..    
+00000d40: 2020 2020 7265 7475 726e 206d 6573 7361      return messa
+00000d50: 6765 0a0a 2020 2020 4070 726f 7065 7274  ge..    @propert
+00000d60: 790a 2020 2020 6465 6620 7661 6c75 6528  y.    def value(
+00000d70: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00000d80: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+00000d90: 6e73 2074 6865 2064 6963 7420 7265 7072  ns the dict repr
+00000da0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+00000db0: 6520 6661 696c 7572 6520 7265 7370 6f6e  e failure respon
+00000dc0: 7365 2e0a 2020 2020 2020 2020 2222 220a  se..        """.
+00000dd0: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00000de0: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
+00000df0: 7065 223a 2073 656c 662e 7479 7065 2c0a  pe": self.type,.
+00000e00: 2020 2020 2020 2020 2020 2020 226d 6573              "mes
+00000e10: 7361 6765 223a 2073 656c 662e 6d65 7373  sage": self.mess
+00000e20: 6167 652c 0a20 2020 2020 2020 2020 2020  age,.           
+00000e30: 2022 7573 655f 6361 7365 5f76 616c 7565   "use_case_value
+00000e40: 223a 2073 656c 662e 7573 655f 6361 7365  ": self.use_case
+00000e50: 5f76 616c 7565 2c0a 2020 2020 2020 2020  _value,.        
+00000e60: 7d0a 0a20 2020 2064 6566 205f 5f62 6f6f  }..    def __boo
+00000e70: 6c5f 5f28 7365 6c66 2920 2d3e 2062 6f6f  l__(self) -> boo
+00000e80: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+00000e90: 2020 2020 2020 2042 6f6f 6c65 616e 2072         Boolean r
+00000ea0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+00000eb0: 2072 6573 706f 6e73 652e 0a20 2020 2020   response..     
+00000ec0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00000ed0: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00000ee0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00000ef0: 2020 6465 6620 7661 6c69 6461 746f 725f    def validator_
+00000f00: 6572 726f 7228 636c 732c 206d 6573 7361  error(cls, messa
+00000f10: 6765 3a20 416e 7929 202d 3e20 2252 6573  ge: Any) -> "Res
+00000f20: 706f 6e73 6546 6169 6c75 7265 223a 0a20  ponseFailure":. 
+00000f30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00000f40: 2020 2043 7265 6174 6573 2072 6573 706f     Creates respo
+00000f50: 6e73 6520 666f 7220 7661 6c69 6461 746f  nse for validato
+00000f60: 7220 6661 696c 7572 652e 0a0a 2020 2020  r failure...    
+00000f70: 2020 2020 5061 7261 6d73 3a0a 2020 2020      Params:.    
+00000f80: 2020 2020 2020 2020 6d65 7373 6167 653a          message:
+00000f90: 204d 6573 7361 6765 2074 6f20 6164 6420   Message to add 
+00000fa0: 746f 2074 6869 7320 6572 726f 720a 0a20  to this error.. 
+00000fb0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00000fc0: 2020 2020 2020 2020 2020 2020 5265 7370              Resp
+00000fd0: 6f6e 7365 4661 696c 7572 6520 6f62 6a65  onseFailure obje
+00000fe0: 6374 0a20 2020 2020 2020 2022 2222 0a20  ct.        """. 
+00000ff0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+00001000: 3d20 5265 7370 6f6e 7365 4661 696c 7572  = ResponseFailur
+00001010: 6528 0a20 2020 2020 2020 2020 2020 2074  e(.            t
+00001020: 7970 653d 5265 7370 6f6e 7365 4661 696c  ype=ResponseFail
+00001030: 7572 652e 5641 4c49 4441 544f 525f 4552  ure.VALIDATOR_ER
+00001040: 524f 522c 206d 6573 7361 6765 3d6d 6573  ROR, message=mes
+00001050: 7361 6765 0a20 2020 2020 2020 2029 0a0a  sage.        )..
+00001060: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001070: 6573 706f 6e73 650a 0a20 2020 2040 636c  esponse..    @cl
+00001080: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00001090: 6620 6275 696c 6465 725f 6572 726f 7228  f builder_error(
+000010a0: 636c 732c 206d 6573 7361 6765 3a20 416e  cls, message: An
+000010b0: 7929 202d 3e20 2252 6573 706f 6e73 6546  y) -> "ResponseF
+000010c0: 6169 6c75 7265 223a 0a20 2020 2020 2020  ailure":.       
+000010d0: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+000010e0: 6174 6573 2072 6573 706f 6e73 6520 666f  ates response fo
+000010f0: 7220 6275 696c 6465 7220 6661 696c 7572  r builder failur
+00001100: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+00001110: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00001120: 6d65 7373 6167 653a 204d 6573 7361 6765  message: Message
+00001130: 2074 6f20 6164 6420 746f 2074 6869 7320   to add to this 
+00001140: 6572 726f 720a 0a20 2020 2020 2020 2052  error..        R
+00001150: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001160: 2020 2020 5265 7370 6f6e 7365 4661 696c      ResponseFail
+00001170: 7572 6520 6f62 6a65 6374 0a20 2020 2020  ure object.     
+00001180: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00001190: 6573 706f 6e73 6520 3d20 5265 7370 6f6e  esponse = Respon
+000011a0: 7365 4661 696c 7572 6528 7479 7065 3d52  seFailure(type=R
+000011b0: 6573 706f 6e73 6546 6169 6c75 7265 2e42  esponseFailure.B
+000011c0: 5549 4c44 4552 5f45 5252 4f52 2c20 6d65  UILDER_ERROR, me
+000011d0: 7373 6167 653d 6d65 7373 6167 6529 0a0a  ssage=message)..
+000011e0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000011f0: 6573 706f 6e73 650a 0a20 2020 2040 636c  esponse..    @cl
+00001200: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00001210: 6620 6461 7461 6261 7365 5f65 7272 6f72  f database_error
+00001220: 2863 6c73 2c20 6d65 7373 6167 653a 2041  (cls, message: A
+00001230: 6e79 2920 2d3e 2022 5265 7370 6f6e 7365  ny) -> "Response
+00001240: 4661 696c 7572 6522 3a0a 2020 2020 2020  Failure":.      
+00001250: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
+00001260: 6561 7465 7320 7265 7370 6f6e 7365 2066  eates response f
+00001270: 6f72 2064 6174 6162 6173 6520 6661 696c  or database fail
+00001280: 7572 652e 0a0a 2020 2020 2020 2020 5061  ure...        Pa
+00001290: 7261 6d73 3a0a 2020 2020 2020 2020 2020  rams:.          
+000012a0: 2020 6d65 7373 6167 653a 204d 6573 7361    message: Messa
+000012b0: 6765 2074 6f20 6164 6420 746f 2074 6869  ge to add to thi
+000012c0: 7320 6572 726f 720a 0a20 2020 2020 2020  s error..       
+000012d0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000012e0: 2020 2020 2020 5265 7370 6f6e 7365 4661        ResponseFa
+000012f0: 696c 7572 6520 6f62 6a65 6374 0a20 2020  ilure object.   
+00001300: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00001310: 2072 6573 706f 6e73 6520 3d20 5265 7370   response = Resp
+00001320: 6f6e 7365 4661 696c 7572 6528 7479 7065  onseFailure(type
+00001330: 3d52 6573 706f 6e73 6546 6169 6c75 7265  =ResponseFailure
+00001340: 2e44 4154 4142 4153 455f 4552 524f 522c  .DATABASE_ERROR,
+00001350: 206d 6573 7361 6765 3d6d 6573 7361 6765   message=message
+00001360: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001370: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
+00001380: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00001390: 2064 6566 206e 6f74 6966 6965 725f 6572   def notifier_er
+000013a0: 726f 7228 636c 732c 206d 6573 7361 6765  ror(cls, message
+000013b0: 3a20 416e 7929 202d 3e20 2252 6573 706f  : Any) -> "Respo
+000013c0: 6e73 6546 6169 6c75 7265 223a 0a20 2020  nseFailure":.   
+000013d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000013e0: 2043 7265 6174 6573 2072 6573 706f 6e73   Creates respons
+000013f0: 6520 666f 7220 6e6f 7469 6669 6572 2066  e for notifier f
+00001400: 6169 6c75 7265 2e0a 0a20 2020 2020 2020  ailure...       
+00001410: 2050 6172 616d 733a 0a20 2020 2020 2020   Params:.       
+00001420: 2020 2020 206d 6573 7361 6765 3a20 4d65       message: Me
+00001430: 7373 6167 6520 746f 2061 6464 2074 6f20  ssage to add to 
+00001440: 7468 6973 2065 7272 6f72 0a0a 2020 2020  this error..    
+00001450: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00001460: 2020 2020 2020 2020 2052 6573 706f 6e73           Respons
+00001470: 6546 6169 6c75 7265 206f 626a 6563 740a  eFailure object.
+00001480: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00001490: 2020 2020 7265 7370 6f6e 7365 203d 2052      response = R
+000014a0: 6573 706f 6e73 6546 6169 6c75 7265 2874  esponseFailure(t
+000014b0: 7970 653d 5265 7370 6f6e 7365 4661 696c  ype=ResponseFail
+000014c0: 7572 652e 4e4f 5449 4649 4552 5f45 5252  ure.NOTIFIER_ERR
+000014d0: 4f52 2c20 6d65 7373 6167 653d 6d65 7373  OR, message=mess
+000014e0: 6167 6529 0a0a 2020 2020 2020 2020 7265  age)..        re
+000014f0: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00001500: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00001510: 2020 2020 6465 6620 7061 7463 6865 725f      def patcher_
+00001520: 6572 726f 7228 636c 732c 206d 6573 7361  error(cls, messa
+00001530: 6765 3a20 416e 7929 202d 3e20 2252 6573  ge: Any) -> "Res
+00001540: 706f 6e73 6546 6169 6c75 7265 223a 0a20  ponseFailure":. 
+00001550: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00001560: 2020 2043 7265 6174 6573 2072 6573 706f     Creates respo
+00001570: 6e73 6520 666f 7220 7061 7463 6865 7220  nse for patcher 
+00001580: 6661 696c 7572 652e 0a0a 2020 2020 2020  failure...      
+00001590: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
+000015a0: 2020 2020 2020 6d65 7373 6167 653a 204d        message: M
+000015b0: 6573 7361 6765 2074 6f20 6164 6420 746f  essage to add to
+000015c0: 2074 6869 7320 6572 726f 720a 0a20 2020   this error..   
+000015d0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+000015e0: 2020 2020 2020 2020 2020 5265 7370 6f6e            Respon
+000015f0: 7365 4661 696c 7572 6520 6f62 6a65 6374  seFailure object
+00001600: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001610: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00001620: 5265 7370 6f6e 7365 4661 696c 7572 6528  ResponseFailure(
+00001630: 7479 7065 3d52 6573 706f 6e73 6546 6169  type=ResponseFai
+00001640: 6c75 7265 2e50 4154 4348 4552 5f45 5252  lure.PATCHER_ERR
+00001650: 4f52 2c20 6d65 7373 6167 653d 6d65 7373  OR, message=mess
+00001660: 6167 6529 0a0a 2020 2020 2020 2020 7265  age)..        re
+00001670: 7475 726e 2072 6573 706f 6e73 650a 0a20  turn response.. 
+00001680: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00001690: 2020 2020 6465 6620 696e 7661 6c69 645f      def invalid_
+000016a0: 7265 7175 6573 745f 6572 726f 7228 636c  request_error(cl
+000016b0: 732c 2072 6571 7565 7374 3a20 5265 7175  s, request: Requ
+000016c0: 6573 7429 202d 3e20 2252 6573 706f 6e73  est) -> "Respons
+000016d0: 6546 6169 6c75 7265 223a 0a20 2020 2020  eFailure":.     
+000016e0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+000016f0: 7265 6174 6573 2072 6573 706f 6e73 6520  reates response 
+00001700: 666f 7220 696e 7661 6c69 6420 7265 7175  for invalid requ
+00001710: 6573 7420 6661 696c 7572 652e 0a0a 2020  est failure...  
+00001720: 2020 2020 2020 5061 7261 6d73 3a0a 2020        Params:.  
+00001730: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+00001740: 743a 2049 6e76 616c 6964 2072 6571 7565  t: Invalid reque
+00001750: 7374 2074 6f20 6164 6420 746f 2074 6869  st to add to thi
+00001760: 7320 6572 726f 720a 0a20 2020 2020 2020  s error..       
+00001770: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00001780: 2020 2020 2020 5265 7370 6f6e 7365 4661        ResponseFa
+00001790: 696c 7572 6520 6f62 6a65 6374 0a20 2020  ilure object.   
+000017a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000017b0: 2072 6573 706f 6e73 6520 3d20 5265 7370   response = Resp
+000017c0: 6f6e 7365 4661 696c 7572 6528 0a20 2020  onseFailure(.   
+000017d0: 2020 2020 2020 2020 2074 7970 653d 5265           type=Re
+000017e0: 7370 6f6e 7365 4661 696c 7572 652e 494e  sponseFailure.IN
+000017f0: 5641 4c49 445f 5245 5155 4553 545f 4552  VALID_REQUEST_ER
+00001800: 524f 522c 206d 6573 7361 6765 3d73 7472  ROR, message=str
+00001810: 2872 6571 7565 7374 2e65 7272 6f72 7329  (request.errors)
+00001820: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00001830: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00001840: 6e73 650a                                nse.
```

### Comparing `the_new_hotness-1.2.3/hotness/responses/response.py` & `the_new_hotness-1.2.4/hotness/responses/response.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/responses/response_success.py` & `the_new_hotness-1.2.4/hotness/responses/response_success.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/__init__.py` & `the_new_hotness-1.2.4/hotness/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/__pycache__/package_scratch_build_use_case.cpython-37.pyc` & `the_new_hotness-1.2.4/hotness/use_cases/package_scratch_build_use_case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,124 @@
-00000000: 420d 0d0a 0000 0000 32ea 5a61 be07 0000  B.......2.Za....
-00000010: e300 0000 0000 0000 0000 0000 0003 0000  ................
-00000020: 0040 0000 0073 4800 0000 6400 6401 6c00  .@...sH...d.d.l.
-00000030: 5a00 6400 6402 6c01 6d02 5a02 0100 6400  Z.d.d.l.m.Z...d.
-00000040: 6403 6c03 6d04 5a04 0100 6400 6404 6c05  d.l.m.Z...d.d.l.
-00000050: 6d06 5a06 0100 6500 a007 6508 a101 5a09  m.Z...e...e...Z.
-00000060: 4700 6405 6406 8400 6406 8302 5a0a 6401  G.d.d...d...Z.d.
-00000070: 5300 2907 e900 0000 004e 2901 da07 4275  S.)......N)...Bu
-00000080: 696c 6465 7229 01da 0c42 7569 6c64 5265  ilder)...BuildRe
-00000090: 7175 6573 7429 01da 0972 6573 706f 6e73  quest)...respons
-000000a0: 6573 6300 0000 0000 0000 0000 0000 0003  esc.............
-000000b0: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
-000000c0: 6400 5a02 6401 5a03 6504 6402 9c01 6403  d.Z.d.Z.e.d...d.
-000000d0: 6404 8404 5a05 6506 6507 6a08 6405 9c02  d...Z.e.e.j.d...
-000000e0: 6406 6407 8404 5a09 6408 5300 2909 da1a  d.d...Z.d.S.)...
-000000f0: 5061 636b 6167 6553 6372 6174 6368 4275  PackageScratchBu
-00000100: 696c 6455 7365 4361 7365 7a8a 0a20 2020  ildUseCasez..   
-00000110: 2054 6869 7320 636c 6173 7320 7265 7072   This class repr
-00000120: 6573 656e 7473 2075 7365 2063 6173 6520  esents use case 
-00000130: 666f 7220 6275 696c 6469 6e67 2074 6865  for building the
-00000140: 2070 6163 6b61 6765 2077 6974 6820 7072   package with pr
-00000150: 6f76 6964 6564 2062 7569 6c64 6572 2e0a  ovided builder..
-00000160: 0a20 2020 2041 7474 7269 6275 7465 733a  .    Attributes:
-00000170: 0a20 2020 2020 2020 2062 7569 6c64 6572  .        builder
-00000180: 3a20 4275 696c 6465 7220 746f 2075 7365  : Builder to use
-00000190: 2e0a 2020 2020 2901 da07 6275 696c 6465  ..    )...builde
-000001a0: 7263 0200 0000 0000 0000 0200 0000 0200  rc..............
-000001b0: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
-000001c0: 0064 0153 0029 027a 240a 2020 2020 2020  .d.S.).z$.      
-000001d0: 2020 436c 6173 7320 636f 6e73 7472 7563    Class construc
-000001e0: 746f 722e 0a20 2020 2020 2020 204e 2901  tor..        N).
-000001f0: 7206 0000 0029 02da 0473 656c 6672 0600  r....)...selfr..
-00000200: 0000 a900 7208 0000 00fa 382f 6170 702f  ....r.....8/app/
-00000210: 686f 746e 6573 732f 7573 655f 6361 7365  hotness/use_case
-00000220: 732f 7061 636b 6167 655f 7363 7261 7463  s/package_scratc
-00000230: 685f 6275 696c 645f 7573 655f 6361 7365  h_build_use_case
-00000240: 2e70 79da 085f 5f69 6e69 745f 5f24 0000  .py..__init__$..
-00000250: 0073 0200 0000 0004 7a23 5061 636b 6167  .s......z#Packag
-00000260: 6553 6372 6174 6368 4275 696c 6455 7365  eScratchBuildUse
-00000270: 4361 7365 2e5f 5f69 6e69 745f 5f29 02da  Case.__init__)..
-00000280: 0772 6571 7565 7374 da06 7265 7475 726e  .request..return
-00000290: 6302 0000 0000 0000 0004 0000 000a 0000  c...............
-000002a0: 0043 0000 0073 6a00 0000 7c01 7310 7400  .C...sj...|.s.t.
-000002b0: 6a01 a002 7c01 a101 5300 791c 7c00 6a03  j...|...S.y.|.j.
-000002c0: a004 7c01 6a05 7c01 6a06 a102 7d02 7400  ..|.j.|.j...}.t.
-000002d0: a007 7c02 a101 5300 0400 7408 6b0a 7264  ..|...S...t.k.rd
-000002e0: 0100 7d03 0100 7a1a 7409 6a0a 6401 6402  ..}...z.t.j.d.d.
-000002f0: 6403 8d02 0100 7400 6a01 a00b 7c03 a101  d.....t.j...|...
-00000300: 5300 6404 7d03 7e03 5800 5900 6e02 5800  S.d.}.~.X.Y.n.X.
-00000310: 6404 5300 2905 7aed 0a20 2020 2020 2020  d.S.).z..       
-00000320: 2043 616c 6c20 7468 6520 6275 696c 6420   Call the build 
-00000330: 6d65 7468 6f64 206f 6e20 7468 6520 6275  method on the bu
-00000340: 696c 6465 722e 0a20 2020 2020 2020 2054  ilder..        T
-00000350: 6869 7320 6d65 7468 6f64 2077 696c 6c20  his method will 
-00000360: 6861 6e64 6c65 2061 6e79 2065 7272 6f72  handle any error
-00000370: 2074 6861 7420 6861 7070 656e 7320 7768   that happens wh
-00000380: 656e 2073 7461 7274 696e 6720 6275 696c  en starting buil
-00000390: 642e 0a0a 2020 2020 2020 2020 5061 7261  d...        Para
-000003a0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-000003b0: 7265 7175 6573 743a 2052 6571 7565 7374  request: Request
-000003c0: 2074 6f20 6861 6e64 6c65 2e0a 0a20 2020   to handle...   
-000003d0: 2020 2020 2052 6574 7572 6e3a 0a20 2020       Return:.   
-000003e0: 2020 2020 2020 2020 4f75 7470 7574 206f          Output o
-000003f0: 6620 7468 6520 6275 696c 642e 0a20 2020  f the build..   
-00000400: 2020 2020 207a 2650 6163 6b61 6765 2073       z&Package s
-00000410: 6372 6174 6368 2062 7569 6c64 2075 7365  cratch build use
-00000420: 2063 6173 6520 6661 696c 7572 6554 2901   case failureT).
-00000430: da08 6578 635f 696e 666f 4e29 0c72 0400  ..exc_infoN).r..
-00000440: 0000 da0f 5265 7370 6f6e 7365 4661 696c  ....ResponseFail
-00000450: 7572 65da 1569 6e76 616c 6964 5f72 6571  ure..invalid_req
-00000460: 7565 7374 5f65 7272 6f72 7206 0000 00da  uest_errorr.....
-00000470: 0562 7569 6c64 da07 7061 636b 6167 65da  .build..package.
-00000480: 046f 7074 73da 0f52 6573 706f 6e73 6553  .opts..ResponseS
-00000490: 7563 6365 7373 da09 4578 6365 7074 696f  uccess..Exceptio
-000004a0: 6eda 066c 6f67 6765 72da 0965 7863 6570  n..logger..excep
-000004b0: 7469 6f6e da0d 6275 696c 6465 725f 6572  tion..builder_er
-000004c0: 726f 7229 0472 0700 0000 720b 0000 00da  ror).r....r.....
-000004d0: 0672 6573 756c 74da 0365 7863 7208 0000  .result..excr...
-000004e0: 0072 0800 0000 7209 0000 0072 1000 0000  .r....r....r....
-000004f0: 2a00 0000 7310 0000 0000 0b04 010c 0102  *...s...........
-00000500: 0112 010a 0110 010e 017a 2050 6163 6b61  .........z Packa
-00000510: 6765 5363 7261 7463 6842 7569 6c64 5573  geScratchBuildUs
-00000520: 6543 6173 652e 6275 696c 644e 290a da08  eCase.buildN)...
-00000530: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000540: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000550: 5f5f da07 5f5f 646f 635f 5f72 0200 0000  __..__doc__r....
-00000560: 720a 0000 0072 0300 0000 7204 0000 00da  r....r....r.....
-00000570: 0852 6573 706f 6e73 6572 1000 0000 7208  .Responser....r.
-00000580: 0000 0072 0800 0000 7208 0000 0072 0900  ...r....r....r..
-00000590: 0000 7205 0000 001c 0000 0073 0600 0000  ..r........s....
-000005a0: 0806 0402 0e06 7205 0000 0029 0bda 076c  ......r....)...l
-000005b0: 6f67 6769 6e67 da10 686f 746e 6573 732e  ogging..hotness.
-000005c0: 6275 696c 6465 7273 7202 0000 00da 1068  buildersr......h
-000005d0: 6f74 6e65 7373 2e72 6571 7565 7374 7372  otness.requestsr
-000005e0: 0300 0000 da07 686f 746e 6573 7372 0400  ......hotnessr..
-000005f0: 0000 da09 6765 744c 6f67 6765 7272 1a00  ....getLoggerr..
-00000600: 0000 7215 0000 0072 0500 0000 7208 0000  ..r....r....r...
-00000610: 0072 0800 0000 7208 0000 0072 0900 0000  .r....r....r....
-00000620: da08 3c6d 6f64 756c 653e 1200 0000 730a  ..<module>....s.
-00000630: 0000 0008 020c 010c 010c 030a 03         .............
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 436f 7079  f-8 -*-.#.# Copy
+00000020: 7269 6768 7420 2843 2920 3230 3231 2052  right (C) 2021 R
+00000030: 6564 2048 6174 2c20 496e 632e 0a23 0a23  ed Hat, Inc..#.#
+00000040: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000050: 2066 7265 6520 736f 6674 7761 7265 3b20   free software; 
+00000060: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000070: 6275 7465 2069 7420 616e 642f 6f72 0a23  bute it and/or.#
+00000080: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+00000090: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+000000a0: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+000000b0: 626c 6963 204c 6963 656e 7365 0a23 2061  blic License.# a
+000000c0: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
+000000d0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
+000000e0: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
+000000f0: 6865 7220 7665 7273 696f 6e20 320a 2320  her version 2.# 
+00000100: 6f66 2074 6865 204c 6963 656e 7365 2c20  of the License, 
+00000110: 6f72 2028 6174 2079 6f75 7220 6f70 7469  or (at your opti
+00000120: 6f6e 2920 616e 7920 6c61 7465 7220 7665  on) any later ve
+00000130: 7273 696f 6e2e 0a23 0a23 2054 6869 7320  rsion..#.# This 
+00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+00000170: 6265 2075 7365 6675 6c2c 0a23 2062 7574  be useful,.# but
+00000180: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+00000190: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+000001a0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+000001b0: 7761 7272 616e 7479 206f 660a 2320 4d45  warranty of.# ME
+000001c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000001d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000001e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000001f0: 452e 2020 5365 6520 7468 650a 2320 474e  E.  See the.# GN
+00000200: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000210: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
+00000220: 6520 6465 7461 696c 732e 0a23 0a23 2059  e details..#.# Y
+00000230: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000240: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+00000250: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 0a23 2061 6c6f 6e67 2077 6974 6820 7468  .# along with th
+00000280: 6973 2070 726f 6772 616d 3b20 6966 206e  is program; if n
+00000290: 6f74 2c20 7772 6974 6520 746f 2074 6865  ot, write to the
+000002a0: 2046 7265 6520 536f 6674 7761 7265 0a23   Free Software.#
+000002b0: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
+000002c0: 2e2c 2035 3120 4672 616e 6b6c 696e 2053  ., 51 Franklin S
+000002d0: 7472 6565 742c 2046 6966 7468 2046 6c6f  treet, Fifth Flo
+000002e0: 6f72 2c20 426f 7374 6f6e 2c20 4d41 2020  or, Boston, MA  
+000002f0: 3032 3131 302d 3133 3031 2c20 5553 412e  02110-1301, USA.
+00000300: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
+00000310: 0a66 726f 6d20 686f 746e 6573 732e 6275  .from hotness.bu
+00000320: 696c 6465 7273 2069 6d70 6f72 7420 4275  ilders import Bu
+00000330: 696c 6465 720a 6672 6f6d 2068 6f74 6e65  ilder.from hotne
+00000340: 7373 2e72 6571 7565 7374 7320 696d 706f  ss.requests impo
+00000350: 7274 2042 7569 6c64 5265 7175 6573 740a  rt BuildRequest.
+00000360: 6672 6f6d 2068 6f74 6e65 7373 2069 6d70  from hotness imp
+00000370: 6f72 7420 7265 7370 6f6e 7365 730a 0a0a  ort responses...
+00000380: 6c6f 6767 6572 203d 206c 6f67 6769 6e67  logger = logging
+00000390: 2e67 6574 4c6f 6767 6572 285f 5f6e 616d  .getLogger(__nam
+000003a0: 655f 5f29 0a0a 0a63 6c61 7373 2050 6163  e__)...class Pac
+000003b0: 6b61 6765 5363 7261 7463 6842 7569 6c64  kageScratchBuild
+000003c0: 5573 6543 6173 653a 0a20 2020 2022 2222  UseCase:.    """
+000003d0: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
+000003e0: 7265 7072 6573 656e 7473 2075 7365 2063  represents use c
+000003f0: 6173 6520 666f 7220 6275 696c 6469 6e67  ase for building
+00000400: 2074 6865 2070 6163 6b61 6765 2077 6974   the package wit
+00000410: 6820 7072 6f76 6964 6564 2062 7569 6c64  h provided build
+00000420: 6572 2e0a 0a20 2020 2041 7474 7269 6275  er...    Attribu
+00000430: 7465 733a 0a20 2020 2020 2020 2062 7569  tes:.        bui
+00000440: 6c64 6572 3a20 4275 696c 6465 7220 746f  lder: Builder to
+00000450: 2075 7365 2e0a 2020 2020 2222 220a 0a20   use..    """.. 
+00000460: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000470: 7365 6c66 2c20 6275 696c 6465 723a 2042  self, builder: B
+00000480: 7569 6c64 6572 293a 0a20 2020 2020 2020  uilder):.       
+00000490: 2022 2222 0a20 2020 2020 2020 2043 6c61   """.        Cla
+000004a0: 7373 2063 6f6e 7374 7275 6374 6f72 2e0a  ss constructor..
+000004b0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000004c0: 2020 2020 7365 6c66 2e62 7569 6c64 6572      self.builder
+000004d0: 203d 2062 7569 6c64 6572 0a0a 2020 2020   = builder..    
+000004e0: 6465 6620 6275 696c 6428 7365 6c66 2c20  def build(self, 
+000004f0: 7265 7175 6573 743a 2042 7569 6c64 5265  request: BuildRe
+00000500: 7175 6573 7429 202d 3e20 7265 7370 6f6e  quest) -> respon
+00000510: 7365 732e 5265 7370 6f6e 7365 3a0a 2020  ses.Response:.  
+00000520: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000530: 2020 4361 6c6c 2074 6865 2062 7569 6c64    Call the build
+00000540: 206d 6574 686f 6420 6f6e 2074 6865 2062   method on the b
+00000550: 7569 6c64 6572 2e0a 2020 2020 2020 2020  uilder..        
+00000560: 5468 6973 206d 6574 686f 6420 7769 6c6c  This method will
+00000570: 2068 616e 646c 6520 616e 7920 6572 726f   handle any erro
+00000580: 7220 7468 6174 2068 6170 7065 6e73 2077  r that happens w
+00000590: 6865 6e20 7374 6172 7469 6e67 2062 7569  hen starting bui
+000005a0: 6c64 2e0a 0a20 2020 2020 2020 2050 6172  ld...        Par
+000005b0: 616d 733a 0a20 2020 2020 2020 2020 2020  ams:.           
+000005c0: 2072 6571 7565 7374 3a20 5265 7175 6573   request: Reques
+000005d0: 7420 746f 2068 616e 646c 652e 0a0a 2020  t to handle...  
+000005e0: 2020 2020 2020 5265 7475 726e 3a0a 2020        Return:.  
+000005f0: 2020 2020 2020 2020 204f 7574 7075 7420           Output 
+00000600: 6f66 2074 6865 2062 7569 6c64 2e0a 2020  of the build..  
+00000610: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000620: 2020 6966 206e 6f74 2072 6571 7565 7374    if not request
+00000630: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000640: 7475 726e 2072 6573 706f 6e73 6573 2e52  turn responses.R
+00000650: 6573 706f 6e73 6546 6169 6c75 7265 2e69  esponseFailure.i
+00000660: 6e76 616c 6964 5f72 6571 7565 7374 5f65  nvalid_request_e
+00000670: 7272 6f72 2872 6571 7565 7374 290a 2020  rror(request).  
+00000680: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00000690: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+000006a0: 7365 6c66 2e62 7569 6c64 6572 2e62 7569  self.builder.bui
+000006b0: 6c64 2872 6571 7565 7374 2e70 6163 6b61  ld(request.packa
+000006c0: 6765 2c20 7265 7175 6573 742e 6f70 7473  ge, request.opts
+000006d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000006e0: 7475 726e 2072 6573 706f 6e73 6573 2e52  turn responses.R
+000006f0: 6573 706f 6e73 6553 7563 6365 7373 2872  esponseSuccess(r
+00000700: 6573 756c 7429 0a20 2020 2020 2020 2065  esult).        e
+00000710: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00000720: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
+00000730: 2020 2020 6c6f 6767 6572 2e65 7863 6570      logger.excep
+00000740: 7469 6f6e 2822 5061 636b 6167 6520 7363  tion("Package sc
+00000750: 7261 7463 6820 6275 696c 6420 7573 6520  ratch build use 
+00000760: 6361 7365 2066 6169 6c75 7265 222c 2065  case failure", e
+00000770: 7863 5f69 6e66 6f3d 5472 7565 290a 2020  xc_info=True).  
+00000780: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000790: 2072 6573 706f 6e73 6573 2e52 6573 706f   responses.Respo
+000007a0: 6e73 6546 6169 6c75 7265 2e62 7569 6c64  nseFailure.build
+000007b0: 6572 5f65 7272 6f72 2865 7863 290a       er_error(exc).
```

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/__pycache__/retrieve_data_use_case.cpython-38.pyc` & `the_new_hotness-1.2.4/hotness/use_cases/retrieve_data_use_case.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,125 @@
-00000000: 550d 0d0a 0000 0000 c070 9862 c707 0000  U........p.b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6500 a007 6508  d.l.m.Z...e...e.
-00000060: a101 5a09 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
-00000070: 5a0a 6401 5300 2907 e900 0000 004e 2901  Z.d.S.)......N).
-00000080: da08 4461 7461 6261 7365 2901 da13 5265  ..Database)...Re
-00000090: 7472 6965 7665 4461 7461 5265 7175 6573  trieveDataReques
-000000a0: 7429 01da 0972 6573 706f 6e73 6573 6300  t)...responsesc.
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000000c0: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
-000000d0: 6400 5a02 6401 5a03 6504 6402 9c01 6403  d.Z.d.Z.e.d...d.
-000000e0: 6404 8404 5a05 6506 6507 6a08 6405 9c02  d...Z.e.e.j.d...
-000000f0: 6406 6407 8404 5a09 6408 5300 2909 da13  d.d...Z.d.S.)...
-00000100: 5265 7472 6965 7665 4461 7461 5573 6543  RetrieveDataUseC
-00000110: 6173 657a 8a0a 2020 2020 5468 6973 2063  asez..    This c
-00000120: 6c61 7373 2072 6570 7265 7365 6e74 7320  lass represents 
-00000130: 7573 6520 6361 7365 2066 6f72 2072 6574  use case for ret
-00000140: 7269 6576 696e 6720 7661 6c75 6520 666f  rieving value fo
-00000150: 7220 6b65 7920 7573 696e 6720 6461 7461  r key using data
-00000160: 6261 7365 732e 0a0a 2020 2020 4174 7472  bases...    Attr
-00000170: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
-00000180: 6461 7461 6261 7365 3a20 4461 7461 6261  database: Databa
-00000190: 7365 2074 6f20 7573 652e 0a20 2020 20a9  se to use..    .
-000001a0: 01da 0864 6174 6162 6173 6563 0200 0000  ...databasec....
-000001b0: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-000001c0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
-000001d0: 0153 0029 027a 240a 2020 2020 2020 2020  .S.).z$.        
-000001e0: 436c 6173 7320 636f 6e73 7472 7563 746f  Class constructo
-000001f0: 722e 0a20 2020 2020 2020 204e 7206 0000  r..        Nr...
-00000200: 0029 02da 0473 656c 6672 0700 0000 a900  .)...selfr......
-00000210: 7209 0000 00fa 502f 7661 722f 686f 6d65  r.....P/var/home
-00000220: 2f7a 6c6f 7065 7a2f 6769 742f 7468 652d  /zlopez/git/the-
-00000230: 6e65 772d 686f 746e 6573 732f 686f 746e  new-hotness/hotn
-00000240: 6573 732f 7573 655f 6361 7365 732f 7265  ess/use_cases/re
-00000250: 7472 6965 7665 5f64 6174 615f 7573 655f  trieve_data_use_
-00000260: 6361 7365 2e70 79da 085f 5f69 6e69 745f  case.py..__init_
-00000270: 5f24 0000 0073 0200 0000 0004 7a1c 5265  _$...s......z.Re
-00000280: 7472 6965 7665 4461 7461 5573 6543 6173  trieveDataUseCas
-00000290: 652e 5f5f 696e 6974 5f5f 2902 da07 7265  e.__init__)...re
-000002a0: 7175 6573 74da 0672 6574 7572 6e63 0200  quest..returnc..
-000002b0: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-000002c0: 0000 4300 0000 7370 0000 007c 0173 1074  ..C...sp...|.s.t
-000002d0: 006a 01a0 027c 01a1 0153 007a 1a7c 006a  .j...|...S.z.|.j
-000002e0: 03a0 047c 016a 05a1 017d 0274 00a0 067c  ...|.j...}.t...|
-000002f0: 02a1 0157 0053 0004 0074 076b 0a72 6a01  ...W.S...t.k.rj.
-00000300: 007d 0301 007a 2274 086a 0964 0164 0264  .}...z"t.j.d.d.d
-00000310: 038d 0201 0074 006a 01a0 0a7c 03a1 0106  .....t.j...|....
-00000320: 0057 0059 00a2 0253 0064 047d 037e 0358  .W.Y...S.d.}.~.X
-00000330: 0059 006e 0258 0064 0453 0029 057a fb0a  .Y.n.X.d.S.).z..
-00000340: 2020 2020 2020 2020 4361 6c6c 2074 6865          Call the
-00000350: 2072 6574 7269 6576 6520 6d65 7468 6f64   retrieve method
-00000360: 206f 6e20 7468 6520 6461 7461 6261 7365   on the database
-00000370: 2e0a 2020 2020 2020 2020 5468 6973 206d  ..        This m
-00000380: 6574 686f 6420 7769 6c6c 2068 616e 646c  ethod will handl
-00000390: 6520 616e 7920 6572 726f 7220 7468 6174  e any error that
-000003a0: 2068 6170 7065 6e73 2077 6865 6e20 7265   happens when re
-000003b0: 7472 6965 7669 6e67 2064 6174 612e 0a0a  trieving data...
-000003c0: 2020 2020 2020 2020 5061 7261 6d73 3a0a          Params:.
-000003d0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-000003e0: 6573 743a 2052 6571 7565 7374 2074 6f20  est: Request to 
-000003f0: 6861 6e64 6c65 2e0a 0a20 2020 2020 2020  handle...       
-00000400: 2052 6574 7572 6e3a 0a20 2020 2020 2020   Return:.       
-00000410: 2020 2020 4f75 7470 7574 206f 6620 7468      Output of th
-00000420: 6520 6461 7461 2069 6e73 6572 7469 6f6e  e data insertion
-00000430: 2e0a 2020 2020 2020 2020 7a1e 5265 7472  ..        z.Retr
-00000440: 6965 7665 2064 6174 6120 7573 6520 6361  ieve data use ca
-00000450: 7365 2066 6169 6c75 7265 5429 01da 0865  se failureT)...e
-00000460: 7863 5f69 6e66 6f4e 290b 7204 0000 00da  xc_infoN).r.....
-00000470: 0f52 6573 706f 6e73 6546 6169 6c75 7265  .ResponseFailure
-00000480: da15 696e 7661 6c69 645f 7265 7175 6573  ..invalid_reques
-00000490: 745f 6572 726f 7272 0700 0000 da08 7265  t_errorr......re
-000004a0: 7472 6965 7665 da03 6b65 79da 0f52 6573  trieve..key..Res
-000004b0: 706f 6e73 6553 7563 6365 7373 da09 4578  ponseSuccess..Ex
-000004c0: 6365 7074 696f 6eda 066c 6f67 6765 72da  ception..logger.
-000004d0: 0965 7863 6570 7469 6f6e da0e 6461 7461  .exception..data
-000004e0: 6261 7365 5f65 7272 6f72 2904 7208 0000  base_error).r...
-000004f0: 0072 0c00 0000 da06 7265 7375 6c74 da03  .r......result..
-00000500: 6578 6372 0900 0000 7209 0000 0072 0a00  excr....r....r..
-00000510: 0000 7211 0000 002a 0000 0073 1000 0000  ..r....*...s....
-00000520: 000b 0401 0c01 0201 0e01 0c01 1001 0e01  ................
-00000530: 7a1c 5265 7472 6965 7665 4461 7461 5573  z.RetrieveDataUs
-00000540: 6543 6173 652e 7265 7472 6965 7665 4e29  eCase.retrieveN)
-00000550: 0ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000560: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000570: 616d 655f 5fda 075f 5f64 6f63 5f5f 7202  ame__..__doc__r.
-00000580: 0000 0072 0b00 0000 7203 0000 0072 0400  ...r....r....r..
-00000590: 0000 da08 5265 7370 6f6e 7365 7211 0000  ....Responser...
-000005a0: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-000005b0: 720a 0000 0072 0500 0000 1c00 0000 7306  r....r........s.
-000005c0: 0000 0008 0104 070e 0672 0500 0000 290b  .........r....).
-000005d0: da07 6c6f 6767 696e 67da 1168 6f74 6e65  ..logging..hotne
-000005e0: 7373 2e64 6174 6162 6173 6573 7202 0000  ss.databasesr...
-000005f0: 00da 1068 6f74 6e65 7373 2e72 6571 7565  ...hotness.reque
-00000600: 7374 7372 0300 0000 da07 686f 746e 6573  stsr......hotnes
-00000610: 7372 0400 0000 da09 6765 744c 6f67 6765  sr......getLogge
-00000620: 7272 1a00 0000 7215 0000 0072 0500 0000  rr....r....r....
-00000630: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00000640: 0a00 0000 da08 3c6d 6f64 756c 653e 1200  ......<module>..
-00000650: 0000 730a 0000 0008 020c 010c 010c 030a  ..s.............
-00000660: 03                                       .
+00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
+00000010: 662d 3820 2d2a 2d0a 230a 2320 436f 7079  f-8 -*-.#.# Copy
+00000020: 7269 6768 7420 2843 2920 3230 3231 2052  right (C) 2021 R
+00000030: 6564 2048 6174 2c20 496e 632e 0a23 0a23  ed Hat, Inc..#.#
+00000040: 2054 6869 7320 7072 6f67 7261 6d20 6973   This program is
+00000050: 2066 7265 6520 736f 6674 7761 7265 3b20   free software; 
+00000060: 796f 7520 6361 6e20 7265 6469 7374 7269  you can redistri
+00000070: 6275 7465 2069 7420 616e 642f 6f72 0a23  bute it and/or.#
+00000080: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+00000090: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+000000a0: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+000000b0: 626c 6963 204c 6963 656e 7365 0a23 2061  blic License.# a
+000000c0: 7320 7075 626c 6973 6865 6420 6279 2074  s published by t
+000000d0: 6865 2046 7265 6520 536f 6674 7761 7265  he Free Software
+000000e0: 2046 6f75 6e64 6174 696f 6e3b 2065 6974   Foundation; eit
+000000f0: 6865 7220 7665 7273 696f 6e20 320a 2320  her version 2.# 
+00000100: 6f66 2074 6865 204c 6963 656e 7365 2c20  of the License, 
+00000110: 6f72 2028 6174 2079 6f75 7220 6f70 7469  or (at your opti
+00000120: 6f6e 2920 616e 7920 6c61 7465 7220 7665  on) any later ve
+00000130: 7273 696f 6e2e 0a23 0a23 2054 6869 7320  rsion..#.# This 
+00000140: 7072 6f67 7261 6d20 6973 2064 6973 7472  program is distr
+00000150: 6962 7574 6564 2069 6e20 7468 6520 686f  ibuted in the ho
+00000160: 7065 2074 6861 7420 6974 2077 696c 6c20  pe that it will 
+00000170: 6265 2075 7365 6675 6c2c 0a23 2062 7574  be useful,.# but
+00000180: 2057 4954 484f 5554 2041 4e59 2057 4152   WITHOUT ANY WAR
+00000190: 5241 4e54 593b 2077 6974 686f 7574 2065  RANTY; without e
+000001a0: 7665 6e20 7468 6520 696d 706c 6965 6420  ven the implied 
+000001b0: 7761 7272 616e 7479 206f 660a 2320 4d45  warranty of.# ME
+000001c0: 5243 4841 4e54 4142 494c 4954 5920 6f72  RCHANTABILITY or
+000001d0: 2046 4954 4e45 5353 2046 4f52 2041 2050   FITNESS FOR A P
+000001e0: 4152 5449 4355 4c41 5220 5055 5250 4f53  ARTICULAR PURPOS
+000001f0: 452e 2020 5365 6520 7468 650a 2320 474e  E.  See the.# GN
+00000200: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00000210: 204c 6963 656e 7365 2066 6f72 206d 6f72   License for mor
+00000220: 6520 6465 7461 696c 732e 0a23 0a23 2059  e details..#.# Y
+00000230: 6f75 2073 686f 756c 6420 6861 7665 2072  ou should have r
+00000240: 6563 6569 7665 6420 6120 636f 7079 206f  eceived a copy o
+00000250: 6620 7468 6520 474e 5520 4765 6e65 7261  f the GNU Genera
+00000260: 6c20 5075 626c 6963 204c 6963 656e 7365  l Public License
+00000270: 0a23 2061 6c6f 6e67 2077 6974 6820 7468  .# along with th
+00000280: 6973 2070 726f 6772 616d 3b20 6966 206e  is program; if n
+00000290: 6f74 2c20 7772 6974 6520 746f 2074 6865  ot, write to the
+000002a0: 2046 7265 6520 536f 6674 7761 7265 0a23   Free Software.#
+000002b0: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
+000002c0: 2e2c 2035 3120 4672 616e 6b6c 696e 2053  ., 51 Franklin S
+000002d0: 7472 6565 742c 2046 6966 7468 2046 6c6f  treet, Fifth Flo
+000002e0: 6f72 2c20 426f 7374 6f6e 2c20 4d41 2020  or, Boston, MA  
+000002f0: 3032 3131 302d 3133 3031 2c20 5553 412e  02110-1301, USA.
+00000300: 0a69 6d70 6f72 7420 6c6f 6767 696e 670a  .import logging.
+00000310: 0a66 726f 6d20 686f 746e 6573 732e 6461  .from hotness.da
+00000320: 7461 6261 7365 7320 696d 706f 7274 2044  tabases import D
+00000330: 6174 6162 6173 650a 6672 6f6d 2068 6f74  atabase.from hot
+00000340: 6e65 7373 2e72 6571 7565 7374 7320 696d  ness.requests im
+00000350: 706f 7274 2052 6574 7269 6576 6544 6174  port RetrieveDat
+00000360: 6152 6571 7565 7374 0a66 726f 6d20 686f  aRequest.from ho
+00000370: 746e 6573 7320 696d 706f 7274 2072 6573  tness import res
+00000380: 706f 6e73 6573 0a0a 0a6c 6f67 6765 7220  ponses...logger 
+00000390: 3d20 6c6f 6767 696e 672e 6765 744c 6f67  = logging.getLog
+000003a0: 6765 7228 5f5f 6e61 6d65 5f5f 290a 0a0a  ger(__name__)...
+000003b0: 636c 6173 7320 5265 7472 6965 7665 4461  class RetrieveDa
+000003c0: 7461 5573 6543 6173 653a 0a20 2020 2022  taUseCase:.    "
+000003d0: 2222 0a20 2020 2054 6869 7320 636c 6173  "".    This clas
+000003e0: 7320 7265 7072 6573 656e 7473 2075 7365  s represents use
+000003f0: 2063 6173 6520 666f 7220 7265 7472 6965   case for retrie
+00000400: 7669 6e67 2076 616c 7565 2066 6f72 206b  ving value for k
+00000410: 6579 2075 7369 6e67 2064 6174 6162 6173  ey using databas
+00000420: 6573 2e0a 0a20 2020 2041 7474 7269 6275  es...    Attribu
+00000430: 7465 733a 0a20 2020 2020 2020 2064 6174  tes:.        dat
+00000440: 6162 6173 653a 2044 6174 6162 6173 6520  abase: Database 
+00000450: 746f 2075 7365 2e0a 2020 2020 2222 220a  to use..    """.
+00000460: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00000470: 5f28 7365 6c66 2c20 6461 7461 6261 7365  _(self, database
+00000480: 3a20 4461 7461 6261 7365 293a 0a20 2020  : Database):.   
+00000490: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000004a0: 2043 6c61 7373 2063 6f6e 7374 7275 6374   Class construct
+000004b0: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
+000004c0: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+000004d0: 6162 6173 6520 3d20 6461 7461 6261 7365  abase = database
+000004e0: 0a0a 2020 2020 6465 6620 7265 7472 6965  ..    def retrie
+000004f0: 7665 2873 656c 662c 2072 6571 7565 7374  ve(self, request
+00000500: 3a20 5265 7472 6965 7665 4461 7461 5265  : RetrieveDataRe
+00000510: 7175 6573 7429 202d 3e20 7265 7370 6f6e  quest) -> respon
+00000520: 7365 732e 5265 7370 6f6e 7365 3a0a 2020  ses.Response:.  
+00000530: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000540: 2020 4361 6c6c 2074 6865 2072 6574 7269    Call the retri
+00000550: 6576 6520 6d65 7468 6f64 206f 6e20 7468  eve method on th
+00000560: 6520 6461 7461 6261 7365 2e0a 2020 2020  e database..    
+00000570: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
+00000580: 7769 6c6c 2068 616e 646c 6520 616e 7920  will handle any 
+00000590: 6572 726f 7220 7468 6174 2068 6170 7065  error that happe
+000005a0: 6e73 2077 6865 6e20 7265 7472 6965 7669  ns when retrievi
+000005b0: 6e67 2064 6174 612e 0a0a 2020 2020 2020  ng data...      
+000005c0: 2020 5061 7261 6d73 3a0a 2020 2020 2020    Params:.      
+000005d0: 2020 2020 2020 7265 7175 6573 743a 2052        request: R
+000005e0: 6571 7565 7374 2074 6f20 6861 6e64 6c65  equest to handle
+000005f0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00000600: 6e3a 0a20 2020 2020 2020 2020 2020 4f75  n:.           Ou
+00000610: 7470 7574 206f 6620 7468 6520 6461 7461  tput of the data
+00000620: 2069 6e73 6572 7469 6f6e 2e0a 2020 2020   insertion..    
+00000630: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00000640: 6966 206e 6f74 2072 6571 7565 7374 3a0a  if not request:.
+00000650: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000660: 726e 2072 6573 706f 6e73 6573 2e52 6573  rn responses.Res
+00000670: 706f 6e73 6546 6169 6c75 7265 2e69 6e76  ponseFailure.inv
+00000680: 616c 6964 5f72 6571 7565 7374 5f65 7272  alid_request_err
+00000690: 6f72 2872 6571 7565 7374 290a 2020 2020  or(request).    
+000006a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000006b0: 2020 2020 2072 6573 756c 7420 3d20 7365       result = se
+000006c0: 6c66 2e64 6174 6162 6173 652e 7265 7472  lf.database.retr
+000006d0: 6965 7665 2872 6571 7565 7374 2e6b 6579  ieve(request.key
+000006e0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000006f0: 7475 726e 2072 6573 706f 6e73 6573 2e52  turn responses.R
+00000700: 6573 706f 6e73 6553 7563 6365 7373 2872  esponseSuccess(r
+00000710: 6573 756c 7429 0a20 2020 2020 2020 2065  esult).        e
+00000720: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00000730: 6173 2065 7863 3a0a 2020 2020 2020 2020  as exc:.        
+00000740: 2020 2020 6c6f 6767 6572 2e65 7863 6570      logger.excep
+00000750: 7469 6f6e 2822 5265 7472 6965 7665 2064  tion("Retrieve d
+00000760: 6174 6120 7573 6520 6361 7365 2066 6169  ata use case fai
+00000770: 6c75 7265 222c 2065 7863 5f69 6e66 6f3d  lure", exc_info=
+00000780: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00000790: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+000007a0: 6573 2e52 6573 706f 6e73 6546 6169 6c75  es.ResponseFailu
+000007b0: 7265 2e64 6174 6162 6173 655f 6572 726f  re.database_erro
+000007c0: 7228 6578 6329 0a                        r(exc).
```

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/insert_data_use_case.py` & `the_new_hotness-1.2.4/hotness/use_cases/insert_data_use_case.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/notify_user_use_case.py` & `the_new_hotness-1.2.4/hotness/use_cases/notify_user_use_case.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/use_cases/package_check_use_case.py` & `the_new_hotness-1.2.4/hotness/use_cases/package_check_use_case.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/validators/__init__.py` & `the_new_hotness-1.2.4/hotness/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/validators/mdapi.py` & `the_new_hotness-1.2.4/hotness/validators/mdapi.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/validators/pagure.py` & `the_new_hotness-1.2.4/hotness/validators/pagure.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/validators/pdc.py` & `the_new_hotness-1.2.4/hotness/validators/pdc.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/hotness/validators/validator.py` & `the_new_hotness-1.2.4/hotness/validators/validator.py`

 * *Files identical despite different names*

### Comparing `the_new_hotness-1.2.3/pyproject.toml` & `the_new_hotness-1.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -56,27 +56,28 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "the-new-hotness"
-version = "1.2.3"
+version = "1.2.4"
 description = "A fedora messaging consumer that files bugzilla bugs for upstream releases"
 authors = ["Ralph Bean <rbean@redhat.com>"]
 maintainers = ["Michal Konecny <mkonecny@redhat.com>"]
 readme = "README.rst"
 homepage = "https://github.com/fedora-infra/the-new-hotness"
 documentation = "https://the-new-hotness.readthedocs.io"
 repository = "https://github.com/fedora-infra/the-new-hotness"
 license = "GPL-2.0-or-later"
 classifiers = [
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10"
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11"
 ]
 include = [
   "LICENSE", "README.rst",
   "config/config.toml.example"
 ]
 packages = [
   { include = "hotness" }
@@ -99,17 +100,21 @@
 diff-cover = "^7.0.1"
 flake8 = "^6.0.0"
 mock = "^5.0.0"
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 
 # Required to test building the docs
-Sphinx = "^6.0.0"
+Sphinx = "^7.0.0"
 
 # Mypy test requirements
 mypy = "^1.0"
 types-requests = "^2.28.11"
 types-redis = "^4.3.21"
 
+[tool.poetry.group.dev.dependencies]
+towncrier = "^22.12.0"
+tox = "^4.5.1"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `the_new_hotness-1.2.3/setup.py` & `the_new_hotness-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'koji>=1.30.0,<2.0.0',
  'python-bugzilla>=3.2.0,<4.0.0',
  'redis>=4.3.4,<5.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'the-new-hotness',
-    'version': '1.2.3',
+    'version': '1.2.4',
     'description': 'A fedora messaging consumer that files bugzilla bugs for upstream releases',
     'long_description': ".. image:: https://img.shields.io/pypi/v/the-new-hotness.svg\n  :target: https://pypi.org/project/the-new-hotness/\n\n.. image:: https://readthedocs.org/projects/the-new-hotness/badge/?version=latest\n  :alt: Documentation Status\n  :target: https://the-new-hotness.readthedocs.io/en/latest/?badge=latest\n\nthe-new-hotness\n---------------\n\n`Fedora-messaging <https://github.com/fedora-infra/fedora-messaging>`_ consumer that listens to `release-monitoring.org\n<http://release-monitoring.org>`_ and files bugzilla bugs in response (to\nnotify packagers that they can update their packages).\n\nFor additional information see `documentation <https://the-new-hotness.readthedocs.io/en/stable/>`_.\n\nSeeing it in action\n^^^^^^^^^^^^^^^^^^^\n\nTo see recent messages from the-new-hotness:\n\n* Check Fedora's `datagrepper\n  <https://apps.fedoraproject.org/datagrepper/raw?category=hotness&delta=2592000>`_\n\n* Or join #fedora-fedmsg IRC channel on `libera <https://libera.chat/>`_ and watch for ``hotness``\n  messages.\n\nTo see recent koji builds started by the-new-hotness:\n\n* Check Fedora's `koji builds\n  <https://koji.fedoraproject.org/koji/tasks?owner=the-new-hotness/release-monitoring.org&state=all>`_\n\nDevelopment\n^^^^^^^^^^^\n\nContributions are welcome, check out `contribution guidelines <https://the-new-hotness.readthedocs.io/en/stable/dev-guide.html#contribution-guidelines>`_.\n",
     'author': 'Ralph Bean',
     'author_email': 'rbean@redhat.com',
     'maintainer': 'Michal Konecny',
     'maintainer_email': 'mkonecny@redhat.com',
     'url': 'https://github.com/fedora-infra/the-new-hotness',
```

### Comparing `the_new_hotness-1.2.3/PKG-INFO` & `the_new_hotness-1.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: the-new-hotness
-Version: 1.2.3
+Version: 1.2.4
 Summary: A fedora messaging consumer that files bugzilla bugs for upstream releases
 Home-page: https://github.com/fedora-infra/the-new-hotness
 License: GPL-2.0-or-later
 Author: Ralph Bean
 Author-email: rbean@redhat.com
 Maintainer: Michal Konecny
 Maintainer-email: mkonecny@redhat.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: anitya-schema (>=2.0.1,<3.0.0)
 Requires-Dist: fedora-messaging (>=3.1.0,<4.0.0)
 Requires-Dist: fedora-messaging-the-new-hotness-schema (>=1.1.2,<2.0.0)
 Requires-Dist: koji (>=1.30.0,<2.0.0)
 Requires-Dist: python-bugzilla (>=3.2.0,<4.0.0)
```

