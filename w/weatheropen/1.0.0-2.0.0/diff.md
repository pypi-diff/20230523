# Comparing `tmp/weatheropen-1.0.0.tar.gz` & `tmp/weatheropen-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatheropen-1.0.0.tar", last modified: Mon May 22 16:11:48 2023, max compression
+gzip compressed data, was "weatheropen-2.0.0.tar", last modified: Tue May 23 04:22:18 2023, max compression
```

## Comparing `weatheropen-1.0.0.tar` & `weatheropen-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:11:48.155588 weatheropen-1.0.0/
--rw-rw-rw-   0        0        0      715 2023-05-22 16:11:48.154595 weatheropen-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-22 16:11:48.156589 weatheropen-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-05-22 16:11:12.000000 weatheropen-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:11:48.138591 weatheropen-1.0.0/weatheropen/
--rw-rw-rw-   0        0        0       45 2023-05-22 16:11:42.000000 weatheropen-1.0.0/weatheropen/__init__.py
--rw-rw-rw-   0        0        0     2439 2023-05-19 16:53:03.000000 weatheropen-1.0.0/weatheropen/weatheropen.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:11:48.151591 weatheropen-1.0.0/weatheropen.egg-info/
--rw-rw-rw-   0        0        0      715 2023-05-22 16:11:48.000000 weatheropen-1.0.0/weatheropen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-22 16:11:48.000000 weatheropen-1.0.0/weatheropen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:11:48.000000 weatheropen-1.0.0/weatheropen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-22 16:11:48.000000 weatheropen-1.0.0/weatheropen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 16:11:48.000000 weatheropen-1.0.0/weatheropen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 04:22:18.780490 weatheropen-2.0.0/
+-rw-rw-rw-   0        0        0      715 2023-05-23 04:22:18.779492 weatheropen-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-23 04:22:18.780490 weatheropen-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1484 2023-05-23 04:19:08.000000 weatheropen-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:22:18.753473 weatheropen-2.0.0/weatheropen/
+-rw-rw-rw-   0        0        0       45 2023-05-22 16:11:42.000000 weatheropen-2.0.0/weatheropen/__init__.py
+-rw-rw-rw-   0        0        0     2601 2023-05-23 04:07:43.000000 weatheropen-2.0.0/weatheropen/weatheropen.py
+drwxrwxrwx   0        0        0        0 2023-05-23 04:22:18.775499 weatheropen-2.0.0/weatheropen.egg-info/
+-rw-rw-rw-   0        0        0      715 2023-05-23 04:22:18.000000 weatheropen-2.0.0/weatheropen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-23 04:22:18.000000 weatheropen-2.0.0/weatheropen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 04:22:18.000000 weatheropen-2.0.0/weatheropen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 04:22:18.000000 weatheropen-2.0.0/weatheropen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 04:22:18.000000 weatheropen-2.0.0/weatheropen.egg-info/top_level.txt
```

### Comparing `weatheropen-1.0.0/PKG-INFO` & `weatheropen-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatheropen
-Version: 1.0.0
+Version: 2.0.0
 Summary: Weather forecast data
 Home-page: https://example.com
 Author: geokzms
 Author-email: geokzms@example.com
 License: MIT
 Keywords: weather,forecast,openweather
 Platform: UNKNOWN
```

### Comparing `weatheropen-1.0.0/setup.py` & `weatheropen-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name='weatheropen',  # (Required) The name of the library
     packages=['weatheropen'],  # (Required) The list of packages to include into the library
-    version='1.0.0',          # (Required) The library version. It will be increased with library changes
+    version='2.0.0',          # (Required) The library version. It will be increased with library changes
     license='MIT',            # Type of license.
     description='Weather forecast data',  # Short description of the library
     author='geokzms',                     # Your name
     author_email='geokzms@example.com',   # Your email
     url='https://example.com',            # Homepage of your library e.g. Github or your website
     keywords=['weather', 'forecast', 'openweather'],  # Keywords users can search on pypi
     install_requires=['requests',],          # Other 3rd party libraries that pip needs to install
```

### Comparing `weatheropen-1.0.0/weatheropen/weatheropen.py` & `weatheropen-2.0.0/weatheropen/weatheropen.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     >>> weather2 = Weather(apikey='1fbdb1902adb7476df1f87e8b5457a05', lat=41.1, lon=-4.1)
     
     # Get complete weather data for the next 12 hours:
     >>> weather1.next_12h
     
     # Get simplified weather data for the next 12 hours:
     >>> weather2.next12h_simplified
+    
+    Sample URL to get sky condition icons:
+    https://openweathermap.org/img/wn/10d@2x.png
     """
     def __init__(self, apikey,  city=None, lat=None, lon=None):
         url = "https://api.openweathermap.org/data/2.5/forecast"
         if city:
             resp = requests.get(f"{url}?q={city}&appid={apikey}&units=metric")
             self.data = resp.json()
         elif lat and lon:
@@ -56,9 +59,10 @@
             list: list of the next 12 hours data, containing tuples
             of the 3-hour data
         """
         simple_data = list()
         for dicty in self.next_12h():
             simple_data.append((dicty['dt_txt'],
                                 dicty['main']['temp'],
-                                dicty['weather'][0]['description']))
+                                dicty['weather'][0]['description'],
+                                dicty['weather'][0]['icon']))
         return simple_data
```

### Comparing `weatheropen-1.0.0/weatheropen.egg-info/PKG-INFO` & `weatheropen-2.0.0/weatheropen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatheropen
-Version: 1.0.0
+Version: 2.0.0
 Summary: Weather forecast data
 Home-page: https://example.com
 Author: geokzms
 Author-email: geokzms@example.com
 License: MIT
 Keywords: weather,forecast,openweather
 Platform: UNKNOWN
```

