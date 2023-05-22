# Comparing `tmp/damo-1.8.1.tar.gz` & `tmp/damo-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.1.tar", last modified: Mon May 15 21:58:18 2023, max compression
+gzip compressed data, was "damo-1.8.2.tar", last modified: Mon May 22 22:44:21 2023, max compression
```

## Comparing `damo-1.8.1.tar` & `damo-1.8.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7182 2023-05-15 21:58:18.537882 damo-1.8.1/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6661 2023-05-15 21:58:14.000000 damo-1.8.1/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-15 21:58:14.000000 damo-1.8.1/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-15 21:58:18.537882 damo-1.8.1/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-15 21:58:14.000000 damo-1.8.1/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.525883 damo-1.8.1/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34688 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    10476 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18504 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3546 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13312 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3052 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1335 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7182 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1164 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6986 2023-05-22 22:44:21.654233 damo-1.8.2/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6465 2023-05-22 22:44:17.000000 damo-1.8.2/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-22 22:44:17.000000 damo-1.8.2/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-22 22:44:21.654233 damo-1.8.2/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-22 22:44:17.000000 damo-1.8.2/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.638234 damo-1.8.2/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      963 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_deprecation_notice.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      620 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9673 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2995 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5345 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      825 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      739 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    35686 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    10453 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8303 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17745 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    20974 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19321 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3753 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2002 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      891 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_convert_record_format.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1147 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      746 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13289 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4668 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3029 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2749 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4458 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5077 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1312 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2947 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1588 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      542 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2383 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1522 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3056 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2786 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      654 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      705 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      627 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3943 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5553 2023-05-22 22:44:17.000000 damo-1.8.2/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-22 22:44:21.654233 damo-1.8.2/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6986 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1240 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-22 22:44:21.000000 damo-1.8.2/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.1/PKG-INFO` & `damo-1.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.1
+Version: 1.8.2
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -94,28 +94,22 @@
 I show --rbuf option from `damo record` is removed.  What happened?
 -------------------------------------------------------------------
 
 The option is deprecated.  Please report your usecase to sj@kernel.org,
 damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
 
-damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
------------------------------------------------------------------------------
-
-Because the DAMOS input you're using is no more supported.  Please report your
-usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
-depend on those.
-
-
 damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
 ----------------------------------------------------------------------------------------
 
-Because the single line DAMOS scheme format is no more supported.  Please
-report your usecase to sj@kernel.org, damon@lists.linux.dev and
-linux-mm@kvack.org if you depend on those.
+Because the single line DAMOS scheme format is no more supported.  You can
+convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
+and using `damo translate_damos` command.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+the old format.
 
 
 damo suddenly prints `Python2 support of damo is deprecated` message. Why?
 --------------------------------------------------------------------------
 
 Because Python2 is no more supported.  Please report your usecase to
 sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
```

### Comparing `damo-1.8.1/README.md` & `damo-1.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -79,28 +79,22 @@
 I show --rbuf option from `damo record` is removed.  What happened?
 -------------------------------------------------------------------
 
 The option is deprecated.  Please report your usecase to sj@kernel.org,
 damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
 
-damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
------------------------------------------------------------------------------
-
-Because the DAMOS input you're using is no more supported.  Please report your
-usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
-depend on those.
-
-
 damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
 ----------------------------------------------------------------------------------------
 
-Because the single line DAMOS scheme format is no more supported.  Please
-report your usecase to sj@kernel.org, damon@lists.linux.dev and
-linux-mm@kvack.org if you depend on those.
+Because the single line DAMOS scheme format is no more supported.  You can
+convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
+and using `damo translate_damos` command.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+the old format.
 
 
 damo suddenly prints `Python2 support of damo is deprecated` message. Why?
 --------------------------------------------------------------------------
 
 Because Python2 is no more supported.  Please report your usecase to
 sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
```

### Comparing `damo-1.8.1/setup.py` & `damo-1.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.1/src/damo/_damo_dist.py` & `damo-1.8.2/src/damo/_damo_dist.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import os
 import subprocess
 
 'return error'
 def plot_dist(data_file, output_file, xlabel, ylabel):
```

### Comparing `damo-1.8.1/src/damo/_damo_fmt_str.py` & `damo-1.8.2/src/damo/_damo_fmt_str.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import platform
 
 def format_nr(nr, machine_friendly):
     raw_string = '%d' % nr
     if machine_friendly:
