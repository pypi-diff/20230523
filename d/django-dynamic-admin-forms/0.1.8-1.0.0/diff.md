# Comparing `tmp/django-dynamic-admin-forms-0.1.8.tar.gz` & `tmp/django-dynamic-admin-forms-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dynamic-admin-forms-0.1.8.tar", last modified: Tue Nov 30 10:20:48 2021, max compression
+gzip compressed data, was "django-dynamic-admin-forms-1.0.0.tar", last modified: Tue May 23 08:50:57 2023, max compression
```

## Comparing `django-dynamic-admin-forms-0.1.8.tar` & `django-dynamic-admin-forms-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,54 @@
--rw-r--r--   0        0        0      881 2021-09-27 15:10:55.346408 django-dynamic-admin-forms-0.1.8/.gitignore
--rw-r--r--   0        0        0     1850 2021-09-27 15:10:55.346408 django-dynamic-admin-forms-0.1.8/.gitlab-ci.yml
--rw-r--r--   0        0        0      512 2021-09-27 15:10:55.346408 django-dynamic-admin-forms-0.1.8/Dockerfile
--rw-r--r--   0        0        0     1099 2021-09-27 15:10:55.347408 django-dynamic-admin-forms-0.1.8/LICENSE
--rw-r--r--   0        0        0     5302 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/README.md
--rw-r--r--   0        0        0   946599 2021-09-27 15:10:55.356409 django-dynamic-admin-forms-0.1.8/docs/demo.gif
--rw-r--r--   0        0        0      101 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/__init__.py
--rw-r--r--   0        0        0     2112 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/admin.py
--rw-r--r--   0        0        0      112 2021-09-27 15:10:55.357409 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/apps.py
--rw-r--r--   0        0        0     2343 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/static/js/dynamic_admin.js
--rw-r--r--   0        0        0     1576 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/templates/admin/change_form.html
--rw-r--r--   0        0        0      206 2021-09-27 15:10:55.359412 django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/urls.py
--rw-r--r--   0        0        0      151 2021-09-27 15:10:55.360409 django-dynamic-admin-forms-0.1.8/e2e/cypress.json
--rw-r--r--   0        0        0     1190 2021-09-27 15:10:55.360409 django-dynamic-admin-forms-0.1.8/e2e/cypress/integration/dynamic-select.spec.js
--rw-r--r--   0        0        0      783 2021-09-27 15:10:55.361410 django-dynamic-admin-forms-0.1.8/e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0      863 2021-09-27 15:10:55.361410 django-dynamic-admin-forms-0.1.8/e2e/cypress/support/commands.js
--rw-r--r--   0        0        0      690 2021-09-27 15:10:55.362408 django-dynamic-admin-forms-0.1.8/e2e/cypress/support/index.js
--rw-r--r--   0        0        0      135 2021-09-27 15:10:55.362408 django-dynamic-admin-forms-0.1.8/e2e/cypress/support/paths.js
--rw-r--r--   0        0        0      278 2021-09-27 15:10:55.362408 django-dynamic-admin-forms-0.1.8/e2e/package.json
--rw-r--r--   0        0        0    49959 2021-09-27 15:10:55.363409 django-dynamic-admin-forms-0.1.8/e2e/yarn.lock
--rw-r--r--   0        0        0      903 2021-09-27 15:10:55.363409 django-dynamic-admin-forms-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-27 15:10:55.364408 django-dynamic-admin-forms-0.1.8/testproj/__init__.py
--rw-r--r--   0        0        0        0 2021-09-27 15:10:55.364408 django-dynamic-admin-forms-0.1.8/testproj/config/__init__.py
--rw-r--r--   0        0        0      409 2021-09-27 15:10:55.365407 django-dynamic-admin-forms-0.1.8/testproj/config/asgi.py
--rw-r--r--   0        0        0     2579 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/testproj/config/settings.py
--rw-r--r--   0        0        0      849 2021-09-27 15:10:55.365407 django-dynamic-admin-forms-0.1.8/testproj/config/urls.py
--rw-r--r--   0        0        0      409 2021-09-27 15:10:55.366408 django-dynamic-admin-forms-0.1.8/testproj/config/wsgi.py
--rw-r--r--   0        0        0     9275 2021-09-27 15:10:55.366408 django-dynamic-admin-forms-0.1.8/testproj/fixtures/fixtures-dev.json
--rw-r--r--   0        0        0      684 2021-09-27 15:10:55.367408 django-dynamic-admin-forms-0.1.8/testproj/manage.py
--rw-r--r--   0        0        0        0 2021-09-27 15:10:55.367408 django-dynamic-admin-forms-0.1.8/testproj/testapp/__init__.py
--rw-r--r--   0        0        0     2089 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/testproj/testapp/admin.py
--rw-r--r--   0        0        0      152 2021-09-27 15:10:55.368410 django-dynamic-admin-forms-0.1.8/testproj/testapp/apps.py
--rw-r--r--   0        0        0     3002 2021-09-27 15:10:55.368410 django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0      593 2021-10-15 08:29:18.253542 django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0002_extend_example.py
--rw-r--r--   0        0        0      594 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0003_example_file_field.py
--rw-r--r--   0        0        0        0 2021-09-27 15:10:55.369409 django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     1235 2021-11-30 10:18:58.670678 django-dynamic-admin-forms-0.1.8/testproj/testapp/models.py
--rw-r--r--   0        0        0      220 2021-09-27 15:10:55.369409 django-dynamic-admin-forms-0.1.8/tox.ini
--rw-r--r--   0        0        0     5961 1970-01-01 00:00:00.000000 django-dynamic-admin-forms-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6307 2023-05-23 08:48:07.314355 django-dynamic-admin-forms-1.0.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.0/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-23 08:48:07.315354 django-dynamic-admin-forms-1.0.0/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-23 08:48:07.316367 django-dynamic-admin-forms-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      889 2023-05-23 08:48:07.317358 django-dynamic-admin-forms-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1850 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        6 2023-05-23 08:48:07.318357 django-dynamic-admin-forms-1.0.0/.python-version
+-rw-r--r--   0        0        0      551 2023-05-23 08:48:07.319356 django-dynamic-admin-forms-1.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0      497 2023-05-23 08:48:07.320553 django-dynamic-admin-forms-1.0.0/CHANGES.md
+-rw-r--r--   0        0        0      512 2023-05-22 13:58:14.235674 django-dynamic-admin-forms-1.0.0/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0      145 2023-05-23 08:48:07.321356 django-dynamic-admin-forms-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     9894 2023-05-23 08:48:07.322359 django-dynamic-admin-forms-1.0.0/README.md
+-rw-r--r--   0        0        0      101 2023-05-23 08:48:07.323355 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-23 08:48:07.323355 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/admin.py
+-rw-r--r--   0        0        0      112 2023-05-23 08:48:07.324357 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/apps.py
+-rw-r--r--   0        0        0     2330 2023-05-23 08:48:07.325356 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/static/js/dynamic_admin.js
+-rw-r--r--   0        0        0     1638 2023-05-23 08:48:07.326356 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/templates/admin/change_form.html
+-rw-r--r--   0        0        0      168 2023-05-23 08:48:07.327356 django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/urls.py
+-rw-r--r--   0        0        0      654 2023-05-23 08:48:07.328355 django-dynamic-admin-forms-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2847 2023-05-23 08:48:07.328864 django-dynamic-admin-forms-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0   946599 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/docs/demo.gif
+-rw-r--r--   0        0        0       31 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0      112 2023-05-23 08:48:07.329876 django-dynamic-admin-forms-1.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-23 08:48:07.330876 django-dynamic-admin-forms-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0      151 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/cypress.json
+-rw-r--r--   0        0        0     1388 2023-05-23 08:48:07.331876 django-dynamic-admin-forms-1.0.0/e2e/cypress/integration/dynamic-select.spec.js
+-rw-r--r--   0        0        0      783 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0      863 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/cypress/support/commands.js
+-rw-r--r--   0        0        0      690 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      135 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/cypress/support/paths.js
+-rw-r--r--   0        0        0      278 2023-05-22 13:58:14.251301 django-dynamic-admin-forms-1.0.0/e2e/package.json
+-rw-r--r--   0        0        0    49959 2023-05-22 13:58:14.266926 django-dynamic-admin-forms-1.0.0/e2e/yarn.lock
+-rw-r--r--   0        0        0     9275 2023-05-23 08:48:07.332876 django-dynamic-admin-forms-1.0.0/fixtures/fixtures-dev.json
+-rw-r--r--   0        0        0      677 2023-05-23 08:48:07.333878 django-dynamic-admin-forms-1.0.0/manage.py
+-rw-r--r--   0        0        0     3715 2023-05-23 08:48:07.335878 django-dynamic-admin-forms-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-23 08:48:07.337426 django-dynamic-admin-forms-1.0.0/pytest.init
+-rw-r--r--   0        0        0     3706 2023-05-23 08:48:07.338499 django-dynamic-admin-forms-1.0.0/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-23 08:48:07.340480 django-dynamic-admin-forms-1.0.0/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-05-23 08:48:07.341477 django-dynamic-admin-forms-1.0.0/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     2579 2023-05-23 08:48:07.342529 django-dynamic-admin-forms-1.0.0/settings.py
+-rw-r--r--   0        0        0       69 2023-05-23 08:48:07.342529 django-dynamic-admin-forms-1.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-23 08:48:07.343558 django-dynamic-admin-forms-1.0.0/testapp/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-23 08:48:07.344555 django-dynamic-admin-forms-1.0.0/testapp/admin.py
+-rw-r--r--   0        0        0      152 2023-05-23 08:48:07.345558 django-dynamic-admin-forms-1.0.0/testapp/apps.py
+-rw-r--r--   0        0        0     3002 2023-05-23 08:48:07.347565 django-dynamic-admin-forms-1.0.0/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      593 2023-05-23 08:48:07.348555 django-dynamic-admin-forms-1.0.0/testapp/migrations/0002_extend_example.py
+-rw-r--r--   0        0        0      594 2023-05-23 08:48:07.350554 django-dynamic-admin-forms-1.0.0/testapp/migrations/0003_example_file_field.py
+-rw-r--r--   0        0        0        0 2023-05-23 08:48:07.351563 django-dynamic-admin-forms-1.0.0/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     1219 2023-05-23 08:48:07.352560 django-dynamic-admin-forms-1.0.0/testapp/models.py
+-rw-r--r--   0        0        0      220 2023-05-22 13:58:14.270434 django-dynamic-admin-forms-1.0.0/tox.ini
+-rw-r--r--   0        0        0      849 2023-05-23 08:48:07.353554 django-dynamic-admin-forms-1.0.0/urls.py
+-rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 django-dynamic-admin-forms-1.0.0/PKG-INFO
```

### Comparing `django-dynamic-admin-forms-0.1.8/.gitignore` & `django-dynamic-admin-forms-1.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -62,10 +62,11 @@
 */db.sqlite3
 
 # Cypress output
 */cypress/*
 
 # Build output
 dist
+_build
 
 # SCSS
 .sass-cache/
```

### Comparing `django-dynamic-admin-forms-0.1.8/.gitlab-ci.yml` & `django-dynamic-admin-forms-1.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/Dockerfile` & `django-dynamic-admin-forms-1.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/LICENSE` & `django-dynamic-admin-forms-1.0.0/LICENSE.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
+MIT License
 
-Copyright (c) 2021 Fabian Binz
+Copyright (c) 2012-2023 Ambient Innovation: GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `django-dynamic-admin-forms-0.1.8/docs/demo.gif` & `django-dynamic-admin-forms-1.0.0/docs/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/admin.py` & `django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,76 @@
-from itertools import filterfalse
 import json
+from itertools import filterfalse
 
-from django.core.exceptions import FieldDoesNotExist
 from django.apps import apps
 from django.contrib import admin
+from django.core.exceptions import FieldDoesNotExist, PermissionDenied
 from django.http import HttpResponse
 
 
 class DynamicModelAdminMixin:
     dynamic_fields = ()
     dynamic_select_fields = None
     dynamic_input_fields = None
 
     def get_form(self, request, obj=None, change=False, **kwargs):
         form = super().get_form(request, obj, **{"change": change, **kwargs})
-        self.dynamic_select_fields = list(
-            filter(self._is_related_field, self.dynamic_fields)
-        )
-        self.dynamic_input_fields = list(
-            filterfalse(self._is_related_field, self.dynamic_fields)
-        )
+        self.dynamic_select_fields = list(filter(self._is_related_field, self.dynamic_fields))
+        self.dynamic_input_fields = list(filterfalse(self._is_related_field, self.dynamic_fields))
         return form
 
     def _is_related_field(self, field_name):
         try:
             return self.opts.get_field(field_name).is_relation
         except FieldDoesNotExist:
             return False
 
     @staticmethod
-    def render_field(request, app_label, model_name, field_name):
+    def render_field(request) -> HttpResponse:
+        app_label = request.GET.get("app_label")
+        model_name = request.GET.get("model_name")
+        field_names = request.GET.getlist("field_names")
+
+        if not (app_label and model_name and field_names):
+            return HttpResponse(400, "Invalid argumnets")
+
         model = apps.get_model(app_label, model_name)
 
-        # instantiate model form from request data and get field
+        # instantiate model_admin form from request data and get field
         model_admin = admin.site._registry[model]
+
+        # check permissions
+        if not model_admin.has_module_permission(request):
+            raise PermissionDenied
+
         model_form = model_admin.get_form(request)
         bound_form = model_form(request.POST)
 
-        bound_field = bound_form[field_name]
+        snippets = []
+        for field_name in field_names:
+            bound_field = bound_form[field_name]
+
+            # save custom queryset in field
+            hidden = False
+            method_name = f"get_dynamic_{field_name}_field"
+            if hasattr(model_admin, method_name):
+                method = getattr(model_admin, method_name)
+                bound_form.full_clean()
+                queryset, value, hidden = method(bound_form.cleaned_data)
+
+                bound_field.field.queryset = queryset
+                bound_field.form.data = bound_field.form.data.copy()
+                bound_field.form.data[field_name] = value
+
+            skip_update = field_name in request.FILES and not hidden
+            html = bound_field.as_widget()
+
+            snippets.append(
+                {
+                    "field_name": field_name,
+                    "html": html,
+                    "hidden": hidden,
+                    "skipUpdate": skip_update,
+                }
+            )
 
-        # save custom queryset in field
-        hidden = False
-        method_name = f"get_dynamic_{field_name}_field"
-        if hasattr(model_admin, method_name):
-            method = getattr(model_admin, method_name)
-            bound_form.full_clean()
-            queryset, value, hidden = method(bound_form.cleaned_data)
-
-            bound_field.field.queryset = queryset
-            bound_field.form.data = bound_field.form.data.copy()
-            bound_field.form.data[field_name] = value
-
-        skip_update = field_name in request.FILES and not hidden
-        html = bound_field.as_widget()
-        return HttpResponse(
-            json.dumps({"html": html, "hidden": hidden, "skipUpdate": skip_update}),
-            status=200,
-        )
+        return HttpResponse(json.dumps(snippets), status=200)
```

### Comparing `django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/static/js/dynamic_admin.js` & `django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/static/js/dynamic_admin.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,11 @@
 var DynamicAdmin = {
     //# sourceURL="dynamic_admin.js"
     handleResponse: function(target, data) {
         var $ = django.jQuery;
-        data = JSON.parse(data);
 
         // set hidden class in parent form-row (or form-group if using jazzmin)
         if (data.hidden) {
             $(target.closest(".form-row,.form-group")).addClass("hidden");
         } else {
             $(target.closest(".form-row,.form-group")).removeClass("hidden");
         }
@@ -16,55 +15,61 @@
         if (data.skipUpdate) {
             return;
         }
 
         // Update the options for the select widget (either select2 instance or normal select element)
         if ($(target).find("select").hasClass("select2-hidden-accessible")) {
             var select2Widget = $(target).find("select");
-            var currentVal = select2Widget.val()
+            var currentVal = select2Widget.val();
             var options = $($.parseHTML(data.html)).find("option");
             select2Widget.find("option").remove();
             select2Widget.append(options);
             select2Widget.val(currentVal);
         } else {
             target.outerHTML = data.html;
         }
     },
 
-    dynamicSelect: function(app_label, model_name, field_name) {
+    dynamicWidgets: function(
+        app_label,
+        model_name,
+        select_field_names,
+        input_field_names
+    ) {
         var $ = django.jQuery;
         var that = this;
 
-        var $form = $('#' + model_name + '_form');
-        $form.on(('change'), function() {
-            $.post({
-                url: '/dynamic-admin-form/' + app_label + '/' + model_name + '/' + field_name + '/',
-                data: new FormData(this),
-                contentType: false,
-                processData: false,
-                success: function(data) {
-                    var target = $('.field-' + field_name + ' .related-widget-wrapper')[0];
-                    that.handleResponse(target, data);
-                }
-            });
-        });
-    },
-
-    dynamicInput: function(app_label, model_name, field_name) {
-        var $ = django.jQuery;
-        var that = this;
+        var $form = $("#" + model_name + "_form");
 
-        var $form = $('#' + model_name + '_form');
-        $form.on(('change'), function() {
+        $form.on("change", function() {
+            var field_names = [...select_field_names, ...input_field_names];
+            var params = new URLSearchParams([
+                ["app_label", app_label],
+                ["model_name", model_name],
+                ...field_names.map((name) => ["field_names", name]),
+            ]);
+            var url = `/dynamic-admin-form/?${params}`;
             $.post({
-                url: '/dynamic-admin-form/' + app_label + '/' + model_name + '/' + field_name + '/',
+                url,
                 data: new FormData(this),
                 contentType: false,
                 processData: false,
                 success: function(data) {
-                    var target = $('#id_' + field_name)[0];
-                    that.handleResponse(target, data);
-                }
+                    snippets = JSON.parse(data);
+                    snippets.forEach(({
+                        field_name,
+                        ...data
+                    }) => {
+                        if (select_field_names.indexOf(field_name) >= 0) {
+                            var target = $(
+                                ".field-" + field_name + " .related-widget-wrapper"
+                            )[0];
+                        } else {
+                            var target = $("#id_" + field_name)[0];
+                        }
+                        that.handleResponse(target, data);
+                    });
+                },
             });
         });
     },
-}
+};
```

### Comparing `django-dynamic-admin-forms-0.1.8/dynamic_admin_forms/templates/admin/change_form.html` & `django-dynamic-admin-forms-1.0.0/django_dynamic_admin_forms/templates/admin/change_form.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 {% extends "admin/change_form.html" %}
 {% load static %}
 
-{% block content %}
+{% block admin_change_form_document_ready %}
   {{ block.super }}
-  {% block admin_change_form_document_ready %}
-    {{ block.super }}
-    <script type="text/javascript" src="{% static 'js/dynamic_admin.js' %}"></script>
-    <script type="text/javascript">
-    {% for field_name in adminform.model_admin.dynamic_select_fields %}
-      DynamicAdmin.dynamicSelect("{{ opts.app_label }}", "{{ opts.model_name }}", "{{ field_name }}");
-    {% endfor %}
-    {% for field_name in adminform.model_admin.dynamic_input_fields %}
-      DynamicAdmin.dynamicInput("{{ opts.app_label }}", "{{ opts.model_name }}", "{{ field_name }}");
-    {% endfor %}
-    </script>
-  {% endblock %}
+  <script type="text/javascript" src="{% static 'js/dynamic_admin.js' %}"></script>
+
+  {{ adminform.model_admin.dynamic_select_fields|json_script:"dynamic_select_fields" }}
+  {{ adminform.model_admin.dynamic_input_fields|json_script:"dynamic_input_fields" }}
+
+  <script type="text/javascript">
+    var dynamic_select_fields = JSON.parse(document.getElementById('dynamic_select_fields').textContent);
+    var dynamic_input_fields = JSON.parse(document.getElementById('dynamic_input_fields').textContent);
+    DynamicAdmin.dynamicWidgets("{{ opts.app_label }}", "{{ opts.model_name }}", dynamic_select_fields, dynamic_input_fields);
+  </script>
 {% endblock %}
 
 {# Jazzmin-Support: the extrajs block is added in the jazzmin admin templates and won't do any harm for normal django admin#}
 {% block extrajs %}
   {{ block.super }}
   <script>
     // Find all select2 instances in the current change form and trigger the change event manually
```

### Comparing `django-dynamic-admin-forms-0.1.8/e2e/cypress/plugins/index.js` & `django-dynamic-admin-forms-1.0.0/e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/e2e/cypress/support/commands.js` & `django-dynamic-admin-forms-1.0.0/e2e/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/e2e/cypress/support/index.js` & `django-dynamic-admin-forms-1.0.0/e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/e2e/yarn.lock` & `django-dynamic-admin-forms-1.0.0/e2e/yarn.lock`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/config/settings.py` & `django-dynamic-admin-forms-1.0.0/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 SECRET_KEY = "7t!88vton98+=cb#=&4_5en37480c7+5qu9u=1@vfz#esaen0e"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
 ALLOWED_HOSTS = ["localhost"]
 
-ROOT_URLCONF = "config.urls"
+ROOT_URLCONF = "urls"
 
 INSTALLED_APPS = [
-    "dynamic_admin_forms",
+    "django_dynamic_admin_forms",
     # "jazzmin",
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
```

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/config/urls.py` & `django-dynamic-admin-forms-1.0.0/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,13 +10,13 @@
     1. Add an import:  from other_app.views import Home
     2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
 Including another URLconf
     1. Import the include() function: from django.urls import include, path
     2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
 """
 from django.contrib import admin
-from django.urls import path, include
+from django.urls import include, path
 
 urlpatterns = [
     path("admin/", admin.site.urls),
     path("dynamic-admin-form/", include("dynamic_admin_forms.urls")),
 ]
```

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/fixtures/fixtures-dev.json` & `django-dynamic-admin-forms-1.0.0/fixtures/fixtures-dev.json`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/manage.py` & `django-dynamic-admin-forms-1.0.0/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Django's command-line utility for administrative tasks."""
 import os
 import sys
 
 
 def main():
     """Run administrative tasks."""
-    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "config.settings")
+    os.environ.setdefault("DJANGO_SETTINGS_MODULE", "settings")
     try:
         from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
```

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/testapp/admin.py` & `django-dynamic-admin-forms-1.0.0/testapp/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from django.contrib import admin
 from django import forms
+from django.contrib import admin
+from django.contrib.admin.widgets import AdminTextInputWidget
+
+from django_dynamic_admin_forms.admin import DynamicModelAdminMixin
 
 from .models import Customer, District, Employee
-from dynamic_admin_forms.admin import DynamicModelAdminMixin
-from django.contrib.admin.widgets import AdminTextInputWidget
 
 
 @admin.register(District)
 class DistrictAdmin(admin.ModelAdmin):
     pass
 
 
@@ -16,17 +17,15 @@
     list_display = ("name", "district")
 
 
 class CustomerForm(forms.ModelForm):
     full_name = forms.CharField(
         max_length=100,
         required=False,
-        widget=AdminTextInputWidget(
-            attrs={"readonly": "true", "disabled": "true", "style": "border: none"}
-        ),
+        widget=AdminTextInputWidget(attrs={"readonly": "true", "disabled": "true", "style": "border: none"}),
     )
 
     class Meta:
         model = Customer
         fields = ()
```

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0001_initial.py` & `django-dynamic-admin-forms-1.0.0/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0002_extend_example.py` & `django-dynamic-admin-forms-1.0.0/testapp/migrations/0002_extend_example.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/testapp/migrations/0003_example_file_field.py` & `django-dynamic-admin-forms-1.0.0/testapp/migrations/0003_example_file_field.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-admin-forms-0.1.8/testproj/testapp/models.py` & `django-dynamic-admin-forms-1.0.0/testapp/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         OTHER = 5, "Other"
 
     first_name = models.CharField(max_length=255)
     last_name = models.CharField(max_length=255)
     district = models.ForeignKey(District, on_delete=models.CASCADE)
     employee = models.ForeignKey(Employee, on_delete=models.CASCADE)
 
-    lead_reason = models.PositiveSmallIntegerField(
-        choices=LeadReason.choices, default=LeadReason.INTERNET
-    )
+    lead_reason = models.PositiveSmallIntegerField(choices=LeadReason.choices, default=LeadReason.INTERNET)
     lead_reason_other = models.CharField(max_length=50, blank=True)
 
     has_profile_picture = models.BooleanField(default=False)
     profile_picture = models.FileField(blank=True)
 
     def __str__(self):
         return self.first_name + " " + self.last_name
```

