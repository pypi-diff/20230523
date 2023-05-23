# Comparing `tmp/seleniumbot-0.0.2.tar.gz` & `tmp/seleniumbot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seleniumbot-0.0.2.tar", last modified: Tue May 23 17:04:55 2023, max compression
+gzip compressed data, was "seleniumbot-0.0.3.tar", last modified: Tue May 23 19:50:39 2023, max compression
```

## Comparing `seleniumbot-0.0.2.tar` & `seleniumbot-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3993 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3731 2023-05-23 16:57:50.000000 seleniumbot-0.0.2/README.md
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/seleniumbot/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       65 2023-05-23 15:57:49.000000 seleniumbot-0.0.2/seleniumbot/__init__.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/seleniumbot/core/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.2/seleniumbot/core/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1450 2023-05-23 15:53:54.000000 seleniumbot-0.0.2/seleniumbot/core/action.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3004 2023-05-23 16:29:38.000000 seleniumbot-0.0.2/seleniumbot/core/client.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1849 2023-05-23 16:44:16.000000 seleniumbot-0.0.2/seleniumbot/core/seleniumbot.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/seleniumbot/utils/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.2/seleniumbot/utils/__init__.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      317 2023-05-23 15:47:17.000000 seleniumbot-0.0.2/seleniumbot/utils/logger.py
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.2/seleniumbot/utils/randomizer.py
-drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/seleniumbot.egg-info/
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3993 2023-05-23 17:04:55.000000 seleniumbot-0.0.2/seleniumbot.egg-info/PKG-INFO
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-23 17:04:55.000000 seleniumbot-0.0.2/seleniumbot.egg-info/SOURCES.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-23 17:04:55.000000 seleniumbot-0.0.2/seleniumbot.egg-info/dependency_links.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        9 2023-05-23 17:04:55.000000 seleniumbot-0.0.2/seleniumbot.egg-info/requires.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-23 17:04:55.000000 seleniumbot-0.0.2/seleniumbot.egg-info/top_level.txt
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-23 17:04:55.699552 seleniumbot-0.0.2/setup.cfg
--rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 17:04:51.000000 seleniumbot-0.0.2/setup.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4528 2023-05-23 19:49:50.000000 seleniumbot-0.0.3/README.md
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/seleniumbot/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       65 2023-05-23 15:57:49.000000 seleniumbot-0.0.3/seleniumbot/__init__.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/seleniumbot/core/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      158 2023-05-23 15:57:49.000000 seleniumbot-0.0.3/seleniumbot/core/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1450 2023-05-23 15:53:54.000000 seleniumbot-0.0.3/seleniumbot/core/action.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     3225 2023-05-23 19:26:14.000000 seleniumbot-0.0.3/seleniumbot/core/client.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     1958 2023-05-23 19:26:14.000000 seleniumbot-0.0.3/seleniumbot/core/seleniumbot.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/seleniumbot/utils/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      100 2023-05-23 15:58:29.000000 seleniumbot-0.0.3/seleniumbot/utils/__init__.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      317 2023-05-23 15:47:17.000000 seleniumbot-0.0.3/seleniumbot/utils/logger.py
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      634 2023-05-23 16:44:25.000000 seleniumbot-0.0.3/seleniumbot/utils/randomizer.py
+drwxrwxr-x   0 xmolly    (1000) xmolly    (1000)        0 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/seleniumbot.egg-info/
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)     4790 2023-05-23 19:50:39.000000 seleniumbot-0.0.3/seleniumbot.egg-info/PKG-INFO
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      421 2023-05-23 19:50:39.000000 seleniumbot-0.0.3/seleniumbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)        1 2023-05-23 19:50:39.000000 seleniumbot-0.0.3/seleniumbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       23 2023-05-23 19:50:39.000000 seleniumbot-0.0.3/seleniumbot.egg-info/requires.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       12 2023-05-23 19:50:39.000000 seleniumbot-0.0.3/seleniumbot.egg-info/top_level.txt
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)       38 2023-05-23 19:50:39.786901 seleniumbot-0.0.3/setup.cfg
+-rw-rw-r--   0 xmolly    (1000) xmolly    (1000)      651 2023-05-23 19:50:31.000000 seleniumbot-0.0.3/setup.py
```

### Comparing `seleniumbot-0.0.2/PKG-INFO` & `seleniumbot-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,14 @@
-Metadata-Version: 2.1
-Name: seleniumbot
-Version: 0.0.2
-Summary: SeleniumBot
-Home-page: https://github.com/Mercurial5
-Author: Mercurial5
-Author-email: dias.nespayev@gmail.com
-Keywords: SeleniumBot
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 # SeleniumBot
 
 This library provides you tools that will help you create selenium bots.
 
 ## Installation
 
-pip install seleniumbot
+`pip install seleniumbot`
 
 ## Actions
 
 Actions are classes that will tell bot what to do. There are two types of actions, `simple` actions
 and `navigation` actions.
 
 Actions also have some required properties. Here's the list of them:
@@ -156,7 +145,41 @@
 
 
 if __name__ == '__main__':
     main()
 
 
 ```
+
+## Using proxy
+
+In order to use proxy, just pass second type of options to SeleniumBot.
+
+```python
+from scroll import ScrollAction
+from selenium.webdriver.chrome.options import Options
+from start import StartAction
+
+from seleniumbot import SeleniumBot
+
+
+def main():
+    # In order to test and see how bot behaves, we need to reassign options
+    # that will not use --headless mode.
+    options = Options()
+    options.add_argument('window-size=1920,1080')
+
+    seleniumwire_options = {
+        'proxy': {
+            'https': 'https://user:password@host:port'
+        }
+    }
+
+    bot = SeleniumBot(start_action=StartAction, options=options, seleniumwire_options=seleniumwire_options)
+    bot.set_navigation_actions([ScrollAction])
+    bot.start()
+
+
+if __name__ == '__main__':
+    main()
+
+```
```

