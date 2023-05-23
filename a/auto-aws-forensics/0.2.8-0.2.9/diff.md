# Comparing `tmp/auto_aws_forensics-0.2.8.tar.gz` & `tmp/auto_aws_forensics-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto_aws_forensics-0.2.8.tar", last modified: Mon Nov  8 02:41:11 2021, max compression
+gzip compressed data, was "dist/auto_aws_forensics-0.2.9.tar", last modified: Mon Nov  8 02:57:38 2021, max compression
```

## Comparing `auto_aws_forensics-0.2.8.tar` & `auto_aws_forensics-0.2.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2732 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/PKG-INFO
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     1876 2021-11-07 20:30:57.000000 auto_aws_forensics-0.2.8/README.md
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       38 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/setup.cfg
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2159 2021-11-08 00:32:31.000000 auto_aws_forensics-0.2.8/setup.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2732 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/PKG-INFO
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2869 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/SOURCES.txt
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        1 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/dependency_links.txt
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)      515 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/requires.txt
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       46 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/top_level.txt
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       50 2021-11-07 23:19:34.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4058 2021-11-07 23:19:20.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/auto_forensics.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:06:16.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/__init__.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/__init__.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2760 2021-02-15 02:26:26.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3132 2021-02-15 02:26:14.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3835 2021-10-12 03:18:04.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-09 21:39:44.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     7219 2021-02-15 02:27:06.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_volume/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_volume/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3337 2021-10-12 17:40:09.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_volume/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2071 2021-02-15 02:26:20.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3030 2021-10-12 03:56:40.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/mount_volume/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/mount_volume/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4835 2021-11-07 16:38:56.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/mount_volume/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/run_instances/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/run_instances/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4890 2021-11-06 16:50:06.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/run_instances/lambda_function.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/share_snapshot/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/share_snapshot/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2882 2021-02-15 02:26:04.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/share_snapshot/lambda_function.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)    19200 2021-11-07 22:38:40.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/construct.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/forensics_resources/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-09 20:42:24.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/forensics_resources/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4983 2021-11-07 20:39:04.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/forensics_resources/construct.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 23:00:28.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/__init__.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-07 22:34:24.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2533 2021-10-29 17:55:52.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/disk_invoke.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2654 2021-10-29 23:00:05.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/disk_invoke_guardduty.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     9186 2021-11-08 00:58:38.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/construct.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/step_function/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 14:24:57.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/step_function/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     8093 2021-11-08 02:39:49.000000 auto_aws_forensics-0.2.8/src/forensic_auto_capture/step_function/construct.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       43 2021-11-07 23:18:56.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/__init__.py
-drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:41:11.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/assets/
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 23:00:28.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/assets/__init__.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3317 2021-11-07 20:38:01.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/components.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2043 2021-11-08 00:58:26.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/construct.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     1324 2021-11-07 20:37:35.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/distro.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3435 2021-11-07 20:30:57.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/infrastructure.py
--rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2058 2021-11-07 20:30:57.000000 auto_aws_forensics-0.2.8/src/forensic_image_pipeline/pipeline.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2732 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/PKG-INFO
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     1876 2021-11-07 20:30:57.000000 auto_aws_forensics-0.2.9/README.md
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       38 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/setup.cfg
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2159 2021-11-08 00:32:31.000000 auto_aws_forensics-0.2.9/setup.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2732 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/PKG-INFO
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2869 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/SOURCES.txt
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        1 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/dependency_links.txt
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)      515 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/requires.txt
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       46 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/top_level.txt
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       50 2021-11-07 23:19:34.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4058 2021-11-07 23:19:20.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/auto_forensics.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:06:16.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/__init__.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/__init__.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2760 2021-02-15 02:26:26.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3132 2021-02-15 02:26:14.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3835 2021-10-12 03:18:04.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-09 21:39:44.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     7219 2021-02-15 02:27:06.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_volume/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_volume/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3337 2021-10-12 17:40:09.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_volume/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2071 2021-02-15 02:26:20.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3030 2021-10-12 03:56:40.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/mount_volume/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/mount_volume/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4835 2021-11-07 16:38:56.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/mount_volume/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/run_instances/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/run_instances/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4890 2021-11-06 16:50:06.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/run_instances/lambda_function.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/share_snapshot/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-09-26 18:22:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/share_snapshot/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2882 2021-02-15 02:26:04.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/share_snapshot/lambda_function.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)    19200 2021-11-07 22:38:40.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/construct.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/forensics_resources/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-09 20:42:24.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/forensics_resources/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     4983 2021-11-07 20:39:04.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/forensics_resources/construct.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 23:00:28.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/__init__.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-07 22:34:24.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2533 2021-10-29 17:55:52.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/disk_invoke.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2654 2021-10-29 23:00:05.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/disk_invoke_guardduty.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     9186 2021-11-08 00:58:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/construct.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/step_function/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 14:24:57.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/step_function/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     8093 2021-11-08 02:39:49.000000 auto_aws_forensics-0.2.9/src/forensic_auto_capture/step_function/construct.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)       43 2021-11-07 23:18:56.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/__init__.py
+drwxr-xr-x   0 cybergoof  (1000) cybergoof  (1000)        0 2021-11-08 02:57:38.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/assets/
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)        0 2021-10-11 23:00:28.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/assets/__init__.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3317 2021-11-07 20:38:01.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/components.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2043 2021-11-08 00:58:26.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/construct.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     1324 2021-11-07 20:37:35.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/distro.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     3435 2021-11-07 20:30:57.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/infrastructure.py
+-rw-r--r--   0 cybergoof  (1000) cybergoof  (1000)     2119 2021-11-08 02:55:01.000000 auto_aws_forensics-0.2.9/src/forensic_image_pipeline/pipeline.py
```

### Comparing `auto_aws_forensics-0.2.8/PKG-INFO` & `auto_aws_forensics-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_aws_forensics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automates the process of creating a forensics capture of an EC2
 Home-page: UNKNOWN
 Author: Shaun McCullough
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `auto_aws_forensics-0.2.8/README.md` & `auto_aws_forensics-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/setup.py` & `auto_aws_forensics-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/PKG-INFO` & `auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-aws-forensics
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automates the process of creating a forensics capture of an EC2
 Home-page: UNKNOWN
 Author: Shaun McCullough
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/SOURCES.txt` & `auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/auto_aws_forensics.egg-info/requires.txt` & `auto_aws_forensics-0.2.9/src/auto_aws_forensics.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/auto_forensics.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/auto_forensics.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_copy_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/check_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/check_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/copy_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/create_volume/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/create_volume/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_check_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/final_copy_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/mount_volume/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/mount_volume/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/run_instances/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/run_instances/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/assets/share_snapshot/lambda_function.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/assets/share_snapshot/lambda_function.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/disk_functions/construct.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/disk_functions/construct.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/forensics_resources/construct.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/forensics_resources/construct.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/disk_invoke.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/disk_invoke.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/assets/disk_invoke_guardduty.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/assets/disk_invoke_guardduty.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/invoke/construct.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/invoke/construct.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_auto_capture/step_function/construct.py` & `auto_aws_forensics-0.2.9/src/forensic_auto_capture/step_function/construct.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_image_pipeline/components.py` & `auto_aws_forensics-0.2.9/src/forensic_image_pipeline/components.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_image_pipeline/construct.py` & `auto_aws_forensics-0.2.9/src/forensic_image_pipeline/construct.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_image_pipeline/distro.py` & `auto_aws_forensics-0.2.9/src/forensic_image_pipeline/distro.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_image_pipeline/infrastructure.py` & `auto_aws_forensics-0.2.9/src/forensic_image_pipeline/infrastructure.py`

 * *Files identical despite different names*

