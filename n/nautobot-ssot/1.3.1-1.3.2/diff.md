# Comparing `tmp/nautobot_ssot-1.3.1.tar.gz` & `tmp/nautobot_ssot-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_ssot-1.3.1.tar", max compression
+gzip compressed data, was "nautobot_ssot-1.3.2.tar", max compression
```

## Comparing `nautobot_ssot-1.3.1.tar` & `nautobot_ssot-1.3.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      591 2023-05-02 18:37:13.177222 nautobot_ssot-1.3.1/LICENSE
--rw-r--r--   0        0        0     4936 2023-05-02 18:37:13.177222 nautobot_ssot-1.3.1/README.md
--rw-r--r--   0        0        0     1089 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/__init__.py
--rw-r--r--   0        0        0       48 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/api/__init__.py
--rw-r--r--   0        0        0      828 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/choices.py
--rw-r--r--   0        0        0     1054 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/filters.py
--rw-r--r--   0        0        0     1541 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/forms.py
--rw-r--r--   0        0        0      916 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/jobs/__init__.py
--rw-r--r--   0        0        0    15543 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/jobs/base.py
--rw-r--r--   0        0        0    25274 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/jobs/examples.py
--rw-r--r--   0        0        0     4846 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/metrics.py
--rw-r--r--   0        0        0     3035 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/migrations/0001_initial.py
--rw-r--r--   0        0        0     2378 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/migrations/0002_performance_metrics.py
--rw-r--r--   0        0        0      586 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
--rw-r--r--   0        0        0      408 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/migrations/0004_sync_summary.py
--rw-r--r--   0        0        0        0 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/migrations/__init__.py
--rw-r--r--   0        0        0     8764 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/models.py
--rw-r--r--   0        0        0      601 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/navigation.py
--rw-r--r--   0        0        0     6527 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/tables.py
--rw-r--r--   0        0        0     1017 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/template_content.py
--rw-r--r--   0        0        0     3847 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/dashboard.html
--rw-r--r--   0        0        0     4682 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
--rw-r--r--   0        0        0      432 2023-05-02 18:37:13.185222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/history.html
--rw-r--r--   0        0        0     8843 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
--rw-r--r--   0        0        0     2513 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_header.html
--rw-r--r--   0        0        0      365 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
--rw-r--r--   0        0        0      322 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
--rw-r--r--   0        0        0      397 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
--rw-r--r--   0        0        0      579 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
--rw-r--r--   0        0        0        0 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templatetags/__init__.py
--rw-r--r--   0        0        0      694 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templatetags/dashboard_helpers.py
--rw-r--r--   0        0        0      787 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templatetags/humanize_bytes.py
--rw-r--r--   0        0        0     2214 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templatetags/render_diff.py
--rw-r--r--   0        0        0      570 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/templatetags/shorter_timedelta.py
--rw-r--r--   0        0        0      257 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/__init__.py
--rw-r--r--   0        0        0      662 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/jobs/__init__.py
--rw-r--r--   0        0        0      983 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_api.py
--rw-r--r--   0        0        0     1518 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_basic.py
--rw-r--r--   0        0        0     5018 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_jobs.py
--rw-r--r--   0        0        0     3058 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_models.py
--rw-r--r--   0        0        0     2437 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_render_diff.py
--rw-r--r--   0        0        0     5634 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/tests/test_views.py
--rw-r--r--   0        0        0     1004 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/urls.py
--rw-r--r--   0        0        0     6326 2023-05-02 18:37:13.189222 nautobot_ssot-1.3.1/nautobot_ssot/views.py
--rw-r--r--   0        0        0     3798 2023-05-02 18:37:23.877069 nautobot_ssot-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6345 1970-01-01 00:00:00.000000 nautobot_ssot-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-23 13:50:19.410350 nautobot_ssot-1.3.2/LICENSE
+-rw-r--r--   0        0        0     4936 2023-05-23 13:50:19.410350 nautobot_ssot-1.3.2/README.md
+-rw-r--r--   0        0        0     1089 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/__init__.py
+-rw-r--r--   0        0        0       48 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/api/__init__.py
+-rw-r--r--   0        0        0      828 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/choices.py
+-rw-r--r--   0        0        0     1088 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/filters.py
+-rw-r--r--   0        0        0     1541 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/forms.py
+-rw-r--r--   0        0        0      916 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/__init__.py
+-rw-r--r--   0        0        0    15543 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/base.py
+-rw-r--r--   0        0        0    25274 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/jobs/examples.py
+-rw-r--r--   0        0        0     4846 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/metrics.py
+-rw-r--r--   0        0        0     3035 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2378 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0002_performance_metrics.py
+-rw-r--r--   0        0        0      586 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py
+-rw-r--r--   0        0        0      408 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/0004_sync_summary.py
+-rw-r--r--   0        0        0        0 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/migrations/__init__.py
+-rw-r--r--   0        0        0     8764 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/models.py
+-rw-r--r--   0        0        0      601 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/navigation.py
+-rw-r--r--   0        0        0     6527 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tables.py
+-rw-r--r--   0        0        0     1017 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/template_content.py
+-rw-r--r--   0        0        0     3847 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/dashboard.html
+-rw-r--r--   0        0        0     4682 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/data_source_target.html
+-rw-r--r--   0        0        0      432 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/history.html
+-rw-r--r--   0        0        0     8843 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_detail.html
+-rw-r--r--   0        0        0     2513 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_header.html
+-rw-r--r--   0        0        0      365 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_jobresult.html
+-rw-r--r--   0        0        0      322 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_logentries.html
+-rw-r--r--   0        0        0      292 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/synclogentry_list.html
+-rw-r--r--   0        0        0      579 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html
+-rw-r--r--   0        0        0        0 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/__init__.py
+-rw-r--r--   0        0        0      694 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/dashboard_helpers.py
+-rw-r--r--   0        0        0      787 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/humanize_bytes.py
+-rw-r--r--   0        0        0     2214 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/render_diff.py
+-rw-r--r--   0        0        0      570 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/templatetags/shorter_timedelta.py
+-rw-r--r--   0        0        0      257 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/__init__.py
+-rw-r--r--   0        0        0      662 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/jobs/__init__.py
+-rw-r--r--   0        0        0      983 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_api.py
+-rw-r--r--   0        0        0     1518 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_basic.py
+-rw-r--r--   0        0        0     5018 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_jobs.py
+-rw-r--r--   0        0        0     3058 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_models.py
+-rw-r--r--   0        0        0     2437 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_render_diff.py
+-rw-r--r--   0        0        0     5634 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/tests/test_views.py
+-rw-r--r--   0        0        0     1004 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/urls.py
+-rw-r--r--   0        0        0     6326 2023-05-23 13:50:19.422351 nautobot_ssot-1.3.2/nautobot_ssot/views.py
+-rw-r--r--   0        0        0     3798 2023-05-23 13:50:32.703160 nautobot_ssot-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 nautobot_ssot-1.3.2/PKG-INFO
```

### Comparing `nautobot_ssot-1.3.1/LICENSE` & `nautobot_ssot-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/README.md` & `nautobot_ssot-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/__init__.py` & `nautobot_ssot-1.3.2/nautobot_ssot/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/choices.py` & `nautobot_ssot-1.3.2/nautobot_ssot/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/filters.py` & `nautobot_ssot-1.3.2/nautobot_ssot/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,8 +29,8 @@
         model = SyncLogEntry
         fields = ["sync", "action", "status", "synced_object_type"]
 
     def search(self, queryset, _name, value):  # pylint: disable=no-self-use
         """String search of SyncLogEntry records."""
         if not value.strip():
             return queryset
