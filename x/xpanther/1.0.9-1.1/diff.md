# Comparing `tmp/xpanther-1.0.9.tar.gz` & `tmp/xpanther-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanther-1.0.9.tar", last modified: Sat May 20 14:10:17 2023, max compression
+gzip compressed data, was "xpanther-1.1.tar", last modified: Tue May 23 12:09:09 2023, max compression
```

## Comparing `xpanther-1.0.9.tar` & `xpanther-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.930113 xpanther-1.0.9/
--rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     5539 2023-05-20 14:10:17.928337 xpanther-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.0.9/README.md
--rw-rw-rw-   0        0        0      624 2023-05-20 14:06:27.000000 xpanther-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 14:10:17.930113 xpanther-1.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.879602 xpanther-1.0.9/xpanther/
--rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.0.9/xpanther/__init__.py
--rw-rw-rw-   0        0        0    19992 2023-05-19 17:48:05.000000 xpanther-1.0.9/xpanther/main.py
--rw-rw-rw-   0        0        0     5411 2023-05-20 14:06:27.000000 xpanther-1.0.9/xpanther/main_ide.py
-drwxrwxrwx   0        0        0        0 2023-05-20 14:10:17.918523 xpanther-1.0.9/xpanther.egg-info/
--rw-rw-rw-   0        0        0     5539 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 14:10:17.000000 xpanther-1.0.9/xpanther.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.205768 xpanther-1.1/
+-rw-rw-rw-   0        0        0     1089 2023-02-09 23:08:35.000000 xpanther-1.1/LICENSE
+-rw-rw-rw-   0        0        0     5537 2023-05-23 12:09:09.205768 xpanther-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5071 2023-05-20 14:06:27.000000 xpanther-1.1/README.md
+-rw-rw-rw-   0        0        0      648 2023-05-23 12:08:35.000000 xpanther-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-23 12:09:09.205768 xpanther-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.144827 xpanther-1.1/xpanther/
+-rw-rw-rw-   0        0        0       79 2023-05-07 13:19:03.000000 xpanther-1.1/xpanther/__init__.py
+-rw-rw-rw-   0        0        0    19990 2023-05-22 18:16:20.000000 xpanther-1.1/xpanther/main.py
+-rw-rw-rw-   0        0        0     5464 2023-05-23 11:57:10.000000 xpanther-1.1/xpanther/main_ide.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:09:09.205768 xpanther-1.1/xpanther.egg-info/
+-rw-rw-rw-   0        0        0     5537 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 12:09:09.000000 xpanther-1.1/xpanther.egg-info/top_level.txt
```

### Comparing `xpanther-1.0.9/LICENSE` & `xpanther-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.9/PKG-INFO` & `xpanther-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.9
+Version: 1.1
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `xpanther-1.0.9/README.md` & `xpanther-1.1/README.md`

 * *Files identical despite different names*

### Comparing `xpanther-1.0.9/pyproject.toml` & `xpanther-1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xpanther"
-version = "1.0.9"
+version = "1.1"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Find Unique Xpath of any HTML/XML element"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "bs4 >= 0.0.1",
     "selenium >= 4.9.0",
+    "requests >= 2.31.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `xpanther-1.0.9/xpanther/main.py` & `xpanther-1.1/xpanther/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,14 @@
 
         possible_indicators_pair = list(combinations(l_items, 2))
         if len(l_items) > 10:
             possible_indicators = possible_indicators_pair
         else:
             possible_indicators_three = list(combinations(l_items, 3))
             possible_indicators = possible_indicators_pair + possible_indicators_three
-
         return possible_indicators, elements
 
     def __find_unique_combinations(self, combinations_list, target_element):
         available_combinations = []
         for index, keys in enumerate(self.__keys):
             if index != target_element[2]:
                 for comb in combinations_list:
```

### Comparing `xpanther-1.0.9/xpanther/main_ide.py` & `xpanther-1.1/xpanther/main_ide.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import sleep
 