### Comparing `seleniumbot-0.0.2/seleniumbot/core/action.py` & `seleniumbot-0.0.3/seleniumbot/core/action.py`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.2/seleniumbot/core/client.py` & `seleniumbot-0.0.3/seleniumbot/core/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import random
 import time
 
-from selenium.webdriver import Chrome
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.wait import WebDriverWait
+from seleniumwire.webdriver import Chrome
 
 from seleniumbot.utils import Randomizer
 
 
 class SeleniumClient:
 
-    def __init__(self, options: Options | None = None, **kwargs):
-        self._driver = self.__get_driver(options)
+    def __init__(self, options: Options | None = None, seleniumwire_options: dict | None = None, **kwargs):
+        self._driver = self.__get_driver(options, seleniumwire_options)
 
         self.__min_action_delay = kwargs.get('min_action_delay', 0.7)
         self.__max_action_delay = kwargs.get('max_action_delay', 3)
         self.__webdriver_wait_time = kwargs.get('webdriver_wait_time', 60)
 
     @staticmethod
     def _delay(foo):
@@ -65,19 +65,21 @@
     @_delay
     def send_keys(self, element: WebElement, value: str) -> None:
         element.send_keys(value)
 
     def __del__(self):
         self._driver.close()
 
-    def __get_driver(self, options: Options | None) -> Chrome:
+    def __get_driver(self, options: Options | None, seleniumwire_options: dict | None) -> Chrome:
         if not options:
             options = self.__get_default_options()
+        if not seleniumwire_options:
+            seleniumwire_options = {}
 
-        driver = Chrome(chrome_options=options)
+        driver = Chrome(chrome_options=options, seleniumwire_options=seleniumwire_options)
         return driver
 
     @staticmethod
     def __get_default_options() -> Options:
         options = Options()
         options.add_argument('window-size=1920,1080')
         options.add_argument('--no-sandbox')
```

### Comparing `seleniumbot-0.0.2/seleniumbot/core/seleniumbot.py` & `seleniumbot-0.0.3/seleniumbot/core/seleniumbot.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from seleniumbot.core.client import SeleniumClient
 from seleniumbot.utils.randomizer import Randomizer
 
 
 class SeleniumBot:
     def __init__(self, start_action: Type[Action], **kwargs):
         options = kwargs.get('options')
-        self.client = SeleniumClient(options=options)
+        seleniumwire_options = kwargs.get('seleniumwire_options')
+        self.client = SeleniumClient(options=options, seleniumwire_options=seleniumwire_options)
 
         self.navigations = []
         self.actions: list[Action] = []
         self.last_action: Action | None = None
 
         start_action().execute(self.client, self.last_action)
```

### Comparing `seleniumbot-0.0.2/seleniumbot/utils/randomizer.py` & `seleniumbot-0.0.3/seleniumbot/utils/randomizer.py`

 * *Files identical despite different names*

### Comparing `seleniumbot-0.0.2/seleniumbot.egg-info/PKG-INFO` & `seleniumbot-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: seleniumbot
-Version: 0.0.2
+Version: 0.0.3
 Summary: SeleniumBot
 Home-page: https://github.com/Mercurial5
 Author: Mercurial5
 Author-email: dias.nespayev@gmail.com
 Keywords: SeleniumBot
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # SeleniumBot
 
 This library provides you tools that will help you create selenium bots.
 
 ## Installation
 
-pip install seleniumbot
+`pip install seleniumbot`
 
 ## Actions
 
 Actions are classes that will tell bot what to do. There are two types of actions, `simple` actions
 and `navigation` actions.
 
 Actions also have some required properties. Here's the list of them:
@@ -156,7 +156,41 @@
 
 
 if __name__ == '__main__':
     main()
 
 
 ```
+
+## Using proxy
+
+In order to use proxy, just pass second type of options to SeleniumBot.
+
+```python
+from scroll import ScrollAction
+from selenium.webdriver.chrome.options import Options
+from start import StartAction
+
+from seleniumbot import SeleniumBot
+
+
+def main():
+    # In order to test and see how bot behaves, we need to reassign options
+    # that will not use --headless mode.
+    options = Options()
+    options.add_argument('window-size=1920,1080')
+
+    seleniumwire_options = {
+        'proxy': {
+            'https': 'https://user:password@host:port'
+        }
+    }
+
+    bot = SeleniumBot(start_action=StartAction, options=options, seleniumwire_options=seleniumwire_options)
+    bot.set_navigation_actions([ScrollAction])
+    bot.start()
+
+
+if __name__ == '__main__':
+    main()
+
+```
```

### Comparing `seleniumbot-0.0.2/setup.py` & `seleniumbot-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='seleniumbot',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     url='https://github.com/Mercurial5',
     author='Mercurial5',
     author_email='dias.nespayev@gmail.com',
     keywords='SeleniumBot',
     description='SeleniumBot',
     python_requires=">=3.11",
-    install_requires=['selenium'],
+    install_requires=['selenium', 'selenium-wire'],
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

