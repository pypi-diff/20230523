# Comparing `tmp/gambit-bromine-0.4.2.tar.gz` & `tmp/gambit-bromine-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gambit-bromine-0.4.2.tar", last modified: Fri Aug 26 14:18:31 2022, max compression
+gzip compressed data, was "gambit-bromine-0.4.3.tar", last modified: Tue May 23 13:35:54 2023, max compression
```

## Comparing `gambit-bromine-0.4.2.tar` & `gambit-bromine-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2022-08-26 14:18:31.053541 gambit-bromine-0.4.2/
--rw-rw-r--   0 piro      (1000) piro      (1000)     2877 2022-08-26 14:18:31.053541 gambit-bromine-0.4.2/PKG-INFO
--rw-rw-r--   0 piro      (1000) piro      (1000)     1767 2020-09-16 10:32:27.000000 gambit-bromine-0.4.2/README.md
-drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2022-08-26 14:18:31.053541 gambit-bromine-0.4.2/bromine/
--rw-rw-r--   0 piro      (1000) piro      (1000)      122 2020-09-16 10:32:27.000000 gambit-bromine-0.4.2/bromine/__init__.py
--rw-rw-r--   0 piro      (1000) piro      (1000)     9539 2022-08-26 14:18:15.000000 gambit-bromine-0.4.2/bromine/browser.py
--rw-rw-r--   0 piro      (1000) piro      (1000)     2075 2022-07-11 18:20:32.000000 gambit-bromine-0.4.2/bromine/django_admin.py
--rw-rw-r--   0 piro      (1000) piro      (1000)     6244 2022-08-26 14:12:39.000000 gambit-bromine-0.4.2/bromine/pytest.py
--rw-rw-r--   0 piro      (1000) piro      (1000)     1537 2022-07-11 18:20:32.000000 gambit-bromine-0.4.2/bromine/select2.py
-drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2022-08-26 14:18:31.053541 gambit-bromine-0.4.2/gambit_bromine.egg-info/
--rw-rw-r--   0 piro      (1000) piro      (1000)     2877 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/PKG-INFO
--rw-rw-r--   0 piro      (1000) piro      (1000)      363 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/SOURCES.txt
--rw-rw-r--   0 piro      (1000) piro      (1000)        1 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/dependency_links.txt
--rw-rw-r--   0 piro      (1000) piro      (1000)       37 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/entry_points.txt
--rw-rw-r--   0 piro      (1000) piro      (1000)        9 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/requires.txt
--rw-rw-r--   0 piro      (1000) piro      (1000)        8 2022-08-26 14:18:31.000000 gambit-bromine-0.4.2/gambit_bromine.egg-info/top_level.txt
--rw-rw-r--   0 piro      (1000) piro      (1000)       75 2022-07-11 18:20:32.000000 gambit-bromine-0.4.2/pyproject.toml
--rw-rw-r--   0 piro      (1000) piro      (1000)       38 2022-08-26 14:18:31.053541 gambit-bromine-0.4.2/setup.cfg
--rw-rw-r--   0 piro      (1000) piro      (1000)      965 2022-08-26 14:17:08.000000 gambit-bromine-0.4.2/setup.py
+drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2023-05-23 13:35:54.889268 gambit-bromine-0.4.3/
+-rw-rw-r--   0 piro      (1000) piro      (1000)     1113 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/LICENSE
+-rw-rw-r--   0 piro      (1000) piro      (1000)     2520 2023-05-23 13:35:54.889268 gambit-bromine-0.4.3/PKG-INFO
+-rw-rw-r--   0 piro      (1000) piro      (1000)     1767 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/README.md
+drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2023-05-23 13:35:54.885268 gambit-bromine-0.4.3/bromine/
+-rw-rw-r--   0 piro      (1000) piro      (1000)      122 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/bromine/__init__.py
+-rw-rw-r--   0 piro      (1000) piro      (1000)    10320 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/bromine/browser.py
+-rw-rw-r--   0 piro      (1000) piro      (1000)     2075 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/bromine/django_admin.py
+-rw-rw-r--   0 piro      (1000) piro      (1000)     6244 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/bromine/pytest.py
+-rw-rw-r--   0 piro      (1000) piro      (1000)     1537 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/bromine/select2.py
+drwxrwxr-x   0 piro      (1000) piro      (1000)        0 2023-05-23 13:35:54.889268 gambit-bromine-0.4.3/gambit_bromine.egg-info/
+-rw-rw-r--   0 piro      (1000) piro      (1000)     2520 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/PKG-INFO
+-rw-rw-r--   0 piro      (1000) piro      (1000)      371 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/SOURCES.txt
+-rw-rw-r--   0 piro      (1000) piro      (1000)        1 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/dependency_links.txt
+-rw-rw-r--   0 piro      (1000) piro      (1000)       37 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/entry_points.txt
+-rw-rw-r--   0 piro      (1000) piro      (1000)        9 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/requires.txt
+-rw-rw-r--   0 piro      (1000) piro      (1000)        8 2023-05-23 13:35:54.000000 gambit-bromine-0.4.3/gambit_bromine.egg-info/top_level.txt
+-rw-rw-r--   0 piro      (1000) piro      (1000)       75 2023-05-23 13:32:33.000000 gambit-bromine-0.4.3/pyproject.toml
+-rw-rw-r--   0 piro      (1000) piro      (1000)       38 2023-05-23 13:35:54.889268 gambit-bromine-0.4.3/setup.cfg
+-rw-rw-r--   0 piro      (1000) piro      (1000)      965 2023-05-23 13:32:56.000000 gambit-bromine-0.4.3/setup.py
```

### Comparing `gambit-bromine-0.4.2/PKG-INFO` & `gambit-bromine-0.4.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 Metadata-Version: 2.1
 Name: gambit-bromine
