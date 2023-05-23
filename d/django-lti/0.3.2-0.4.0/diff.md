# Comparing `tmp/django-lti-0.3.2.tar.gz` & `tmp/django-lti-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lti-0.3.2.tar", last modified: Tue Dec 20 15:30:10 2022, max compression
+gzip compressed data, was "django-lti-0.4.0.tar", last modified: Tue May 23 17:08:11 2023, max compression
```

## Comparing `django-lti-0.3.2.tar` & `django-lti-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2022-12-20 15:29:59.000000 django-lti-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2022-12-20 15:30:10.466941 django-lti-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2022-12-20 15:29:59.000000 django-lti-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.462941 django-lti-0.3.2/django_lti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 15:30:10.000000 django-lti-0.3.2/django_lti.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/lti_tool/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/lti_tool/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/lti_tool/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/management/commands/rotate_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/lti_tool/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/migrations/0002_create_lti_domain_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/migrations/0003_lticontext_memberships_url_ltimembership_is_active.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25202 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:30:10.466941 django-lti-0.3.2/lti_tool/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/services/nrps.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9141 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2022-12-20 15:29:59.000000 django-lti-0.3.2/lti_tool/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2022-12-20 15:29:59.000000 django-lti-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-20 15:30:10.466941 django-lti-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 15:29:59.000000 django-lti-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.975377 django-lti-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 17:08:03.000000 django-lti-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-23 17:08:11.975377 django-lti-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-23 17:08:03.000000 django-lti-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.967377 django-lti-0.4.0/django_lti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 17:08:11.000000 django-lti-0.4.0/django_lti.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.971377 django-lti-0.4.0/lti_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.971377 django-lti-0.4.0/lti_tool/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.971377 django-lti-0.4.0/lti_tool/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/management/commands/rotate_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.975377 django-lti-0.4.0/lti_tool/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/0002_create_lti_domain_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/0003_lticontext_memberships_url_ltimembership_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/0004_lticontext_can_access_results_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/0005_ltilineitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26839 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.975377 django-lti-0.4.0/lti_tool/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/services/nrps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-05-23 17:08:03.000000 django-lti-0.4.0/lti_tool/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 17:08:03.000000 django-lti-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-23 17:08:11.975377 django-lti-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:08:03.000000 django-lti-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:08:11.975377 django-lti-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-23 17:08:03.000000 django-lti-0.4.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-23 17:08:03.000000 django-lti-0.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-23 17:08:03.000000 django-lti-0.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 17:08:03.000000 django-lti-0.4.0/tests/test_views.py
```

### Comparing `django-lti-0.3.2/LICENSE` & `django-lti-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/PKG-INFO` & `django-lti-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: django-lti
-Version: 0.3.2
+Version: 0.4.0
 Summary: LTI tool support for Django
 Home-page: https://github.com/academic-innovation/django-lti
+Project-URL: Documentation, https://academic-innovation.github.io/django-lti/
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-lti-0.3.2/README.md` & `django-lti-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/django_lti.egg-info/PKG-INFO` & `django-lti-0.4.0/django_lti.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: django-lti
-Version: 0.3.2
+Version: 0.4.0
 Summary: LTI tool support for Django
 Home-page: https://github.com/academic-innovation/django-lti
+Project-URL: Documentation, https://academic-innovation.github.io/django-lti/
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-lti-0.3.2/django_lti.egg-info/SOURCES.txt` & `django-lti-0.4.0/django_lti.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,10 +22,16 @@
 lti_tool/views.py
 lti_tool/management/__init__.py
 lti_tool/management/commands/__init__.py
 lti_tool/management/commands/rotate_keys.py
 lti_tool/migrations/0001_initial.py
 lti_tool/migrations/0002_create_lti_domain_models.py
 lti_tool/migrations/0003_lticontext_memberships_url_ltimembership_is_active.py
+lti_tool/migrations/0004_lticontext_can_access_results_and_more.py
+lti_tool/migrations/0005_ltilineitem.py
 lti_tool/migrations/__init__.py
 lti_tool/services/__init__.py
