# Comparing `tmp/django-dashboards-0.1.2.tar.gz` & `tmp/django-dashboards-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dashboards-0.1.2.tar", last modified: Mon May 22 08:17:33 2023, max compression
+gzip compressed data, was "django-dashboards-0.1.3.tar", last modified: Tue May 23 11:55:44 2023, max compression
```

## Comparing `django-dashboards-0.1.2.tar` & `django-dashboards-0.1.3.tar`

### file list

```diff
@@ -1,224 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 08:17:33.613286 django-dashboards-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.569285 django-dashboards-0.1.2/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.569285 django-dashboards-0.1.2/dashboards/component/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/component/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/component/table/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/menus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.553284 django-dashboards-0.1.2/dashboards/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/static/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/dashboards.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/dashboards.css
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/grid.css
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/layout.css
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/menu.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/datatables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.577285 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/alpine.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/datatables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/form/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/form/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/loading.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/html.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/stat.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/text.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/dashboard_partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.561284 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/js.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/style.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.561284 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/card.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/container.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/tab.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templatetags/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/django_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/dashboards/howto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.601286 django-dashboards-0.1.2/docs/dashboards/howto/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/async_component.gif
--rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_add_form.png
--rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_chart_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_gauge.png
--rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_map_examples.png
--rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_table.png
--rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/dependent_table_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_basic.png
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_complex.png
--rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_chart.png
--rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_layout.png
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_component_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_loading.png
--rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_style.png
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/async.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/docs/dashboards/howto/components/
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/included.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/dashboards.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/dynamic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/menus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/docs/dashboards/howto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/chart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/table.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/sse.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/docs_dj_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-22 08:17:33.613286 django-dashboards-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/app1/dashboards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/components/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_model_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/menu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/test_menutags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/views/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_form_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_form_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/meta/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/chart/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/component/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/component/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.937655 django-dashboards-0.1.3/dashboards/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/menus/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.929654 django-dashboards-0.1.3/dashboards/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/static/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    14519 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/dashboards.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/buttons.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/cards.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/dashboards.css
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/forms.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/layout.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/menu.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/css/src/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/js/dashboard.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/datatables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.941655 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/alpine.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/datatables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.945654 django-dashboards-0.1.3/dashboards/templates/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/form/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/loading.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/stat.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/dashboard_partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/includes/static/style.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.933654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/tabs/tab.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/dashboards/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/templatetags/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/dashboards/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.949654 django-dashboards-0.1.3/django_dashboards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-23 11:55:44.000000 django-dashboards-0.1.3/django_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.953654 django-dashboards-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.953654 django-dashboards-0.1.3/docs/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.957655 django-dashboards-0.1.3/docs/dashboards/howto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/async_component.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_add_form.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_chart_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_gauge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_map_examples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/components_table.png
+-rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/dependent_table_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_chart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_layout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_component_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_loading.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_style.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/async.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/included.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/dashboards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/dynamic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/menus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/docs/dashboards/howto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/chart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/serializers/table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/sse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/howto/views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/dashboards/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/docs_dj_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/app1/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.969654 django-dashboards-0.1.3/tests/dashboards/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/components/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/components/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_model_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/dashboard/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/menu/test_menutags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.973654 django-dashboards-0.1.3/tests/dashboards/views/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_form_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/dashboards/views/test_form_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:44.977655 django-dashboards-0.1.3/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/meta/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 11:55:36.000000 django-dashboards-0.1.3/tests/utils.py
```

### Comparing `django-dashboards-0.1.2/LICENSE` & `django-dashboards-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/PKG-INFO` & `django-dashboards-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dashboards-0.1.2/README.rst` & `django-dashboards-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/base.py` & `django-dashboards-0.1.3/dashboards/component/base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/chart/chart.py` & `django-dashboards-0.1.3/dashboards/component/chart/chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/chart/serializers.py` & `django-dashboards-0.1.3/dashboards/component/chart/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/form.py` & `django-dashboards-0.1.3/dashboards/component/form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/layout.py` & `django-dashboards-0.1.3/dashboards/component/layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/map.py` & `django-dashboards-0.1.3/dashboards/component/map.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/table/mixins.py` & `django-dashboards-0.1.3/dashboards/component/table/mixins.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/table/serializers.py` & `django-dashboards-0.1.3/dashboards/component/table/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/table/table.py` & `django-dashboards-0.1.3/dashboards/component/table/table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/component/text.py` & `django-dashboards-0.1.3/dashboards/component/text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/config.py` & `django-dashboards-0.1.3/dashboards/config.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/dashboard.py` & `django-dashboards-0.1.3/dashboards/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/forms.py` & `django-dashboards-0.1.3/dashboards/forms.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/menus/menu.py` & `django-dashboards-0.1.3/dashboards/menus/menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/meta/__init__.py` & `django-dashboards-0.1.3/dashboards/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/permissions.py` & `django-dashboards-0.1.3/dashboards/permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/registry.py` & `django-dashboards-0.1.3/dashboards/registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/css/src/layout.css` & `django-dashboards-0.1.3/dashboards/static/dashboards/css/src/layout.css`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-:root {
-  --dark-one: #343434;
-  --dark-two: #393939;
-  --dark-three: #b2b2b2;
-  --grey: #ececec;
-  --white: #fff;
-  --primary: rgba(82, 198, 53, 0.82);
-}
-
 * {
   -webkit-box-sizing: border-box;
   box-sizing: border-box;
   text-rendering: optimizeLegibility;
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
   font-kerning: auto;
 }
 
 html {
   font-size: 1.2em;
   line-height: 1.4;
   font-weight: 400;
-  font-family: 'Helvetica Neue', serif;
-  background-color: var(--dark-one);
-  color: var(--white);
+  font-family: Inter var,ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;
 }
 
 body {
   padding: 1em;
   margin: 0 auto;
   max-width: 95%;
+  min-height: 100vh;
+  background: var(--root-background);
+  color: var(--color-text-primary);
 }
 
 a{
-  color: var(--primary);
+  color: var(--color-text-primary);
   cursor: pointer;
   font-size: 1.1rem;
   text-decoration: none;
 }
 
 
 h1, h2, h3, h4, h5, h6 {
   margin: 0 0 .5em 0;
   line-height: 1.2;
   letter-spacing: -.02em;
 }
 
 hr{
-  border-color: var(--primary);
+  border-color: var(--color-text-primary);
 }
```

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/datatables.min.css` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/alpine.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/datatables.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.sse.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/htmx.sse.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/jquery.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/plotly.min.js` & `django-dashboards-0.1.3/dashboards/static/dashboards/vendor/js/plotly.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/base.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/base.html`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     <head>
         <title>Django Dashboards | {% block title %}{{ dashboard.get_meta.name }}{% endblock title %}</title>
         <meta charset="utf-8">
         <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
         {% block dashboards_js %}{% endblock dashboards_js %}
         {% block dashboards_style %}{% endblock dashboards_style %}
     </head>