```

### Comparing `damo-1.8.1/src/damo/_damo_fs.py` & `damo-1.8.2/src/damo/_damo_fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import os
 
 import _damon
 
 '''Returns content and error'''
```

### Comparing `damo-1.8.1/src/damo/_damo_paddr_layout.py` & `damo-1.8.2/src/damo/_damo_paddr_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import os
 
 import _damon
```

### Comparing `damo-1.8.1/src/damo/_damo_python2_support.py` & `damo-1.8.2/src/damo/_damo_python2_support.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import os
 import subprocess
 import sys
 
-if sys.version.startswith('2.'):
-    sys.stderr.write('''
-Python2 support of damo is deprecated.  This will not work suddenly.
-
-Please report your usecase to sj@kernel.org, damon@lists.linux.dev and
-linux-mm@kvack.org if you depend on those.
+import _damo_deprecation_notice
 
-''')
+if sys.version.startswith('2.'):
+    _damo_deprecation_notice.deprecated(feature='Python2 support of damo',
+            deadline='2023-Q2')
 
 # For supporting python 2.6
 try:
     subprocess.DEVNULL = subprocess.DEVNULL
 except AttributeError:
     subprocess.DEVNULL = open(os.devnull, 'wb')
```

### Comparing `damo-1.8.1/src/damo/_damo_subcmds.py` & `damo-1.8.2/src/damo/_damo_subcmds.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 class DamoSubCmdModule:
     set_argparser = lambda self, args: args
     main = lambda self, args: args
```

### Comparing `damo-1.8.1/src/damo/_damon.py` & `damo-1.8.2/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Contains core functions for DAMON control.
 """
 
 import collections
@@ -112,14 +111,21 @@
         if unit == unit_percent:
             return '%s %%' % (_damo_fmt_str.format_nr(self.percent, raw))
         elif unit == unit_samples:
             return '%s %s' % (_damo_fmt_str.format_nr(self.samples, raw),
                     unit_samples)
         raise Exception('unsupported unit for NrAccesses (%s)' % unit)
 
+    @classmethod
+    def from_kvpairs(cls, kv):
+        ret = DamonNrAccesses(None, None)
+        ret.samples = kv['samples']
+        ret.percent = kv['percent']
+        return ret
+
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict(
                 [('samples', self.samples), ('percent', self.percent)])
 
 class DamonAge:
     usec = None
     aggr_intervals = None
@@ -147,17 +153,30 @@
 
     def to_str(self, unit, raw):
         if unit == unit_usec:
             return _damo_fmt_str.format_time_us_exact(self.usec, raw)
         return '%s %s' % (_damo_fmt_str.format_nr(self.aggr_intervals, raw),
                 unit_aggr_intervals)
 
+    @classmethod
+    def from_kvpairs(cls, kv):
+        ret = DamonAge(None, unit_usec)
+        if kv['usec'] != None:
+            ret.usec = _damo_fmt_str.text_to_us(kv['usec'])
+        if kv['aggr_intervals'] != None:
+            ret.aggr_intervals = _damo_fmt_str.text_to_nr(kv['aggr_intervals'])
+        return ret
+
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict(
-                [('usec', self.usec), ('aggr_intervals', self.aggr_intervals)])
+                [('usec', _damo_fmt_str.format_time_us_exact(self.usec, raw)
+                    if self.usec != None else None),
+                    ('aggr_intervals',
+                        _damo_fmt_str.format_nr(self.aggr_intervals, raw)
+                        if self.aggr_intervals != None else None)])
 
 class DamonRegion:
     # [start, end)
     start = None
     end = None
     # nr_accesses and age could be None
     nr_accesses = None
@@ -202,15 +221,21 @@
     # For aggregate_snapshots() support
     def __hash__(self):
         identification = '%s-%s' % (self.start, self.end)
         return hash(identification)
 
     @classmethod
     def from_kvpairs(cls, kvpairs):
-        return DamonRegion(kvpairs['start'], kvpairs['end'])
+        if not 'nr_accesses' in kvpairs:
+            return DamonRegion(kvpairs['start'], kvpairs['end'])
+        region = DamonRegion(kvpairs['start'], kvpairs['end'])
+        region.nr_accesses = DamonNrAccesses.from_kvpairs(
+                kvpairs['nr_accesses'])
+        region.age = DamonAge.from_kvpairs(kvpairs['age'])
+        return region
 
     def to_kvpairs(self, raw=False):
         if self.nr_accesses == None:
             return collections.OrderedDict([
                 ('start', _damo_fmt_str.format_nr(self.start, raw)),
                 ('end', _damo_fmt_str.format_nr(self.end, raw))])
         return collections.OrderedDict([
```

### Comparing `damo-1.8.1/src/damo/_damon_args.py` & `damo-1.8.2/src/damo/_damon_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Command line arguments handling
 """
 
 import argparse
