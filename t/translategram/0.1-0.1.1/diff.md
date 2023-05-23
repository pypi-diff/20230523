# Comparing `tmp/translategram-0.1.tar.gz` & `tmp/translategram-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translategram-0.1.tar", last modified: Sun May  7 15:47:12 2023, max compression
+gzip compressed data, was "translategram-0.1.1.tar", last modified: Tue May 23 00:42:39 2023, max compression
```

## Comparing `translategram-0.1.tar` & `translategram-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-07 15:47:12.582630 translategram-0.1/
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1069 2023-05-06 14:12:58.000000 translategram-0.1/LICENSE
--rw-r--r--   0 akbar     (1000) akbar     (1000)       26 2023-05-06 14:28:03.000000 translategram-0.1/MANIFEST.in
--rw-r--r--   0 akbar     (1000) akbar     (1000)     4140 2023-05-07 15:47:12.581630 translategram-0.1/PKG-INFO
--rw-r--r--   0 akbar     (1000) akbar     (1000)     3351 2023-05-07 15:28:54.000000 translategram-0.1/README.md
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-07 15:47:12.578630 translategram-0.1/auto_translategram/
--rw-r--r--   0 akbar     (1000) akbar     (1000)      188 2023-05-06 14:22:50.000000 translategram-0.1/auto_translategram/__init__.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-07 15:47:12.579630 translategram-0.1/auto_translategram/auto_translategram/
--rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-29 15:46:48.000000 translategram-0.1/auto_translategram/auto_translategram/__init__.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)       69 2023-05-06 13:39:39.000000 translategram-0.1/auto_translategram/auto_translategram/service_libs.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1120 2023-05-07 13:51:02.000000 translategram-0.1/auto_translategram/auto_translategram/translator.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1278 2023-05-06 13:39:33.000000 translategram-0.1/auto_translategram/auto_translategram/translator_services.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-07 15:47:12.580630 translategram-0.1/auto_translategram/python_telegram_bot_translator/
--rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-30 15:04:38.000000 translategram-0.1/auto_translategram/python_telegram_bot_translator/__init__.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)     2655 2023-05-07 13:54:10.000000 translategram-0.1/auto_translategram/python_telegram_bot_translator/adapter.py
--rw-r--r--   0 akbar     (1000) akbar     (1000)       38 2023-05-07 15:47:12.582630 translategram-0.1/setup.cfg
--rw-r--r--   0 akbar     (1000) akbar     (1000)     1152 2023-05-07 15:47:05.000000 translategram-0.1/setup.py
-drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-07 15:47:12.581630 translategram-0.1/translategram.egg-info/
--rw-r--r--   0 akbar     (1000) akbar     (1000)     4140 2023-05-07 15:47:12.000000 translategram-0.1/translategram.egg-info/PKG-INFO
--rw-r--r--   0 akbar     (1000) akbar     (1000)      593 2023-05-07 15:47:12.000000 translategram-0.1/translategram.egg-info/SOURCES.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)        1 2023-05-07 15:47:12.000000 translategram-0.1/translategram.egg-info/dependency_links.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)       11 2023-05-07 15:47:12.000000 translategram-0.1/translategram.egg-info/requires.txt
--rw-r--r--   0 akbar     (1000) akbar     (1000)       19 2023-05-07 15:47:12.000000 translategram-0.1/translategram.egg-info/top_level.txt
+drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.419198 translategram-0.1.1/
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     1069 2023-05-06 14:12:58.000000 translategram-0.1.1/LICENSE
+-rw-r--r--   0 akbar     (1000) akbar     (1000)       26 2023-05-06 14:28:03.000000 translategram-0.1.1/MANIFEST.in
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     4142 2023-05-23 00:42:39.418198 translategram-0.1.1/PKG-INFO
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     3351 2023-05-07 15:28:54.000000 translategram-0.1.1/README.md
+drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.417198 translategram-0.1.1/auto_translategram/
+-rw-r--r--   0 akbar     (1000) akbar     (1000)      188 2023-05-06 14:22:50.000000 translategram-0.1.1/auto_translategram/__init__.py
+drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.417198 translategram-0.1.1/auto_translategram/auto_translategram/
+-rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-29 15:46:48.000000 translategram-0.1.1/auto_translategram/auto_translategram/__init__.py
+-rw-r--r--   0 akbar     (1000) akbar     (1000)       69 2023-05-17 17:58:22.000000 translategram-0.1.1/auto_translategram/auto_translategram/service_libs.py
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     1183 2023-05-22 23:44:48.000000 translategram-0.1.1/auto_translategram/auto_translategram/translator.py
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     1283 2023-05-17 18:00:58.000000 translategram-0.1.1/auto_translategram/auto_translategram/translator_services.py
+drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.418198 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/
+-rw-r--r--   0 akbar     (1000) akbar     (1000)        0 2023-04-30 15:04:38.000000 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/__init__.py
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     2769 2023-05-22 23:56:52.000000 translategram-0.1.1/auto_translategram/python_telegram_bot_translator/adapter.py
+-rw-r--r--   0 akbar     (1000) akbar     (1000)       38 2023-05-23 00:42:39.419198 translategram-0.1.1/setup.cfg
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     1154 2023-05-23 00:38:41.000000 translategram-0.1.1/setup.py
+drwxr-xr-x   0 akbar     (1000) akbar     (1000)        0 2023-05-23 00:42:39.418198 translategram-0.1.1/translategram.egg-info/
+-rw-r--r--   0 akbar     (1000) akbar     (1000)     4142 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/PKG-INFO
+-rw-r--r--   0 akbar     (1000) akbar     (1000)      593 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/SOURCES.txt
+-rw-r--r--   0 akbar     (1000) akbar     (1000)        1 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/dependency_links.txt
+-rw-r--r--   0 akbar     (1000) akbar     (1000)       11 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/requires.txt
+-rw-r--r--   0 akbar     (1000) akbar     (1000)       19 2023-05-23 00:42:39.000000 translategram-0.1.1/translategram.egg-info/top_level.txt
```

### Comparing `translategram-0.1/LICENSE` & `translategram-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `translategram-0.1/PKG-INFO` & `translategram-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1
+Version: 0.1.1
 Summary: Python library for translating messages in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `translategram-0.1/README.md` & `translategram-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `translategram-0.1/auto_translategram/auto_translategram/translator.py` & `translategram-0.1.1/auto_translategram/auto_translategram/translator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import ABC, abstractmethod
-from typing import Callable
+from typing import Any, Callable, Coroutine, TypeVar
 from .translator_services import TranslatorService
 
+T = TypeVar('T')
+
 
 class Translator(ABC):
     """
     Abstract base class for implementing translation functionality in various frameworks.
     This class provides a uniform interface for translation, allowing adapters to be written for different frameworks.
     This class is meant to be subclassed, and the `handler_translator` method should be implemented in the subclass.
     """
@@ -14,14 +16,14 @@
         Initializes a new Translator instance using the specified `translator_service`.
 
         :param translator_service: The `BaseTranslatorService` to use for translations.
         """
         ...
 
     @abstractmethod
-    def handler_translator(self, func: Callable[..., None], message: str) -> Callable[..., None]:
+    def handler_translator(self, func: Callable[..., None], message: str) -> Callable[..., Coroutine[Any, Any, Any]]:
         """
         Translate a message based on the users' language
         :param func: The handler function that is used for handling commands by Frameworks.
         :param message: The message to translate.
         """
         ...
```