-    <body hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}'>
+    <body hx-headers='{"X-CSRFToken": "{{ csrf_token }}"}' class="{{ request.COOKIES.appearanceMode }}">
         {% block body %}
             {% block content_title %}{% endblock content_title %}
             <div class="content">
                 {% block content %}{% endblock content %}
             </div>
         {% endblock body %}
     </body>
```

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/chart.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/chart/chart.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/component.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/component.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/map.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/map/map.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/basic.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/basic.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/index.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/table/index.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/stat.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/components/text/stat.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/card.html` & `django-dashboards-0.1.3/dashboards/templates/dashboards/layout/components/card.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/templatetags/dashboards.py` & `django-dashboards-0.1.3/dashboards/templatetags/dashboards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random
 from typing import Dict, List, Type, Union, cast
 
 from django import template
 from django.template import RequestContext
+from django.utils.translation import gettext as _
 
 from dashboards.component import Component
 from dashboards.dashboard import Dashboard
 from dashboards.menus.menu import DashboardMenuItem, Menu, MenuItem
 from dashboards.menus.registry import menu_registry
 from dashboards.registry import registry
 
@@ -88,7 +89,46 @@
                     # only do the first one found
                     if active_section is None and menu_item.selected or menu_item.open:
                         active_section = menu.name
 
         context["sections"] = sections
         context["active_section"] = active_section
         return ""
+
+
+@register.filter()
+def get_form_context(form):
+    """
+    In the form template we use `form.get_context`, this doesnt exist in dj 3.2.
+    This filter provides similar functionality when `get_context` is missing.
+
+    This will be removed when the oldest supported version supports
+    `form.get_context`
+    """
+    if hasattr(form, "get_context"):
+        return form.get_context()
+
+    # patch to account for Form.get_context not existing in dj 3.2
+    fields = []
+    hidden_fields = []
+    top_errors = form.non_field_errors().copy()
+
+    bound_items = [(name, form[name]) for name in form.fields]
+    for name, bf in bound_items:
+        bf_errors = form.error_class(bf.errors)
+        if bf.is_hidden:
+            if bf_errors:
+                top_errors += [
+                    _("(Hidden field %(name)s) %(error)s")
+                    % {"name": name, "error": str(e)}
+                    for e in bf_errors
+                ]
+            hidden_fields.append(bf)
+        else:
+            errors_str = str(bf_errors)
+            fields.append((bf, errors_str))
+    return {
+        "form": form,
+        "fields": fields,
+        "hidden_fields": hidden_fields,
+        "errors": top_errors,
+    }
```