```

### Comparing `damo-1.8.1/src/damo/_damon_args_schemes.py` & `damo-1.8.2/src/damo/_damon_args_schemes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Change human readable data access monitoring-based operation schemes input for
 'damo' to a '_damon.Damos' object.  Currently,
 
 - simple human-readable single line per scheme text (will be deprecated) and
@@ -70,18 +69,18 @@
             "filters": []
         }
     ]
 """
 
 import json
 import os
-import sys
 
 import _damon
 
+import _damo_deprecation_notice
 import _damo_fmt_str
 
 def fields_to_v0_scheme(fields):
     scheme = _damon.Damos()
     scheme.access_pattern = _damon.DamosAccessPattern(
             sz_bytes = [_damo_fmt_str.text_to_bytes(fields[0]),
                 _damo_fmt_str.text_to_bytes(fields[1])],
@@ -136,40 +135,30 @@
     return scheme
 
 avoid_crashing_single_line_scheme_for_testing = False
 avoid_crashing_v1_v3_schemes_for_testing = False
 def damo_single_line_scheme_to_damos(line):
     '''Returns Damos object and err'''
 
-    # Remove below if someone depends on single scheme is found.
-    if not avoid_crashing_single_line_scheme_for_testing:
-        sys.stderr.write('''
-You're using deprecated single line DAMOS format (%s)
-''' % line)
-        exit(1)
-
-    sys.stderr.write('''
-WARNING: single line per-scheme scheme input is deprecated.  The support will
-be removed by 2023-Q2.  Please use json format or --damos_* commandline options
-instead.
-
-Please report your usecase to sj@kernel.org, damon@liss.linux.dev
-and linux-mm@kvack.org if you depend on it.
-
-''')
+    _damo_deprecation_notice.deprecated(
+            feature='single line scheme input',
+            deadline='2023-Q2',
+            do_exit=not avoid_crashing_single_line_scheme_for_testing,
+            exit_code=1,
+            additional_notice='Please use json format or --damo_* options')
 
     fields = line.split()
 
     # Remove below if someone depends on the v1-v3  DAMOS input is found.
-    if not avoid_crashing_v1_v3_schemes_for_testing:
-        if len(fields) in [9, 12, 17]:
-            sys.stderr.write('''
-You're using unsupported DAMOS format (%s)
-    ''' % ' '.join(fields))
-            exit(1)
+    if len(fields) in [9, 12, 17]:
+        _damo_deprecation_notice.deprecated(
+                feature='9, 12, or 17 fields single line scheme input',
+                do_exit=not avoid_crashing_v1_v3_schemes_for_testing,
+                exit_code=1,
+                deadline='2023-Q2')
 
     try:
         if len(fields) == 7:
             return fields_to_v0_scheme(fields), None
         elif len(fields) == 9:
             return fields_to_v1_scheme(fields), None
         elif len(fields) == 12:
```

### Comparing `damo-1.8.1/src/damo/_damon_dbgfs.py` & `damo-1.8.2/src/damo/_damon_dbgfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Contains core functions for DAMON debugfs control.
 """
 
 import os
-import sys
 
+import _damo_deprecation_notice
 import _damo_fs
 import _damon
 
 debugfs = '/sys/kernel/debug'
 debugfs_damon = os.path.join(debugfs, 'damon')
 debugfs_attrs = os.path.join(debugfs_damon, 'attrs')
 debugfs_record = os.path.join(debugfs_damon, 'record')
@@ -413,22 +412,14 @@
     # Previous value might be invalid now (e.g., process terminated), so ignore
     # error
     err = _damo_fs.write_file(debugfs_target_ids, orig_target_ids)
     err = _damo_fs.write_file(debugfs_init_regions, orig_init_regions)
 
     return version
 