-        return queryset.filter(Q(diff__icontains=value) | Q(message__icontains=value))
+        return queryset.filter(Q(diff__icontains=value) | Q(message__icontains=value) | Q(object_repr__icontains=value))
```

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/forms.py` & `nautobot_ssot-1.3.2/nautobot_ssot/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/jobs/__init__.py` & `nautobot_ssot-1.3.2/nautobot_ssot/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/jobs/base.py` & `nautobot_ssot-1.3.2/nautobot_ssot/jobs/base.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/jobs/examples.py` & `nautobot_ssot-1.3.2/nautobot_ssot/jobs/examples.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/metrics.py` & `nautobot_ssot-1.3.2/nautobot_ssot/metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/migrations/0001_initial.py` & `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/migrations/0002_performance_metrics.py` & `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0002_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py` & `nautobot_ssot-1.3.2/nautobot_ssot/migrations/0003_alter_synclogentry_textfields.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/models.py` & `nautobot_ssot-1.3.2/nautobot_ssot/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/navigation.py` & `nautobot_ssot-1.3.2/nautobot_ssot/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tables.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/template_content.py` & `nautobot_ssot-1.3.2/nautobot_ssot/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/dashboard.html` & `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/dashboard.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/data_source_target.html` & `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/data_source_target.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_detail.html` & `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_detail.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/sync_header.html` & `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/sync_header.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html` & `nautobot_ssot-1.3.2/nautobot_ssot/templates/nautobot_ssot/templatetags/dashboard_data.html`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templatetags/dashboard_helpers.py` & `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/dashboard_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templatetags/humanize_bytes.py` & `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/humanize_bytes.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templatetags/render_diff.py` & `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/render_diff.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/templatetags/shorter_timedelta.py` & `nautobot_ssot-1.3.2/nautobot_ssot/templatetags/shorter_timedelta.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/jobs/__init__.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_api.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_basic.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_jobs.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_models.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_render_diff.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_render_diff.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/tests/test_views.py` & `nautobot_ssot-1.3.2/nautobot_ssot/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/urls.py` & `nautobot_ssot-1.3.2/nautobot_ssot/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/nautobot_ssot/views.py` & `nautobot_ssot-1.3.2/nautobot_ssot/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_ssot-1.3.1/pyproject.toml` & `nautobot_ssot-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-ssot"
-version = "v1.3.1"
+version = "v1.3.2"
 description = "Nautobot Single Source of Truth"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-ssot"
 repository = "https://github.com/nautobot/nautobot-plugin-ssot"
 documentation = "https://nautobot-plugin-ssot.readthedocs.io"
