# Comparing `tmp/django-choicefield-0.2.1.tar.gz` & `tmp/django-choicefield-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-choicefield-0.2.1.tar", last modified: Thu Sep 29 20:00:59 2022, max compression
+gzip compressed data, was "django-choicefield-0.2.2.tar", last modified: Tue May 23 20:05:17 2023, max compression
```

## Comparing `django-choicefield-0.2.1.tar` & `django-choicefield-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 20:00:59.251678 django-choicefield-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-09-29 20:00:59.251678 django-choicefield-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4513 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-09-29 20:00:59.251678 django-choicefield-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 20:00:59.247678 django-choicefield-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 20:00:59.247678 django-choicefield-0.2.1/src/choicefield/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/src/choicefield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5964 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/src/choicefield/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 20:00:49.000000 django-choicefield-0.2.1/src/choicefield/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 20:00:59.251678 django-choicefield-0.2.1/src/django_choicefield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-09-29 20:00:59.000000 django-choicefield-0.2.1/src/django_choicefield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-29 20:00:59.000000 django-choicefield-0.2.1/src/django_choicefield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 20:00:59.000000 django-choicefield-0.2.1/src/django_choicefield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-09-29 20:00:59.000000 django-choicefield-0.2.1/src/django_choicefield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-29 20:00:59.000000 django-choicefield-0.2.1/src/django_choicefield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/src/choicefield/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/src/choicefield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/src/choicefield/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 20:05:00.000000 django-choicefield-0.2.2/src/choicefield/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:05:17.368053 django-choicefield-0.2.2/src/django_choicefield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-23 20:05:17.000000 django-choicefield-0.2.2/src/django_choicefield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 20:05:17.000000 django-choicefield-0.2.2/src/django_choicefield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:05:17.000000 django-choicefield-0.2.2/src/django_choicefield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 20:05:17.000000 django-choicefield-0.2.2/src/django_choicefield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 20:05:17.000000 django-choicefield-0.2.2/src/django_choicefield.egg-info/top_level.txt
```

### Comparing `django-choicefield-0.2.1/LICENSE` & `django-choicefield-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-choicefield-0.2.1/PKG-INFO` & `django-choicefield-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-choicefield
-Version: 0.2.1
+Version: 0.2.2
 Summary: ChoiceField for Django models
 Home-page: https://github.com/flaeppe/django-choicefield/
 Author: Petter Friberg
 Author-email: petter_friberg@hotmail.com
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
@@ -198,10 +199,11 @@
 
 ### Compatibility
 
 `django-choicefield` is tested according to the table below
 
 | Django version | Python version |
 | -------------- | -------------- |
+| 4.2.x          | ^3.9           |
 | 4.1.x          | ^3.9           |
 | 4.0.x          | ^3.9           |
 | 3.2.x          | ^3.9           |
```

### Comparing `django-choicefield-0.2.1/README.md` & `django-choicefield-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -171,10 +171,11 @@
 
 ### Compatibility
 
 `django-choicefield` is tested according to the table below
 
 | Django version | Python version |
 | -------------- | -------------- |
+| 4.2.x          | ^3.9           |
 | 4.1.x          | ^3.9           |
 | 4.0.x          | ^3.9           |
 | 3.2.x          | ^3.9           |
```

### Comparing `django-choicefield-0.2.1/setup.cfg` & `django-choicefield-0.2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 classifiers = 
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Development Status :: 4 - Beta
@@ -43,16 +44,11 @@
 [options.extras_require]
 test = 
 	pytest
 	pytest-django
 	pytest-cov
 	parameterized
 
-[flake8]
-max-complexity = 8
-max-line-length = 88
-show-source = true
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `django-choicefield-0.2.1/src/choicefield/fields.py` & `django-choicefield-0.2.2/src/choicefield/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,19 +64,15 @@
     empty_strings_allowed = False
 
     def __init__(self, enum: type[T], *args: Any, **kwargs: Any) -> None:
         self.enum = enum
         self._values = kwargs.pop("_values", None) or tuple(
             member.value for member in self.enum
         )
-        # Mypy: IMO `type[T]` should already support `iter()`. As it works for concrete
-        # subclasses of `enum.Enum`.
-        self.python_type = type(
-            next(iter(self.enum)).value  # type: ignore[call-overload]
-        )
+        self.python_type = type(next(iter(self.enum)).value)
         try:
             self._internal_type = supported_internal_types[self.python_type]
         except KeyError as exc:
             raise TypeError(
                 f"Enum with values of type {self.python_type.__name__!r}"
                 f" is not supported"
             ) from exc
@@ -84,16 +80,15 @@
         kwargs.setdefault("choices", self.enum_to_choices(self.enum))
         if self._internal_type == "CharField":
             kwargs.setdefault("max_length", 255)
         super().__init__(*args, **kwargs)
 
     def enum_to_choices(self, enum: type[T]) -> _ChoicesList:
         if hasattr(enum, "choices"):
-            # TODO: See https://github.com/typeddjango/django-stubs/pull/1154
-            return cast(type[Choices], enum).choices  # type: ignore[return-value]
+            return cast(type[Choices], enum).choices
         return [(member.value, member.name) for member in enum]
 
     def get_internal_type(self) -> str:
         return self._internal_type
 
     def from_db_value(
         self, value: Any, expression: Any, connection: Any
@@ -124,15 +119,18 @@
     def get_prep_value(self, value: Any) -> Any:
         value = self.to_python(super().get_prep_value(value))
         if isinstance(value, self.enum):
             return value.value
         return value
 
     def get_db_prep_value(
-        self, value: Any, connection: BaseDatabaseWrapper, prepared: bool = False
+        self,
+        value: Any,
+        connection: BaseDatabaseWrapper,
+        prepared: bool = False,  # noqa: FBT001,FBT002
     ) -> Any:
         prepared_value = super().get_db_prep_value(value, connection, prepared)
         if prepared_value is None and not self.null:
             raise ValidationError(self.error_messages["null"], code="null")
         elif isinstance(prepared_value, self.enum):
             prepared_value = prepared_value.value
```

### Comparing `django-choicefield-0.2.1/src/django_choicefield.egg-info/PKG-INFO` & `django-choicefield-0.2.2/src/django_choicefield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-choicefield
-Version: 0.2.1
+Version: 0.2.2
 Summary: ChoiceField for Django models
 Home-page: https://github.com/flaeppe/django-choicefield/
 Author: Petter Friberg
 Author-email: petter_friberg@hotmail.com
 License: BSD 3-Clause License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
@@ -198,10 +199,11 @@
 
 ### Compatibility
 
 `django-choicefield` is tested according to the table below
 
 | Django version | Python version |
 | -------------- | -------------- |
+| 4.2.x          | ^3.9           |
 | 4.1.x          | ^3.9           |
 | 4.0.x          | ^3.9           |
 | 3.2.x          | ^3.9           |
```