-def warn_deprecated_kernel():
-    sys.stderr.write('''
-WARNING: This kernel is running non-mainlined DAMOS implementation.  Support of
-    it from DAMO is deprecated.  The support will be removed by 2023-Q2.
-    Please report your usecase to sj@kernel.org, damon@lists.linux.dev and
-    linux-mm@kvack.org if you depend on those.
-''')
-
 def update_supported_features():
     global feature_supports
     if feature_supports != None:
         return None
     feature_supports = {x: False for x in _damon.features}
 
     if not os.path.isdir(debugfs_damon):
@@ -474,9 +465,12 @@
             feature_supports['schemes_prioritization'] = True
             feature_supports['schemes_wmarks'] = True
             feature_supports['schemes_quotas'] = True
             feature_supports['schemes_stat_succ'] = True
             feature_supports['schemes_stat_qt_exceed'] = True
 
     if 0 < get_scheme_version() and get_scheme_version() < 4:
-        warn_deprecated_kernel()
+        _damo_deprecation_notice.deprecated(
+                feature='support of non-mainlined DAMOS implementation',
+                deadline='2023-Q2')
+
     return None
```

### Comparing `damo-1.8.1/src/damo/_damon_result.py` & `damo-1.8.2/src/damo/_damon_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import collections
+import json
 import os
 import signal
 import struct
 import subprocess
 import time
+import zlib
 
+import _damo_deprecation_notice
+import _damo_fmt_str
 import _damon
 
 PERF = 'perf'
 PERF_EVENT = 'damon:damon_aggregated'
 
 class DAMONSnapshot:
     start_time = None
@@ -19,31 +22,49 @@
     regions = None
 
     def __init__(self, start_time, end_time):
         self.start_time = start_time
         self.end_time = end_time
         self.regions = []
 
-    def to_kvpairs(self):
+    @classmethod
+    def from_kvpairs(cls, kv):
+        snapshot = DAMONSnapshot(_damo_fmt_str.text_to_ns(kv['start_time']),
+                _damo_fmt_str.text_to_ns(kv['end_time']))
+        snapshot.regions = [_damon.DamonRegion.from_kvpairs(r)
+                for r in kv['regions']]
+        return snapshot
+
+    def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
-            ('start_time', self.start_time), ('end_time', self.end_time),
+            ('start_time', _damo_fmt_str.format_time_ns_exact(
+                self.start_time, raw)),
+            ('end_time', _damo_fmt_str.format_time_ns_exact(
+                self.end_time, raw)),
             ('regions', [r.to_kvpairs() for r in self.regions])])
 
 class DAMONRecord:
     target_id = None
     snapshots = None
 
     def __init__(self, target_id):
         self.target_id = target_id
         self.snapshots = []
 
-    def to_kvpairs(self):
+    @classmethod
+    def from_kvpairs(cls, kv):
+        record = DAMONRecord(kv['target_id'])
+        record.snapshots = [DAMONSnapshot.from_kvpairs(s)
+                for s in kv['snapshots']]
+        return record
+
+    def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('target_id', self.target_id),
-            ('snapshots', [s.to_kvpairs() for s in self.snapshots])])
+            ('snapshots', [s.to_kvpairs(raw) for s in self.snapshots])])
 
 class DAMONResult:
     records = None
 
     def __init__(self):
         self.records = []
 
@@ -219,35 +240,63 @@
                     stderr=subprocess.PIPE)
         except:
             err = 'perf record not working with "%s"' % PERF
     except:
         err = 'perf not found at "%s"' % PERF
     return err
 
+def warn_record_type_deprecation():
+    _damo_deprecation_notice.will_be_deprecated(
+            feature='\'record\' file type support',
+            deadline='2023-Q3',
+            additional_notice='use json_compressed type instead.')
+
+def parse_damon_record_json_compressed(result_file):
+    with open(result_file, 'rb') as f:
+        compressed = f.read()
+    decompressed = zlib.decompress(compressed).decode()
+    kvpairs = json.loads(decompressed)
+    result = DAMONResult()
+    result.records = [DAMONRecord.from_kvpairs(kvp) for kvp in kvpairs]
+    return result
+
 def parse_damon_result(result_file):
     script_output = None