### Comparing `auto_aws_forensics-0.2.8/src/forensic_image_pipeline/pipeline.py` & `auto_aws_forensics-0.2.9/src/forensic_image_pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,22 @@
                                             distribution=distribution)
 
     def build_pipeline(self, image_recipe: imagebuilder.CfnImageRecipe,
                        infrastructure_config: imagebuilder.CfnInfrastructureConfiguration,
                        distribution: imagebuilder.CfnDistributionConfiguration = None) -> imagebuilder.CfnImagePipeline:
         if distribution is None:
             distro_attr = None
+        else:
+            distro_attr = distribution.attr_arn
 
         pipeline = imagebuilder.CfnImagePipeline(self, "forensic_pipeline",
                                                  name="forensic_pipeline",
                                                  description="Disk forensic AMI build pipeline",
                                                  enhanced_image_metadata_enabled=True,
                                                  image_recipe_arn=image_recipe.attr_arn,
-                                                 #distribution_configuration_arn=distro_attr,
+                                                 distribution_configuration_arn=distro_attr,
                                                  infrastructure_configuration_arn=infrastructure_config.attr_arn,
                                                  schedule={
                                                      "pipelineExecutionStartCondition": "EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE",
                                                      "scheduleExpression": "cron(10,20,30,40,50 * * * ? *)"})
 
         return pipeline
```

