# Comparing `tmp/seven_studio-1.4.0.tar.gz` & `tmp/seven_studio-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seven_studio-1.4.0.tar", last modified: Fri Apr 28 07:40:19 2023, max compression
+gzip compressed data, was "dist/seven_studio-1.5.0.tar", last modified: Tue May 23 07:45:43 2023, max compression
```

## Comparing `seven_studio-1.4.0.tar` & `seven_studio-1.5.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.818382 seven_studio-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     3015 2023-04-28 07:40:19.818382 seven_studio-1.4.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1556 2023-04-28 07:39:41.000000 seven_studio-1.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 07:40:19.818382 seven_studio-1.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1262 2023-04-28 07:39:41.000000 seven_studio-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.801374 seven_studio-1.4.0/seven_studio/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.804376 seven_studio-1.4.0/seven_studio/handlers/
--rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    26036 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/studio_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.805376 seven_studio-1.4.0/seven_studio/handlers/system/
--rwxrwxrwx   0 root         (0) root         (0)      224 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9452 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/core.py
--rwxrwxrwx   0 root         (0) root         (0)    22072 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/file.py
--rwxrwxrwx   0 root         (0) root         (0)    17655 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/menu.py
--rwxrwxrwx   0 root         (0) root         (0)    32048 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/power.py
--rwxrwxrwx   0 root         (0) root         (0)     6678 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/product.py
--rwxrwxrwx   0 root         (0) root         (0)     2636 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/handlers/system/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.806377 seven_studio-1.4.0/seven_studio/libs/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.808378 seven_studio-1.4.0/seven_studio/libs/file/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8612 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/bos.py
--rwxrwxrwx   0 root         (0) root         (0)     8613 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/cos.py
--rwxrwxrwx   0 root         (0) root         (0)    19074 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/ks3.py
--rwxrwxrwx   0 root         (0) root         (0)     9588 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/oss2.py
--rwxrwxrwx   0 root         (0) root         (0)     8593 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/s3.py
--rwxrwxrwx   0 root         (0) root         (0)    14037 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/file/upload.py
--rwxrwxrwx   0 root         (0) root         (0)     6306 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/libs/geetest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.810378 seven_studio-1.4.0/seven_studio/models/
--rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.810378 seven_studio-1.4.0/seven_studio/models/db_models/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.812379 seven_studio-1.4.0/seven_studio/models/db_models/file/
--rwxrwxrwx   0 root         (0) root         (0)      308 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1492 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_history_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_resource_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2433 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1578 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_pic_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1451 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_storage_path_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/file/file_water_image_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.812379 seven_studio-1.4.0/seven_studio/models/db_models/log/
--rwxrwxrwx   0 root         (0) root         (0)       29 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/log/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1298 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/log/log_action_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.813380 seven_studio-1.4.0/seven_studio/models/db_models/menu/
--rwxrwxrwx   0 root         (0) root         (0)       67 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1583 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_cote_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2174 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)    19404 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model_ex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.814381 seven_studio-1.4.0/seven_studio/models/db_models/product/
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/product_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/product/product_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.816381 seven_studio-1.4.0/seven_studio/models/db_models/role/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1014 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model.py
--rwxrwxrwx   0 root         (0) root         (0)      952 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1036 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/role/role_user_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.816381 seven_studio-1.4.0/seven_studio/models/db_models/settings/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/settings/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1152 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/settings/settings_base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.817382 seven_studio-1.4.0/seven_studio/models/db_models/user/
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2025 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model.py
--rwxrwxrwx   0 root         (0) root         (0)     1148 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model_ex.py
--rwxrwxrwx   0 root         (0) root         (0)     1035 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/db_models/user/user_login_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2933 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/dto_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2419 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/enum.py
--rwxrwxrwx   0 root         (0) root         (0)    37633 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/power_model.py
--rwxrwxrwx   0 root         (0) root         (0)     2689 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/models/seven_model.py
--rwxrwxrwx   0 root         (0) root         (0)     4391 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.818382 seven_studio-1.4.0/seven_studio/utils/
--rwxrwxrwx   0 root         (0) root         (0)      156 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1959 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/dict.py
--rwxrwxrwx   0 root         (0) root         (0)      637 2023-04-28 07:39:41.000000 seven_studio-1.4.0/seven_studio/utils/random.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:40:19.803375 seven_studio-1.4.0/seven_studio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3015 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2636 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 07:40:19.000000 seven_studio-1.4.0/seven_studio.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.016873 seven_studio-1.5.0/
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-05-23 07:45:43.015872 seven_studio-1.5.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1616 2023-05-23 07:44:57.000000 seven_studio-1.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 07:45:43.016873 seven_studio-1.5.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1262 2023-05-23 07:44:57.000000 seven_studio-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.971850 seven_studio-1.5.0/seven_studio/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.976853 seven_studio-1.5.0/seven_studio/handlers/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    26037 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/studio_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.980855 seven_studio-1.5.0/seven_studio/handlers/system/
+-rwxrwxrwx   0 root         (0) root         (0)      224 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9452 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/core.py
+-rwxrwxrwx   0 root         (0) root         (0)    22072 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/file.py
+-rwxrwxrwx   0 root         (0) root         (0)    17655 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/menu.py
+-rwxrwxrwx   0 root         (0) root         (0)    32048 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/power.py
+-rwxrwxrwx   0 root         (0) root         (0)     6678 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/product.py
+-rwxrwxrwx   0 root         (0) root         (0)     2636 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/handlers/system/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.983856 seven_studio-1.5.0/seven_studio/libs/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.987858 seven_studio-1.5.0/seven_studio/libs/file/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8612 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/bos.py
+-rwxrwxrwx   0 root         (0) root         (0)     8613 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/cos.py
+-rwxrwxrwx   0 root         (0) root         (0)    19074 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/ks3.py
+-rwxrwxrwx   0 root         (0) root         (0)     9588 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/oss2.py
+-rwxrwxrwx   0 root         (0) root         (0)     8593 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/s3.py
+-rwxrwxrwx   0 root         (0) root         (0)    14037 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/file/upload.py
+-rwxrwxrwx   0 root         (0) root         (0)     6306 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/libs/geetest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.991860 seven_studio-1.5.0/seven_studio/models/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.993861 seven_studio-1.5.0/seven_studio/models/db_models/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.996863 seven_studio-1.5.0/seven_studio/models/db_models/file/
+-rwxrwxrwx   0 root         (0) root         (0)      308 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1492 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_history_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_resource_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2433 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_restrict_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1578 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_restrict_pic_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1451 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_storage_path_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/file/file_water_image_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.997863 seven_studio-1.5.0/seven_studio/models/db_models/log/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/log/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1298 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/log/log_action_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.999864 seven_studio-1.5.0/seven_studio/models/db_models/menu/
+-rwxrwxrwx   0 root         (0) root         (0)       67 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/menu/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_cote_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2174 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)    19404 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_info_model_ex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.003866 seven_studio-1.5.0/seven_studio/models/db_models/product/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/product/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/product/product_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/product/product_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.006868 seven_studio-1.5.0/seven_studio/models/db_models/role/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/role/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/role/role_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1014 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/role/role_power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)      952 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/role/role_power_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1036 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/role/role_user_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.007868 seven_studio-1.5.0/seven_studio/models/db_models/settings/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/settings/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1152 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/settings/settings_base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.009869 seven_studio-1.5.0/seven_studio/models/db_models/user/
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/user/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2025 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/user/user_info_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     1148 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/user/user_info_model_ex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1035 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/db_models/user/user_login_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2933 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/dto_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2419 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/enum.py
+-rwxrwxrwx   0 root         (0) root         (0)    37633 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/power_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     2689 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/models/seven_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     4391 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:43.013871 seven_studio-1.5.0/seven_studio/utils/
+-rwxrwxrwx   0 root         (0) root         (0)      156 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1959 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/utils/dict.py
+-rwxrwxrwx   0 root         (0) root         (0)      637 2023-05-23 07:44:57.000000 seven_studio-1.5.0/seven_studio/utils/random.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 07:45:42.973851 seven_studio-1.5.0/seven_studio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-05-23 07:45:42.000000 seven_studio-1.5.0/seven_studio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-05-23 07:45:42.000000 seven_studio-1.5.0/seven_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 07:45:42.000000 seven_studio-1.5.0/seven_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 07:45:42.000000 seven_studio-1.5.0/seven_studio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 07:45:42.000000 seven_studio-1.5.0/seven_studio.egg-info/top_level.txt
```

### Comparing `seven_studio-1.4.0/PKG-INFO` & `seven_studio-1.5.0/seven_studio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seven_studio
-Version: 1.4.0
+Name: seven-studio
+Version: 1.5.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: <!--
          * @Author: ChenXiaolei
