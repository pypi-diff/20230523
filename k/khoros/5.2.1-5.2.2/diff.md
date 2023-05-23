# Comparing `tmp/khoros-5.2.1.tar.gz` & `tmp/khoros-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khoros-5.2.1.tar", last modified: Mon Jan  2 19:16:52 2023, max compression
+gzip compressed data, was "khoros-5.2.2.tar", last modified: Tue May 23 21:10:34 2023, max compression
```

## Comparing `khoros-5.2.1.tar` & `khoros-5.2.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.910569 khoros-5.2.1/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.2.1/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-01-02 19:16:52.910172 khoros-5.2.1/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.2.1/README.md
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.846464 khoros-5.2.1/khoros/
--rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    71382 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11278 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/auth.py
--rw-r--r--   0 shurtj     (501) staff       (20)    14393 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)   275817 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.853150 khoros-5.2.1/khoros/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.2.1/khoros/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11124 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.2.1/khoros/errors/translations.py
--rw-r--r--   0 shurtj     (501) staff       (20)    22871 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/liql.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.871722 khoros-5.2.1/khoros/objects/
--rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.2.1/khoros/objects/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.2.1/khoros/objects/albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/objects/archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.2.1/khoros/objects/attachments.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/objects/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)      519 2021-10-11 04:30:21.000000 khoros-5.2.1/khoros/objects/labels.py
--rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.2.1/khoros/objects/messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/objects/roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.2.1/khoros/objects/settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.2.1/khoros/objects/subscriptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/objects/tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/objects/users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/saml.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.883888 khoros-5.2.1/khoros/structures/
--rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/structures/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.2.1/khoros/structures/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27629 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/structures/boards.py
--rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.2.1/khoros/structures/categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/structures/communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/structures/grouphubs.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.2.1/khoros/structures/nodes.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.886323 khoros-5.2.1/khoros/studio/
--rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.2.1/khoros/studio/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2880 2020-10-30 02:28:27.000000 khoros-5.2.1/khoros/studio/base.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.891376 khoros-5.2.1/khoros/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.2.1/khoros/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/environment.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.909064 khoros-5.2.1/khoros/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.2.1/khoros/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/utils/tests/test_archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_board_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/utils/tests/test_bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.2.1/khoros/utils/tests/test_categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.2.1/khoros/utils/tests/test_communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_error_handling.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.2.1/khoros/utils/tests/test_exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_grouphub_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_helper_file.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_http_headers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_library_import.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.2.1/khoros/utils/tests/test_liql.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_mentions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_node_id_extract.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.2.1/khoros/utils/tests/test_ssl_verify.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_studio.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.2.1/khoros/utils/tests/test_users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.2.1/khoros/utils/tests/test_version.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3786 2023-01-02 18:07:54.000000 khoros-5.2.1/khoros/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-01-02 19:16:52.849352 khoros-5.2.1/khoros.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-01-02 19:16:52.000000 khoros-5.2.1/khoros.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-01-02 19:16:52.000000 khoros-5.2.1/khoros.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-01-02 19:16:52.000000 khoros-5.2.1/khoros.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-01-02 19:16:52.000000 khoros-5.2.1/khoros.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-01-02 19:16:52.000000 khoros-5.2.1/khoros.egg-info/top_level.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      863 2023-01-02 18:47:48.000000 khoros-5.2.1/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-01-02 19:16:52.910658 khoros-5.2.1/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.2.1/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.582821 khoros-5.2.2/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.2.2/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-05-23 21:10:34.582563 khoros-5.2.2/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.2.2/README.md
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.530787 khoros-5.2.2/khoros/
+-rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    71382 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11278 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/auth.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14393 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)   275817 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.537177 khoros-5.2.2/khoros/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.2.2/khoros/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11124 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.2.2/khoros/errors/translations.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    22871 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/liql.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.552338 khoros-5.2.2/khoros/objects/
+-rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.2.2/khoros/objects/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/objects/albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/objects/archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/objects/attachments.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/objects/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      519 2021-10-11 04:30:21.000000 khoros-5.2.2/khoros/objects/labels.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/objects/messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/objects/roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.2.2/khoros/objects/settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.2.2/khoros/objects/subscriptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/objects/tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/objects/users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/saml.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.559944 khoros-5.2.2/khoros/structures/
+-rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/structures/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27629 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/boards.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/structures/categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/grouphubs.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.2.2/khoros/structures/nodes.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.562274 khoros-5.2.2/khoros/studio/
+-rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.2.2/khoros/studio/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2880 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/studio/base.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.566354 khoros-5.2.2/khoros/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.2.2/khoros/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/environment.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.581698 khoros-5.2.2/khoros/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.2.2/khoros/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_board_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.2.2/khoros/utils/tests/test_categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/utils/tests/test_communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_error_handling.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_grouphub_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_helper_file.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_http_headers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_library_import.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/utils/tests/test_liql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_mentions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_node_id_extract.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_ssl_verify.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_studio.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/utils/tests/test_version.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3786 2023-05-23 20:51:39.000000 khoros-5.2.2/khoros/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.533414 khoros-5.2.2/khoros.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/top_level.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      913 2023-05-23 20:51:39.000000 khoros-5.2.2/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-23 21:10:34.582898 khoros-5.2.2/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.2.2/setup.py
```

### Comparing `khoros-5.2.1/LICENSE` & `khoros-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/PKG-INFO` & `khoros-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.2.1
+Version: 5.2.2
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.2.1 Summary: Useful tools and
+Metadata-Version: 2.1 Name: khoros Version: 5.2.2 Summary: Useful tools and
 utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