-    if subprocess.check_output(
-            ['file', '-b', result_file]).decode().strip() == 'ASCII text':
+    file_type = subprocess.check_output(
+            ['file', '-b', result_file]).decode().strip()
+    if file_type == 'zlib compressed data':
+        try:
+            return parse_damon_record_json_compressed(result_file), None
+        except Exception as e:
+            return None, 'failed parsing json compressed file (%s)' % e
+    elif file_type == 'ASCII text':
         with open(result_file, 'r') as f:
             script_output = f.read()
     else:
         try:
             with open(os.devnull, 'w') as fnull:
                 script_output = subprocess.check_output(
                         [PERF, 'script', '-i', result_file],
                         stderr=fnull).decode()
         except:
             pass
     if script_output:
         result, err = perf_script_to_damon_result(script_output)
     else:
+        warn_record_type_deprecation()
         result, err = record_to_damon_result(result_file)
 
     return result, err
 
+def write_damon_record_json_compressed(result, file_path):
+    json_str = json.dumps([r.to_kvpairs(r) for r in result.records], indent=4)
+    compressed = zlib.compress(json_str.encode())
+    with open(file_path, 'wb') as f:
+        f.write(compressed)
+
 def write_damon_record(result, file_path, format_version):
     with open(file_path, 'wb') as f:
         f.write(b'damon_recfmt_ver')
         f.write(struct.pack('i', format_version))
 
         for record in result.records:
             snapshots = record.snapshots
@@ -298,44 +347,56 @@
         return None, 'parsing failed (%s)' % e
     if file_permission < 0o0 or file_permission > 0o777:
         return None, 'out of available permission range'
     return file_permission, None
 
 file_type_record = 'record'             # damo defined binary format
 file_type_perf_script = 'perf_script'   # perf script output
+file_type_perf_data = 'perf_data'       # perf record result file
+file_type_json_compressed = 'json_compressed'
+
+file_types = [file_type_json_compressed, file_type_perf_script,
+        file_type_perf_data, file_type_record]
+self_write_supported_file_types = [file_type_json_compressed,
+        file_type_perf_script, file_type_record]
 
 def write_damon_result(result, file_path, file_type, file_permission=None):