-lti_tool/services/nrps.py
+lti_tool/services/nrps.py
+tests/test_commands.py
+tests/test_models.py
+tests/test_utils.py
+tests/test_views.py
```

### Comparing `django-lti-0.3.2/lti_tool/decorators.py` & `django-lti-0.4.0/lti_tool/decorators.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/factories.py` & `django-lti-0.4.0/lti_tool/factories.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/management/commands/rotate_keys.py` & `django-lti-0.4.0/lti_tool/management/commands/rotate_keys.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/middleware.py` & `django-lti-0.4.0/lti_tool/middleware.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/migrations/0001_initial.py` & `django-lti-0.4.0/lti_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/migrations/0002_create_lti_domain_models.py` & `django-lti-0.4.0/lti_tool/migrations/0002_create_lti_domain_models.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/migrations/0003_lticontext_memberships_url_ltimembership_is_active.py` & `django-lti-0.4.0/lti_tool/migrations/0003_lticontext_memberships_url_ltimembership_is_active.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/models.py` & `django-lti-0.4.0/lti_tool/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,16 +331,21 @@
         related_name="contexts",
         through="LtiMembership",
         verbose_name="members",
     )
     is_course_template = models.BooleanField(_("is course template"), default=False)
     is_course_offering = models.BooleanField(_("is course offering"), default=False)
     is_course_section = models.BooleanField(_("is course section"), default=False)
-    memberships_url = models.URLField(blank=True)
     is_group = models.BooleanField(_("is group"), default=False)
+    memberships_url = models.URLField(blank=True)
+    lineitems_url = models.URLField(_("lineitems URL"), blank=True)
+    can_query_lineitems = models.BooleanField(_("can query lineitems"), default=False)
+    can_manage_lineitems = models.BooleanField(_("can manage lineitems"), default=False)
+    can_publish_scores = models.BooleanField(_("can publish scores"), default=False)
+    can_access_results = models.BooleanField(_("can access results"), default=False)
     datetime_created = models.DateTimeField(_("created"), default=now, editable=False)
     datetime_modified = models.DateTimeField(_("modified"), auto_now=True)
 
     class Meta:
         verbose_name = _("LTI context")
         verbose_name_plural = _("LTI contexts")
         constraints = [
@@ -457,14 +462,43 @@
             )
         ]
 
     def __str__(self):
         return self.title if self.title else self.id_on_platform
 
 
+class LtiLineItem(models.Model):
+    """Represents an LTI LineItem for assignment scoring.
+
+    The line item scope and methods are described in the LTI Assignment and Grade
+    Services 2.0 spec at
+    https://www.imsglobal.org/spec/lti-ags/v2p0#line-item-service-scope-and-allowed-http-methods
+    """
+
+    context = models.ForeignKey(
+        LtiContext,
+        related_name="line_items",
+        on_delete=models.CASCADE,
+        verbose_name=_("context"),
+    )
+    url = models.URLField(_("URL on platform"), unique=True)
+    maximum_score = models.FloatField(_("maximum score"))
+    label = models.CharField(_("label"), max_length=255)
+    tag = models.CharField(_("tag"), max_length=255, blank=True)
+    resource_id = models.CharField(_("resource ID"), max_length=255, blank=True)
+    resource_link = models.ForeignKey(
+        LtiResourceLink, on_delete=models.SET_NULL, null=True
+    )
+    start_datetime = models.DateTimeField(_("start date/time"), null=True)
+    end_datetime = models.DateTimeField(_("end date/time"), null=True)
+
+    def __str__(self):
+        return self.label
+
+
 class ViewportDimensions(NamedTuple):
     width: int
     height: int
 
 
 class LtiLaunch:
     """A LTI launch."""
@@ -563,14 +597,18 @@
     @property
     def nrps_claim(self):
         return self.get_claim(
             "https://purl.imsglobal.org/spec/lti-nrps/claim/namesroleservice"
         )
 
     @property