```

### Comparing `khoros-5.2.1/README.md` & `khoros-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/__init__.py` & `khoros-5.2.2/khoros/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/api.py` & `khoros-5.2.2/khoros/api.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/auth.py` & `khoros-5.2.2/khoros/auth.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/bulk_data.py` & `khoros-5.2.2/khoros/bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/core.py` & `khoros-5.2.2/khoros/core.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/errors/__init__.py` & `khoros-5.2.2/khoros/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/errors/exceptions.py` & `khoros-5.2.2/khoros/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/errors/handlers.py` & `khoros-5.2.2/khoros/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/errors/translations.py` & `khoros-5.2.2/khoros/errors/translations.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/liql.py` & `khoros-5.2.2/khoros/liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/__init__.py` & `khoros-5.2.2/khoros/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/albums.py` & `khoros-5.2.2/khoros/objects/albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/archives.py` & `khoros-5.2.2/khoros/objects/archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/attachments.py` & `khoros-5.2.2/khoros/objects/attachments.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/base.py` & `khoros-5.2.2/khoros/objects/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/labels.py` & `khoros-5.2.2/khoros/objects/labels.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/messages.py` & `khoros-5.2.2/khoros/objects/messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/roles.py` & `khoros-5.2.2/khoros/objects/roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/settings.py` & `khoros-5.2.2/khoros/objects/settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/subscriptions.py` & `khoros-5.2.2/khoros/objects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/tags.py` & `khoros-5.2.2/khoros/objects/tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/objects/users.py` & `khoros-5.2.2/khoros/objects/users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/saml.py` & `khoros-5.2.2/khoros/saml.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/__init__.py` & `khoros-5.2.2/khoros/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/base.py` & `khoros-5.2.2/khoros/structures/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/boards.py` & `khoros-5.2.2/khoros/structures/boards.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/categories.py` & `khoros-5.2.2/khoros/structures/categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/communities.py` & `khoros-5.2.2/khoros/structures/communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/grouphubs.py` & `khoros-5.2.2/khoros/structures/grouphubs.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/structures/nodes.py` & `khoros-5.2.2/khoros/structures/nodes.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/studio/base.py` & `khoros-5.2.2/khoros/studio/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/core_utils.py` & `khoros-5.2.2/khoros/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/environment.py` & `khoros-5.2.2/khoros/utils/environment.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/helper.py` & `khoros-5.2.2/khoros/utils/helper.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/log_utils.py` & `khoros-5.2.2/khoros/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/resources.py` & `khoros-5.2.2/khoros/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_albums.py` & `khoros-5.2.2/khoros/utils/tests/test_albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_archives.py` & `khoros-5.2.2/khoros/utils/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_board_creation.py` & `khoros-5.2.2/khoros/utils/tests/test_board_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_bulk_data.py` & `khoros-5.2.2/khoros/utils/tests/test_bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_categories.py` & `khoros-5.2.2/khoros/utils/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_communities.py` & `khoros-5.2.2/khoros/utils/tests/test_communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_core_utils.py` & `khoros-5.2.2/khoros/utils/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_error_handling.py` & `khoros-5.2.2/khoros/utils/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_exceptions.py` & `khoros-5.2.2/khoros/utils/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_grouphub_creation.py` & `khoros-5.2.2/khoros/utils/tests/test_grouphub_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_helper_file.py` & `khoros-5.2.2/khoros/utils/tests/test_helper_file.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_http_headers.py` & `khoros-5.2.2/khoros/utils/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_library_import.py` & `khoros-5.2.2/khoros/utils/tests/test_library_import.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_liql.py` & `khoros-5.2.2/khoros/utils/tests/test_liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_mentions.py` & `khoros-5.2.2/khoros/utils/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_messages.py` & `khoros-5.2.2/khoros/utils/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_node_id_extract.py` & `khoros-5.2.2/khoros/utils/tests/test_node_id_extract.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_roles.py` & `khoros-5.2.2/khoros/utils/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_settings.py` & `khoros-5.2.2/khoros/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_ssl_verify.py` & `khoros-5.2.2/khoros/utils/tests/test_ssl_verify.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_studio.py` & `khoros-5.2.2/khoros/utils/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_tags.py` & `khoros-5.2.2/khoros/utils/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_users.py` & `khoros-5.2.2/khoros/utils/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/tests/test_version.py` & `khoros-5.2.2/khoros/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/khoros/utils/version.py` & `khoros-5.2.2/khoros/utils/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 """
 :Module:            khoros.utils.version
 :Synopsis:          This simple script contains the package version
 :Usage:             ``from .utils import version``
 :Example:           ``__version__ = version.get_full_version()``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     02 Jan 2023
+:Modified Date:     23 May 2023
 """
 
 import json
 import urllib.request
 
 from . import log_utils
 
 # Define special and global variables
