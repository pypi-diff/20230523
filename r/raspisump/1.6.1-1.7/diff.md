# Comparing `tmp/raspisump-1.6.1.tar.gz` & `tmp/raspisump-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.6.1.tar", last modified: Thu May 18 16:54:00 2023, max compression
+gzip compressed data, was "raspisump-1.7.tar", last modified: Tue May 23 14:50:21 2023, max compression
```

## Comparing `raspisump-1.6.1.tar` & `raspisump-1.7.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.070026 raspisump-1.6.1/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.6.1/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.6.1/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3942 2023-05-18 16:54:00.070026 raspisump-1.6.1/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3168 2023-05-11 10:55:58.000000 raspisump-1.6.1/README.md
--rw-r--r--   0 al        (1000) users      (984)       25 2023-05-18 16:52:54.000000 raspisump-1.6.1/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      866 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      619 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      662 2023-05-16 16:38:14.000000 raspisump-1.6.1/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/csv/README.md
--rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.6.1/conf/lighttpd.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/raspi.css
--rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/css/raspi.css~
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.063360 raspisump-1.6.1/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/images/logo.png
--rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.6.1/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.6.1/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.6.1/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.6.1/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    11066 2023-05-16 16:38:14.000000 raspisump-1.6.1/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.6.1/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.066693 raspisump-1.6.1/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6.1/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4910 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-05-18 16:52:54.000000 raspisump-1.6.1/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     1962 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4594 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      821 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2704 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2565 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-16 16:38:14.000000 raspisump-1.6.1/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-18 16:54:00.070026 raspisump-1.6.1/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3942 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      784 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-05-18 16:53:59.000000 raspisump-1.6.1/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-05-18 16:54:00.070026 raspisump-1.6.1/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2318 2023-05-18 16:52:54.000000 raspisump-1.6.1/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.133427 raspisump-1.7/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.7/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      251 2023-05-23 14:47:34.000000 raspisump-1.7/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3946 2023-05-23 14:50:21.133427 raspisump-1.7/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3174 2023-05-23 14:47:34.000000 raspisump-1.7/README.md
+-rw-r--r--   0 al        (1000) users      (984)       23 2023-05-23 14:47:34.000000 raspisump-1.7/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.116761 raspisump-1.7/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-05-16 16:38:14.000000 raspisump-1.7/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      905 2023-05-23 14:47:34.000000 raspisump-1.7/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      670 2023-05-23 14:47:34.000000 raspisump-1.7/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-16 16:38:14.000000 raspisump-1.7/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      703 2023-05-23 14:47:34.000000 raspisump-1.7/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.116761 raspisump-1.7/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.120094 raspisump-1.7/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.7/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.120094 raspisump-1.7/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.7/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.120094 raspisump-1.7/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.7/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.7/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.120094 raspisump-1.7/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.126761 raspisump-1.7/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.7/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.7/conf/web/css/raspi.css
+-rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.7/conf/web/css/raspi.css~
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.126761 raspisump-1.7/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.7/conf/web/images/logo.png
+-rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.7/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.130094 raspisump-1.7/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.7/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.7/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.130094 raspisump-1.7/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.7/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10745 2023-05-23 14:47:34.000000 raspisump-1.7/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-05-23 14:47:34.000000 raspisump-1.7/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.130094 raspisump-1.7/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.7/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4950 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-05-18 16:52:54.000000 raspisump-1.7/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2002 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4644 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      872 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2745 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2606 2023-05-23 14:47:34.000000 raspisump-1.7/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-16 16:38:14.000000 raspisump-1.7/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-23 14:50:21.133427 raspisump-1.7/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3946 2023-05-23 14:50:21.000000 raspisump-1.7/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      765 2023-05-23 14:50:21.000000 raspisump-1.7/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-05-23 14:50:21.000000 raspisump-1.7/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-05-23 14:50:21.000000 raspisump-1.7/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-05-23 14:50:21.000000 raspisump-1.7/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-05-23 14:50:21.133427 raspisump-1.7/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2300 2023-05-23 14:47:34.000000 raspisump-1.7/setup.py
```

### Comparing `raspisump-1.6.1/LICENSE` & `raspisump-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/PKG-INFO` & `raspisump-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.6.1
+Version: 1.7
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,15 +59,15 @@
     sudo pip3 install -U --no-binary :all: raspisump
 
 This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
 
 
 Read the configuration docs copied during setup on your pi at the following location;
 