-Version: 0.4.2
+Version: 0.4.3
 Summary: Pythonic web testing
 Home-page: https://github.com/dvarrazzo/bromine
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: UNKNOWN
-Description: # Bromine: pythonic web testing
-        
-        Bromine is a wrapper around [selenium] to allow writing testing in a terse and
-        *pythonic* rather that *java-esque* way.
-        
-        [selenium]: https://www.seleniumhq.org/
-        
-        Selenium is cool: you register browser to a hub, you ask browsers from a hub,
-        you use the browser, and you put it back. It works like magic.
-        
-        Except if you want to use https. But who needs https these days?
-        
-        Anyway, enough dissing well intentioned web testing systems. Let's talk bad
-        about bad testing system. You know what you have to do to wait for a page to
-        load after a get, and then check if an element is visible? The selenium docs
-        [will tell you](https://selenium-python.readthedocs.io/waits.html#explicit-waits):
-        
-        ```python
-        from selenium.webdriver.common.by import By
-        from selenium.webdriver.support.ui import WebDriverWait
-        from selenium.webdriver.support import expected_conditions as EC
-        
-        # ...
-        driver.get("http://example.com")
-        element = WebDriverWait(driver, 10).until(
-        	EC.presence_of_element_located((By.ID, "myDynamicElement"))
-        )
-        ```
-        
-        I've been kind and I've stripped some boilerplate. If you are happy about
-        importing three objects from 4 levels of namespaces and create a wait object
-        and pass a 2-element tuple to the "convenience method"
-        `selenium.webdriver.support.expected_conditions.visibility_of_element_located`
-        for a thing you have to do pretty much every time you click on a link, please
-        stop reading here: type `pip install selenium` and off you go. The following
-        paragraph is only for people who think the above is unsatisfactory in Python.
-        
-        Still reading? Sure?
-        
-        Well, I'll be honest: what I prefer to do is:
-        
-        ```python
-        import bromine
-        browser = bromine.Browser(driver)
-        element = browser.get("http://example.com/").wait(id='myDynamicElement')
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier:         Framework :: Pytest
 Classifier:         Intended Audience :: Developers
 Classifier:         License :: OSI Approved :: MIT License
 Classifier:         Operating System :: OS Independent
 Classifier:         Programming Language :: Python :: 3
 Classifier:         Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier:         Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bromine: pythonic web testing
+
+Bromine is a wrapper around [selenium] to allow writing testing in a terse and
+*pythonic* rather that *java-esque* way.
+
+[selenium]: https://www.seleniumhq.org/
+
+Selenium is cool: you register browser to a hub, you ask browsers from a hub,
+you use the browser, and you put it back. It works like magic.
+
+Except if you want to use https. But who needs https these days?
+
+Anyway, enough dissing well intentioned web testing systems. Let's talk bad
+about bad testing system. You know what you have to do to wait for a page to
+load after a get, and then check if an element is visible? The selenium docs
+[will tell you](https://selenium-python.readthedocs.io/waits.html#explicit-waits):
+
+```python
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+
+# ...
+driver.get("http://example.com")
+element = WebDriverWait(driver, 10).until(
+	EC.presence_of_element_located((By.ID, "myDynamicElement"))
+)
+```
+
+I've been kind and I've stripped some boilerplate. If you are happy about
+importing three objects from 4 levels of namespaces and create a wait object
+and pass a 2-element tuple to the "convenience method"
+`selenium.webdriver.support.expected_conditions.visibility_of_element_located`
+for a thing you have to do pretty much every time you click on a link, please
+stop reading here: type `pip install selenium` and off you go. The following
+paragraph is only for people who think the above is unsatisfactory in Python.
+
+Still reading? Sure?
+
+Well, I'll be honest: what I prefer to do is:
+
+```python
+import bromine
+browser = bromine.Browser(driver)
+element = browser.get("http://example.com/").wait(id='myDynamicElement')
+```
+
+
```

### Comparing `gambit-bromine-0.4.2/README.md` & `gambit-bromine-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `gambit-bromine-0.4.2/bromine/browser.py` & `gambit-bromine-0.4.3/bromine/browser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,47 @@
+import functools
+import time
 from urllib.parse import urlparse
 
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import WebDriverException
+from selenium.common.exceptions import WebDriverException, StaleElementReferenceException, TimeoutException
 import selenium.webdriver.common.keys
 from selenium.webdriver.support.ui import Select, WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 on_pytest = 0
 
 
+def retry_stale(func):
+    @functools.wraps(func)
+    def wrapper(self, *args, **kwargs):
+        start = time.time()
+        while True:
+            try:
+                return func(self, *args, **kwargs)
+            except StaleElementReferenceException as e:
+                if time.time() > start + self._browser.timeout:
+                    raise TimeoutException(
+                        f"Retry failed; {e} has been repeatedly raised for {self._browser.timeout} seconds"
+                    )
+                time.sleep(1)
+    return wrapper
+
+
 class Browser:
     """
     A wrapper for a selenium driver to simplify interaction.
     """
 
     Keys = selenium.webdriver.common.keys.Keys
     exceptions = selenium.common.exceptions
 
     def __init__(self, driver):
         self._driver = driver
-        self.timeout = 2.0
+        self.timeout = 10.0
 
     def __getattr__(self, attr):
         return getattr(self._driver, attr)
 
     def get(self, url):
         # Add the domain to a path-only url
         if url.startswith("/"):
@@ -53,15 +71,16 @@
         else:
             meth, args = self._get_condition(kwargs)
             return ElemWrapper(waiter.until(meth(*args)))
 
     def _get_waiter(self, timeout=None):
         if not timeout:
             timeout = self.timeout
-        return WebDriverWait(self._driver, timeout, poll_frequency=0.1)
+        return WebDriverWait(self._driver, timeout, poll_frequency=0.1,
+                             ignored_exceptions=[StaleElementReferenceException])
 
     selectors = {
         "id": By.ID,
         "xpath": By.XPATH,
         "link": By.LINK_TEXT,
         "partial_link": By.PARTIAL_LINK_TEXT,
         "name": By.NAME,
@@ -201,26 +220,30 @@
             except WebDriverException as e:
                 do_raise(e)
 
         return getattr(self._elem, attr)
 
     # Methods always requiring some sort of wait to be useful
 
+    @retry_stale
     def clear(self):
         elem = self.wait("clickable")
         return elem.clear()
 
+    @retry_stale
     def click(self):
         elem = self.wait("clickable")
         return elem.click()
 
+    @retry_stale
     def send_keys(self, *args):
         elem = self.wait("clickable")
         return elem.send_keys(*args)
 
+    @retry_stale
     def select(self, **kwargs):
         elem = self.wait("clickable")
         return elem.select(**kwargs)
 
 
 class ElemWrapper:
     def __init__(self, elem):
```

### Comparing `gambit-bromine-0.4.2/bromine/django_admin.py` & `gambit-bromine-0.4.3/bromine/django_admin.py`

 * *Files identical despite different names*

### Comparing `gambit-bromine-0.4.2/bromine/pytest.py` & `gambit-bromine-0.4.3/bromine/pytest.py`

 * *Files identical despite different names*

### Comparing `gambit-bromine-0.4.2/bromine/select2.py` & `gambit-bromine-0.4.3/bromine/select2.py`

 * *Files identical despite different names*

### Comparing `gambit-bromine-0.4.2/gambit_bromine.egg-info/PKG-INFO` & `gambit-bromine-0.4.3/gambit_bromine.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 Metadata-Version: 2.1
 Name: gambit-bromine
-Version: 0.4.2
+Version: 0.4.3
 Summary: Pythonic web testing
 Home-page: https://github.com/dvarrazzo/bromine
 Author: Daniele Varrazzo
 Author-email: daniele.varrazzo@gmail.com
 License: UNKNOWN
-Description: # Bromine: pythonic web testing
-        
-        Bromine is a wrapper around [selenium] to allow writing testing in a terse and
-        *pythonic* rather that *java-esque* way.
-        
-        [selenium]: https://www.seleniumhq.org/
-        
-        Selenium is cool: you register browser to a hub, you ask browsers from a hub,
-        you use the browser, and you put it back. It works like magic.
-        
-        Except if you want to use https. But who needs https these days?
-        
-        Anyway, enough dissing well intentioned web testing systems. Let's talk bad
-        about bad testing system. You know what you have to do to wait for a page to
-        load after a get, and then check if an element is visible? The selenium docs
-        [will tell you](https://selenium-python.readthedocs.io/waits.html#explicit-waits):
-        
-        ```python
-        from selenium.webdriver.common.by import By
-        from selenium.webdriver.support.ui import WebDriverWait
-        from selenium.webdriver.support import expected_conditions as EC
-        
-        # ...
-        driver.get("http://example.com")
-        element = WebDriverWait(driver, 10).until(
-        	EC.presence_of_element_located((By.ID, "myDynamicElement"))
-        )
-        ```
-        
-        I've been kind and I've stripped some boilerplate. If you are happy about
-        importing three objects from 4 levels of namespaces and create a wait object
-        and pass a 2-element tuple to the "convenience method"
-        `selenium.webdriver.support.expected_conditions.visibility_of_element_located`
-        for a thing you have to do pretty much every time you click on a link, please
-        stop reading here: type `pip install selenium` and off you go. The following
-        paragraph is only for people who think the above is unsatisfactory in Python.
-        
-        Still reading? Sure?
-        
-        Well, I'll be honest: what I prefer to do is:
-        
-        ```python
-        import bromine
-        browser = bromine.Browser(driver)
-        element = browser.get("http://example.com/").wait(id='myDynamicElement')
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier:         Framework :: Pytest
 Classifier:         Intended Audience :: Developers
 Classifier:         License :: OSI Approved :: MIT License
 Classifier:         Operating System :: OS Independent
 Classifier:         Programming Language :: Python :: 3
 Classifier:         Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier:         Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Bromine: pythonic web testing
+
+Bromine is a wrapper around [selenium] to allow writing testing in a terse and
+*pythonic* rather that *java-esque* way.
+
+[selenium]: https://www.seleniumhq.org/
+
+Selenium is cool: you register browser to a hub, you ask browsers from a hub,
+you use the browser, and you put it back. It works like magic.
+
+Except if you want to use https. But who needs https these days?
+
+Anyway, enough dissing well intentioned web testing systems. Let's talk bad
+about bad testing system. You know what you have to do to wait for a page to
+load after a get, and then check if an element is visible? The selenium docs
+[will tell you](https://selenium-python.readthedocs.io/waits.html#explicit-waits):
+
+```python
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support.ui import WebDriverWait
+from selenium.webdriver.support import expected_conditions as EC
+
+# ...
+driver.get("http://example.com")
+element = WebDriverWait(driver, 10).until(
+	EC.presence_of_element_located((By.ID, "myDynamicElement"))
+)
+```
+
+I've been kind and I've stripped some boilerplate. If you are happy about
+importing three objects from 4 levels of namespaces and create a wait object
+and pass a 2-element tuple to the "convenience method"
+`selenium.webdriver.support.expected_conditions.visibility_of_element_located`
+for a thing you have to do pretty much every time you click on a link, please
+stop reading here: type `pip install selenium` and off you go. The following
+paragraph is only for people who think the above is unsatisfactory in Python.
+
+Still reading? Sure?
+
+Well, I'll be honest: what I prefer to do is:
+
+```python
+import bromine
+browser = bromine.Browser(driver)
+element = browser.get("http://example.com/").wait(id='myDynamicElement')
+```
+
+
```

### Comparing `gambit-bromine-0.4.2/setup.py` & `gambit-bromine-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="gambit-bromine",
-    version="0.4.2",
+    version="0.4.3",
     author="Daniele Varrazzo",
     author_email="daniele.varrazzo@gmail.com",
     description="Pythonic web testing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dvarrazzo/bromine",
     packages=setuptools.find_packages(),
```