### Comparing `django-dashboards-0.1.2/dashboards/urls.py` & `django-dashboards-0.1.3/dashboards/urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/dashboards/views.py` & `django-dashboards-0.1.3/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/django_dashboards.egg-info/PKG-INFO` & `django-dashboards-0.1.3/django_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django-dashboards-0.1.2/django_dashboards.egg-info/SOURCES.txt` & `django-dashboards-0.1.3/django_dashboards.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,24 @@
 dashboards/component/table/serializers.py
 dashboards/component/table/table.py
 dashboards/menus/__init__.py
 dashboards/menus/menu.py
 dashboards/menus/registry.py
 dashboards/meta/__init__.py
 dashboards/static/dashboards/css/dashboards.css
+dashboards/static/dashboards/css/src/buttons.css
+dashboards/static/dashboards/css/src/cards.css
 dashboards/static/dashboards/css/src/dashboards.css
+dashboards/static/dashboards/css/src/forms.css
 dashboards/static/dashboards/css/src/grid.css
 dashboards/static/dashboards/css/src/index.css
 dashboards/static/dashboards/css/src/layout.css
 dashboards/static/dashboards/css/src/menu.css
+dashboards/static/dashboards/css/src/theme.css
+dashboards/static/dashboards/js/dashboard.js
 dashboards/static/dashboards/vendor/css/datatables.min.css
 dashboards/static/dashboards/vendor/js/alpine.min.js
 dashboards/static/dashboards/vendor/js/datatables.min.js
 dashboards/static/dashboards/vendor/js/htmx.min.js
 dashboards/static/dashboards/vendor/js/htmx.sse.min.js
 dashboards/static/dashboards/vendor/js/jquery.min.js
 dashboards/static/dashboards/vendor/js/plotly.min.js
```

### Comparing `django-dashboards-0.1.2/docs/Makefile` & `django-dashboards-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/conf.py` & `django-dashboards-0.1.3/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "django-dashboards"
 copyright = "2023, Wildfish"
 author = "Wildfish"