+    def ags_claim(self):
+        return self.get_claim("https://purl.imsglobal.org/spec/lti-ags/claim/endpoint")
+
+    @property
     def context_claim(self):
         return self.get_claim("https://purl.imsglobal.org/spec/lti/claim/context")
 
     @cached_property
     def context(self) -> LtiContext:
         context_id = self.context_claim["id"] if self.context_claim is not None else ""
         return LtiContext.objects.get(
```

### Comparing `django-lti-0.3.2/lti_tool/services/nrps.py` & `django-lti-0.4.0/lti_tool/services/nrps.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/lti_tool/utils.py` & `django-lti-0.4.0/lti_tool/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from django.http.request import HttpRequest
 
 from pylti1p3.contrib.django.launch_data_storage.cache import DjangoCacheDataStorage
 from pylti1p3.contrib.django.message_launch import DjangoMessageLaunch
 from pylti1p3.deployment import Deployment
 from pylti1p3.tool_config.abstract import ToolConfAbstract
 
-from .constants import ContextRole
+from .constants import AgsScope, ContextRole, ContextType
 from .models import (
     LtiContext,
     LtiDeployment,
     LtiLaunch,
     LtiMembership,
     LtiPlatformInstance,
     LtiRegistration,
@@ -134,52 +134,49 @@
         registration=lti_launch.registration,
         sub=sub,
         defaults={k: v for k, v in user_claims.items() if v is not None},
     )
     return lti_user
 
 
+def _get_ags_props(lti_launch: LtiLaunch) -> dict:
+    ags_claim = lti_launch.ags_claim
+    if ags_claim is None:
+        return {}
+    ags_scope = ags_claim.get("scope", [])
+    return {
+        "lineitems_url": ags_claim.get("lineitems", ""),
+        "can_query_lineitems": AgsScope.QUERY_LINEITEMS in ags_scope,
+        "can_manage_lineitems": AgsScope.MANAGE_LINEITEMS in ags_scope,
+        "can_publish_scores": AgsScope.PUBLISH_SCORES in ags_scope,
+        "can_access_results": AgsScope.ACCESS_RESULTS in ags_scope,
+    }
+
+
 def sync_context_from_launch(lti_launch: LtiLaunch) -> LtiContext:
-    context_claim = lti_launch.context_claim
+    context_claim = {} if lti_launch.context_claim is None else lti_launch.context_claim
     nrps_claim = lti_launch.nrps_claim
     nrps_endpoint = "" if nrps_claim is None else nrps_claim["context_memberships_url"]
-    context_types = [] if context_claim is None else context_claim.get("type", [])
-    if context_claim is None:
-        context, _created = LtiContext.objects.get_or_create(
-            deployment=lti_launch.deployment,
-            id_on_platform="",
-            memberships_url=nrps_endpoint,
-        )
-    else:
-        defaults = {
-            "title": context_claim.get("title", ""),
-            "label": context_claim.get("label", ""),
-            "is_course_template": (
-                "http://purl.imsglobal.org/vocab/lis/v2/course#CourseTemplate"
-                in context_types
-            ),
-            "is_course_offering": (
-                "http://purl.imsglobal.org/vocab/lis/v2/course#CourseOffering"
-                in context_types
-            ),
-            "is_course_section": (
-                "http://purl.imsglobal.org/vocab/lis/v2/course#CourseSection"
-                in context_types
-            ),
-            "is_group": (
-                "http://purl.imsglobal.org/vocab/lis/v2/course#Group" in context_types
-            ),
-        }
-        if nrps_endpoint:
-            defaults["memberships_url"] = nrps_endpoint
-        context, _created = LtiContext.objects.update_or_create(
-            deployment=lti_launch.deployment,
-            id_on_platform=context_claim["id"],
-            defaults=defaults,
-        )
+    context_types = context_claim.get("type", [])
+    defaults = {
+        "title": context_claim.get("title", ""),
+        "label": context_claim.get("label", ""),
+        "is_course_template": (ContextType.COURSE_TEMPLATE in context_types),
+        "is_course_offering": (ContextType.COURSE_OFFERING in context_types),
+        "is_course_section": (ContextType.COURSE_SECTION in context_types),
+        "is_group": (ContextType.GROUP in context_types),
+    }
+    if nrps_endpoint:
+        defaults["memberships_url"] = nrps_endpoint
+    defaults.update(_get_ags_props(lti_launch))
+    context, _created = LtiContext.objects.update_or_create(
+        deployment=lti_launch.deployment,
+        id_on_platform=context_claim.get("id", ""),
+        defaults=defaults,
+    )
     return context
 
 
 def sync_membership_from_launch(
     lti_launch: LtiLaunch, user: LtiUser, context: LtiContext
 ) -> LtiMembership:
     roles = [normalize_role(role) for role in lti_launch.roles_claim]
```

### Comparing `django-lti-0.3.2/lti_tool/views.py` & `django-lti-0.4.0/lti_tool/views.py`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/pyproject.toml` & `django-lti-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-lti-0.3.2/setup.cfg` & `django-lti-0.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [metadata]
 name = django-lti
 version = attr: lti_tool.__version__
 description = LTI tool support for Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/academic-innovation/django-lti
+project_urls = 
+	Documentation = https://academic-innovation.github.io/django-lti/
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
```

