# Comparing `tmp/hdsr_fewspy-1.8.tar.gz` & `tmp/hdsr_fewspy-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hdsr_fewspy-1.8.tar", last modified: Wed May 10 11:47:10 2023, max compression
+gzip compressed data, was "dist\hdsr_fewspy-1.9.tar", last modified: Tue May 16 15:16:55 2023, max compression
```

## Comparing `hdsr_fewspy-1.8.tar` & `hdsr_fewspy-1.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/
--rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.8/LICENSE.txt
--rw-rw-rw-   0        0        0    23553 2023-05-10 11:47:11.000000 hdsr_fewspy-1.8/PKG-INFO
--rw-rw-rw-   0        0        0    22677 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/
--rw-rw-rw-   0        0        0      462 2023-05-03 11:03:03.000000 hdsr_fewspy-1.8/hdsr_fewspy/__init__.py
--rw-rw-rw-   0        0        0    14235 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/
--rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/__init__.py
--rw-rw-rw-   0        0        0     7535 2023-05-02 15:42:12.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/base.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_filters.py
--rw-rw-rw-   0        0        0     2963 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_locations.py
--rw-rw-rw-   0        0        0     2592 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_parameters.py
--rw-rw-rw-   0        0        0     2931 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_qualifiers.py
--rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_samples.py
--rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/__init__.py
--rw-rw-rw-   0        0        0     9493 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/base.py
--rw-rw-rw-   0        0        0     6091 2023-05-02 15:54:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
--rw-rw-rw-   0        0        0     2915 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
--rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/__init__.py
--rw-rw-rw-   0        0        0     4730 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/choices.py
--rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/custom_types.py
--rw-rw-rw-   0        0        0      403 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/github.py
--rw-rw-rw-   0        0        0      470 2023-05-10 11:39:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/paths.py
--rw-rw-rw-   0        0        0     6259 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/pi_settings.py
--rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.8/hdsr_fewspy/constants/request_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/__init__.py
--rw-rw-rw-   0        0        0     5986 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/download.py
--rw-rw-rw-   0        0        0     6900 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/json_to_df_timeseries.py
--rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/manager.py
--rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/utils.py
--rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/converters/xml_to_python_obj.py
--rw-rw-rw-   0        0        0     4573 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/date_frequency.py
--rw-rw-rw-   0        0        0      612 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/exceptions.py
--rw-rw-rw-   0        0        0     2806 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/permissions.py
--rw-rw-rw-   0        0        0     5880 2023-05-02 08:51:33.000000 hdsr_fewspy-1.8/hdsr_fewspy/retry_session.py
--rw-rw-rw-   0        0        0     3798 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/secrets.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/__init__.py
--rw-rw-rw-   0        0        0     1837 2023-05-02 18:38:33.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures.py
--rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures_requests.py
--rw-rw-rw-   0        0        0     1842 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_custom_secrets.py
--rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_filters.py
--rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_locations.py
--rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_parameters.py
--rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_qualifiers.py
--rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
--rw-rw-rw-   0        0        0     7743 2023-05-03 11:53:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
--rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
--rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_timezone_id.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/
--rw-rw-rw-   0        0        0    23553 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1994 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       92 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 11:47:09.000000 hdsr_fewspy-1.8/hdsr_fewspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.8/pyproject.toml
--rw-rw-rw-   0        0        0      439 2023-05-10 11:47:11.000000 hdsr_fewspy-1.8/setup.cfg
--rw-rw-rw-   0        0        0     1658 2023-05-10 11:39:50.000000 hdsr_fewspy-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/
+-rw-rw-rw-   0        0        0     1086 2023-02-14 19:47:44.000000 hdsr_fewspy-1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    23553 2023-05-16 15:17:00.000000 hdsr_fewspy-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    22677 2023-05-10 11:39:49.000000 hdsr_fewspy-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/
+-rw-rw-rw-   0        0        0      452 2023-05-16 15:14:40.000000 hdsr_fewspy-1.9/hdsr_fewspy/__init__.py
+-rw-rw-rw-   0        0        0    15004 2023-05-16 15:14:40.000000 hdsr_fewspy-1.9/hdsr_fewspy/api.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/
+-rw-rw-rw-   0        0        0      983 2023-04-26 12:02:05.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/__init__.py
+-rw-rw-rw-   0        0        0     7535 2023-05-16 11:39:56.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/base.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 12:02:05.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_filters.py
+-rw-rw-rw-   0        0        0     2963 2023-05-10 11:39:49.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_locations.py
+-rw-rw-rw-   0        0        0     2592 2023-05-10 11:39:49.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_parameters.py
+-rw-rw-rw-   0        0        0     2931 2023-05-10 11:39:49.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_qualifiers.py
+-rw-rw-rw-   0        0        0      800 2023-04-26 16:27:58.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_samples.py
+-rw-rw-rw-   0        0        0     1313 2023-04-26 16:27:58.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/__init__.py
+-rw-rw-rw-   0        0        0     9493 2023-05-10 11:39:49.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/base.py
+-rw-rw-rw-   0        0        0     6296 2023-05-16 15:14:40.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py
+-rw-rw-rw-   0        0        0     2915 2023-05-16 11:39:56.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_single.py
+-rw-rw-rw-   0        0        0     1423 2023-04-26 16:27:58.000000 hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/__init__.py
+-rw-rw-rw-   0        0        0     5065 2023-05-16 15:14:40.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/choices.py
+-rw-rw-rw-   0        0        0       62 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/custom_types.py
+-rw-rw-rw-   0        0        0      415 2023-05-16 15:14:40.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/github.py
+-rw-rw-rw-   0        0        0      439 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/paths.py
+-rw-rw-rw-   0        0        0     6402 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/pi_settings.py
+-rw-rw-rw-   0        0        0      911 2023-05-02 16:23:52.000000 hdsr_fewspy-1.9/hdsr_fewspy/constants/request_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/__init__.py
+-rw-rw-rw-   0        0        0     5986 2023-05-10 11:39:50.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/download.py
+-rw-rw-rw-   0        0        0     6900 2023-05-10 11:39:50.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/json_to_df_timeseries.py
+-rw-rw-rw-   0        0        0     1812 2023-05-02 11:23:01.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/manager.py
+-rw-rw-rw-   0        0        0     3054 2023-05-02 10:26:47.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/utils.py
+-rw-rw-rw-   0        0        0     6026 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/converters/xml_to_python_obj.py
+-rw-rw-rw-   0        0        0     4573 2023-05-10 11:39:50.000000 hdsr_fewspy-1.9/hdsr_fewspy/date_frequency.py
+-rw-rw-rw-   0        0        0      612 2023-05-10 11:39:50.000000 hdsr_fewspy-1.9/hdsr_fewspy/exceptions.py
+-rw-rw-rw-   0        0        0     4147 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/permissions.py
+-rw-rw-rw-   0        0        0     5880 2023-05-16 11:39:56.000000 hdsr_fewspy-1.9/hdsr_fewspy/retry_session.py
+-rw-rw-rw-   0        0        0     2263 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/secrets.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/__init__.py
+-rw-rw-rw-   0        0        0     1755 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/fixtures.py
+-rw-rw-rw-   0        0        0     4580 2023-05-02 10:03:04.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/fixtures_requests.py
+-rw-rw-rw-   0        0        0      470 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_general.py
+-rw-rw-rw-   0        0        0      713 2023-05-02 12:17:38.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_filters.py
+-rw-rw-rw-   0        0        0     2957 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_locations.py
+-rw-rw-rw-   0        0        0     1343 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_parameters.py
+-rw-rw-rw-   0        0        0      679 2023-04-26 16:27:58.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_qualifiers.py
+-rw-rw-rw-   0        0        0    11741 2023-05-02 15:44:49.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
+-rw-rw-rw-   0        0        0     7743 2023-05-03 11:53:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_single.py
+-rw-rw-rw-   0        0        0     3978 2023-05-02 09:25:03.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
+-rw-rw-rw-   0        0        0      578 2023-04-26 12:02:06.000000 hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_timezone_id.py
+drwxrwxrwx   0        0        0        0 2023-05-16 15:16:59.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/
+-rw-rw-rw-   0        0        0    23553 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1990 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       92 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 15:16:58.000000 hdsr_fewspy-1.9/hdsr_fewspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1038 2023-02-14 19:47:44.000000 hdsr_fewspy-1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      439 2023-05-16 15:17:00.000000 hdsr_fewspy-1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1658 2023-05-16 15:14:41.000000 hdsr_fewspy-1.9/setup.py
```

### Comparing `hdsr_fewspy-1.8/LICENSE.txt` & `hdsr_fewspy-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/PKG-INFO` & `hdsr_fewspy-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr_fewspy
-Version: 1.8
+Version: 1.9
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.8.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.9.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hdsr_fewspy-1.8/README.md` & `hdsr_fewspy-1.9/README.md`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime
 from hdsr_fewspy import api_calls
 from hdsr_fewspy import exceptions
+from hdsr_fewspy.constants.choices import DefaultPiSettingsChoices
 from hdsr_fewspy.constants.choices import OutputChoices
 from hdsr_fewspy.constants.choices import TimeZoneChoices
 from hdsr_fewspy.constants.custom_types import ResponseType
 from hdsr_fewspy.constants.paths import SECRETS_ENV_PATH
-from hdsr_fewspy.constants.pi_settings import github_pi_setting_defaults
+from hdsr_fewspy.constants.pi_settings import GithubPiSettingDefaults
 from hdsr_fewspy.constants.pi_settings import PiSettings
 from hdsr_fewspy.constants.request_settings import get_default_request_settings
 from hdsr_fewspy.constants.request_settings import RequestSettings
 from hdsr_fewspy.permissions import Permissions
 from hdsr_fewspy.retry_session import RetryBackoffSession
 from hdsr_fewspy.secrets import Secrets
 from pathlib import Path
@@ -35,22 +36,20 @@
 
     The methods corresponding with the FEWS PI-REST requests. For more info on how to work with the FEWS REST Web
     Service, visit the Deltares website: https://publicwiki.deltares.nl/display/FEWSDOC/FEWS+PI+REST+Web+Service.
     """
 
     def __init__(
         self,
-        github_email: str = None,
         github_personal_access_token: str = None,
         secrets_env_path: Union[str, Path] = SECRETS_ENV_PATH,
-        pi_settings: PiSettings = None,
+        pi_settings: Union[PiSettings, DefaultPiSettingsChoices] = None,
         output_directory_root: Union[str, Path] = None,
     ):
         self.secrets = Secrets(
-            github_email=github_email,
             github_personal_access_token=github_personal_access_token,
             secrets_env_path=secrets_env_path,
         )
         self.permissions = Permissions(secrets=self.secrets)
         self.output_dir = self.__get_output_dir(output_directory_root=output_directory_root)
         self.pi_settings = self.__validate_pi_settings(pi_settings=pi_settings)
         self.request_settings: RequestSettings = get_default_request_settings()
@@ -93,35 +92,47 @@
             if response.ok:
                 logger.info("PiWebService is running")
                 return
             self.__log_not_running_service(err=None, response=response)
         except Exception as err:
             self.__log_not_running_service(err=err, response=None)
 
-    def __validate_pi_settings(self, pi_settings: PiSettings = None) -> PiSettings:
-        if not pi_settings:
-            pi_settings = github_pi_setting_defaults.get_pi_settings(settings_name="production")
-        if not isinstance(pi_settings, PiSettings):
-            raise AssertionError("pi_settings must be a PiSettings, see README.ml example how to create one")
-        mapper = {
-            # setting: (used, allowed)
-            "domain": (pi_settings.domain, self.permissions.allowed_domain),
-            "module_instance_id": (pi_settings.module_instance_ids, self.permissions.allowed_module_instance_id),
-            "timezone": (pi_settings.time_zone, TimeZoneChoices.get_all()),
-            "filter_id": (pi_settings.filter_id, self.permissions.allowed_filter_id),
-            "service": (pi_settings.service, self.permissions.allowed_service),
-        }
-        for setting, value in mapper.items():
-            used_value, allowed_values = value
-            assert isinstance(allowed_values, list), f"code error, allowed_values {allowed_values} must be a list"
-            if used_value in allowed_values:
-                continue
-            msg = f"setting='{setting}' used_value='{used_value}' is not in allowed_values='{allowed_values}'"
-            raise exceptions.PiSettingsError(msg)
-
+    def __validate_pi_settings(self, pi_settings: Union[PiSettings, DefaultPiSettingsChoices] = None) -> PiSettings:
+        github_pi_setting_defaults = GithubPiSettingDefaults(self.secrets.github_personal_access_token)
+        is_none = pi_settings is None
+        is_default = isinstance(pi_settings, str) and pi_settings in DefaultPiSettingsChoices.get_all()
+        is_custom = isinstance(pi_settings, PiSettings)
+
+        if is_none:
+            pi_settings = github_pi_setting_defaults.get_pi_settings(DefaultPiSettingsChoices.wis_production)
+        elif is_default:
+            pi_settings = github_pi_setting_defaults.get_pi_settings(settings_name=pi_settings)
+        elif is_custom:
+            mapper = {
+                # setting: (used, allowed)
+                "domain": (pi_settings.domain, self.permissions.allowed_domain),
+                "module_instance_id": (pi_settings.module_instance_ids, self.permissions.allowed_module_instance_id),
+                "timezone": (pi_settings.time_zone, TimeZoneChoices.get_all()),
+                "filter_id": (pi_settings.filter_id, self.permissions.allowed_filter_id),
+                "service": (pi_settings.service, self.permissions.allowed_service),
+            }
+            for setting, value in mapper.items():
+                used_value, allowed_values = value
+                assert isinstance(allowed_values, list), f"code error, allowed_values {allowed_values} must be a list"
+                if used_value in allowed_values:
+                    continue
+                msg = f"setting='{setting}' used_value='{used_value}' is not in allowed_values='{allowed_values}'"
+                raise exceptions.PiSettingsError(msg)
+        else:
+            default_options = DefaultPiSettingsChoices.get_all()
+            msg = (
+                f"pi_settings {pi_settings} must be a either None, or a str (choose from {default_options}), or a "
+                f"custom PiSettings (see README.ml example how to create one)"
+            )
+            raise NotImplementedError(msg)
         return pi_settings
 
     def get_parameters(self, output_choice: str) -> Union[ResponseType, pd.DataFrame]:
         """Get FEWS parameters as a pandas DataFrame."""
         # show_attributes does not make a difference in response (both for Pi_JSON and PI_XML)
         api_call = api_calls.GetParameters(
             output_choice=output_choice,
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/__init__.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/base.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_filters.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_locations.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_parameters.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_qualifiers.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_samples.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_samples.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/get_timezone_id.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/get_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/base.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/base.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             OutputChoices.csv_file_in_download_dir,
         ]
 
     def run(self) -> List[Path]:
         all_file_paths = []
         responses = []
         cartesian_parameters_list = self._get_cartesian_parameters_list(parameters=self.initial_fews_parameters)
+        nr_total = len(cartesian_parameters_list)
         for index, request_params in enumerate(cartesian_parameters_list):
             # eventually continue with request_period of last request (avoiding all freq update iterations)
             frequency = (
                 self.request_settings.updated_request_period
                 if self.request_settings.updated_request_period
                 else self.request_settings.default_request_period
             )
@@ -73,14 +74,16 @@
             file_paths_created = self.response_manager.run(
                 responses=responses,
                 file_name_values=file_name_values,
                 drop_missing_values=self.drop_missing_values,
                 flag_threshold=self.flag_threshold,
             )
             all_file_paths.extend(file_paths_created)
+            progress_percentage = int((index + 1) / nr_total * 100)
+            logger.info(f"get_time_series_multi progress = {progress_percentage}%")
         logger.info(f"finished download and writing to {len(all_file_paths)} file(s)")
         return all_file_paths
 
     @classmethod
     def _get_cartesian_parameters_list(cls, parameters: Dict) -> List[Dict]:
         """Create all possible combinations of locationIds, parameterIds, and qualifierIds.
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_single.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py` & `hdsr_fewspy-1.9/hdsr_fewspy/api_calls/time_series/get_time_series_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/constants/choices.py` & `hdsr_fewspy-1.9/hdsr_fewspy/constants/choices.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,25 @@
     json = "PI_JSON"
 
     @classmethod
     def get_all(cls) -> List[str]:
         return [cls.xml, cls.json]
 
 
+class DefaultPiSettingsChoices:
+    wis_production = "wis_production"
+    wis_stand_alone = "wis_stand_alone"
+    # TODO: efcis_production = "efcis_production"
+    # TODO: efcis_stand_alone = "efcis_stand_alone"
+
+    @classmethod
+    def get_all(cls) -> List[str]:
+        return [cls.wis_production, cls.wis_stand_alone]
+
+
 class OutputChoices:
     xml_file_in_download_dir = "xml_file_in_download_dir"
     json_file_in_download_dir = "json_file_in_download_dir"
     csv_file_in_download_dir = "csv_file_in_download_dir"
     xml_response_in_memory = "xml_response_in_memory"
     json_response_in_memory = "json_response_in_memory"
     pandas_dataframe_in_memory = "pandas_dataframe_in_memory"
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/constants/pi_settings.py` & `hdsr_fewspy-1.9/hdsr_fewspy/constants/pi_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,31 +53,31 @@
         - http://webwis-prd01.ad.hdsr.nl:8081/OwdPiService/rest/fewspiservice/v1/
         """
         return f"http://{self.domain}:{self.port}/{self.service}/rest/fewspiservice/v1/"
 
     @property
     def test_url(self) -> str:
         """For example:
-        - http://localhost:8081/FewsWebServices/test/fewspiservicerest/index.jsp
-        - http://webwis-prd01.ad.hdsr.nl:8081/OwdPiService/test/fewspiservicerest/index.jsp
+        - http://localhost:8081/FewsWebServices/test/fewspiservicerest/test.html
+        - http://webwis-prd01.ad.hdsr.nl:8081/OwdPiService/test/fewspiservicerest/test.html
         """
-        return f"http://{self.domain}:{self.port}/{self.service}/test/fewspiservicerest/index.jsp"
+        return f"http://{self.domain}:{self.port}/{self.service}/test/fewspiservicerest/test.html"
 
     def __post_init__(self) -> None:
         """Validate dtypes and ensure that str objects not being empty."""
-        for field_name, field_def in self.__dataclass_fields__.items():
-            if isinstance(field_def.type, typing._SpecialForm):
+        for field_name, field_def in self.__dataclass_fields__.items():  # noqa
+            if isinstance(field_def.type, typing._SpecialForm):  # noqa
                 # No check for typing.Any, typing.Union, typing.ClassVar (without parameters)
                 continue
             try:
                 expected_dtype = field_def.type.__origin__
             except AttributeError:
                 # In case of non-typing types (such as <class 'int'>, for instance)
                 expected_dtype = field_def.type
-            if isinstance(expected_dtype, typing._SpecialForm):
+            if isinstance(expected_dtype, typing._SpecialForm):  # noqa
                 # case of typing.Union[…] or typing.ClassVar[…]
                 expected_dtype = field_def.type.__args__
 
             if field_name == "document_format":
                 continue
             actual_value = getattr(self, field_name)
             assert isinstance(actual_value, expected_dtype), (
@@ -107,27 +107,29 @@
         "port",
         "service",
         "filter_id",
         "module_instance_ids",
         "time_zone",
     ]
 
-    def __init__(self):
+    def __init__(self, github_personal_access_token: str):
+        self.github_personal_access_token = github_personal_access_token
         self._df_github_settings = None
 
     @property
     def df_github_settings(self) -> pd.DataFrame:
         if self._df_github_settings is not None:
             return self._df_github_settings
         github_downloader = GithubFileDownloader(
             target_file=github.GITHUB_HDSR_FEWSPY_AUTH_SETTINGS_TARGET_FILE,
             allowed_period_no_updates=github.GITHUB_HDSR_FEWSPY_AUTH_ALLOWED_PERIOD_NO_UPDATES,
             repo_name=github.GITHUB_HDSR_FEWSPY_AUTH_REPO_NAME,
             branch_name=github.GITHUB_HDSR_FEWSPY_AUTH_BRANCH_NAME,
             repo_organisation=github.GITHUB_ORGANISATION,
+            personal_access_token=self.github_personal_access_token,
         )
         df = pd.read_csv(filepath_or_buffer=github_downloader.get_download_url(), sep=";")
         assert sorted(df.columns) == sorted(self.expected_columns), "code_error"
         self._df_github_settings = df
         return self._df_github_settings
 
     def _read_github(self, settings_name: str) -> pd.Series:
@@ -151,10 +153,7 @@
             port=int(pd_series["port"]),
             service=pd_series["service"],
             filter_id=pd_series["filter_id"],
             module_instance_ids=pd_series["module_instance_ids"],
             time_zone=float(pd_series["time_zone"]),
         )
         return pi_settings
-
-
-github_pi_setting_defaults = GithubPiSettingDefaults()
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/constants/request_settings.py` & `hdsr_fewspy-1.9/hdsr_fewspy/constants/request_settings.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/converters/download.py` & `hdsr_fewspy-1.9/hdsr_fewspy/converters/download.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/converters/json_to_df_timeseries.py` & `hdsr_fewspy-1.9/hdsr_fewspy/converters/json_to_df_timeseries.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/converters/manager.py` & `hdsr_fewspy-1.9/hdsr_fewspy/converters/manager.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/converters/utils.py` & `hdsr_fewspy-1.9/hdsr_fewspy/converters/utils.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/converters/xml_to_python_obj.py` & `hdsr_fewspy-1.9/hdsr_fewspy/converters/xml_to_python_obj.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/date_frequency.py` & `hdsr_fewspy-1.9/hdsr_fewspy/date_frequency.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/exceptions.py` & `hdsr_fewspy-1.9/hdsr_fewspy/exceptions.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/retry_session.py` & `hdsr_fewspy-1.9/hdsr_fewspy/retry_session.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/fixtures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from hdsr_fewspy.api import Api
-from hdsr_fewspy.constants.pi_settings import github_pi_setting_defaults
+from hdsr_fewspy.constants.choices import DefaultPiSettingsChoices
 from pathlib import Path
 
 import pytest
 
 
 @pytest.fixture(scope="function")
 def fixture_api_sa_no_download_dir():
-    api = Api(pi_settings=github_pi_setting_defaults.get_pi_settings(settings_name="standalone"))
+    api = Api(pi_settings=DefaultPiSettingsChoices.wis_stand_alone)
     assert api.pi_settings.ssl_verify == True  # noqa
-    assert api.pi_settings.settings_name == "standalone"
+    assert api.pi_settings.settings_name == "wis_stand_alone"
     assert api.pi_settings.domain == "localhost"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     assert api.pi_settings.document_version == 1.25
     assert api.pi_settings.port == 8080
     assert not api.request_settings.updated_request_period
@@ -21,21 +21,18 @@
 
 
 @pytest.fixture(scope="function")
 def fixture_api_sa_with_download_dir(tmpdir_factory):
     output_dir = tmpdir_factory.mktemp("hdsr_fewspy_test_dir")  # tmpdir_factory can do session scope. nice!
     output_dir_path = Path(output_dir)
     assert output_dir_path.is_dir()
-    api = Api(
-        pi_settings=github_pi_setting_defaults.get_pi_settings(settings_name="standalone"),
-        output_directory_root=output_dir_path,
-    )
+    api = Api(pi_settings=DefaultPiSettingsChoices.wis_stand_alone, output_directory_root=output_dir_path)
     assert isinstance(api.output_dir, Path)
     assert api.pi_settings.ssl_verify == True  # noqa
-    assert api.pi_settings.settings_name == "standalone"
+    assert api.pi_settings.settings_name == "wis_stand_alone"
     assert api.pi_settings.domain == "localhost"
     assert api.pi_settings.filter_id == "INTERNAL-API"
     assert api.pi_settings.service == "FewsWebServices"
     assert api.pi_settings.module_instance_ids == "WerkFilter"
     assert api.pi_settings.document_version == 1.25
     assert api.pi_settings.port == 8080
     assert not api.request_settings.updated_request_period
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/fixtures_requests.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/fixtures_requests.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_filters.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_filters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_locations.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_locations.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_parameters.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_parameters.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_qualifiers.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_qualifiers.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_multi.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_single.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_single.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy/tests/test_sa_timezone_id.py` & `hdsr_fewspy-1.9/hdsr_fewspy/tests/test_sa_timezone_id.py`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy.egg-info/PKG-INFO` & `hdsr_fewspy-1.9/hdsr_fewspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hdsr-fewspy
-Version: 1.8
+Version: 1.9
 Summary: A python project to request data (locations, timeseries, etc.) from a HDSR FEWS PiWebService
 Home-page: https://github.com/hdsr-mid/hdsr_fewspy
 Author: Renier Kramer
 Author-email: renier.kramer@hdsr.nl
 License: MIT
-Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.8.tar.gz
+Download-URL: https://github.com/hdsr-mid/hdsr_fewspy/archive/v1.9.tar.gz
 Keywords: hdsr,fews,api,fewspy,wis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `hdsr_fewspy-1.8/hdsr_fewspy.egg-info/SOURCES.txt` & `hdsr_fewspy-1.9/hdsr_fewspy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 hdsr_fewspy/converters/json_to_df_timeseries.py
 hdsr_fewspy/converters/manager.py
 hdsr_fewspy/converters/utils.py
 hdsr_fewspy/converters/xml_to_python_obj.py
 hdsr_fewspy/tests/__init__.py
 hdsr_fewspy/tests/fixtures.py
 hdsr_fewspy/tests/fixtures_requests.py
-hdsr_fewspy/tests/test_custom_secrets.py
+hdsr_fewspy/tests/test_sa_general.py
 hdsr_fewspy/tests/test_sa_get_filters.py
 hdsr_fewspy/tests/test_sa_get_locations.py
 hdsr_fewspy/tests/test_sa_get_parameters.py
 hdsr_fewspy/tests/test_sa_get_qualifiers.py
 hdsr_fewspy/tests/test_sa_get_timeseries_multi.py
 hdsr_fewspy/tests/test_sa_get_timeseries_single.py
 hdsr_fewspy/tests/test_sa_get_timeseries_statistics.py
```

### Comparing `hdsr_fewspy-1.8/pyproject.toml` & `hdsr_fewspy-1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdsr_fewspy-1.8/setup.py` & `hdsr_fewspy-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 # read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "1.8"
+version = "1.9"
 
 install_requires = [
     "requests",
     "geopandas",
     "pandas",
     "hdsr-pygithub",
     "pathlib",
```