-release = "0.1.2"
+release = "0.1.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
```

### Comparing `django-dashboards-0.1.2/docs/contributing.rst` & `django-dashboards-0.1.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/async_component.gif` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/async_component.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_add_form.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_add_form.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_chart_example.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_chart_example.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_gauge.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_gauge.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_map_examples.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_map_examples.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_table.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/components_table.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/demo.gif` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/dependent_table_dashboard.gif` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/dependent_table_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_basic.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_basic.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_complex.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/layout_complex.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.gif` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/quickstart_dashboard.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_chart.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_chart.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_layout.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/serializers_layout.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_component_template.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_component_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_loading.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_loading.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_template.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_custom_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_style.png` & `django-dashboards-0.1.3/docs/dashboards/howto/_images/templates_style.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/async.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/async.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/components/attributes.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/components/attributes.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/components/custom.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/components/custom.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/components/included.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/components/included.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/components/index.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/components/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/dashboards.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/dashboards.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/demo.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/demo.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/dynamic.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/dynamic.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/layout.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/layout.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/menus.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/menus.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/permissions.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/quickstart.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/serializers/chart.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/serializers/chart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/serializers/table.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/serializers/table.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/settings.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/settings.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/sse.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/sse.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/templates.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/templates.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/howto/views.rst` & `django-dashboards-0.1.3/docs/dashboards/howto/views.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/dashboards/index.rst` & `django-dashboards-0.1.3/docs/dashboards/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/docs_dj_settings.py` & `django-dashboards-0.1.3/docs/docs_dj_settings.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/index.rst` & `django-dashboards-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/make.bat` & `django-dashboards-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/docs/requirements.txt` & `django-dashboards-0.1.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/setup.cfg` & `django-dashboards-0.1.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dashboards
-version = 0.1.2
+version = 0.1.3
 description = Tools for building data dashboards with Django
 long_description = file: README.rst
 url = https://github.com/wildfish/django-dashboards
 author = Wildfish
 author_email = developers@wildfish.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-dashboards-0.1.2/tests/conftest.py` & `django-dashboards-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/app1/dashboards.py` & `django-dashboards-0.1.3/tests/dashboards/app1/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_base.py` & `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_chart.py` & `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_form.py` & `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,32 @@
     "test_form_component__renders_value[False] 1"
 ] = """
 
 
 
     
         <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
-            <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+            
+<form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><td><label for="id_number">Number:</label><br></td><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+  }
         </div>
     
 
 
 """
 
 snapshots[
     "test_form_component__renders_value[True] 1"
 ] = """
 
 
 
     
         <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
-            <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+            
+<form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><td><label for="id_number">Number:</label><br></td><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+  }
         </div>
     
 
 
 """
```

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_table.py` & `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_text.py` & `django-dashboards-0.1.3/tests/dashboards/components/snapshots/snap_test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/test_base.py` & `django-dashboards-0.1.3/tests/dashboards/components/test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/test_chart.py` & `django-dashboards-0.1.3/tests/dashboards/components/test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/test_form.py` & `django-dashboards-0.1.3/tests/dashboards/components/test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/test_table.py` & `django-dashboards-0.1.3/tests/dashboards/components/test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/components/test_text.py` & `django-dashboards-0.1.3/tests/dashboards/components/test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_form.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_layout.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/test_dashboard.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/test_layout.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/test_model_dashboard.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/test_model_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/dashboard/test_permissions.py` & `django-dashboards-0.1.3/tests/dashboards/dashboard/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/fixtures.py` & `django-dashboards-0.1.3/tests/dashboards/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/menu/test_menu.py` & `django-dashboards-0.1.3/tests/dashboards/menu/test_menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/menu/test_menutags.py` & `django-dashboards-0.1.3/tests/dashboards/menu/test_menutags.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard_form.py` & `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_dashboard_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_layout.py` & `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_schema.py` & `django-dashboards-0.1.3/tests/dashboards/snapshots/snap_test_schema.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/test_registry.py` & `django-dashboards-0.1.3/tests/dashboards/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/test_urls.py` & `django-dashboards-0.1.3/tests/dashboards/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_component.py` & `django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_dashboard.py` & `django-dashboards-0.1.3/tests/dashboards/views/snapshots/snap_test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/views/test_component.py` & `django-dashboards-0.1.3/tests/dashboards/views/test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/views/test_dashboard.py` & `django-dashboards-0.1.3/tests/dashboards/views/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/dashboards/views/test_form_component.py` & `django-dashboards-0.1.3/tests/dashboards/views/test_form_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/meta/test_meta.py` & `django-dashboards-0.1.3/tests/meta/test_meta.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.2/tests/settings.py` & `django-dashboards-0.1.3/tests/settings.py`

 * *Files identical despite different names*