```

### Comparing `nautobot_ssot-1.3.1/PKG-INFO` & `nautobot_ssot-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-ssot
-Version: 1.3.1
+Version: 1.3.2
 Summary: Nautobot Single Source of Truth
 Home-page: https://github.com/nautobot/nautobot-plugin-ssot
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
@@ -13,18 +13,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: nautobot
 Requires-Dist: Markdown (!=3.3.5)
 Requires-Dist: diffsync (>=1.6.0,<2.0.0)
 Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra == "nautobot"
 Requires-Dist: packaging (>=21.3,<24)
 Requires-Dist: prometheus-client (>=0.14.1,<0.15.0)
 Project-URL: Documentation, https://nautobot-plugin-ssot.readthedocs.io
```

#### html2text {}

```diff
@@ -1,27 +1,24 @@
-Metadata-Version: 2.1 Name: nautobot-ssot Version: 1.3.1 Summary: Nautobot
+Metadata-Version: 2.1 Name: nautobot-ssot Version: 1.3.2 Summary: Nautobot
 Single Source of Truth Home-page: https://github.com/nautobot/nautobot-plugin-
 ssot License: Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network to
 Code, LLC Author-email: info@networktocode.com Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Provides-Extra: nautobot
-Requires-Dist: Markdown (!=3.3.5) Requires-Dist: diffsync (>=1.6.0,<2.0.0)
-Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra == "nautobot" Requires-Dist:
-packaging (>=21.3,<24) Requires-Dist: prometheus-client (>=0.14.1,<0.15.0)
-Project-URL: Documentation, https://nautobot-plugin-ssot.readthedocs.io
-Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-ssot
-Description-Content-Type: text/markdown # Nautobot Single Source of Truth
-(SSoT)
+Provides-Extra: nautobot Requires-Dist: Markdown (!=3.3.5) Requires-Dist:
+diffsync (>=1.6.0,<2.0.0) Requires-Dist: nautobot (>=1.4.0,<2.0.0) ; extra ==
+"nautobot" Requires-Dist: packaging (>=21.3,<24) Requires-Dist: prometheus-
+client (>=0.14.1,<0.15.0) Project-URL: Documentation, https://nautobot-plugin-
+ssot.readthedocs.io Project-URL: Repository, https://github.com/nautobot/
+nautobot-plugin-ssot Description-Content-Type: text/markdown # Nautobot Single
+Source of Truth (SSoT)
 [https://raw.githubusercontent.com/nautobot/nautobot-plugin-ssot/develop/docs/
                         images/icon-nautobot-ssot.png]
  [https://github.com/nautobot/nautobot-plugin-ssot//actions/workflows/ci.yml/
 badge.svg?branch=main] [https://readthedocs.org/projects/nautobot-plugin-ssot/
 badge/] [https://img.shields.io/pypi/v/nautobot-ssot] [https://img.shields.io/
                             pypi/dm/nautobot-ssot]
                              An App for Nautobot.
```