-from selenium.common.exceptions import TimeoutException, WebDriverException
+from selenium.common.exceptions import TimeoutException, WebDriverException, NoAlertPresentException
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from selenium import webdriver
 from xpanther import XPanther
 
 
 class XPantherIDE:
@@ -14,17 +14,31 @@
         self.alert = custom_alert
 
     def wait_for_alert(self):
         for _ in range(100):
             try:
                 WebDriverWait(self.__driver, 1).until(ec.alert_is_present())
                 sleep(1)
-            except TimeoutException:
+            except TimeoutException or NoAlertPresentException:
                 return True
 
+    def find_and_alert_xpath(self, return_value):
+        self.__driver.execute_script("alert('Capturing...')")
+        xpath = XPanther(
+            return_value[1], print_output=False, speed='fast'
+        ).capture(return_value[0])[0]
+        if not xpath:
+            xpath = 'Could not find XPATH...'
+        try:
+            self.__driver.switch_to.alert.accept()
+        except NoAlertPresentException:
+            return None
+        self.__driver.execute_script(f"alert('{xpath}')")
+        return xpath
+
     def start(self):
         program_return = []
         self.__driver.get(self.__page_url)
         print("---XPantherIDE Started---")
         event_js = """
         var array_events = []
 
@@ -56,15 +70,15 @@
                 """
         self.__driver.set_script_timeout(10000)
         self.__driver.execute_script(event_js)
         self.__driver.execute_script(sweetalert_js)
         current_url = self.__driver.current_url
         try:
             index = 0
-            for _ in range(1000):
+            for _ in range(9999):
                 try:
                     if (new_url := self.__driver.current_url) != current_url:
                         current_url = new_url
                         self.__driver.execute_script(event_js)
                         self.__driver.execute_script(sweetalert_js)
                     return_value = WebDriverWait(self.__driver, 1).until(
                         lambda driver: self.__driver.execute_script(return_js)
@@ -79,41 +93,34 @@
                                           text: 'Capturing...',
                                           padding: '50'
                                           })"""
                                 )
                                 xpath = XPanther(
                                     return_value[1], print_output=False, speed='fast'
                                 ).capture(return_value[0])[0]
+                                if not xpath:
+                                    xpath = 'Could not find XPATH...'
                                 self.__driver.execute_script(
                                     f"""
                                        Swal.fire({{
                                           position: 'top-end',
                                           text: '{xpath}',
                                           timer: 10000,
                                           padding: '50'
                                           }})"""
                                 )
                             except WebDriverException:
-                                self.__driver.execute_script("alert('Capturing...')")
-                                xpath = XPanther(
-                                    return_value[1], print_output=False, speed='fast'
-                                ).capture(return_value[0])[0]
-                                self.__driver.switch_to.alert.accept()
-                                self.__driver.execute_script(f"alert('{xpath}')")
+                                xpath = self.find_and_alert_xpath(return_value)
                         else:
-                            self.__driver.execute_script("alert('Capturing...')")
-                            xpath = XPanther(
-                                return_value[1], print_output=False, speed='fast'
-                            ).capture(return_value[0])[0]
-                            self.__driver.switch_to.alert.accept()
-                            self.__driver.execute_script(f"alert('{xpath}')")
+                            xpath = self.find_and_alert_xpath(return_value)
                         index += 1
-                        print(f"#{index} SELECTION -> {xpath}")
-                        program_return += [xpath]
-                        self.wait_for_alert()
+                        if xpath is not None:
+                            print(f"#{index} SELECTION -> {xpath}")
+                            program_return += [xpath]
+                            self.wait_for_alert()
                 except TimeoutException:
                     pass
         except WebDriverException:
             print("---XPantherIDE Closed---")
             pass
         finally:
             if program_return:
```

### Comparing `xpanther-1.0.9/xpanther.egg-info/PKG-INFO` & `xpanther-1.1/xpanther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanther
-Version: 1.0.9
+Version: 1.1
 Summary: Find Unique Xpath of any HTML/XML element
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Check Github, https://github.com/riflosnake/XPanther
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