+    '''Returns None if success, an error string otherwise'''
+    if not file_type in self_write_supported_file_types:
+        return 'write unsupported file type: %s' % file_type
+
     for record in result.records:
         snapshots = record.snapshots
         if len(snapshots) == 1:
             # we cannot know start/end time of single snapshot from the file
             # to allow it with later read, write a fake snapshot
             snapshot = snapshots[0]
             snap_duration = snapshot.end_time - snapshot.start_time
             fake_snapshot = DAMONSnapshot(snapshot.end_time,
                     snapshot.end_time + snap_duration)
             # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
             fake_snapshot.regions = [_damon.DamonRegion(0, 0,
                 -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
             snapshots.append(fake_snapshot)
     if file_type == file_type_record:
+        warn_record_type_deprecation()
         write_damon_record(result, file_path, 2)
     elif file_type == file_type_perf_script:
         write_damon_perf_script(result, file_path)
-    else:
-        print('write unsupported file type: %s' % file_type)
+    elif file_type == file_type_json_compressed:
+        write_damon_record_json_compressed(result, file_path)
     if file_permission != None:
         os.chmod(file_path, file_permission)
+    return None
 
 def update_result_file(file_path, file_format, file_permission=None):
     result, err = parse_damon_result(file_path)
     if err:
         return err
-    write_damon_result(result, file_path, file_format, file_permission)
-    return None
+    return write_damon_result(result, file_path, file_format, file_permission)
 
 def regions_intersect(r1, r2):
     return not (r1.end <= r2.start or r2.end <= r1.start)
 
 def add_region(regions, region, nr_acc_to_add):
     for r in regions:
         if regions_intersect(r, region):
@@ -415,15 +476,15 @@
     file_path, file_format, file_permission = record_requests[perf_pipe]
     try:
         perf_pipe.send_signal(signal.SIGINT)
         perf_pipe.wait()
     except:
         # perf might already finished
         pass
-    if file_format != 'perf_data':
+    if file_format != file_type_perf_data:
         err = update_result_file(file_path, file_format)
         if err != None:
             print('converting format from perf_data to %s failed (%s)' %
                     (file_format, err))
     os.chmod(file_path, file_permission)
 
 def install_scheme(scheme_to_install):
```

### Comparing `damo-1.8.1/src/damo/_damon_sysfs.py` & `damo-1.8.2/src/damo/_damon_sysfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Contains core functions for DAMON sysfs control.
 """
 
 import os
```

### Comparing `damo-1.8.1/src/damo/damo.py` & `damo-1.8.2/src/damo/damo.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 import os
 os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 import sys
 
 import _damo_python2_support
 
 import damo_adjust
+import damo_convert_record_format
 import damo_features
 import damo_fmt_json
 import damo_lru_sort
 import damo_monitor
 import damo_reclaim
 import damo_record
 import damo_report
 import damo_schemes
 import damo_start
 import damo_stat
 import damo_stop
+import damo_translate_damos
 import damo_tune
 import damo_validate
 import damo_version
-import damo_translate_damos
 
 import _damo_subcmds
 
 def pr_damo_version(args_not_use):
     print(damo_version.__version__)
 
 subcmds = [
@@ -61,15 +62,18 @@
         _damo_subcmds.DamoSubCmd(name='fmt_json', module=damo_fmt_json,
             msg='convert damo-start cmdline option to DAMON json input'),
         _damo_subcmds.DamoSubCmd(name='version',
             module=_damo_subcmds.DamoSubCmdModule(None, pr_damo_version),
             msg='print the version number'),
         _damo_subcmds.DamoSubCmd(name='translate_damos',
             module=damo_translate_damos,
-            msg='translate old .damos to the new json format')
+            msg='translate old .damos to the new json format'),
+        _damo_subcmds.DamoSubCmd(name='convert_record_format',
+            module=damo_convert_record_format,
+            msg='convert DAMON result record file\'s format')
         ]
 
 class SubCmdHelpFormatter(argparse.RawDescriptionHelpFormatter):
     def _format_action(self, action):
         parts = super(argparse.RawDescriptionHelpFormatter,
                 self)._format_action(action)
         # skip sub parsers help
```

### Comparing `damo-1.8.1/src/damo/damo_adjust.py` & `damo-1.8.2/src/damo/damo_adjust.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Adjust a damon monitoring result with new attributes"
 
 import argparse
 
 import _damon_result
@@ -10,16 +9,18 @@
 def set_argparser(parser):
     parser.add_argument('--aggregate_interval', type=int, default=None,
             metavar='<microseconds>', help='new aggregation interval')
     parser.add_argument('--input', '-i', type=str, metavar='<file>',
             default='damon.data', help='input file name')
     parser.add_argument('--output', '-o', type=str, metavar='<file>',
             default='damon.adjusted.data', help='output file name')
-    parser.add_argument('--output_type', choices=['record', 'perf_script'],
-            default='record', help='output file\'s type')
+    parser.add_argument('--output_type',
+            choices=_damon_result.self_write_supported_file_types,
+            default=_damon_result.file_type_json_compressed,
+            help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--skip', type=int, metavar='<int>', default=20,
             help='number of first snapshots to skip')
 
 def main(args=None):
     if not args:
@@ -40,12 +41,15 @@
     if err:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (file_path, err))
         exit(1)
 
     if args.aggregate_interval != None:
         _damon_result.adjust_result(result, args.aggregate_interval, args.skip)
-    _damon_result.write_damon_result(result, args.output, args.output_type,
+    err = _damon_result.write_damon_result(result, args.output, args.output_type,
             output_permission)
+    if err != None:
+        print('writing adjusted result failed (%s)' % err)
+        exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.1/src/damo/damo_features.py` & `damo-1.8.2/src/damo/damo_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import json
 
 import _damon
 import _damon_args
```

### Comparing `damo-1.8.1/src/damo/damo_heats.py` & `damo-1.8.2/src/damo/damo_heats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Transform binary trace data into human readable text that can be used for
 heatmap drawing, or directly plot the data in a heatmap format.
 
 Format of the text is:
```

### Comparing `damo-1.8.1/src/damo/damo_lru_sort.py` & `damo-1.8.2/src/damo/damo_lru_sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Control DAMON_LRU_SORT"
 
 import argparse
 import os
 import time
```

### Comparing `damo-1.8.1/src/damo/damo_monitor.py` & `damo-1.8.2/src/damo/damo_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Record and report data access pattern in realtime"
 
 import argparse
 import os
 import signal
```

### Comparing `damo-1.8.1/src/damo/damo_nr_regions.py` & `damo-1.8.2/src/damo/damo_nr_regions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Print out distribution of the number of regions in the given record"
 
 import argparse
 import sys
 import tempfile
```

### Comparing `damo-1.8.1/src/damo/damo_reclaim.py` & `damo-1.8.2/src/damo/damo_reclaim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Control DAMON_RECLAIM"
 
 import argparse
 import os
 import time
```

### Comparing `damo-1.8.1/src/damo/damo_record.py` & `damo-1.8.2/src/damo/damo_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Record monitored data access patterns.
 """
 
 import os
 import signal
-import sys
 
+import _damo_deprecation_notice
 import _damon
 import _damon_args
 import _damon_result
 
 class DataForCleanup:
     kdamonds_names = None
     orig_kdamonds = None
@@ -34,15 +33,15 @@
     if exit_code in [-2, -3]:
         exit(exit_code)
 
     if data_for_cleanup.perf_pipe:
         _damon_result.stop_monitoring_record(data_for_cleanup.perf_pipe)
         exit(exit_code)
 
-    if data_for_cleanup.rfile_format != 'record':
+    if data_for_cleanup.rfile_format != _damon_result.file_type_record:
         err = _damon_result.update_result_file(data_for_cleanup.rfile_path,
                 data_for_cleanup.rfile_format)
         if err != None:
             print('converting format from record to %s failed (%s)' %
                     (data_for_cleanup.rfile_format, err))
     os.chmod(data_for_cleanup.rfile_path, data_for_cleanup.rfile_permission)
 
@@ -64,20 +63,17 @@
 
     damon_record_supported = _damon.feature_supported('record')
     if not damon_record_supported:
         if args.rbuf:
             print('# \'--rbuf\' will be ignored')
 
     if damon_record_supported or args.rbuf:
-        sys.stderr.write('''
-WARNING: --rbuf option and in-kernel record feature support is deprecated.
-    The support will be removed by 2023-Q2.
-    Please report your usecase to sj@kernel.org, damon@lists.linux.dev and
-    linux-mm@kvack.org if you depend on those.
-''')
+        _damo_deprecation_notice.deprecated(
+                feature='--rbuf option and in-kernel record feature support',
+                deadline='2023-Q2')
 
     if not args.rbuf:
         args.rbuf = 1024 * 1024
 
     return damon_record_supported
 
 def chk_handle_output_permission(output_permission_option):
@@ -92,16 +88,17 @@
 def backup_duplicate_output_file(output_file):
     if os.path.isfile(output_file):
         os.rename(output_file, output_file + '.old')
 
 def set_argparser(parser):
     parser = _damon_args.set_argparser(parser, add_record_options=True)
     parser.add_argument('--output_type',
-            choices=['record', 'perf_data', 'perf_script'],
-            default='record', help='output file\'s type')
+            choices=_damon_result.file_types,
+            default=_damon_result.file_type_json_compressed,
+            help='output file\'s type')
     parser.add_argument('--output_permission', type=str, default='600',
             help='permission of the output file')
     parser.add_argument('--perf_path', type=str, default='perf',
             help='path of perf tool ')
     return parser
 
 def main(args=None):
```

### Comparing `damo-1.8.1/src/damo/damo_report.py` & `damo-1.8.2/src/damo/damo_report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import damo_heats
 import damo_nr_regions
 import damo_report_json
```

### Comparing `damo-1.8.1/src/damo/damo_report_json.py` & `damo-1.8.2/src/damo/damo_report_json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 import os
 import sys
 
@@ -33,11 +32,12 @@
                 (file_path, err))
         exit(1)
 
     if not result:
         print('no monitoring result in the file')
         exit(1)
 