@@ -13,14 +13,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.5.0 更新内容
+        * 修改登录过滤器login_filter
+        
         ### 1.4.0 更新内容
         * 优化配置文件
         * 修改json_dumps
         
         ### 1.3.2 更新内容
         * 登录问题修改
```

### Comparing `seven_studio-1.4.0/README.md` & `seven_studio-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
  * @LastEditors: ChenXiaolei
  * @Description: 
 -->
 # seven_studio
 
 ## 天志互联Python公共基础后台管理平台
 
+### 1.5.0 更新内容
+* 修改登录过滤器login_filter
+
 ### 1.4.0 更新内容
 * 优化配置文件
 * 修改json_dumps
 
 ### 1.3.2 更新内容
 * 登录问题修改
```

### Comparing `seven_studio-1.4.0/setup.py` & `seven_studio-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_studio",
-    version="1.4.0",
+    version="1.5.0",
     author="seven",
     author_email="tech@gao7.com",
     description="seven studio",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/python/seven_studio",
```

### Comparing `seven_studio-1.4.0/seven_studio/handlers/studio_base.py` & `seven_studio-1.5.0/seven_studio/handlers/studio_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 :Author: ChenXiaolei
 :Date: 2020-03-24 10:42:34
-:LastEditTime: 2023-04-28 15:26:27
+:LastEditTime: 2023-05-23 15:42:28
 :LastEditors: HuangJingCan
 :Description: StudioBaseHandler
 """
 import ast
 from seven_framework.web_tornado.base_handler.base_cookie_handler import *
 from seven_framework.redis import *
 
@@ -511,32 +511,35 @@
 
             user_login.ExpireTime = TimeHelper.add_hours_by_format_time(hour=config.get_value("login_expire", 10))
             user_login_model.update_table(f"ExpireTime='{user_login.ExpireTime}'", "UserID=%s", user_login.UserID)
 
         return invoke_result
 
     def login_filter(self, is_need_login, optional_params):
-        # sourcery skip: class-extract-method
         """
         :description: 登录过滤器
         :param is_need_login: 是否需要登录（true需要false不需要）
         :param optional_params: 其他参数
         :return: InvokeResult
         """
         invoke_result = InvokeResult()
+
+        if not is_need_login:
+            return invoke_result
+
         # 获取头部信息
         header_token = self.request_header_token()
         user_id = header_token["UserID"] if header_token.__contains__("UserID") else ""
         user_token = header_token["UserToken"] if header_token.__contains__("UserToken") else ""
         user_id_md5 = header_token["UserIDMD5"] if header_token.__contains__("UserIDMD5") else ""
         if user_id.strip() == "" or user_token.strip() == "" or user_id_md5.strip() == "":
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
-        if is_need_login and CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key", "7C34A5212F7845CB85D4BBB589502D9B")) != user_id_md5:
+        if CryptoHelper.md5_encrypt(user_id, config.get_value("login_encrypt_key", "7C34A5212F7845CB85D4BBB589502D9B")) != user_id_md5:
             invoke_result.ResultCode = "error"
             invoke_result.ResultMessage = "操作失败，用户未登录"
             return invoke_result
 
         invoke_result = self.check_login_user(user_id, user_token, is_need_login)
 
         return invoke_result
```

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/core.py` & `seven_studio-1.5.0/seven_studio/handlers/system/core.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/file.py` & `seven_studio-1.5.0/seven_studio/handlers/system/file.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/menu.py` & `seven_studio-1.5.0/seven_studio/handlers/system/menu.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/power.py` & `seven_studio-1.5.0/seven_studio/handlers/system/power.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/product.py` & `seven_studio-1.5.0/seven_studio/handlers/system/product.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/handlers/system/settings.py` & `seven_studio-1.5.0/seven_studio/handlers/system/settings.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/bos.py` & `seven_studio-1.5.0/seven_studio/libs/file/bos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/cos.py` & `seven_studio-1.5.0/seven_studio/libs/file/cos.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/ks3.py` & `seven_studio-1.5.0/seven_studio/libs/file/ks3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/oss2.py` & `seven_studio-1.5.0/seven_studio/libs/file/oss2.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/s3.py` & `seven_studio-1.5.0/seven_studio/libs/file/s3.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/file/upload.py` & `seven_studio-1.5.0/seven_studio/libs/file/upload.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/libs/geetest.py` & `seven_studio-1.5.0/seven_studio/libs/geetest.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_history_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_history_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_resource_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_resource_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_restrict_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_restrict_pic_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_restrict_pic_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_storage_path_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_storage_path_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/file/file_water_image_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/file/file_water_image_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/log/log_action_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/log/log_action_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_cote_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_cote_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/menu/menu_info_model_ex.py` & `seven_studio-1.5.0/seven_studio/models/db_models/menu/menu_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/product/product_info_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/product/product_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/product/product_user_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/product/product_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/role/role_info_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/role/role_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/role/role_power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/role/role_power_model_ex.py` & `seven_studio-1.5.0/seven_studio/models/db_models/role/role_power_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/role/role_user_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/role/role_user_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/settings/settings_base_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/settings/settings_base_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/user/user_info_model_ex.py` & `seven_studio-1.5.0/seven_studio/models/db_models/user/user_info_model_ex.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/db_models/user/user_login_model.py` & `seven_studio-1.5.0/seven_studio/models/db_models/user/user_login_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/dto_model.py` & `seven_studio-1.5.0/seven_studio/models/dto_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/enum.py` & `seven_studio-1.5.0/seven_studio/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/power_model.py` & `seven_studio-1.5.0/seven_studio/models/power_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/models/seven_model.py` & `seven_studio-1.5.0/seven_studio/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/route.py` & `seven_studio-1.5.0/seven_studio/route.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/utils/dict.py` & `seven_studio-1.5.0/seven_studio/utils/dict.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio/utils/random.py` & `seven_studio-1.5.0/seven_studio/utils/random.py`

 * *Files identical despite different names*

### Comparing `seven_studio-1.4.0/seven_studio.egg-info/PKG-INFO` & `seven_studio-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: seven-studio
-Version: 1.4.0
+Name: seven_studio
+Version: 1.5.0
 Summary: seven studio
 Home-page: http://gitlab.tdtech.gao7.com/python/seven_studio
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: <!--
          * @Author: ChenXiaolei
@@ -13,14 +13,17 @@
          * @LastEditors: ChenXiaolei
          * @Description: 
         -->
         # seven_studio
         
         ## 天志互联Python公共基础后台管理平台
         
+        ### 1.5.0 更新内容
+        * 修改登录过滤器login_filter
+        
         ### 1.4.0 更新内容
         * 优化配置文件
         * 修改json_dumps
         
         ### 1.3.2 更新内容
         * 登录问题修改
```

### Comparing `seven_studio-1.4.0/seven_studio.egg-info/SOURCES.txt` & `seven_studio-1.5.0/seven_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