-    /home/pi/raspi-sump/docs
+    /home/username/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
 Python2 installs of Raspi-Sump are no longer supported.
```

### Comparing `raspisump-1.6.1/README.md` & `raspisump-1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     sudo pip3 install -U --no-binary :all: raspisump
 
 This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
 
 
 Read the configuration docs copied during setup on your pi at the following location;
 
-    /home/pi/raspi-sump/docs
+    /home/username/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
 Python2 installs of Raspi-Sump are no longer supported.
```

### Comparing `raspisump-1.6.1/bin/rsump.py` & `raspisump-1.7/bin/rsump.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
-
+import os
 import configparser
 from raspisump import reading, log
 
 config = configparser.RawConfigParser()
-
-config.read('/home/pi/raspi-sump/raspisump.conf')
+user = os.getlogin()
+config.read('/home/' + user + '/raspi-sump/raspisump.conf')
 reading_interval = config.getint('pit', 'reading_interval')
 
 if reading_interval == 0:
     try:
         reading.water_depth()
     except RuntimeError:
         print("ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.")
```

### Comparing `raspisump-1.6.1/bin/rsumpchart.py` & `raspisump-1.7/bin/rsumpmonitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
-import time
-from raspisump import todaychart
+from raspisump import checkpid
 
 
 def main():
-    """Initiate todaychart.py module to graph sump pit activity."""
-    csv_file = "/home/pi/raspi-sump/csv/waterlevel-{}.csv".format(
-        time.strftime("%Y%m%d")
-    )
-    filename = "/home/pi/raspi-sump/charts/today.png"
-    todaychart.graph(csv_file, filename)
-
+    '''run checkpid.py module to restart Raspi-Sump if the rsump.py process is
+    stopped or has spawned multiple processes.'''
+    process = '/usr/local/bin/rsump.py'
+    checkpid.check_pid(process)
 
 if __name__ == "__main__":
     main()