-__version__ = "5.2.1"
+__version__ = "5.2.2"
 latest_version_reported = False
 logger = log_utils.initialize_logging(__name__)
 
 
 def get_full_version():
     """This function returns the current full version of the khoros package."""
     return __version__
```

### Comparing `khoros-5.2.1/khoros.egg-info/PKG-INFO` & `khoros-5.2.2/khoros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.2.1
+Version: 5.2.2
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.2.1 Summary: Useful tools and
+Metadata-Version: 2.1 Name: khoros Version: 5.2.2 Summary: Useful tools and
 utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
```

### Comparing `khoros-5.2.1/khoros.egg-info/SOURCES.txt` & `khoros-5.2.2/khoros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khoros-5.2.1/pyproject.toml` & `khoros-5.2.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "khoros"
-version = "5.2.1"
+version = "5.2.2"
 description = "Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment."
 authors = ["Jeff Shurtliff <jeff.shurtliff@rsa.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 defusedxml = ">=0.7.1"
 pytest = {version = ">=7.2.0", markers = "python_version > \"3.7\""}
 pyyaml = ">=5.3.1"
 urllib3 = ">=1.26.2,<1.27.0"
-requests = ">=2.23.0"
+requests = {version = ">=2.31.0", markers = "python_version > \"3.6\""}
 setuptools = {version = ">=65.5.1,<65.6.0", markers = "python_version > \"3.6\""}
 sphinx = ">=5.3.0"
 sphinxcontrib-applehelp = ">=1.0.2"
 sphinxcontrib-devhelp = ">=1.0.2"
 sphinxcontrib-htmlhelp = ">=2.0.0"
 sphinxcontrib-jsmath = ">=1.0.1"
 sphinxcontrib-qthelp = ">=1.0.3"
```

### Comparing `khoros-5.2.1/setup.py` & `khoros-5.2.2/setup.py`

 * *Files identical despite different names*