-    print(json.dumps([r.to_kvpairs() for r in result.records], indent=4))
+    print(json.dumps([r.to_kvpairs(args.raw_number) for r in result.records],
+        indent=4))
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.1/src/damo/damo_report_raw.py` & `damo-1.8.2/src/damo/damo_report_raw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import os
 import sys
 
 import _damon_result
```

### Comparing `damo-1.8.1/src/damo/damo_schemes.py` & `damo-1.8.2/src/damo/damo_schemes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Apply given operation schemes.
 """
 
 import os
```

### Comparing `damo-1.8.1/src/damo/damo_start.py` & `damo-1.8.2/src/damo/damo_start.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Start DAMON with given parameters.
 """
 
 import _damon
```

### Comparing `damo-1.8.1/src/damo/damo_stat.py` & `damo-1.8.2/src/damo/damo_stat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import signal
 import time
 
 import damo_stat_kdamonds
 import damo_stat_regions
```

### Comparing `damo-1.8.1/src/damo/damo_stat_kdamonds.py` & `damo-1.8.2/src/damo/damo_stat_kdamonds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 import json
 
 import damo_stat
```

### Comparing `damo-1.8.1/src/damo/damo_stat_regions.py` & `damo-1.8.2/src/damo/damo_stat_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import damo_stat
 
 import _damo_fmt_str