```

### Comparing `raspisump-1.6.1/conf/raspisump.conf` & `raspisump-1.7/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/conf/web/css/raspi.css` & `raspisump-1.7/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/conf/web/css/raspi.css~` & `raspisump-1.7/conf/web/css/raspi.css~`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/conf/web/images/logo.png` & `raspisump-1.7/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/conf/web/index.html` & `raspisump-1.7/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/docs/install.md` & `raspisump-1.7/docs/install.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,88 +10,79 @@
 Raspberry Pi OS 11 (Bullseye)
 
 Raspbian OS 10 (Buster)
 
 Raspbian OS 9 (Stretch) - Support ended on June 30, 2022.  Upgrade to Bullseye.
 
 
-Default 'pi' User Account
-=========================
-
-Raspberry Pi OS have changed the automatic creation of the 'pi' user account on Raspberry Pi OS 11 (Bullseye).  Raspi-Sump depends on that account existing.  When installing Raspberry Pi OS for the first time, you must create a user named pi for Raspi-Sump to work. Future versions of Raspi-Sump will not have this requirement, but for the time being it is still required.
-
-For more information see the [Raspberry PI OS Announcement](https://www.raspberrypi.com/news/raspberry-pi-bullseye-update-april-2022/) on the default pi user account.
-
-
-Creating a pi user
-==================
-
-** Note (if user 'pi' already exists then skip this step)
+Install Dependencies
+====================
 
-If you are installing Raspi-Sump on an existing Raspberry Pi OS that does not have a pi user, create it as follows. This command will also add the pi user to the sudo and gpio groups.  The gpio group is required for accessing the gpio pins as a regular user.
+**Note**:  Your account must have sudo access to install Raspi-Sump.
 
-    sudo useradd -m -g users -G sudo,gpio -s /bin/bash pi
+Login to your Raspberry Pi running Raspberry Pi OS.
 
-Give the pi user a password
+Check that your user account is a member of the gpio group.  This is needed for accessing the gpio pins.
 
-    sudo passwd pi
+    groups
 
-You must log out and log back in for the new groups to take effect.
+You should see all groups your account belongs to.  If gpio is not listed run the following command (where 'username' is your account name);
 
-Install Dependencies
-====================
+    sudo usermod -aG gpio username
 
-Login as the pi user on Raspberry Pi OS.
+Logout and log back into your account for the groups to take effect.
 
 Install Pip, RPi.GPIO and Matplotlib
 
     sudo apt update && sudo apt -y upgrade
     sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
 
-RPi.GPIO is the library that controls the sensor.  Matplotlib is used to generate charts.
+RPi.GPIO is the library that controls the sensor.  
+
+Matplotlib is used to generate charts.
+
+
 The Pip package manager is required to install Raspi-Sump in the next step.
 
 
 
 Install Raspi-Sump
 ==================
 
-The following will automatically install hcsr04sensor if it is not already
-installed on your Pi.
+The following will automatically install hcsr04sensor if it is not already installed on your Pi.
 
     sudo pip3 install --no-binary :all: raspisump
 
 
-Navigate to /home/pi/raspi-sump/ and move the sample config file
+Navigate to /home/username/raspi-sump/ and move the sample config file
 to this directory.
 
-    cd /home/pi/raspi-sump
+    cd /home/username/raspi-sump
     mv sample_config/raspisump.conf .
 
-The /home/pi/raspi-sump folder is setup as follows on install;
+The /home/username/raspi-sump folder is setup as follows on install;
 
 * raspi-sump/sample_config/raspisump.conf (all configurations for raspisump).
 * raspi-sump/csv (location of waterlevel readings to csv file)
 * raspi-sump/charts (location of charts if using rsumpchart.py)
 * raspi-sump/logs (location of rsumpmonitor.py logs if using raspisump as a continuous process)
 * raspi-sump/web (all files needed for the optional pi webserver install)
 * raspi-sump/cron (example crontab for scheduling readings)
 
 
 **Note take care with your raspisump.conf file if you are using Gmail or any
 other mail system that requires authentication.  Your username and password
-will be viewable in the file. You should change the default pi and root
-passwords on your RaspberryPi.  The installer also tightens file security on
+will be viewable in the file. You should have a strong password on your account..  The installer also tightens file security on
 the file automatically.
 
 
 Edit raspisump.conf 
 ====================
 
-All configurations are recorded in /home/pi/raspi-sump/raspisump.conf
+All configurations are recorded in /home/username/raspi-sump/raspisump.conf
 
 See the configuration file for explanations of variables.  You can choose to
 take imperial (inches) or metric (centimetres) water level readings.
 
 
 Hardware
 ========
@@ -122,35 +113,35 @@
 see https://www.linuxnorth.org/raspi-sump/ for information on pins I used.
 
 Google soldering resistors for good information on how to do this if you have never done it.
 
 
 Starting Raspi-Sump
 ===================
-To start raspi-sump manually issue the command;
+To start raspi-sump manually and take your first waterlevel reading issue the command;
 
     rsump.py
 
 To run raspisump at 1 minute intervals enter the following line in crontab as follows;
 
 1 - crontab -e
 
-2 - enter line in crontab as follows;
+2 - enter line at the end of the crontab as follows;
 
     */1 * * * * /usr/local/bin/rsump.py &> /dev/null
 
 
 3 - Save crontab
 
 (See cron documentation for questions on configuring crontab)
 
 
 1) To monitor the log file in the csv folder while raspi-sump is running;
 
-    tail -f 'csvlogfilename'
+    e.g.   tail -f 'waterlevel-20230523.csv'
 
 If running as a continuous process 
 ==================================
 
 There may be times where you want to run Raspi-Sump more than once every
 minute.  The default setting is 0 which will run rsump.py for one reading and
 then exit. This allows you to use the linux Cron scheduler to run at a specific
@@ -177,26 +168,26 @@
 
 6) To stop Raspi-Sump:
 
     sudo killall 09 rsump.py
 
 7) To monitor the log file in the csv folder while raspi-sump is running;
 
-    tail -f 'csvlogfilename'
+    e.g.    tail -f 'waterlevel-20230523.csv'
 
 Health check with rsumpmonitor.py. If checking level more than once per minute only.
 ================================================================================
 
 To check for the health of the rsump.py process run the rsumpmonitor.py script as
 root. 
 Add to pi user crontab as follows;
 
 1 - crontab -e
 
-2 - enter line in crontab as follows;
+2 - enter line at the end of the crontab as follows;
 
     */5 * * * * /usr/local/bin/rsumpmonitor.py &> /dev/null
 
 3 - Save crontab
 
 This will check the rsump.py process every 5 minutes and restart it if it is stopped.
 
@@ -210,16 +201,16 @@
 
     rsumpchart.py
 
 
 This will create a line chart of sump pump activity.  You can easily modify the file to save to a different location with another name.
 Combined with a scheduled cron job it is an easy way to see the latest activity graphically.
 
-**Note that this requires matplotlib and numpy on your RaspberryPi which can be
-installed with the apt-get command.  See the Install Dependencies section at the
+**Note that this requires matplotlib on your RaspberryPi which can be
+installed with the apt command.  See the Install Dependencies section at the
 beginning of this file.
 
 You can also use the move_file.sh script provided as an example of how you
 transfer files offsite to a webserver or save historical chart information.
 
 Test Email Alerts
 =================
@@ -230,15 +221,15 @@
 
     emailtest
 
 ### Heartbeat Alerts
 
 Raspi-Sump can send email tests at predefined intervals.  See the raspisump.conf file option 'heartbeat' and 'heartbeat_interval'.
 
-In /home/pi/raspisump.conf, this will send an email heartbeat once per week.
+In /home/username/raspi-sump/raspisump.conf, this section configures the email heartbeat once per week.
 
     # Set a heartbeat sms or email interval in order to regularly test that your
     # notifications are working as intended.
     # 0 = No notifications
     # 1 = Send notifications
     heartbeat = 1
 
@@ -255,17 +246,15 @@
 
 
 Setting Up The Local Webserver on the Pi
 
 Purpose
 =======
 
-The following instructions allow you to configure your raspberry pi to view
-graphs of sump pit activity through your web browser.  This is accomplished by
-configuring a local webserver on your pi.
+The following instructions allow you to configure your raspberry pi to view graphs of sump pit activity through your web browser.  This is accomplished by configuring a local webserver on your pi.
 
 Once complete you will be able to view sump pump activity by connecting to
 http://ip_address_of_your_pi
 
 Preparation
 ===========
 
@@ -278,56 +267,65 @@
 
 
 Getting Started
 ===============
 
 These instructions will do the following
 - install the Lighttpd webserver on your Pi
-- copy the provided index.html file to your webserver
-- link charts to web folder to view charts
+- create your webcharts folder structure
 - configure cron to run the script to create for graphs of sump pump activity
 
 
-To view your sump pit activity install the Lighttpd webserver on your
+Install the Lighttpd webserver on your
 Raspberry Pi as follows.
 
     sudo apt install lighttpd
 
-Copy the provided lighttpd.conf as follows;
+Create your first webcharts. This will create the needed folder under '/home/username/raspi-sump/charts/
+
+    rsumpwebchart.py
+
+    
+Change to the web server root folder at /var/www/html    
 
+    cd /var/www/html
 
-    sudo cp /home/pi/raspi-sump/sample_config/lighttpd.conf /etc/lighttpd
+
+Create the symlinks for your folders to be viewable with the web server. Replace 'username' with your account name.
+
+    sudo ln -s /home/username/raspi-sump/web/index.html index.html
+    sudo ln -s /home/username/raspi-sump/web/css css
+    sudo ln -s /home/username/raspi-sump/web/images images
+    sudo ln -s /home/username/raspi-sump/charts charts
 
 
 Enable directory listing for historical charts
 
     sudo lighttpd-enable-mod dir-listing
 
 Restart the web server
 
-    sudo /etc/init.d/lighttpd force-reload
+    sudo systemctl restart lighttpd
 
 
-Create a cron job to generate an hourly graph of your sump pit activity for
-viewing on your pi webserver
+Create a cron job to generate an hourly graph of your sump pit activity for viewing on your pi webserver.
 
     1 - crontab -e
 
-    2 - enter line in crontab as follows;
+    2 - enter line at the end of the crontab as follows;
 
     59 * * * * /usr/local/bin/rsumpwebchart.py &> /dev/null
 
     3 - Save crontab
 
-    4 - run the script manually to create the first chart
-        
-        rsumpwebchart.py
 
 Open a web browser to http://ip_of_your_pi.  At the 59th minute of every hour
 you will create a chart of sump pit activity for the day which will be viewable
 on this page.  It will also copy historical information that you can access
 from the link in the web page.
 
-You are only limited by your own imagination on how to view your charts.  I
-have setup a bash script that automatically creates the graph on my Pi and
-moves it to an offsite webserver where I can view today's readouts and
-historical data.
+Support
+==========
+
+For support open an issue on the Github Issue Tracker or consider joining our discord server.  
+
+For Discord simply send an email to alaudet@linuxnorth.org and request an invite link.
```