### Comparing `translategram-0.1/auto_translategram/auto_translategram/translator_services.py` & `translategram-0.1.1/auto_translategram/auto_translategram/translator_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
         if not isinstance(text, str) or not isinstance(target_language, str) or not isinstance(source_language, str):
             raise TypeError('`text`, `target_language` and `source_language` must be a string')
         translated_text = self.service.translate(
             to_translate=text,
             to_language=target_language,
             from_language=source_language
             )
-        return translated_text
+        return str(translated_text)
```

### Comparing `translategram-0.1/auto_translategram/python_telegram_bot_translator/adapter.py` & `translategram-0.1.1/auto_translategram/python_telegram_bot_translator/adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import inspect
-from typing import Any, Coroutine, Callable
+from typing import Any, Coroutine, Callable, Type, TypeVar
 from telegram.ext import ContextTypes
 from telegram import Update
 from ..auto_translategram.translator_services import TranslatorService
 from ..auto_translategram.translator import Translator
 
+_T = TypeVar('_T')
+
 
 class PythonTelegramBotAdapter(Translator):
     """
     A Translator adapter for the python-telegram-bot framework.
 
     Inherits from the abstract class `Translator` and implements its `handler_translator` method
     to provide translation functionality for the python-telegram-bot framework.
 
     :param translator_service: The `TranslatorService` to use for translations.
     """
 
-    def __init__(self, translator_service: TranslatorService):
+    def __init__(self, translator_service: Type[TranslatorService]):
         """
         Initializes a new PythonTelegramBotAdapter instance using the specified `translator_service`.
 
         :param translator_service: The `TranslatorService` to use for translations.
         """
         self._translator_service = translator_service()
 
     def handler_translator(
             self,
-            func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], None],
+            func: Callable[[Update, ContextTypes.DEFAULT_TYPE, str], _T],
             message: str) -> Callable[[Update, ContextTypes.DEFAULT_TYPE, str], Coroutine[Any, Any, Any]]:
         """
         A decorator that wraps a python-telegram-bot `handler` function to provide translation functionality.
 
         The decorated function will be executed after being wrapped with a new function that translates
         the incoming message into the user's preferred language (if it is not already in that language).
         If the user does not have a preferred language set or if it is set to 'en', the message will not be translated.
@@ -46,11 +48,14 @@
             if user_lang != 'en' and user_lang is not None:
                 message = await self._translator_service.translate_str(
                     text=message,
                     target_language=user_lang,
                     source_language='en'
                     )
             is_async = inspect.iscoroutinefunction(func)
-            result = (await func(update, context, message)) if is_async else func(update, context, message)
+            if is_async:
+                result = await func(update, context, message)  # type: ignore[misc]
+            else:
+                result = func(update, context, message)
             return result
 
         return wrapper
```

### Comparing `translategram-0.1/setup.py` & `translategram-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='translategram',
-    version='0.1',
+    version='0.1.1',
     description='Python library for translating messages in Telegram',
     url='https://github.com/EkberHasanov/translategram',
     author='Akbar',
     author_email='hasanvakbar@gmail.com',
     license='MIT',
     install_requires=[
         'mtranslate',
```

### Comparing `translategram-0.1/translategram.egg-info/PKG-INFO` & `translategram-0.1.1/translategram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translategram
-Version: 0.1
+Version: 0.1.1
 Summary: Python library for translating messages in Telegram
 Home-page: https://github.com/EkberHasanov/translategram
 Author: Akbar
 Author-email: hasanvakbar@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `translategram-0.1/translategram.egg-info/SOURCES.txt` & `translategram-0.1.1/translategram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