```

### Comparing `damo-1.8.1/src/damo/damo_stat_schemes.py` & `damo-1.8.2/src/damo/damo_stat_schemes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import damo_stat
 
 import _damo_fmt_str
```

### Comparing `damo-1.8.1/src/damo/damo_stop.py` & `damo-1.8.2/src/damo/damo_stop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Stop DAMON.
 """
 
 import _damon
```

### Comparing `damo-1.8.1/src/damo/damo_translate_damos.py` & `damo-1.8.2/src/damo/damo_translate_damos.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Convert old damos schemes to json format.
 """
 
 import argparse
```

### Comparing `damo-1.8.1/src/damo/damo_tune.py` & `damo-1.8.2/src/damo/damo_tune.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 """
 Update DAMON input parameters.
 """
 
 import _damon
```

### Comparing `damo-1.8.1/src/damo/damo_validate.py` & `damo-1.8.2/src/damo/damo_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Validate a given damo-record result file"
 
 import argparse
 import os
```

### Comparing `damo-1.8.1/src/damo/damo_wss.py` & `damo-1.8.2/src/damo/damo_wss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 "Print out the distribution of the working set sizes of the given trace"
 
 import argparse
 import sys
 import tempfile
```

### Comparing `damo-1.8.1/src/damo.egg-info/PKG-INFO` & `damo-1.8.2/src/damo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.1
+Version: 1.8.2
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.2/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.2/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -94,28 +94,22 @@
 I show --rbuf option from `damo record` is removed.  What happened?
 -------------------------------------------------------------------
 
 The option is deprecated.  Please report your usecase to sj@kernel.org,
 damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
 
-damo suddenly exit with `You're using unsupported DAMOS format` message.  Why?
------------------------------------------------------------------------------
-
-Because the DAMOS input you're using is no more supported.  Please report your
-usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you
-depend on those.
-
-
 damo suddenly exit with `You're using deprecated single line DAMOS format` message. Why?
 ----------------------------------------------------------------------------------------
 
-Because the single line DAMOS scheme format is no more supported.  Please
-report your usecase to sj@kernel.org, damon@lists.linux.dev and
-linux-mm@kvack.org if you depend on those.
+Because the single line DAMOS scheme format is no more supported.  You can
+convert your old DAMOS schemes to supported format by checking v1.8.1 of damo
+and using `damo translate_damos` command.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+the old format.
 
 
 damo suddenly prints `Python2 support of damo is deprecated` message. Why?
 --------------------------------------------------------------------------
 
 Because Python2 is no more supported.  Please report your usecase to
 sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
```

### Comparing `damo-1.8.1/src/damo.egg-info/SOURCES.txt` & `damo-1.8.2/src/damo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 README.md
 pyproject.toml
 setup.py
 src/damo/__init__.py
+src/damo/_damo_deprecation_notice.py
 src/damo/_damo_dist.py
 src/damo/_damo_fmt_str.py
 src/damo/_damo_fs.py
 src/damo/_damo_paddr_layout.py
 src/damo/_damo_python2_support.py
 src/damo/_damo_subcmds.py
 src/damo/_damon.py
 src/damo/_damon_args.py
 src/damo/_damon_args_schemes.py
 src/damo/_damon_dbgfs.py
 src/damo/_damon_result.py
 src/damo/_damon_sysfs.py
 src/damo/damo.py
 src/damo/damo_adjust.py
+src/damo/damo_convert_record_format.py
 src/damo/damo_features.py
 src/damo/damo_fmt_json.py
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
```