### Comparing `raspisump-1.6.1/raspisump/alerts.py` & `raspisump-1.7/raspisump/alerts.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import configparser
 from collections import deque
 import csv
 from raspisump import log
 
 
 config = configparser.RawConfigParser()
-
-config.read('/home/pi/raspi-sump/raspisump.conf')
+user = os.getlogin()
+config.read('/home/' + user + '/raspi-sump/raspisump.conf')
 
 configs = {'email_to': config.get('email', 'email_to'),
            'email_from': config.get('email', 'email_from'),
            'smtp_authentication': config.getint(
                'email', 'smtp_authentication'),
            'smtp_tls': config.getint('email', 'smtp_tls'),
            'smtp_server': config.get('email', 'smtp_server'),
@@ -124,15 +124,15 @@
 def determine_if_alert(water_depth):
     '''Determine if an alert is required.  Only send if last alert has been
     sent more than the amount of time identified in the raspisump.conf file.
     Entry in conf file is alert_interval under the [email] section.'''
 
     alert_interval = configs['alert_interval']
 
-    alert_log = '/home/pi/raspi-sump/logs/alert_log'
+    alert_log = '/home/' + user + '/raspi-sump/logs/alert_log'
 
     if not os.path.isfile(alert_log):
         smtp_alerts(water_depth)
         log.log_event('alert_log', 'Email SMS Alert Sent')
 
     else:
         with open(alert_log, 'rt') as f:
```

### Comparing `raspisump-1.6.1/raspisump/checkpid.py` & `raspisump-1.7/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/raspisump/emailtest.py` & `raspisump-1.7/raspisump/emailtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
+import os
 import smtplib
 import configparser
 from raspisump import alerts
 
 
 config = configparser.RawConfigParser()
-
-config.read("/home/pi/raspi-sump/raspisump.conf")
+user = os.getlogin()
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
 configs = {
     "email_to": config.get("email", "email_to"),
     "email_from": config.get("email", "email_from"),
     "smtp_authentication": config.getint("email", "smtp_authentication"),
     "smtp_tls": config.getint("email", "smtp_tls"),
     "smtp_server": config.get("email", "smtp_server"),
```

### Comparing `raspisump-1.6.1/raspisump/heartbeat.py` & `raspisump-1.7/raspisump/heartbeat.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import configparser
 from collections import deque
 import csv
 from raspisump import log, alerts
 
 
 config = configparser.RawConfigParser()
-
-config.read('/home/pi/raspi-sump/raspisump.conf')
+user = os.getlogin()
+config.read('/home/' + user + '/raspi-sump/raspisump.conf')
 
 configs = {'email_to': config.get('email', 'email_to'),
            'email_from': config.get('email', 'email_from'),
            'smtp_authentication': config.getint(
            'email', 'smtp_authentication'),
            'smtp_tls': config.getint('email', 'smtp_tls'),
            'smtp_server': config.get('email', 'smtp_server'),
@@ -36,15 +36,15 @@
                                                   'heartbeat_interval')
 except configparser.NoOptionError:
     configs['heartbeat_interval'] = 10080
 
 
 def get_last_alert_time():
     '''Retrieve the last alert time string from logfile'''
-    heartbeat_log = '/home/pi/raspi-sump/logs/heartbeat_log'
+    heartbeat_log = '/home/' + user + '/raspi-sump/logs/heartbeat_log'
     with open(heartbeat_log, 'rt') as f:
         last_row = deque(csv.reader(f), 1)[0]
         return last_row[0]
 
 
 def heartbeat_email_content():
     '''Build the contents of email body which will be sent as an alert'''
@@ -104,15 +104,15 @@
     server.quit()
 
 
 def determine_if_heartbeat():
     '''Determine if a heartbeat notification is required and if so, send
     the notification.'''
 
-    heartbeat_log = '/home/pi/raspi-sump/logs/heartbeat_log'
+    heartbeat_log = '/home/' + user + '/raspi-sump/logs/heartbeat_log'
     if not os.path.isfile(heartbeat_log):
         heartbeat_alerts()
         log.log_event("heartbeat_log", "Heartbeat Email Sent")
 
     else:
         heartbeat_interval_time = configs['heartbeat_interval']
         last_email_sent = get_last_alert_time()
```

### Comparing `raspisump-1.6.1/raspisump/log.py` & `raspisump-1.7/raspisump/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
+import os
 
+user = os.getlogin()
 
 def log_event(logfile, notification):
-    _logfile = "/home/pi/raspi-sump/logs/{}".format(logfile)
+    _logfile = "/home/" + user + "/raspi-sump/logs/{}".format(logfile)
     with open(_logfile, 'a') as f:
         f.write(time.strftime("%Y-%m-%d %H:%M:%S,")),
         f.write(notification + "\n"),
 
 
 def log_reading(water_depth):
     '''Log time and water depth reading.'''
-    filename = "/home/pi/raspi-sump/csv/waterlevel-{}.csv".format(
+    filename = "/home/" + user + "/raspi-sump/csv/waterlevel-{}.csv".format(
         time.strftime("%Y%m%d"))
     with open(filename, 'a') as f:
         f.write(time.strftime("%H:%M:%S,")),
         f.write(str(water_depth) + "\n"),
```

### Comparing `raspisump-1.6.1/raspisump/reading.py` & `raspisump-1.7/raspisump/reading.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
+import os
 import configparser
 from hcsr04sensor import sensor
 from raspisump import log, alerts, heartbeat
 
 config = configparser.RawConfigParser()
-config.read("/home/pi/raspi-sump/raspisump.conf")
+user = os.getlogin()
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
 configs = {
     "critical_water_level": config.getint("pit", "critical_water_level"),
     "pit_depth": config.getint("pit", "pit_depth"),
     "temperature": config.getint("pit", "temperature"),
     "trig_pin": config.getint("gpio_pins", "trig_pin"),
     "echo_pin": config.getint("gpio_pins", "echo_pin"),
```

### Comparing `raspisump-1.6.1/raspisump/todaychart.py` & `raspisump-1.7/raspisump/todaychart.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
+import os
 import numpy as np
 import matplotlib as mpl
 
 mpl.use("Agg")
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib import rcParams
 
 rcParams.update({"figure.autolayout": True})
 import configparser
 
 config = configparser.RawConfigParser()
-config.read("/home/pi/raspi-sump/raspisump.conf")
+user = os.getlogin()
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 configs = {"unit": config.get("pit", "unit")}
 
 try:
     configs["line_color"] = config.get("charts", "line_color")
 except configparser.NoSectionError:
     configs["line_color"] = "FB921D"
```

### Comparing `raspisump-1.6.1/raspisump/webchart.py` & `raspisump-1.7/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.6.1/raspisump.egg-info/PKG-INFO` & `raspisump-1.7/raspisump.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.6.1
+Version: 1.7
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -59,15 +59,15 @@
     sudo pip3 install -U --no-binary :all: raspisump
 
 This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
 
 
 Read the configuration docs copied during setup on your pi at the following location;
 
-    /home/pi/raspi-sump/docs
+    /home/username/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
 Python2 installs of Raspi-Sump are no longer supported.
```

### Comparing `raspisump-1.6.1/raspisump.egg-info/SOURCES.txt` & `raspisump-1.7/raspisump.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 VERSION
 setup.py
 bin/emailtest
 bin/rsump.py
 bin/rsumpchart.py
 bin/rsumpmonitor.py
 bin/rsumpwebchart.py
-conf/lighttpd.conf
 conf/raspisump.conf
 conf/charts/README.md
 conf/csv/README.md
 conf/logs/README.md
 conf/web/index.html
 conf/web/css/index.html
 conf/web/css/raspi.css
```

### Comparing `raspisump-1.6.1/setup.py` & `raspisump-1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup
 import os
 
-version = "1.6.1"
+version = "1.7"
+user = os.getlogin()
 
-homedir = "/home/pi/raspi-sump/"
+homedir = "/home/" + user + "/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
 
 raspi_sump_files = [
     "bin/rsump.py",
@@ -15,15 +16,14 @@
     "bin/rsumpmonitor.py",
     "bin/rsumpwebchart.py",
     "bin/emailtest",
 ]
 
 add_files = [
     (homedir + "sample_config", ["conf/raspisump.conf"]),
-    (homedir + "sample_config", ["conf/lighttpd.conf"]),
     (homedir + "csv", ["conf/csv/README.md"]),
     (homedir + "logs", ["conf/logs/README.md"]),
     (homedir + "charts", ["conf/charts/README.md"]),
     (homedir + "docs", ["docs/README.md"]),
     (homedir + "docs", ["docs/install.md"]),
     (homedir + "cron", ["cron/README.md"]),
     (homedir + "cron", ["cron/picrontab"]),
@@ -59,13 +59,13 @@
     packages=["raspisump"],
     scripts=raspi_sump_files,
     data_files=add_files,
     install_requires=["hcsr04sensor"],
 )
 
 if os.path.isdir(homedir):
-    cmd = "chown -R pi " + homedir
+    cmd = "chown -R " + user + " " + homedir
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "raspisump.conf"
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "sample_config/raspisump.conf"
     os.system(cmd)
```

