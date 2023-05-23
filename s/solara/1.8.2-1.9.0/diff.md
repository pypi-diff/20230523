# Comparing `tmp/solara-1.8.2.tar.gz` & `tmp/solara-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solara-1.8.2.tar", last modified: Thu Mar 16 11:21:28 2023, max compression
+gzip compressed data, was "solara-1.9.0.tar", last modified: Thu Mar 30 16:57:10 2023, max compression
```

## Comparing `solara-1.8.2.tar` & `solara-1.9.0.tar`

### file list

```diff
@@ -1,430 +1,435 @@
--rw-r--r--   0        0        0      681 2023-03-16 11:18:45.533979 solara-1.8.2/.bumpversion.cfg
--rw-r--r--   0        0        0      136 2023-03-16 11:18:45.533979 solara-1.8.2/.flake8
--rw-r--r--   0        0        0      780 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/codequality.yaml
--rw-r--r--   0        0        0     1769 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/installation.yml
--rw-r--r--   0        0        0     1614 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/integration.yml
--rw-r--r--   0        0        0      898 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/javascript.yaml
--rw-r--r--   0        0        0     1588 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0      998 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/release_solara_vuetify_app.yaml
--rw-r--r--   0        0        0      976 2023-03-16 11:18:45.533979 solara-1.8.2/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      917 2023-03-16 11:18:45.533979 solara-1.8.2/.gitignore
--rw-r--r--   0        0        0      971 2023-03-16 11:18:45.533979 solara-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1086 2023-03-16 11:18:45.533979 solara-1.8.2/LICENSE
--rw-r--r--   0        0        0      614 2023-03-16 11:18:45.533979 solara-1.8.2/Procfile
--rw-r--r--   0        0        0     1213 2023-03-16 11:18:45.533979 solara-1.8.2/README.md
--rw-r--r--   0        0        0      115 2023-03-16 11:18:45.533979 solara-1.8.2/mypy.ini
--rw-r--r--   0        0        0       85 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/.gitignore
--rw-r--r--   0        0        0     1086 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/LICENSE
--rw-r--r--   0        0        0      501 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/RELEASE.md
--rw-r--r--   0        0        0      451 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/download_cdn_test.py
--rw-r--r--   0        0        0     2119 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/hatch_build.py
--rw-r--r--   0        0        0      672 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/pyproject.toml
--rw-r--r--   0        0        0       46 2023-03-16 11:18:45.533979 solara-1.8.2/packages/assets/solara_assets/__init__.py
--rw-r--r--   0        0        0       59 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/LICENSE
--rw-r--r--   0        0        0      247 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/RELEASE.md
--rw-r--r--   0        0        0      725 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/pyproject.toml
--rw-r--r--   0        0        0       55 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/__init__.py
--rw-r--r--   0        0        0       47 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/__init__.py
--rw-r--r--   0        0        0     1941 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/base.py
--rw-r--r--   0        0        0     1190 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/disk.py
--rw-r--r--   0        0        0      816 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/memory_size.py
--rw-r--r--   0        0        0      710 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/multi_level.py
--rw-r--r--   0        0        0      779 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/redis.py
--rw-r--r--   0        0        0      411 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/license.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/__init__.py
--rw-r--r--   0        0        0     3307 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/index.py
--rw-r--r--   0        0        0      467 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/search.py
--rw-r--r--   0        0        0     6127 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/search.vue
--rw-r--r--   0        0        0     7118 2023-03-16 11:18:45.533979 solara-1.8.2/packages/solara-enterprise/solara_enterprise/ssg.py
--rw-r--r--   0        0        0   427583 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-milkdown/package-lock.json
--rw-r--r--   0        0        0      915 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-milkdown/package.json
--rw-r--r--   0        0        0      461 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-milkdown/src/index.js
--rw-r--r--   0        0        0     1025 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-milkdown/webpack.config.js
--rw-r--r--   0        0        0      422 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/.bumpversion.cfg
--rw-r--r--   0        0        0      239 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/README.md
--rw-r--r--   0        0        0   126731 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/package-lock.json
--rw-r--r--   0        0        0     1076 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/package.json
--rwxr-xr-x   0        0        0      289 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/release.sh
--rw-r--r--   0        0        0      436 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/src/solara-vuetify-app.js
--rw-r--r--   0        0        0      142 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/src/solara.js
--rwxr-xr-x   0        0        0     1204 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-vuetify-app/webpack.config.js
--rw-r--r--   0        0        0     1538 2023-03-16 11:18:45.537979 solara-1.8.2/packages/solara-widget-manager/LICENSE.voila.txt
--rw-r--r--   0        0        0   717713 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/package-lock.json
--rw-r--r--   0        0        0     1913 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/package.json
--rw-r--r--   0        0        0      934 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/index.ts
--rw-r--r--   0        0        0     1452 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/kernel.ts
--rw-r--r--   0        0        0     3290 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/loader.ts
--rw-r--r--   0        0        0     8500 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/manager.ts
--rw-r--r--   0        0        0     1319 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/mathjax.ts
--rw-r--r--   0        0        0     1236 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/rendermime.ts
--rw-r--r--   0        0        0      127 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/src/typings.d.ts
--rw-r--r--   0        0        0     3446 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/style/index.css
--rw-r--r--   0        0        0      135 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/tsconfig.json
--rw-r--r--   0        0        0     1205 2023-03-16 11:18:45.541979 solara-1.8.2/packages/solara-widget-manager/webpack.config.js
--rw-r--r--   0        0        0      115 2023-03-16 11:18:45.541979 solara-1.8.2/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
--rw-r--r--   0        0        0      113 2023-03-16 11:18:45.541979 solara-1.8.2/prefix/etc/jupyter/jupyter_server_config.d/solara.json
--rw-r--r--   0        0        0     2138 2023-03-16 11:18:45.541979 solara-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      462 2023-03-16 11:18:45.541979 solara-1.8.2/release.md
--rwxr-xr-x   0        0        0      232 2023-03-16 11:18:45.541979 solara-1.8.2/release.sh
--rw-r--r--   0        0        0      123 2023-03-16 11:18:45.541979 solara-1.8.2/requirements.txt
--rw-r--r--   0        0        0       14 2023-03-16 11:18:45.541979 solara-1.8.2/runtime.txt
--rw-r--r--   0        0        0     3091 2023-03-16 11:18:45.541979 solara-1.8.2/solara/__init__.py
--rw-r--r--   0        0        0    21260 2023-03-16 11:18:45.541979 solara-1.8.2/solara/__main__.py
--rw-r--r--   0        0        0      216 2023-03-16 11:18:45.541979 solara-1.8.2/solara/alias.py
--rw-r--r--   0        0        0    17763 2023-03-16 11:18:45.541979 solara-1.8.2/solara/autorouting.py
--rw-r--r--   0        0        0    10743 2023-03-16 11:18:45.541979 solara-1.8.2/solara/cache.py
--rw-r--r--   0        0        0     3254 2023-03-16 11:18:45.541979 solara-1.8.2/solara/checks.html
--rw-r--r--   0        0        0     4283 2023-03-16 11:18:45.541979 solara-1.8.2/solara/checks.py
--rw-r--r--   0        0        0     2337 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/__init__.py
--rw-r--r--   0        0        0     4639 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/alert.py
--rw-r--r--   0        0        0    12992 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/applayout.py
--rw-r--r--   0        0        0     1791 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/button.py
--rw-r--r--   0        0        0      890 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/checkbox.py
--rw-r--r--   0        0        0      235 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/code_highlight_css.py
--rw-r--r--   0        0        0     5776 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/code_highlight_css.vue
--rw-r--r--   0        0        0     4698 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/columns.py
--rw-r--r--   0        0        0    13473 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/cross_filter.py
--rw-r--r--   0        0        0    21030 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/dataframe.py
--rw-r--r--   0        0        0     7869 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/datatable.py
--rw-r--r--   0        0        0     7061 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/datatable.vue
--rw-r--r--   0        0        0      675 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/details.py
--rw-r--r--   0        0        0     1069 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/download.vue
--rw-r--r--   0        0        0     2589 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/echarts.py
--rw-r--r--   0        0        0     3695 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/echarts.vue
--rw-r--r--   0        0        0      962 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/figure_altair.py
--rw-r--r--   0        0        0     6960 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/file_browser.py
--rw-r--r--   0        0        0     6900 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/file_download.py
--rw-r--r--   0        0        0     3165 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/file_drop.py
--rw-r--r--   0        0        0     1870 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/file_drop.vue
--rw-r--r--   0        0        0     1860 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/file_list_widget.vue
--rw-r--r--   0        0        0      623 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/head.py
--rw-r--r--   0        0        0     1566 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/head_tag.py
--rw-r--r--   0        0        0     1658 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/head_tag.vue
--rw-r--r--   0        0        0     1910 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/image.py
--rw-r--r--   0        0        0     3284 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/input.py
--rw-r--r--   0        0        0     1390 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/link.py
--rw-r--r--   0        0        0     6895 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/markdown.py
--rw-r--r--   0        0        0      634 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/markdown_editor.py
--rw-r--r--   0        0        0     8864 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/markdown_editor.vue
--rw-r--r--   0        0        0     1952 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/matplotlib.py
--rw-r--r--   0        0        0     1629 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/meta.py
--rw-r--r--   0        0        0    10039 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/misc.py
--rw-r--r--   0        0        0     9871 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/pivot_table.py
--rw-r--r--   0        0        0     4674 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/pivot_table.vue
--rw-r--r--   0        0        0     1668 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/select.py
--rw-r--r--   0        0        0      950 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/select.vue
--rw-r--r--   0        0        0     7939 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/slider.py
--rw-r--r--   0        0        0     1351 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/slider_date.vue
--rw-r--r--   0        0        0     1189 2023-03-16 11:18:45.541979 solara-1.8.2/solara/components/sql_code.py
--rw-r--r--   0        0        0     3937 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/sql_code.vue
--rw-r--r--   0        0        0      883 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/style.py
--rw-r--r--   0        0        0     1047 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/tab_navigation.py
--rw-r--r--   0        0        0     2159 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/title.py
--rw-r--r--   0        0        0      901 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/title.vue
--rw-r--r--   0        0        0     2630 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/togglebuttons.py
--rw-r--r--   0        0        0     1636 2023-03-16 11:18:45.545980 solara-1.8.2/solara/components/tooltip.py
--rw-r--r--   0        0        0     4150 2023-03-16 11:18:45.545980 solara-1.8.2/solara/datatypes.py
--rw-r--r--   0        0        0     6781 2023-03-16 11:18:45.545980 solara-1.8.2/solara/express.py
--rw-r--r--   0        0        0       85 2023-03-16 11:18:45.545980 solara-1.8.2/solara/hooks/__init__.py
--rw-r--r--   0        0        0     3180 2023-03-16 11:18:45.545980 solara-1.8.2/solara/hooks/dataframe.py
--rw-r--r--   0        0        0    13555 2023-03-16 11:18:45.545980 solara-1.8.2/solara/hooks/misc.py
--rw-r--r--   0        0        0      249 2023-03-16 11:18:45.545980 solara-1.8.2/solara/kitchensink.py
--rw-r--r--   0        0        0      740 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/components/__init__.py
--rw-r--r--   0        0        0      186 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/components/cross_filter.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/hooks/__init__.py
--rw-r--r--   0        0        0      268 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/hooks/dataframe.py
--rw-r--r--   0        0        0    10814 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/toestand.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/utils/__init__.py
--rw-r--r--   0        0        0     3044 2023-03-16 11:18:45.545980 solara-1.8.2/solara/lab/utils/dataframe.py
--rw-r--r--   0        0        0     1782 2023-03-16 11:18:45.545980 solara-1.8.2/solara/layout.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.545980 solara-1.8.2/solara/py.typed
--rw-r--r--   0        0        0     6109 2023-03-16 11:18:45.545980 solara-1.8.2/solara/routing.py
--rw-r--r--   0        0        0     1137 2023-03-16 11:18:45.545980 solara-1.8.2/solara/scope/__init__.py
--rw-r--r--   0        0        0     1540 2023-03-16 11:18:45.545980 solara-1.8.2/solara/scope/types.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/__init__.py
--rw-r--r--   0        0        0    23086 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/app.py
--rw-r--r--   0        0        0       15 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/custom.css
--rw-r--r--   0        0        0       16 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/custom.js
--rw-r--r--   0        0        0     1924 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/favicon.png
--rw-r--r--   0        0        0     1240 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/favicon.svg
--rw-r--r--   0        0        0     1810 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/style.css
--rw-r--r--   0        0        0       21 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/assets/theme.js
--rw-r--r--   0        0        0     2152 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/cdn_helper.py
--rw-r--r--   0        0        0       93 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/fastapi.py
--rw-r--r--   0        0        0     5549 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/flask.py
--rw-r--r--   0        0        0      137 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/jupyter/__init__.py
--rw-r--r--   0        0        0      835 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/jupyter/cdn_handler.py
--rw-r--r--   0        0        0      680 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/jupyter/server_extension.py
--rw-r--r--   0        0        0     9005 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/kernel.py
--rw-r--r--   0        0        0     8063 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/patch.py
--rw-r--r--   0        0        0      916 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/pyodide.py
--rw-r--r--   0        0        0     8189 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/reload.py
--rw-r--r--   0        0        0    10339 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/server.py
--rw-r--r--   0        0        0     2744 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/settings.py
--rw-r--r--   0        0        0    12114 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/starlette.py
--rw-r--r--   0        0        0     7797 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/ansi.js
--rw-r--r--   0        0        0     6809 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/highlight-dark.css
--rw-r--r--   0        0        0     2637 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/highlight.css
--rw-r--r--   0        0        0     7981 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/main-vuetify.js
--rw-r--r--   0        0        0     5679 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/main.js
--rw-r--r--   0        0        0     3194 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/solara_bootstrap.py
--rw-r--r--   0        0        0     6855 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/sun.svg
--rw-r--r--   0        0        0     1372 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/static/webworker.js
--rw-r--r--   0        0        0     3415 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/telemetry.py
--rw-r--r--   0        0        0       31 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/index.html.j2
--rw-r--r--   0        0        0      205 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/loader-plain.css
--rw-r--r--   0        0        0      678 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/loader-plain.html
--rw-r--r--   0        0        0     1900 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/loader-solara.css
--rw-r--r--   0        0        0     2730 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/loader-solara.html
--rw-r--r--   0        0        0     2762 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/plain.html
--rw-r--r--   0        0        0    17042 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/templates/solara.html.j2
--rw-r--r--   0        0        0     2088 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/threaded.py
--rw-r--r--   0        0        0      935 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/utils.py
--rw-r--r--   0        0        0     1057 2023-03-16 11:18:45.545980 solara-1.8.2/solara/server/websocket.py
--rw-r--r--   0        0        0     1120 2023-03-16 11:18:45.545980 solara-1.8.2/solara/settings.py
--rw-r--r--   0        0        0      325 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/button.py
--rw-r--r--   0        0        0     1137 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/markdown.py
--rw-r--r--   0        0        0      136 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/.flake8
--rw-r--r--   0        0        0      791 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1066 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/LICENSE
--rw-r--r--   0        0        0      407 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/Procfile
--rw-r--r--   0        0        0       63 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/mypy.ini
--rw-r--r--   0        0        0      450 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/pyproject.toml
--rw-r--r--   0        0        0       99 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/__init__.py
--rw-r--r--   0        0        0       70 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/components/__init__.py
--rw-r--r--   0        0        0      854 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/components/article.py
--rw-r--r--   0        0        0      828 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/components/data.py
--rw-r--r--   0        0        0       57 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/components/header.py
--rw-r--r--   0        0        0      101 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/components/layout.py
--rw-r--r--   0        0        0     3619 2023-03-16 11:18:45.545980 solara-1.8.2/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
--rw-r--r--   0        0        0     3092 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
--rw-r--r--   0        0        0     1911 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/data.py
--rw-r--r--   0        0        0     2565 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/pages/__init__.py
--rw-r--r--   0        0        0      814 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/pages/article/__init__.py
--rw-r--r--   0        0        0      938 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/pages/tabular.py
--rw-r--r--   0        0        0     2857 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/pages/viz/__init__.py
--rw-r--r--   0        0        0      365 2023-03-16 11:18:45.549980 solara-1.8.2/solara/template/portal/solara_portal/pages/viz/overview.py
--rw-r--r--   0        0        0     3834 2023-03-16 11:18:45.549980 solara-1.8.2/solara/util.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/__init__.py
--rw-r--r--   0        0        0     4523 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/assets/custom.css
--rw-r--r--   0        0        0    86383 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/assets/images/logo-small.png
--rw-r--r--   0        0        0     4858 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/assets/images/logo.svg
--rw-r--r--   0        0        0       67 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/assets/theme.js
--rw-r--r--   0        0        0       80 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/components/__init__.py
--rw-r--r--   0        0        0     1940 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/components/header.py
--rw-r--r--   0        0        0      670 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/components/hero.py
--rw-r--r--   0        0        0     1192 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/README.md
--rw-r--r--   0        0        0    11388 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/__init__.py
--rw-r--r--   0        0        0     7911 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/__init__.py
--rw-r--r--   0        0        0      792 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/altair.py
--rw-r--r--   0        0        0      198 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/app_bar.py
--rw-r--r--   0        0        0      452 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/app_layout.py
--rw-r--r--   0        0        0      432 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/button.py
--rw-r--r--   0        0        0      522 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/checkbox.py
--rw-r--r--   0        0        0      719 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/column.py
--rw-r--r--   0        0        0      953 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/columns.py
--rw-r--r--   0        0        0     3280 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/columns_responsive.py
--rw-r--r--   0        0        0      236 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/common.py
--rw-r--r--   0        0        0      502 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/cross_filter_dataframe.py
--rw-r--r--   0        0        0      485 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/cross_filter_report.py
--rw-r--r--   0        0        0      461 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/cross_filter_select.py
--rw-r--r--   0        0        0      491 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/cross_filter_slider.py
--rw-r--r--   0        0        0     1229 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/dataframe.py
--rw-r--r--   0        0        0      355 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/default_layout.py
--rw-r--r--   0        0        0      182 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/display.py
--rw-r--r--   0        0        0     2595 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/echarts.py
--rw-r--r--   0        0        0     1129 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/error.py
--rw-r--r--   0        0        0     1022 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/file_browser.py
--rw-r--r--   0        0        0      196 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/file_download.py
--rw-r--r--   0        0        0      962 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/file_drop.py
--rw-r--r--   0        0        0      239 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/generate_routes.py
--rw-r--r--   0        0        0      269 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/generate_routes_directory.py
--rw-r--r--   0        0        0     2130 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/griddraggable.py
--rw-r--r--   0        0        0      405 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/gridfixed.py
--rw-r--r--   0        0        0      346 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/hbox.py
--rw-r--r--   0        0        0      475 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/head.py
--rw-r--r--   0        0        0      335 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/html.py
--rw-r--r--   0        0        0      723 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/image.py
--rw-r--r--   0        0        0     1126 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/info.py
--rw-r--r--   0        0        0     1907 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/input.py
--rw-r--r--   0        0        0      733 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/link.py
--rw-r--r--   0        0        0     1158 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/markdown.py
--rw-r--r--   0        0        0     1004 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/markdown_editor.py
--rw-r--r--   0        0        0      763 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/matplotlib.py
--rw-r--r--   0        0        0      992 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/memoize.py
--rw-r--r--   0        0        0      589 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/meta.py
--rw-r--r--   0        0        0     2928 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/pivot_table.py
--rw-r--r--   0        0        0     1376 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/plotly.py
--rw-r--r--   0        0        0      957 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/plotly_express.py
--rw-r--r--   0        0        0     1211 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/resolve_path.py
--rw-r--r--   0        0        0     1026 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/route.py
--rw-r--r--   0        0        0      704 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/row.py
--rw-r--r--   0        0        0     1110 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/select.py
--rw-r--r--   0        0        0      484 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/sidebar.py
--rw-r--r--   0        0        0     2513 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/slider.py
--rw-r--r--   0        0        0     2782 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/sql_code.py
--rw-r--r--   0        0        0     1023 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/style.py
--rw-r--r--   0        0        0     1135 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/success.py
--rw-r--r--   0        0        0      897 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/title.py
--rw-r--r--   0        0        0     1950 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/togglebuttons.py
--rw-r--r--   0        0        0      181 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/tooltip.py
--rw-r--r--   0        0        0      512 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_cross_filter.py
--rw-r--r--   0        0        0      898 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_exception.py
--rw-r--r--   0        0        0      579 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_previous.py
--rw-r--r--   0        0        0     3953 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_route.py
--rw-r--r--   0        0        0      225 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_state.py
--rw-r--r--   0        0        0     2681 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_state_or_update.py
--rw-r--r--   0        0        0     2251 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_thread.md
--rw-r--r--   0        0        0     1473 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/use_thread.py
--rw-r--r--   0        0        0      348 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/vbox.py
--rw-r--r--   0        0        0     1385 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/warning.py
--rw-r--r--   0        0        0     2744 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/api/widget.py
--rw-r--r--   0        0        0      189 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/__init__.py
--rw-r--r--   0        0        0     1675 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/layout-demo.py
--rw-r--r--   0        0        0      547 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/multipage/__init__.py
--rw-r--r--   0        0        0      783 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/multipage/page1.py
--rw-r--r--   0        0        0      401 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/multipage/page2.py
--rw-r--r--   0        0        0     4682 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/scatter.py
--rw-r--r--   0        0        0      426 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/apps/tutorial-streamlit.py
--rw-r--r--   0        0        0     3131 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/doc_use_download.py
--rw-r--r--   0        0        0      339 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/docs/__init__.py
--rw-r--r--   0        0        0     6004 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/docs/content/00-introduction.md
--rw-r--r--   0        0        0     1219 2023-03-16 11:18:45.549980 solara-1.8.2/solara/website/pages/docs/content/02-installing.md
--rw-r--r--   0        0        0     2526 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/03-quickstart.md
--rw-r--r--   0        0        0      795 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/00-overview.md
--rw-r--r--   0        0        0     2565 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/10_data_science.py
--rw-r--r--   0        0        0     3011 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/20-web-app.md
--rw-r--r--   0        0        0     4160 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/30-ipywidgets.md
--rw-r--r--   0        0        0     5612 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/40-streamlit.md
--rw-r--r--   0        0        0     4841 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/50-dash.md
--rw-r--r--   0        0        0    28317 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/04-tutorial/_data_science.ipynb
--rw-r--r--   0        0        0      182 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/10-howto/00-overview.md
--rw-r--r--   0        0        0     6640 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/10-howto/20-multipage.md
--rw-r--r--   0        0        0     5021 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/10-howto/30-layout.md
--rw-r--r--   0        0        0      232 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/00-overview.md
--rw-r--r--   0        0        0      874 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/40-static_files.md
--rw-r--r--   0        0        0     1571 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/41-asset-files.md
--rw-r--r--   0        0        0     2515 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/60-static-site-generation.md
--rw-r--r--   0        0        0      890 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/70-search.md
--rw-r--r--   0        0        0      948 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/80-reloading.md
--rw-r--r--   0        0        0      267 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/90-notebook-support.md
--rw-r--r--   0        0        0     4187 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/15-reference/95-caching.md
--rw-r--r--   0        0        0      268 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/00-introduction.md
--rw-r--r--   0        0        0     1790 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/05-ipywidgets.md
--rw-r--r--   0        0        0     1383 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/06-ipyvuetify.md
--rw-r--r--   0        0        0     1226 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/10-reacton.md
--rw-r--r--   0        0        0     5071 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/12-reacton-basics.md
--rw-r--r--   0        0        0     1776 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/15-anatomy.md
--rw-r--r--   0        0        0      111 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/17-rules-of-hooks.md
--rw-r--r--   0        0        0     4579 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/18-containers.md
--rw-r--r--   0        0        0      454 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/20-solara.md
--rw-r--r--   0        0        0     7774 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/40-routing.md
--rw-r--r--   0        0        0      837 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/50-solara-server.md
--rw-r--r--   0        0        0      864 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/20-understanding/60-voila.md
--rw-r--r--   0        0        0      138 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/30-deploying/00-overview.md
--rw-r--r--   0        0        0     6178 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/30-deploying/10-self-hosted.md
--rw-r--r--   0        0        0     3636 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/30-deploying/20-cloud-hosted.md
--rw-r--r--   0        0        0     1620 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/90-development/10-setup.md
--rw-r--r--   0        0        0     1564 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/90-troubleshoot.md
--rw-r--r--   0        0        0     3096 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/99-faq.md
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/__init__.py
--rw-r--r--   0        0        0      141 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/lab/00-what-is-lab.md
--rw-r--r--   0        0        0     7100 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docs/content/lab/toestand.md
--rw-r--r--   0        0        0      742 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/docutils.py
--rw-r--r--   0        0        0     2113 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/__init__.py
--rw-r--r--   0        0        0      105 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/basics/__init__.py
--rw-r--r--   0        0        0      676 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/basics/sine.py
--rw-r--r--   0        0        0      410 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/fullscreen.py
--rw-r--r--   0        0        0      105 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/general/__init__.py
--rw-r--r--   0        0        0     2055 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/general/pokemon_search.py
--rw-r--r--   0        0        0     1846 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/ipycanvas.py
--rw-r--r--   0        0        0      105 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/utilities/__init__.py
--rw-r--r--   0        0        0     5529 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/utilities/calculator.py
--rw-r--r--   0        0        0     2143 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/utilities/countdown_timer.py
--rw-r--r--   0        0        0      105 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/visualization/__init__.py
--rw-r--r--   0        0        0     1147 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/visualization/bqplot.py
--rw-r--r--   0        0        0     2700 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/visualization/linked_views.py
--rw-r--r--   0        0        0     1243 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/pages/examples/visualization/plotly.py
--rw-r--r--   0        0        0    37437 2023-03-16 11:18:45.553980 solara-1.8.2/solara/website/public/beach.jpeg
--rw-r--r--   0        0        0   365019 2023-03-16 11:18:45.557980 solara-1.8.2/solara/website/public/docs/anatomy.png
--rw-r--r--   0        0        0   197645 2023-03-16 11:18:45.557980 solara-1.8.2/solara/website/public/docs/reacton-basics.png
--rw-r--r--   0        0        0   366251 2023-03-16 11:18:45.561980 solara-1.8.2/solara/website/public/docs/solara-stack.png
--rw-r--r--   0        0        0   571029 2023-03-16 11:18:45.565981 solara-1.8.2/solara/website/public/hero.png
--rw-r--r--   0        0        0   132307 2023-03-16 11:18:45.565981 solara-1.8.2/solara/website/public/landing/complexity.png
--rw-r--r--   0        0        0   150332 2023-03-16 11:18:45.565981 solara-1.8.2/solara/website/public/landing/python-love-react.png
--rw-r--r--   0        0        0   591427 2023-03-16 11:18:45.569981 solara-1.8.2/solara/website/public/landing/what.png
--rw-r--r--   0        0        0   156765 2023-03-16 11:18:45.569981 solara-1.8.2/solara/website/public/quickstart-notebook.png
--rw-r--r--   0        0        0     1470 2023-03-16 11:18:45.569981 solara-1.8.2/solara/website/templates/index.html.j2
--rw-r--r--   0        0        0      855 2023-03-16 11:18:45.569981 solara-1.8.2/solara/website/utils.py
--rw-r--r--   0        0        0       43 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/__init__.py
--rw-r--r--   0        0        0     3559 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/vue/gridlayout.vue
--rw-r--r--   0        0        0      404 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/vue/html.vue
--rw-r--r--   0        0        0     3467 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/vue/navigator.vue
--rw-r--r--   0        0        0     3231 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/vue/vegalite.vue
--rw-r--r--   0        0        0     1894 2023-03-16 11:18:45.569981 solara-1.8.2/solara/widgets/widgets.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.569981 solara-1.8.2/tests/__init__.py
--rw-r--r--   0        0        0      426 2023-03-16 11:18:45.569981 solara-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/__init__.py
--rw-r--r--   0        0        0     4027 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/api_test.py
--rw-r--r--   0        0        0      233 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/app_widget.py
--rw-r--r--   0        0        0     1374 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/cmdline_test.py
--rw-r--r--   0        0        0     4147 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/conftest.py
--rw-r--r--   0        0        0     1850 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/create_test.py
--rw-r--r--   0        0        0      475 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/error_test.py
--rw-r--r--   0        0        0     1083 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/file_download_test.py
--rw-r--r--   0        0        0     2408 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/markdown_test.py
--rw-r--r--   0        0        0     6044 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/reload_test.py
--rw-r--r--   0        0        0     2000 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/router_test.py
--rw-r--r--   0        0        0     4410 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/server_test.py
--rw-r--r--   0        0        0     2210 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/ssg_test.py
--rw-r--r--   0        0        0       48 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/test.vue
--rw-r--r--   0        0        0      920 2023-03-16 11:18:45.573981 solara-1.8.2/tests/integration/testapp.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/__init__.py
--rw-r--r--   0        0        0     5735 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/app_test.py
--rw-r--r--   0        0        0     2686 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/applayout_test.py
--rw-r--r--   0        0        0     7719 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/autorouting_test.py
--rw-r--r--   0        0        0     6713 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/cache_test.py
--rw-r--r--   0        0        0     2742 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/cdn_helper_test.py
--rw-r--r--   0        0        0     1652 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/common.py
--rw-r--r--   0        0        0      622 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/conftest.py
--rw-r--r--   0        0        0     3933 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/cross_filter_component_test.py
--rw-r--r--   0        0        0     2678 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/cross_filter_test.py
--rw-r--r--   0        0        0     5548 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/dataframe_test.py
--rw-r--r--   0        0        0      468 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/datatable_test.py
--rw-r--r--   0        0        0      707 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/express_test.py
--rw-r--r--   0        0        0     5985 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/file_browser_test.py
--rw-r--r--   0        0        0     1798 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/file_download_test.py
--rw-r--r--   0        0        0     7018 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/hooks_test.py
--rw-r--r--   0        0        0      576 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/kernel_test.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/lab/__init__.py
--rw-r--r--   0        0        0    19994 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/lab/toestand_test.py
--rw-r--r--   0        0        0      349 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/matplotlib_test.py
--rw-r--r--   0        0        0      747 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/patch_test.py
--rw-r--r--   0        0        0     3909 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/pivottable_test.py
--rw-r--r--   0        0        0     6527 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/router_test.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/food/__init__.py
--rw-r--r--   0        0        0       16 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/food/food.py
--rw-r--r--   0        0        0      101 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/food/index.py
--rw-r--r--   0        0        0      207 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
--rw-r--r--   0        0        0      324 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/01-views.py
--rw-r--r--   0        0        0      328 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
--rw-r--r--   0        0        0      364 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
--rw-r--r--   0        0        0     1251 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
--rw-r--r--   0        0        0       63 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/01-home.py
--rw-r--r--   0        0        0       86 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/02-my_fruit.py
--rw-r--r--   0        0        0      564 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/03-some-markdown.md
--rw-r--r--   0        0        0       15 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
--rw-r--r--   0        0        0       70 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
--rw-r--r--   0        0        0      154 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
--rw-r--r--   0        0        0      347 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
--rw-r--r--   0        0        0       14 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
--rw-r--r--   0        0        0        0 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
--rw-r--r--   0        0        0       31 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/multipage/some_other_file.txt
--rw-r--r--   0        0        0      704 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/notebookapp_component.ipynb
--rw-r--r--   0        0        0      651 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/notebookapp_element.ipynb
--rw-r--r--   0        0        0      671 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/solara_test_apps/notebookapp_widget.ipynb
--rw-r--r--   0        0        0      854 2023-03-16 11:18:45.573981 solara-1.8.2/tests/unit/telemetry_tests.py
--rw-r--r--   0        0        0      513 2023-03-16 11:18:45.573981 solara-1.8.2/tsconfigbase.json
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 solara-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      681 2023-03-30 16:54:48.677600 solara-1.9.0/.bumpversion.cfg
+-rw-r--r--   0        0        0      136 2023-03-30 16:54:48.677600 solara-1.9.0/.flake8
+-rw-r--r--   0        0        0      780 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/codequality.yaml
+-rw-r--r--   0        0        0     1769 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/installation.yml
+-rw-r--r--   0        0        0     2699 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      975 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/javascript.yaml
+-rw-r--r--   0        0        0     1588 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      998 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/release_solara_vuetify_app.yaml
+-rw-r--r--   0        0        0     1203 2023-03-30 16:54:48.677600 solara-1.9.0/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      917 2023-03-30 16:54:48.677600 solara-1.9.0/.gitignore
+-rw-r--r--   0        0        0      971 2023-03-30 16:54:48.677600 solara-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1086 2023-03-30 16:54:48.677600 solara-1.9.0/LICENSE
+-rw-r--r--   0        0        0      614 2023-03-30 16:54:48.677600 solara-1.9.0/Procfile
+-rw-r--r--   0        0        0     1213 2023-03-30 16:54:48.677600 solara-1.9.0/README.md
+-rw-r--r--   0        0        0      115 2023-03-30 16:54:48.677600 solara-1.9.0/mypy.ini
+-rw-r--r--   0        0        0       85 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/.gitignore
+-rw-r--r--   0        0        0     1086 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/LICENSE
+-rw-r--r--   0        0        0      501 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/RELEASE.md
+-rw-r--r--   0        0        0      451 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/download_cdn_test.py
+-rw-r--r--   0        0        0     2119 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/hatch_build.py
+-rw-r--r--   0        0        0      672 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-03-30 16:54:48.677600 solara-1.9.0/packages/assets/solara_assets/__init__.py
+-rw-r--r--   0        0        0       59 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/LICENSE
+-rw-r--r--   0        0        0      247 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/RELEASE.md
+-rw-r--r--   0        0        0      725 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/__init__.py
+-rw-r--r--   0        0        0     1941 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/base.py
+-rw-r--r--   0        0        0     1190 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/disk.py
+-rw-r--r--   0        0        0      816 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/memory_size.py
+-rw-r--r--   0        0        0      710 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/multi_level.py
+-rw-r--r--   0        0        0      779 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/redis.py
+-rw-r--r--   0        0        0      411 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/license.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/__init__.py
+-rw-r--r--   0        0        0     3307 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/index.py
+-rw-r--r--   0        0        0      467 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/search.py
+-rw-r--r--   0        0        0     6127 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/search.vue
+-rw-r--r--   0        0        0     7118 2023-03-30 16:54:48.677600 solara-1.9.0/packages/solara-enterprise/solara_enterprise/ssg.py
+-rw-r--r--   0        0        0   427583 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-milkdown/package-lock.json
+-rw-r--r--   0        0        0      915 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-milkdown/package.json
+-rw-r--r--   0        0        0      461 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-milkdown/src/index.js
+-rw-r--r--   0        0        0     1025 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-milkdown/webpack.config.js
+-rw-r--r--   0        0        0      422 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/.bumpversion.cfg
+-rw-r--r--   0        0        0      239 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/README.md
+-rw-r--r--   0        0        0   129847 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/package-lock.json
+-rw-r--r--   0        0        0     1150 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/package.json
+-rwxr-xr-x   0        0        0      289 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/release.sh
+-rw-r--r--   0        0        0      438 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/src/solara-vuetify-app.js
+-rw-r--r--   0        0        0      142 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/src/solara.js
+-rwxr-xr-x   0        0        0     2791 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-vuetify-app/webpack.config.js
+-rw-r--r--   0        0        0     1538 2023-03-30 16:54:48.681600 solara-1.9.0/packages/solara-widget-manager/LICENSE.voila.txt
+-rw-r--r--   0        0        0   741390 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/package-lock.json
+-rw-r--r--   0        0        0     2147 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/package.json
+-rw-r--r--   0        0        0      934 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/index.ts
+-rw-r--r--   0        0        0     1452 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/kernel.ts
+-rw-r--r--   0        0        0     3290 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/loader.ts
+-rw-r--r--   0        0        0     8500 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/manager.ts
+-rw-r--r--   0        0        0     1319 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/mathjax.ts
+-rw-r--r--   0        0        0     1236 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/rendermime.ts
+-rw-r--r--   0        0        0      127 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/src/typings.d.ts
+-rw-r--r--   0        0        0     3446 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/style/index.css
+-rw-r--r--   0        0        0      135 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/tsconfig.json
+-rw-r--r--   0        0        0     2607 2023-03-30 16:54:48.685600 solara-1.9.0/packages/solara-widget-manager/webpack.config.js
+-rw-r--r--   0        0        0      115 2023-03-30 16:54:48.685600 solara-1.9.0/prefix/etc/jupyter/jupyter_notebook_config.d/solara.json
+-rw-r--r--   0        0        0      113 2023-03-30 16:54:48.685600 solara-1.9.0/prefix/etc/jupyter/jupyter_server_config.d/solara.json
+-rw-r--r--   0        0        0     2169 2023-03-30 16:54:48.685600 solara-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-03-30 16:54:48.685600 solara-1.9.0/release.md
+-rwxr-xr-x   0        0        0      232 2023-03-30 16:54:48.685600 solara-1.9.0/release.sh
+-rw-r--r--   0        0        0      123 2023-03-30 16:54:48.685600 solara-1.9.0/requirements.txt
+-rw-r--r--   0        0        0       14 2023-03-30 16:54:48.685600 solara-1.9.0/runtime.txt
+-rw-r--r--   0        0        0     3142 2023-03-30 16:54:48.685600 solara-1.9.0/solara/__init__.py
+-rw-r--r--   0        0        0    21260 2023-03-30 16:54:48.685600 solara-1.9.0/solara/__main__.py
+-rw-r--r--   0        0        0      216 2023-03-30 16:54:48.685600 solara-1.9.0/solara/alias.py
+-rw-r--r--   0        0        0    17952 2023-03-30 16:54:48.685600 solara-1.9.0/solara/autorouting.py
+-rw-r--r--   0        0        0    10743 2023-03-30 16:54:48.685600 solara-1.9.0/solara/cache.py
+-rw-r--r--   0        0        0     3254 2023-03-30 16:54:48.685600 solara-1.9.0/solara/checks.html
+-rw-r--r--   0        0        0     4283 2023-03-30 16:54:48.685600 solara-1.9.0/solara/checks.py
+-rw-r--r--   0        0        0      642 2023-03-30 16:54:48.685600 solara-1.9.0/solara/comm.py
+-rw-r--r--   0        0        0     2402 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/__init__.py
+-rw-r--r--   0        0        0     4639 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/alert.py
+-rw-r--r--   0        0        0    12992 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/applayout.py
+-rw-r--r--   0        0        0     1791 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/button.py
+-rw-r--r--   0        0        0     2574 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/card.py
+-rw-r--r--   0        0        0      890 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/checkbox.py
+-rw-r--r--   0        0        0      235 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/code_highlight_css.py
+-rw-r--r--   0        0        0     5776 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/code_highlight_css.vue
+-rw-r--r--   0        0        0     4896 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/columns.py
+-rw-r--r--   0        0        0    13473 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/cross_filter.py
+-rw-r--r--   0        0        0    21030 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/dataframe.py
+-rw-r--r--   0        0        0     7869 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/datatable.py
+-rw-r--r--   0        0        0     7061 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/datatable.vue
+-rw-r--r--   0        0        0      675 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/details.py
+-rw-r--r--   0        0        0     1069 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/download.vue
+-rw-r--r--   0        0        0     2589 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/echarts.py
+-rw-r--r--   0        0        0     3695 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/echarts.vue
+-rw-r--r--   0        0        0      962 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/figure_altair.py
+-rw-r--r--   0        0        0     6960 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/file_browser.py
+-rw-r--r--   0        0        0     6900 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/file_download.py
+-rw-r--r--   0        0        0     3165 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/file_drop.py
+-rw-r--r--   0        0        0     1870 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/file_drop.vue
+-rw-r--r--   0        0        0     1860 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/file_list_widget.vue
+-rw-r--r--   0        0        0      623 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/head.py
+-rw-r--r--   0        0        0     1566 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/head_tag.py
+-rw-r--r--   0        0        0     1658 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/head_tag.vue
+-rw-r--r--   0        0        0     1910 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/image.py
+-rw-r--r--   0        0        0    10041 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/input.py
+-rw-r--r--   0        0        0     1390 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/link.py
+-rw-r--r--   0        0        0     6895 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/markdown.py
+-rw-r--r--   0        0        0      634 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/markdown_editor.py
+-rw-r--r--   0        0        0     8864 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/markdown_editor.vue
+-rw-r--r--   0        0        0     1952 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/matplotlib.py
+-rw-r--r--   0        0        0     1629 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/meta.py
+-rw-r--r--   0        0        0     9521 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/misc.py
+-rw-r--r--   0        0        0     9871 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/pivot_table.py
+-rw-r--r--   0        0        0     4674 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/pivot_table.vue
+-rw-r--r--   0        0        0     1668 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/select.py
+-rw-r--r--   0        0        0      950 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/select.vue
+-rw-r--r--   0        0        0     7939 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/slider.py
+-rw-r--r--   0        0        0     1351 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/slider_date.vue
+-rw-r--r--   0        0        0     1189 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/sql_code.py
+-rw-r--r--   0        0        0     3937 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/sql_code.vue
+-rw-r--r--   0        0        0      883 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/style.py
+-rw-r--r--   0        0        0     1047 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/tab_navigation.py
+-rw-r--r--   0        0        0     2159 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/title.py
+-rw-r--r--   0        0        0      901 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/title.vue
+-rw-r--r--   0        0        0     2630 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/togglebuttons.py
+-rw-r--r--   0        0        0     1636 2023-03-30 16:54:48.685600 solara-1.9.0/solara/components/tooltip.py
+-rw-r--r--   0        0        0     4150 2023-03-30 16:54:48.685600 solara-1.9.0/solara/datatypes.py
+-rw-r--r--   0        0        0     6781 2023-03-30 16:54:48.689600 solara-1.9.0/solara/express.py
+-rw-r--r--   0        0        0       85 2023-03-30 16:54:48.689600 solara-1.9.0/solara/hooks/__init__.py
+-rw-r--r--   0        0        0     3421 2023-03-30 16:54:48.689600 solara-1.9.0/solara/hooks/dataframe.py
+-rw-r--r--   0        0        0    13555 2023-03-30 16:54:48.689600 solara-1.9.0/solara/hooks/misc.py
+-rw-r--r--   0        0        0      249 2023-03-30 16:54:48.689600 solara-1.9.0/solara/kitchensink.py
+-rw-r--r--   0        0        0      740 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/components/__init__.py
+-rw-r--r--   0        0        0      186 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/components/cross_filter.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/hooks/__init__.py
+-rw-r--r--   0        0        0      268 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/hooks/dataframe.py
+-rw-r--r--   0        0        0    15893 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/toestand.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/utils/__init__.py
+-rw-r--r--   0        0        0     3044 2023-03-30 16:54:48.689600 solara-1.9.0/solara/lab/utils/dataframe.py
+-rw-r--r--   0        0        0     1782 2023-03-30 16:54:48.689600 solara-1.9.0/solara/layout.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/py.typed
+-rw-r--r--   0        0        0     6105 2023-03-30 16:54:48.689600 solara-1.9.0/solara/routing.py
+-rw-r--r--   0        0        0     1137 2023-03-30 16:54:48.689600 solara-1.9.0/solara/scope/__init__.py
+-rw-r--r--   0        0        0     1540 2023-03-30 16:54:48.689600 solara-1.9.0/solara/scope/types.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/__init__.py
+-rw-r--r--   0        0        0    22774 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/app.py
+-rw-r--r--   0        0        0       15 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/custom.css
+-rw-r--r--   0        0        0       16 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/custom.js
+-rw-r--r--   0        0        0     1924 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/favicon.png
+-rw-r--r--   0        0        0     1240 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/favicon.svg
+-rw-r--r--   0        0        0     1626 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/style.css
+-rw-r--r--   0        0        0       21 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/assets/theme.js
+-rw-r--r--   0        0        0     2481 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/cdn_helper.py
+-rw-r--r--   0        0        0       93 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/fastapi.py
+-rw-r--r--   0        0        0     5549 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/flask.py
+-rw-r--r--   0        0        0      137 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/jupyter/__init__.py
+-rw-r--r--   0        0        0      835 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/jupyter/cdn_handler.py
+-rw-r--r--   0        0        0      680 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/jupyter/server_extension.py
+-rw-r--r--   0        0        0     9179 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/kernel.py
+-rw-r--r--   0        0        0     9477 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/patch.py
+-rw-r--r--   0        0        0      916 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/pyodide.py
+-rw-r--r--   0        0        0     8189 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/reload.py
+-rw-r--r--   0        0        0    10471 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/server.py
+-rw-r--r--   0        0        0     2744 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/settings.py
+-rw-r--r--   0        0        0    12114 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/starlette.py
+-rw-r--r--   0        0        0     7797 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/ansi.js
+-rw-r--r--   0        0        0     6809 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/highlight-dark.css
+-rw-r--r--   0        0        0     2637 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/highlight.css
+-rw-r--r--   0        0        0     7981 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/main-vuetify.js
+-rw-r--r--   0        0        0     5679 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/main.js
+-rw-r--r--   0        0        0     3194 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/solara_bootstrap.py
+-rw-r--r--   0        0        0     6855 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/sun.svg
+-rw-r--r--   0        0        0     1372 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/static/webworker.js
+-rw-r--r--   0        0        0     3415 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/telemetry.py
+-rw-r--r--   0        0        0       31 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/index.html.j2
+-rw-r--r--   0        0        0      205 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/loader-plain.css
+-rw-r--r--   0        0        0      678 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/loader-plain.html
+-rw-r--r--   0        0        0     1900 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/loader-solara.css
+-rw-r--r--   0        0        0     2730 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/loader-solara.html
+-rw-r--r--   0        0        0     2762 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/plain.html
+-rw-r--r--   0        0        0    17096 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/templates/solara.html.j2
+-rw-r--r--   0        0        0     2088 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/threaded.py
+-rw-r--r--   0        0        0      935 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/utils.py
+-rw-r--r--   0        0        0     1057 2023-03-30 16:54:48.689600 solara-1.9.0/solara/server/websocket.py
+-rw-r--r--   0        0        0     1120 2023-03-30 16:54:48.689600 solara-1.9.0/solara/settings.py
+-rw-r--r--   0        0        0      325 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/button.py
+-rw-r--r--   0        0        0     1137 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/markdown.py
+-rw-r--r--   0        0        0      136 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/.flake8
+-rw-r--r--   0        0        0      791 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1066 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/LICENSE
+-rw-r--r--   0        0        0      407 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/Procfile
+-rw-r--r--   0        0        0       63 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/mypy.ini
+-rw-r--r--   0        0        0      450 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/pyproject.toml
+-rw-r--r--   0        0        0       99 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/__init__.py
+-rw-r--r--   0        0        0       70 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/components/__init__.py
+-rw-r--r--   0        0        0      854 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/components/article.py
+-rw-r--r--   0        0        0      828 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/components/data.py
+-rw-r--r--   0        0        0       57 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/components/header.py
+-rw-r--r--   0        0        0      101 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/components/layout.py
+-rw-r--r--   0        0        0     3619 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md
+-rw-r--r--   0        0        0     3092 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md
+-rw-r--r--   0        0        0     1911 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/data.py
+-rw-r--r--   0        0        0     2565 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/pages/__init__.py
+-rw-r--r--   0        0        0      814 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/pages/article/__init__.py
+-rw-r--r--   0        0        0      938 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/pages/tabular.py
+-rw-r--r--   0        0        0     2857 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/pages/viz/__init__.py
+-rw-r--r--   0        0        0      365 2023-03-30 16:54:48.689600 solara-1.9.0/solara/template/portal/solara_portal/pages/viz/overview.py
+-rw-r--r--   0        0        0     3834 2023-03-30 16:54:48.689600 solara-1.9.0/solara/util.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/__init__.py
+-rw-r--r--   0        0        0     4523 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/assets/custom.css
+-rw-r--r--   0        0        0    86383 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/assets/images/logo-small.png
+-rw-r--r--   0        0        0     4858 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/assets/images/logo.svg
+-rw-r--r--   0        0        0       67 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/assets/theme.js
+-rw-r--r--   0        0        0       80 2023-03-30 16:54:48.689600 solara-1.9.0/solara/website/components/__init__.py
+-rw-r--r--   0        0        0     1940 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/components/header.py
+-rw-r--r--   0        0        0      670 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/components/hero.py
+-rw-r--r--   0        0        0     1192 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/README.md
+-rw-r--r--   0        0        0    11122 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/__init__.py
+-rw-r--r--   0        0        0     7983 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/__init__.py
+-rw-r--r--   0        0        0      792 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/altair.py
+-rw-r--r--   0        0        0      198 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/app_bar.py
+-rw-r--r--   0        0        0      452 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/app_layout.py
+-rw-r--r--   0        0        0      432 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/button.py
+-rw-r--r--   0        0        0      191 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/card.py
+-rw-r--r--   0        0        0      213 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/card_actions.py
+-rw-r--r--   0        0        0      522 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/checkbox.py
+-rw-r--r--   0        0        0      699 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/column.py
+-rw-r--r--   0        0        0      910 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/columns.py
+-rw-r--r--   0        0        0     3073 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/columns_responsive.py
+-rw-r--r--   0        0        0      236 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/common.py
+-rw-r--r--   0        0        0      502 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/cross_filter_dataframe.py
+-rw-r--r--   0        0        0      485 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/cross_filter_report.py
+-rw-r--r--   0        0        0      461 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/cross_filter_select.py
+-rw-r--r--   0        0        0      491 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/cross_filter_slider.py
+-rw-r--r--   0        0        0     1229 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/dataframe.py
+-rw-r--r--   0        0        0      355 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/default_layout.py
+-rw-r--r--   0        0        0      182 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/display.py
+-rw-r--r--   0        0        0     2595 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/echarts.py
+-rw-r--r--   0        0        0     1129 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/error.py
+-rw-r--r--   0        0        0     1022 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/file_browser.py
+-rw-r--r--   0        0        0      196 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/file_download.py
+-rw-r--r--   0        0        0      962 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/file_drop.py
+-rw-r--r--   0        0        0      239 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/generate_routes.py
+-rw-r--r--   0        0        0      269 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/generate_routes_directory.py
+-rw-r--r--   0        0        0     2130 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/griddraggable.py
+-rw-r--r--   0        0        0      405 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/gridfixed.py
+-rw-r--r--   0        0        0      346 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/hbox.py
+-rw-r--r--   0        0        0      475 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/head.py
+-rw-r--r--   0        0        0      335 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/html.py
+-rw-r--r--   0        0        0      723 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/image.py
+-rw-r--r--   0        0        0     1126 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/info.py
+-rw-r--r--   0        0        0     2305 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/input.py
+-rw-r--r--   0        0        0      733 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/link.py
+-rw-r--r--   0        0        0     1158 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/markdown.py
+-rw-r--r--   0        0        0     1004 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/markdown_editor.py
+-rw-r--r--   0        0        0      763 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/matplotlib.py
+-rw-r--r--   0        0        0      992 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/memoize.py
+-rw-r--r--   0        0        0      589 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/meta.py
+-rw-r--r--   0        0        0     2928 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/pivot_table.py
+-rw-r--r--   0        0        0     1376 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/plotly.py
+-rw-r--r--   0        0        0      957 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/plotly_express.py
+-rw-r--r--   0        0        0     1211 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/resolve_path.py
+-rw-r--r--   0        0        0     1026 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/route.py
+-rw-r--r--   0        0        0      684 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/row.py
+-rw-r--r--   0        0        0     1110 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/select.py
+-rw-r--r--   0        0        0      485 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/sidebar.py
+-rw-r--r--   0        0        0     2513 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/slider.py
+-rw-r--r--   0        0        0     2782 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/sql_code.py
+-rw-r--r--   0        0        0     1023 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/style.py
+-rw-r--r--   0        0        0     1135 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/success.py
+-rw-r--r--   0        0        0      897 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/title.py
+-rw-r--r--   0        0        0     1950 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/togglebuttons.py
+-rw-r--r--   0        0        0      181 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/tooltip.py
+-rw-r--r--   0        0        0      512 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_cross_filter.py
+-rw-r--r--   0        0        0      898 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_exception.py
+-rw-r--r--   0        0        0      579 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_previous.py
+-rw-r--r--   0        0        0     3953 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_route.py
+-rw-r--r--   0        0        0      225 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_state.py
+-rw-r--r--   0        0        0     2681 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_state_or_update.py
+-rw-r--r--   0        0        0     2251 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_thread.md
+-rw-r--r--   0        0        0     1473 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/use_thread.py
+-rw-r--r--   0        0        0      348 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/vbox.py
+-rw-r--r--   0        0        0     1385 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/warning.py
+-rw-r--r--   0        0        0     2744 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/api/widget.py
+-rw-r--r--   0        0        0      189 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/__init__.py
+-rw-r--r--   0        0        0     1675 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/layout-demo.py
+-rw-r--r--   0        0        0      547 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/multipage/__init__.py
+-rw-r--r--   0        0        0      783 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/multipage/page1.py
+-rw-r--r--   0        0        0      401 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/multipage/page2.py
+-rw-r--r--   0        0        0     4452 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/scatter.py
+-rw-r--r--   0        0        0      426 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/apps/tutorial-streamlit.py
+-rw-r--r--   0        0        0     3131 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/doc_use_download.py
+-rw-r--r--   0        0        0      339 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/__init__.py
+-rw-r--r--   0        0        0     6004 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/00-introduction.md
+-rw-r--r--   0        0        0     1219 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/02-installing.md
+-rw-r--r--   0        0        0     2526 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/03-quickstart.md
+-rw-r--r--   0        0        0      795 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/00-overview.md
+-rw-r--r--   0        0        0     2565 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/10_data_science.py
+-rw-r--r--   0        0        0     3011 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/20-web-app.md
+-rw-r--r--   0        0        0     4160 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/30-ipywidgets.md
+-rw-r--r--   0        0        0     5613 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/40-streamlit.md
+-rw-r--r--   0        0        0     4841 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/50-dash.md
+-rw-r--r--   0        0        0    28317 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/04-tutorial/_data_science.ipynb
+-rw-r--r--   0        0        0      182 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/10-howto/00-overview.md
+-rw-r--r--   0        0        0     6640 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/10-howto/20-multipage.md
+-rw-r--r--   0        0        0     5023 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/10-howto/30-layout.md
+-rw-r--r--   0        0        0      232 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/00-overview.md
+-rw-r--r--   0        0        0      874 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/40-static_files.md
+-rw-r--r--   0        0        0     1571 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/41-asset-files.md
+-rw-r--r--   0        0        0     2515 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/60-static-site-generation.md
+-rw-r--r--   0        0        0      890 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/70-search.md
+-rw-r--r--   0        0        0      948 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/80-reloading.md
+-rw-r--r--   0        0        0      267 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/90-notebook-support.md
+-rw-r--r--   0        0        0     4187 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/15-reference/95-caching.md
+-rw-r--r--   0        0        0      268 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/00-introduction.md
+-rw-r--r--   0        0        0     1790 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/05-ipywidgets.md
+-rw-r--r--   0        0        0     1383 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/06-ipyvuetify.md
+-rw-r--r--   0        0        0     1226 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/10-reacton.md
+-rw-r--r--   0        0        0     5071 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/12-reacton-basics.md
+-rw-r--r--   0        0        0     1776 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/15-anatomy.md
+-rw-r--r--   0        0        0      111 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/17-rules-of-hooks.md
+-rw-r--r--   0        0        0     4579 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/18-containers.md
+-rw-r--r--   0        0        0      454 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/20-solara.md
+-rw-r--r--   0        0        0     7774 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/40-routing.md
+-rw-r--r--   0        0        0      837 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/50-solara-server.md
+-rw-r--r--   0        0        0      864 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/20-understanding/60-voila.md
+-rw-r--r--   0        0        0      138 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/30-deploying/00-overview.md
+-rw-r--r--   0        0        0     6178 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/30-deploying/10-self-hosted.md
+-rw-r--r--   0        0        0     3636 2023-03-30 16:54:48.693600 solara-1.9.0/solara/website/pages/docs/content/30-deploying/20-cloud-hosted.md
+-rw-r--r--   0        0        0     1620 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/90-development/10-setup.md
+-rw-r--r--   0        0        0     1564 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/90-troubleshoot.md
+-rw-r--r--   0        0        0     3096 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/99-faq.md
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/__init__.py
+-rw-r--r--   0        0        0      141 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/lab/00-what-is-lab.md
+-rw-r--r--   0        0        0     7100 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docs/content/lab/toestand.md
+-rw-r--r--   0        0        0      742 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/docutils.py
+-rw-r--r--   0        0        0     2113 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/__init__.py
+-rw-r--r--   0        0        0      105 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/basics/__init__.py
+-rw-r--r--   0        0        0      676 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/basics/sine.py
+-rw-r--r--   0        0        0      410 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/fullscreen.py
+-rw-r--r--   0        0        0      105 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/general/__init__.py
+-rw-r--r--   0        0        0     2079 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/general/pokemon_search.py
+-rw-r--r--   0        0        0     1846 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/ipycanvas.py
+-rw-r--r--   0        0        0      105 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/utilities/__init__.py
+-rw-r--r--   0        0        0     5529 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/utilities/calculator.py
+-rw-r--r--   0        0        0     2143 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/utilities/countdown_timer.py
+-rw-r--r--   0        0        0      105 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/visualization/__init__.py
+-rw-r--r--   0        0        0     1147 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/visualization/bqplot.py
+-rw-r--r--   0        0        0     2700 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/visualization/linked_views.py
+-rw-r--r--   0        0        0     1243 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/pages/examples/visualization/plotly.py
+-rw-r--r--   0        0        0    37437 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/public/beach.jpeg
+-rw-r--r--   0        0        0   365019 2023-03-30 16:54:48.697600 solara-1.9.0/solara/website/public/docs/anatomy.png
+-rw-r--r--   0        0        0   197645 2023-03-30 16:54:48.701600 solara-1.9.0/solara/website/public/docs/reacton-basics.png
+-rw-r--r--   0        0        0   366251 2023-03-30 16:54:48.701600 solara-1.9.0/solara/website/public/docs/solara-stack.png
+-rw-r--r--   0        0        0   571029 2023-03-30 16:54:48.705600 solara-1.9.0/solara/website/public/hero.png
+-rw-r--r--   0        0        0   132307 2023-03-30 16:54:48.705600 solara-1.9.0/solara/website/public/landing/complexity.png
+-rw-r--r--   0        0        0   150332 2023-03-30 16:54:48.709600 solara-1.9.0/solara/website/public/landing/python-love-react.png
+-rw-r--r--   0        0        0   591427 2023-03-30 16:54:48.713600 solara-1.9.0/solara/website/public/landing/what.png
+-rw-r--r--   0        0        0   156765 2023-03-30 16:54:48.713600 solara-1.9.0/solara/website/public/quickstart-notebook.png
+-rw-r--r--   0        0        0     1470 2023-03-30 16:54:48.713600 solara-1.9.0/solara/website/templates/index.html.j2
+-rw-r--r--   0        0        0      855 2023-03-30 16:54:48.713600 solara-1.9.0/solara/website/utils.py
+-rw-r--r--   0        0        0       43 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/__init__.py
+-rw-r--r--   0        0        0     3559 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/vue/gridlayout.vue
+-rw-r--r--   0        0        0      404 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/vue/html.vue
+-rw-r--r--   0        0        0     3467 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/vue/navigator.vue
+-rw-r--r--   0        0        0     3231 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/vue/vegalite.vue
+-rw-r--r--   0        0        0     1894 2023-03-30 16:54:48.713600 solara-1.9.0/solara/widgets/widgets.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      426 2023-03-30 16:54:48.713600 solara-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     4027 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/api_test.py
+-rw-r--r--   0        0        0      233 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/app_widget.py
+-rw-r--r--   0        0        0     1374 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/cmdline_test.py
+-rw-r--r--   0        0        0     4147 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     1850 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/create_test.py
+-rw-r--r--   0        0        0      475 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/error_test.py
+-rw-r--r--   0        0        0     1083 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/file_download_test.py
+-rw-r--r--   0        0        0     2408 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/markdown_test.py
+-rw-r--r--   0        0        0     6044 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/reload_test.py
+-rw-r--r--   0        0        0     2000 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/router_test.py
+-rw-r--r--   0        0        0     4410 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/server_test.py
+-rw-r--r--   0        0        0     2210 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/ssg_test.py
+-rw-r--r--   0        0        0       48 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/test.vue
+-rw-r--r--   0        0        0      920 2023-03-30 16:54:48.713600 solara-1.9.0/tests/integration/testapp.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5735 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/app_test.py
+-rw-r--r--   0        0        0     2686 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/applayout_test.py
+-rw-r--r--   0        0        0     7719 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/autorouting_test.py
+-rw-r--r--   0        0        0     6713 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/cache_test.py
+-rw-r--r--   0        0        0     2742 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/cdn_helper_test.py
+-rw-r--r--   0        0        0     1652 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/common.py
+-rw-r--r--   0        0        0      622 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3933 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/cross_filter_component_test.py
+-rw-r--r--   0        0        0     2678 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/cross_filter_test.py
+-rw-r--r--   0        0        0     5548 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/dataframe_test.py
+-rw-r--r--   0        0        0      468 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/datatable_test.py
+-rw-r--r--   0        0        0      707 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/express_test.py
+-rw-r--r--   0        0        0     5985 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/file_browser_test.py
+-rw-r--r--   0        0        0     1798 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/file_download_test.py
+-rw-r--r--   0        0        0     7018 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/hooks_test.py
+-rw-r--r--   0        0        0     5052 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/input_test.py
+-rw-r--r--   0        0        0      576 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/kernel_test.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/lab/__init__.py
+-rw-r--r--   0        0        0    27172 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/lab/toestand_test.py
+-rw-r--r--   0        0        0      349 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/matplotlib_test.py
+-rw-r--r--   0        0        0     1240 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/patch_test.py
+-rw-r--r--   0        0        0     3909 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/pivottable_test.py
+-rw-r--r--   0        0        0     6527 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/router_test.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/food/__init__.py
+-rw-r--r--   0        0        0       16 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/food/food.py
+-rw-r--r--   0        0        0      101 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/food/index.py
+-rw-r--r--   0        0        0      207 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/00-overview.md
+-rw-r--r--   0        0        0      324 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/01-views.py
+-rw-r--r--   0        0        0      328 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/02-likes.py
+-rw-r--r--   0        0        0      364 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/03-volume.py
+-rw-r--r--   0        0        0     1251 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb
+-rw-r--r--   0        0        0       63 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/01-home.py
+-rw-r--r--   0        0        0       86 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/02-my_fruit.py
+-rw-r--r--   0        0        0      564 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md
+-rw-r--r--   0        0        0       15 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/04-a_directory/00-another-markdown.md
+-rw-r--r--   0        0        0       70 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/04-a_directory/01-not-an-app.py
+-rw-r--r--   0        0        0      154 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/04-a_directory/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/05-and-notebooks.ipynb
+-rw-r--r--   0        0        0       14 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/10-single-file-directory/single-file.md
+-rw-r--r--   0        0        0        0 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/99-some_other_python_script.py
+-rw-r--r--   0        0        0       31 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/multipage/some_other_file.txt
+-rw-r--r--   0        0        0      704 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/notebookapp_component.ipynb
+-rw-r--r--   0        0        0      651 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/notebookapp_element.ipynb
+-rw-r--r--   0        0        0      671 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb
+-rw-r--r--   0        0        0      854 2023-03-30 16:54:48.713600 solara-1.9.0/tests/unit/telemetry_tests.py
+-rw-r--r--   0        0        0      513 2023-03-30 16:54:48.713600 solara-1.9.0/tsconfigbase.json
+-rw-r--r--   0        0        0     2801 1970-01-01 00:00:00.000000 solara-1.9.0/PKG-INFO
```

### Comparing `solara-1.8.2/.bumpversion.cfg` & `solara-1.9.0/.bumpversion.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.8.2
+current_version = 1.9.0
 commit = True
 tag = True
 parse = (?P<major>\d+)(\.(?P<minor>\d+))(\.(?P<patch>\d+))((?P<release>.)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `solara-1.8.2/.github/workflows/codequality.yaml` & `solara-1.9.0/.github/workflows/codequality.yaml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/.github/workflows/installation.yml` & `solara-1.9.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/.github/workflows/integration.yml` & `solara-1.9.0/.github/workflows/integration.yml`

 * *Files 27% similar despite different names*

```diff
@@ -15,27 +15,55 @@
       fail-fast: false
       matrix:
         # just ubuntu and windows give enough confidence
         # osx should work fine (and we test that locally often)
         os: [ubuntu, windows]
         # just 1 version, it's heavy
         python-version: [3.8]
+        ipywidgets: ["7.7", "8.0"]
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
+      - uses: actions/setup-node@v3
+        with:
+          node-version: 14
+      - name: Cache JS bundle
+        id: cache-js-bundle
+        uses: actions/cache@v3
+        with:
+          path: packages/solara-vuetify-app/dist
+          key: ${{ runner.os }}-js-bundle-${{ hashFiles('packages/solara-vuetify-app/src/**', 'packages/solara-vuetify-app/package.json', 'packages/solara-widget-manager/src/**', 'packages/solara-widget-manager/package.json') }}
+
+      - name: Build solara widget manager
+        if: steps.cache-js-bundle.outputs.cache-hit != 'true'
+        run: |
+          cd packages/solara-widget-manager
+          npm install
+          npm run build
+          cd ../../
+      - name: Build solara app package
+        if: steps.cache-js-bundle.outputs.cache-hit != 'true'
+        run: |
+          cd packages/solara-vuetify-app
+          npm install
+          npm run build
+      - name: Link solara app package
+        run: |
+          cd packages/solara-vuetify-app
+          npm run devlink
       - name: Prepare
         run: mkdir test-results
       - name: Install
         run: |
           pip install ".[dev,server,flask,documentation]"
-          (cd packages/solara-enterprise && pip install ".[ssg]")
+          (cd packages/solara-enterprise && pip install ".[ssg]" "ipywidgets~=${{ matrix.ipywidgets }}")
       - name: Install playwright
         run: playwright install
       - name: test
         # TODO: we used to also run the (cheap) unittests, to get better coverage report, but that gives errors
         # it seems on CI that the default playwright timeout is not (always?) respected, also, if the --timeout argument
         # is shorter than the timeout of playwright, we get no good error message, summary: always keep above 30!
         run: pytest --cov=solara tests/integration --timeout=360 --video=retain-on-failure -vv -s --log-cli-level=warning --assert=plain
```

### Comparing `solara-1.8.2/.github/workflows/javascript.yaml` & `solara-1.9.0/.github/workflows/javascript.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python 3.7
         uses: actions/setup-python@v2
         with:
           python-version: 3.7
+      - uses: actions/setup-node@v3
+        with:
+          node-version: 14
       - name: Install flit
         run: pip install flit
       - name: Build
         run: flit build
       - name: Install solara Python package
         run: pip install dist/*.whl
       - name: Build solara widget manager
```

### Comparing `solara-1.8.2/.github/workflows/release.yaml` & `solara-1.9.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/.github/workflows/release_solara_vuetify_app.yaml` & `solara-1.9.0/.github/workflows/release_solara_vuetify_app.yaml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/.github/workflows/unittest.yml` & `solara-1.9.0/.github/workflows/unittest.yml`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,34 @@
   test:
     runs-on: ${{ matrix.os }}-${{matrix.os == 'ubuntu' && '20.04' || 'latest' }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, macos, windows]
         python: [3.6, 3.9]
+        ipywidgets: ["7.7", "8.0"]
         exclude:
           - os: windows
             python: 3.6
+          - os: ubuntu
+            python: 3.6
+            ipywidgets: "8.0"
+          - os: macos
+            python: 3.6
+            ipywidgets: "8.0"
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           cache: "pip"
       - name: Install
         run: |
           pip install ".[dev]" diskcache redis
-          (cd packages/solara-enterprise && pip install ".[ssg]")
+          (cd packages/solara-enterprise && pip install ".[ssg]" "ipywidgets~=${{ matrix.ipywidgets }}")
       - name: Start Redis
         if: matrix.os != 'windows'
         uses: shogo82148/actions-setup-redis@v1
       - name: test
         run: pytest --cov=solara tests/unit --doctest-modules solara/util.py --timeout=60
```

### Comparing `solara-1.8.2/.gitignore` & `solara-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/.pre-commit-config.yaml` & `solara-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/LICENSE` & `solara-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/Procfile` & `solara-1.9.0/Procfile`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/README.md` & `solara-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/assets/LICENSE` & `solara-1.9.0/packages/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/assets/hatch_build.py` & `solara-1.9.0/packages/assets/hatch_build.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import subprocess
 import tempfile
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
 packages = [
-    ["@widgetti/solara-vuetify-app", "3.0.1"],
+    ["@widgetti/solara-vuetify-app", "4.0.0"],
     ["requirejs", "2.3.6"],
     ["mermaid", "8.6.4"],
     ["codemirror", "5.65.3"],
     ["vega", "5.21.0"],
     ["vega-lite", "5.2.0"],
     ["vega-embed", "6.20.2"],
     ["@widgetti/vue-grid-layout", "2.3.13-alpha.2"],
```

### Comparing `solara-1.8.2/packages/assets/pyproject.toml` & `solara-1.9.0/packages/assets/pyproject.toml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/pyproject.toml` & `solara-1.9.0/packages/solara-enterprise/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "Maarten A. Breddels", email = "maartenbreddels@gmail.com"},
     {name = "Mario Buikhuizen", email = "mariobuikhuizen@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: Free for non-commercial use"]
 dynamic = ["version", "description"]
 dependencies = [
-    "solara==1.8.2",
+    "solara==1.9.0",
 ]
 
 ssg = [
     "beautifulsoup4",
     "playwright; python_version > '3.6'",
 ]
```

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/base.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/base.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/disk.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/disk.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/memory_size.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/memory_size.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/multi_level.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/multi_level.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/cache/redis.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/cache/redis.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/index.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/index.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/search/search.vue` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/search/search.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-enterprise/solara_enterprise/ssg.py` & `solara-1.9.0/packages/solara-enterprise/solara_enterprise/ssg.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-milkdown/package-lock.json` & `solara-1.9.0/packages/solara-milkdown/package-lock.json`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-milkdown/package.json` & `solara-1.9.0/packages/solara-milkdown/package.json`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-milkdown/webpack.config.js` & `solara-1.9.0/packages/solara-milkdown/webpack.config.js`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-vuetify-app/package-lock.json` & `solara-1.9.0/packages/solara-vuetify-app/package-lock.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9148607705578593%*

 * *Differences: {"'dependencies'": "{'ajv-formats': {'requires': {replace: OrderedDict()}, 'dependencies': {'ajv': "*

 * *                   "{'version': 'https://registry.npmjs.org/ajv/-/ajv-8.11.2.tgz', 'optional': "*

 * *                   "True, 'peer': True, delete: ['resolved']}, 'json-schema-traverse': "*

 * *                   "{'optional': True, 'peer': True}}}, '@widgetti/solara-widget-manager8': "*

 * *                   "OrderedDict([('version', 'file:../solara-widget-manager8'), ('requires', "*

 * *                   "OrderedDict([('@ […]*

```diff
@@ -308,14 +308,51 @@
                 "typescript": "~4.1.3",
                 "url-loader": "^1.0.0",
                 "webpack": "^4.29.3",
                 "webpack-cli": "^3.2.3"
             },
             "version": "file:../solara-widget-manager"
         },
+        "@widgetti/solara-widget-manager8": {
+            "requires": {
+                "@babel/core": "^7.2.2",
+                "@babel/preset-env": "^7.3.1",
+                "@jupyter-widgets/base": "^6.0.1",
+                "@jupyter-widgets/controls": "^5.0.1",
+                "@jupyter-widgets/jupyterlab-manager": "^5.0.3",
+                "@jupyterlab/application": "^3.0.0",
+                "@jupyterlab/apputils": "^3.0.0",
+                "@jupyterlab/coreutils": "^5.0.0",
+                "@jupyterlab/docregistry": "^3.0.0",
+                "@jupyterlab/javascript-extension": "~3.0.0",
+                "@jupyterlab/notebook": "^3.0.0",
+                "@jupyterlab/outputarea": "^3.0.0",
+                "@jupyterlab/rendermime": "^3.0.0",
+                "@jupyterlab/services": "^6.1.8",
+                "@lumino/algorithm": "^1.3.3",
+                "@lumino/commands": "^1.12.0",
+                "@lumino/domutils": "^1.2.3",
+                "@lumino/messaging": "^1.4.3",
+                "@lumino/signaling": "^1.4.3",
+                "@lumino/virtualdom": "^1.8.0",
+                "@lumino/widgets": "^1.18.0",
+                "babel-loader": "^8.0.5",
+                "css-loader": "^5.0.0",
+                "file-loader": "^4.0.0",
+                "mathjax-full": "^3.0.0",
+                "npm-run-all": "^4.1.5",
+                "p-limit": "^2.2.2",
+                "style-loader": "^2.0.0",
+                "typescript": "~4.1.3",
+                "url-loader": "^1.0.0",
+                "webpack": "^4.29.3",
+                "webpack-cli": "^3.2.3"
+            },
+            "version": "file:../solara-widget-manager8"
+        },
         "@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "@xtuc/long": {
@@ -357,35 +394,36 @@
             "version": "1.0.1"
         },
         "ajv-formats": {
             "dependencies": {
                 "ajv": {
                     "dev": true,
                     "integrity": "sha512-E4bfmKAhGiSTvMfL1Myyycaub+cUEU2/IvpylXkUu7CHBkBj1f/ikdzbD7YQ6FKUbixDxeYvB/xY4fvyroDlQg==",
+                    "optional": true,
+                    "peer": true,
                     "requires": {
                         "fast-deep-equal": "^3.1.1",
                         "json-schema-traverse": "^1.0.0",
                         "require-from-string": "^2.0.2",
                         "uri-js": "^4.2.2"
                     },
-                    "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.11.2.tgz",
-                    "version": "8.11.2"
+                    "version": "https://registry.npmjs.org/ajv/-/ajv-8.11.2.tgz"
                 },
                 "json-schema-traverse": {
                     "dev": true,
                     "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
+                    "optional": true,
+                    "peer": true,
                     "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
                     "version": "1.0.0"
                 }
             },
             "dev": true,
             "integrity": "sha512-Wx0Kx52hxE7C18hkMEggYlEifqWZtYaRgouJor+WMdPnQyEK13vgEWyVNup7SoeeoLMsr4kf5h6dOW11I15MUA==",
-            "requires": {
-                "ajv": "^8.0.0"
-            },
+            "requires": {},
             "resolved": "https://registry.npmjs.org/ajv-formats/-/ajv-formats-2.1.1.tgz",
             "version": "2.1.1"
         },
         "ajv-keywords": {
             "dev": true,
             "integrity": "sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==",
             "requires": {},
@@ -1371,14 +1409,15 @@
     "name": "@widgetti/solara-vuetify-app",
     "packages": {
         "": {
             "dependencies": {
                 "@mariobuikhuizen/vue-compiler-addon": "^2.6.10-alpha.2",
                 "@mdi/font": "^4.9.95",
                 "@widgetti/solara-widget-manager": "file:../solara-widget-manager",
+                "@widgetti/solara-widget-manager8": "file:../solara-widget-manager8",
                 "material-design-icons-iconfont": "^5.0.1",
                 "typeface-roboto": "0.0.54",
                 "vue": "~2.6.14",
                 "vuetify": "~2.2.26"
             },
             "devDependencies": {
                 "css-loader": "^3.1.1",
@@ -1386,15 +1425,15 @@
                 "mini-css-extract-plugin": "^2.7.2",
                 "style-loader": "^0.23.1",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.10.0"
             },
             "license": "MIT",
             "name": "@widgetti/solara-vuetify-app",
-            "version": "2.1.0"
+            "version": "3.0.1"
         },
         "../solara-widget-manager": {
             "dependencies": {
                 "@jupyter-widgets/base": "^4.1.0",
                 "@jupyter-widgets/controls": "^3.1.0",
                 "@jupyter-widgets/jupyterlab-manager": "^3.1.0",
                 "@jupyterlab/application": "^3.0.0",
@@ -1427,15 +1466,55 @@
                 "typescript": "~4.1.3",
                 "url-loader": "^1.0.0",
                 "webpack": "^4.29.3",
                 "webpack-cli": "^3.2.3"
             },
             "license": "MIT",
             "name": "@widgetti/solara-widget-manager",
-            "version": "0.3.4"
+            "version": "0.4.0"
+        },
+        "../solara-widget-manager8": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.1",
+                "@jupyter-widgets/controls": "^5.0.1",
+                "@jupyter-widgets/jupyterlab-manager": "^5.0.3",
+                "@jupyterlab/application": "^3.0.0",
+                "@jupyterlab/apputils": "^3.0.0",
+                "@jupyterlab/coreutils": "^5.0.0",
+                "@jupyterlab/docregistry": "^3.0.0",
+                "@jupyterlab/javascript-extension": "~3.0.0",
+                "@jupyterlab/notebook": "^3.0.0",
+                "@jupyterlab/outputarea": "^3.0.0",
+                "@jupyterlab/rendermime": "^3.0.0",
+                "@jupyterlab/services": "^6.1.8",
+                "@lumino/algorithm": "^1.3.3",
+                "@lumino/commands": "^1.12.0",
+                "@lumino/domutils": "^1.2.3",
+                "@lumino/messaging": "^1.4.3",
+                "@lumino/signaling": "^1.4.3",
+                "@lumino/virtualdom": "^1.8.0",
+                "@lumino/widgets": "^1.18.0",
+                "mathjax-full": "^3.0.0"
+            },
+            "devDependencies": {
+                "@babel/core": "^7.2.2",
+                "@babel/preset-env": "^7.3.1",
+                "babel-loader": "^8.0.5",
+                "css-loader": "^5.0.0",
+                "file-loader": "^4.0.0",
+                "npm-run-all": "^4.1.5",
+                "p-limit": "^2.2.2",
+                "style-loader": "^2.0.0",
+                "typescript": "~4.1.3",
+                "url-loader": "^1.0.0",
+                "webpack": "^4.29.3",
+                "webpack-cli": "^3.2.3"
+            },
+            "license": "MIT",
+            "version": "0.4.0"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -1733,14 +1812,18 @@
             "resolved": "https://registry.npmjs.org/@webpack-cli/serve/-/serve-1.7.0.tgz",
             "version": "1.7.0"
         },
         "node_modules/@widgetti/solara-widget-manager": {
             "link": true,
             "resolved": "../solara-widget-manager"
         },
+        "node_modules/@widgetti/solara-widget-manager8": {
+            "link": true,
+            "resolved": "../solara-widget-manager8"
+        },
         "node_modules/@xtuc/ieee754": {
             "dev": true,
             "integrity": "sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==",
             "resolved": "https://registry.npmjs.org/@xtuc/ieee754/-/ieee754-1.2.0.tgz",
             "version": "1.2.0"
         },
         "node_modules/@xtuc/long": {
@@ -1821,20 +1904,24 @@
             },
             "dev": true,
             "funding": {
                 "type": "github",
                 "url": "https://github.com/sponsors/epoberezkin"
             },
             "integrity": "sha512-E4bfmKAhGiSTvMfL1Myyycaub+cUEU2/IvpylXkUu7CHBkBj1f/ikdzbD7YQ6FKUbixDxeYvB/xY4fvyroDlQg==",
+            "optional": true,
+            "peer": true,
             "resolved": "https://registry.npmjs.org/ajv/-/ajv-8.11.2.tgz",
             "version": "8.11.2"
         },
         "node_modules/ajv-formats/node_modules/json-schema-traverse": {
             "dev": true,
             "integrity": "sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==",
+            "optional": true,
+            "peer": true,
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-1.0.0.tgz",
             "version": "1.0.0"
         },
         "node_modules/ajv-keywords": {
             "dev": true,
             "integrity": "sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==",
             "peerDependencies": {
@@ -3226,9 +3313,9 @@
             "dev": true,
             "integrity": "sha512-JcKqAHLPxcdb9KM49dufGXn2x3ssnfjbcaQdLlfZsL9rH9wgDQjUtDxbo8NE0F6SFvydeu1VhZe7hZuHsB2/pw==",
             "resolved": "https://registry.npmjs.org/wildcard/-/wildcard-2.0.0.tgz",
             "version": "2.0.0"
         }
     },
     "requires": true,
-    "version": "2.1.0"
+    "version": "3.0.1"
 }
```

### Comparing `solara-1.8.2/packages/solara-vuetify-app/package.json` & `solara-1.9.0/packages/solara-vuetify-app/package.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9305555555555556%*

 * *Differences: {"'dependencies'": "{'@widgetti/solara-widget-manager8': 'file:../solara-widget-manager8'}",*

 * * "'scripts'": '{\'devlink\': \'TARGET_DIR=`python -c "import sys; '*

 * *              'print(sys.prefix)"`/share/solara/cdn/@widgetti/solara-vuetify-app@4.0.0/; mkdir -p '*

 * *              "$TARGET_DIR && rm -rf $TARGET_DIR/dist && ln -sf $PWD/dist $TARGET_DIR/dist'}",*

 * * "'version'": "'4.0.0'"}*

```diff
@@ -1,13 +1,14 @@
 {
     "author": "",
     "dependencies": {
         "@mariobuikhuizen/vue-compiler-addon": "^2.6.10-alpha.2",
         "@mdi/font": "^4.9.95",
         "@widgetti/solara-widget-manager": "file:../solara-widget-manager",
+        "@widgetti/solara-widget-manager8": "file:../solara-widget-manager8",
         "material-design-icons-iconfont": "^5.0.1",
         "typeface-roboto": "0.0.54",
         "vue": "~2.6.14",
         "vuetify": "~2.2.26"
     },
     "description": "Solara Vuetify App",
     "devDependencies": {
@@ -19,13 +20,13 @@
         "webpack-cli": "^4.10.0"
     },
     "license": "MIT",
     "main": "dist/solara-vuetify-app.js",
     "name": "@widgetti/solara-vuetify-app",
     "scripts": {
         "build": "webpack",
-        "devlink": "TARGET_DIR=`python -c \"import sys; print(sys.prefix)\"`/share/solara/cdn/@widgetti/solara-vuetify-app@3.0.1/; mkdir -p $TARGET_DIR && rm -rf $TARGET_DIR/dist && ln -sf $PWD/dist $TARGET_DIR/dist",
+        "devlink": "TARGET_DIR=`python -c \"import sys; print(sys.prefix)\"`/share/solara/cdn/@widgetti/solara-vuetify-app@4.0.0/; mkdir -p $TARGET_DIR && rm -rf $TARGET_DIR/dist && ln -sf $PWD/dist $TARGET_DIR/dist",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "3.0.1"
+    "version": "4.0.0"
 }
```

### Comparing `solara-1.8.2/packages/solara-widget-manager/LICENSE.voila.txt` & `solara-1.9.0/packages/solara-widget-manager/LICENSE.voila.txt`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/package-lock.json` & `solara-1.9.0/packages/solara-widget-manager/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9135586186620324%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': {'version': '4.1.2', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@jupyter-widgets/base/-/base-4.1.2.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-URaQ6rUR0ZC1G1g0pSZHcV8W9x5pK/FnC/zSF5/i2QHmjLVfwVRBFt7a8VL88xZG8V4G8tOIDZTTg1NZcHfB0A=='}, "*

 * *                   "'@jupyter-widgets/controls': {'version': '3.1.2', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-3.1.2.tgz', "*

 * * […]*

```diff
@@ -1206,46 +1206,185 @@
         },
         "@juggle/resize-observer": {
             "integrity": "sha512-zMM9Ds+SawiUkakS7y94Ymqx+S0ORzpG3frZirN3l+UlXUmSUR7hF4wxCVqW+ei94JzV5kt0uXBcoOEAuiydrw==",
             "resolved": "https://registry.npmjs.org/@juggle/resize-observer/-/resize-observer-3.3.1.tgz",
             "version": "3.3.1"
         },
         "@jupyter-widgets/base": {
-            "integrity": "sha512-bw3Qib1FbUaRXjXol0HcjzYnKzEvmevGXyXjxIiVXGIG43cwMipFLwL9mPa7RWUim/5u1H+XzGdWpfyNj4zdDA==",
+            "integrity": "sha512-URaQ6rUR0ZC1G1g0pSZHcV8W9x5pK/FnC/zSF5/i2QHmjLVfwVRBFt7a8VL88xZG8V4G8tOIDZTTg1NZcHfB0A==",
             "requires": {
                 "@jupyterlab/services": "^6.0.0",
                 "@lumino/coreutils": "^1.2.0",
                 "@lumino/messaging": "^1.2.1",
                 "@lumino/widgets": "^1.3.0",
                 "@types/backbone": "^1.4.1",
                 "@types/lodash": "^4.14.134",
                 "backbone": "1.2.3",
                 "base64-js": "^1.2.1",
                 "jquery": "^3.1.1",
                 "lodash": "^4.17.4"
             },
-            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-4.1.1.tgz",
-            "version": "4.1.1"
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-4.1.2.tgz",
+            "version": "4.1.2"
+        },
+        "@jupyter-widgets/base-manager": {
+            "dependencies": {
+                "@jupyter-widgets/base": {
+                    "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+                    "requires": {
+                        "@jupyterlab/services": "^6.0.0",
+                        "@lumino/coreutils": "^1.11.1",
+                        "@lumino/messaging": "^1.10.1",
+                        "@lumino/widgets": "^1.30.0",
+                        "@types/backbone": "1.4.14",
+                        "@types/lodash": "^4.14.134",
+                        "backbone": "1.4.0",
+                        "jquery": "^3.1.1",
+                        "lodash": "^4.17.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+                    "version": "6.0.2"
+                },
+                "@types/backbone": {
+                    "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+                    "requires": {
+                        "@types/jquery": "*",
+                        "@types/underscore": "*"
+                    },
+                    "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+                    "version": "1.4.14"
+                },
+                "backbone": {
+                    "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+                    "requires": {
+                        "underscore": ">=1.8.3"
+                    },
+                    "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+                    "version": "1.4.0"
+                }
+            },
+            "integrity": "sha512-u/SfuOGc1Z3OUOj/hCNXzS/OWfk6jrrrqRYAhVXiIEJqvql0Nd6fGW/zHxZB+FpqG5I5DzZzBNI20H+4mB+TGQ==",
+            "requires": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "base64-js": "^1.2.1",
+                "sanitize-html": "^2.3"
+            },
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base-manager/-/base-manager-1.0.3.tgz",
+            "version": "1.0.3"
+        },
+        "@jupyter-widgets/base8": {
+            "dependencies": {
+                "@types/backbone": {
+                    "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+                    "requires": {
+                        "@types/jquery": "*",
+                        "@types/underscore": "*"
+                    },
+                    "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+                    "version": "1.4.14"
+                },
+                "backbone": {
+                    "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+                    "requires": {
+                        "underscore": ">=1.8.3"
+                    },
+                    "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+                    "version": "1.4.0"
+                }
+            },
+            "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+            "requires": {
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "@types/lodash": "^4.14.134",
+                "backbone": "1.4.0",
+                "jquery": "^3.1.1",
+                "lodash": "^4.17.4"
+            },
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+            "version": "npm:@jupyter-widgets/base@6.0.2"
         },
         "@jupyter-widgets/controls": {
-            "integrity": "sha512-zo+LZYqn/rIQc9o9TiPO5WX8n7g/jN8eFCwP0tjg6tRfv5Tl/uvdcByv1pIyFm/qB5fsn6k01NKrAc6NlKh2SQ==",
+            "integrity": "sha512-uxRfsuS5F2IJgG4o+jJqqrVtRuOItS1vTExK8GBXr/iljTyQ57qSGcCKZ67qXYi6L/t/RYDr9Fohyu0eWV3Zyg==",
             "requires": {
-                "@jupyter-widgets/base": "^4.1.1",
+                "@jupyter-widgets/base": "^4.1.2",
                 "@lumino/algorithm": "^1.1.0",
                 "@lumino/domutils": "^1.1.0",
                 "@lumino/messaging": "^1.2.1",
                 "@lumino/signaling": "^1.2.0",
                 "@lumino/widgets": "^1.3.0",
                 "d3-format": "^1.3.0",
                 "jquery": "^3.1.1",
                 "jquery-ui": "^1.12.1",
                 "underscore": "^1.8.3"
             },
-            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-3.1.1.tgz",
-            "version": "3.1.1"
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-3.1.2.tgz",
+            "version": "3.1.2"
+        },
+        "@jupyter-widgets/controls8": {
+            "dependencies": {
+                "@jupyter-widgets/base": {
+                    "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+                    "requires": {
+                        "@jupyterlab/services": "^6.0.0",
+                        "@lumino/coreutils": "^1.11.1",
+                        "@lumino/messaging": "^1.10.1",
+                        "@lumino/widgets": "^1.30.0",
+                        "@types/backbone": "1.4.14",
+                        "@types/lodash": "^4.14.134",
+                        "backbone": "1.4.0",
+                        "jquery": "^3.1.1",
+                        "lodash": "^4.17.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+                    "version": "6.0.2"
+                },
+                "@types/backbone": {
+                    "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+                    "requires": {
+                        "@types/jquery": "*",
+                        "@types/underscore": "*"
+                    },
+                    "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+                    "version": "1.4.14"
+                },
+                "backbone": {
+                    "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+                    "requires": {
+                        "underscore": ">=1.8.3"
+                    },
+                    "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+                    "version": "1.4.0"
+                },
+                "d3-format": {
+                    "integrity": "sha512-YyUI6AEuY/Wpt8KWLgZHsIU86atmikuoOmCfommt0LYHiQSPjvX2AcFc38PX0CBpr2RCyZhjex+NS/LPOv6YqA==",
+                    "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-3.1.0.tgz",
+                    "version": "3.1.0"
+                }
+            },
+            "integrity": "sha512-IVPGC+yLDEiFD7YzdSrn/dLNlpQJ4fcsikT2ksw3Vemc7d+CJ9N/uPM6yNMSVcsMCuMuC8LB6T/ecl2STcXaQQ==",
+            "requires": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@lumino/algorithm": "^1.9.1",
+                "@lumino/domutils": "^1.8.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/signaling": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "d3-color": "^3.0.1",
+                "d3-format": "^3.0.1",
+                "jquery": "^3.1.1",
+                "nouislider": "15.4.0"
+            },
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-5.0.3.tgz",
+            "version": "npm:@jupyter-widgets/controls@5.0.3"
         },
         "@jupyter-widgets/jupyterlab-manager": {
             "integrity": "sha512-whjFC46lteMtF5l2f6nmOArUYiFHTgB7Ymtod2+zwBYRIjG4eN0euEqJvqvrfDy2IQaclddhIYXCem3NxeNUwA==",
             "requires": {
                 "@jupyter-widgets/base": "^4.1.1",
                 "@jupyter-widgets/controls": "^3.1.1",
                 "@jupyter-widgets/output": "^4.1.1",
@@ -1270,14 +1409,132 @@
                 "@types/backbone": "^1.4.1",
                 "jquery": "^3.1.1",
                 "semver": "^6.1.1"
             },
             "resolved": "https://registry.npmjs.org/@jupyter-widgets/jupyterlab-manager/-/jupyterlab-manager-3.1.1.tgz",
             "version": "3.1.1"
         },
+        "@jupyter-widgets/jupyterlab-manager8": {
+            "dependencies": {
+                "@jupyter-widgets/base": {
+                    "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+                    "requires": {
+                        "@jupyterlab/services": "^6.0.0",
+                        "@lumino/coreutils": "^1.11.1",
+                        "@lumino/messaging": "^1.10.1",
+                        "@lumino/widgets": "^1.30.0",
+                        "@types/backbone": "1.4.14",
+                        "@types/lodash": "^4.14.134",
+                        "backbone": "1.4.0",
+                        "jquery": "^3.1.1",
+                        "lodash": "^4.17.4"
+                    },
+                    "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+                    "version": "6.0.2"
+                },
+                "@jupyter-widgets/controls": {
+                    "integrity": "sha512-IVPGC+yLDEiFD7YzdSrn/dLNlpQJ4fcsikT2ksw3Vemc7d+CJ9N/uPM6yNMSVcsMCuMuC8LB6T/ecl2STcXaQQ==",
+                    "requires": {
+                        "@jupyter-widgets/base": "^6.0.2",
+                        "@lumino/algorithm": "^1.9.1",
+                        "@lumino/domutils": "^1.8.1",
+                        "@lumino/messaging": "^1.10.1",
+                        "@lumino/signaling": "^1.10.1",
+                        "@lumino/widgets": "^1.30.0",
+                        "d3-color": "^3.0.1",
+                        "d3-format": "^3.0.1",
+                        "jquery": "^3.1.1",
+                        "nouislider": "15.4.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-5.0.3.tgz",
+                    "version": "5.0.3"
+                },
+                "@jupyter-widgets/output": {
+                    "integrity": "sha512-S2AP3ffJTOo1j8oXAa/NPg1uH3GXw6i8GbsQVPiQcolOnBG+M6mDJWQFUpMblu7FdfXy9K9Qdf2cpv8m67krRA==",
+                    "requires": {
+                        "@jupyter-widgets/base": "^6.0.2"
+                    },
+                    "resolved": "https://registry.npmjs.org/@jupyter-widgets/output/-/output-6.0.2.tgz",
+                    "version": "6.0.2"
+                },
+                "@types/backbone": {
+                    "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+                    "requires": {
+                        "@types/jquery": "*",
+                        "@types/underscore": "*"
+                    },
+                    "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+                    "version": "1.4.14"
+                },
+                "backbone": {
+                    "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+                    "requires": {
+                        "underscore": ">=1.8.3"
+                    },
+                    "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+                    "version": "1.4.0"
+                },
+                "d3-format": {
+                    "integrity": "sha512-YyUI6AEuY/Wpt8KWLgZHsIU86atmikuoOmCfommt0LYHiQSPjvX2AcFc38PX0CBpr2RCyZhjex+NS/LPOv6YqA==",
+                    "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-3.1.0.tgz",
+                    "version": "3.1.0"
+                },
+                "lru-cache": {
+                    "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
+                    "requires": {
+                        "yallist": "^4.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
+                    "version": "6.0.0"
+                },
+                "semver": {
+                    "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
+                    "requires": {
+                        "lru-cache": "^6.0.0"
+                    },
+                    "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
+                    "version": "7.3.8"
+                },
+                "yallist": {
+                    "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
+                    "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
+                    "version": "4.0.0"
+                }
+            },
+            "integrity": "sha512-EJMcF/GedUkhVzonQJqSnenOiL8UahXede62mO79pqVlZuzVez6wJRgP3Zlkia8mqiuuF560dtI7Y0Txy4MEGQ==",
+            "requires": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@jupyter-widgets/base-manager": "^1.0.3",
+                "@jupyter-widgets/controls": "^5.0.3",
+                "@jupyter-widgets/output": "^6.0.2",
+                "@jupyterlab/application": "^3.0.0",
+                "@jupyterlab/docregistry": "^3.0.0",
+                "@jupyterlab/logconsole": "^3.0.0",
+                "@jupyterlab/mainmenu": "^3.0.0",
+                "@jupyterlab/nbformat": "^3.0.0",
+                "@jupyterlab/notebook": "^3.0.0",
+                "@jupyterlab/outputarea": "^3.0.0",
+                "@jupyterlab/rendermime": "^3.0.0",
+                "@jupyterlab/rendermime-interfaces": "^3.0.0",
+                "@jupyterlab/services": "^6.0.0",
+                "@jupyterlab/settingregistry": "^3.0.0",
+                "@jupyterlab/translation": "^3.0.0",
+                "@lumino/algorithm": "^1.9.1",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/disposable": "^1.10.1",
+                "@lumino/properties": "^1.8.1",
+                "@lumino/signaling": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "jquery": "^3.1.1",
+                "semver": "^7.3.5"
+            },
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/jupyterlab-manager/-/jupyterlab-manager-5.0.5.tgz",
+            "version": "npm:@jupyter-widgets/jupyterlab-manager@5.0.5"
+        },
         "@jupyter-widgets/output": {
             "integrity": "sha512-XYNabDT3MtPGNAx1yLFYHn9mJTqGWqRRsejyJkv1KrAlUhJJQTJwvoBInP2OdaGAUMk8n6pE16qzzQcCS1+Qog==",
             "requires": {
                 "@jupyter-widgets/base": "^4.1.1"
             },
             "resolved": "https://registry.npmjs.org/@jupyter-widgets/output/-/output-4.1.1.tgz",
             "version": "4.1.1"
@@ -1775,15 +2032,14 @@
                 "@lumino/commands": "^1.19.0",
                 "@lumino/coreutils": "^1.11.0",
                 "@lumino/disposable": "^1.10.0",
                 "@lumino/signaling": "^1.10.0",
                 "@lumino/virtualdom": "^1.14.0",
                 "@lumino/widgets": "^1.33.0",
                 "@rjsf/core": "^3.1.0",
-                "react": "^17.0.1",
                 "react-dom": "^17.0.1",
                 "typestyle": "^2.0.4"
             },
             "resolved": "https://registry.npmjs.org/@jupyterlab/ui-components/-/ui-components-3.4.5.tgz",
             "version": "3.4.5"
         },
         "@lumino/algorithm": {
@@ -3240,14 +3496,19 @@
         },
         "cyclist": {
             "dev": true,
             "integrity": "sha512-NJGVKPS81XejHcLhaLJS7plab0fK3slPh11mESeeDq2W4ZI5kUKK/LRRdVDvjJseojbPB7ZwjnyOybg3Igea/A==",
             "resolved": "https://registry.npmjs.org/cyclist/-/cyclist-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "d3-color": {
+            "integrity": "sha512-zg/chbXyeBtMQ1LbD/WSoW2DpC3I0mpmPdW+ynRTj/x2DAWYrIY7qeZIHidozwV24m4iavr15lNwIwLxRmOxhA==",
+            "resolved": "https://registry.npmjs.org/d3-color/-/d3-color-3.1.0.tgz",
+            "version": "3.1.0"
+        },
         "d3-format": {
             "integrity": "sha512-J0piedu6Z8iB6TbIGfZgDzfXxUFN3qQRMofy2oPdXzQibYGqPB/9iMcxr/TGalU+2RsyDO+U4f33id8tbnSRMQ==",
             "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-1.4.5.tgz",
             "version": "1.4.5"
         },
         "debug": {
             "dev": true,
@@ -5308,14 +5569,19 @@
             "version": "3.0.0"
         },
         "normalize.css": {
             "integrity": "sha512-qizSNPO93t1YUuUhP22btGOo3chcvDFqFaj2TRybP0DMxkHOCTYwp3n34fel4a31ORXy4m1Xq0Gyqpb5m33qIg==",
             "resolved": "https://registry.npmjs.org/normalize.css/-/normalize.css-8.0.1.tgz",
             "version": "8.0.1"
         },
+        "nouislider": {
+            "integrity": "sha512-AV7UMhGhZ4Mj6ToMT812Ib8OJ4tAXR2/Um7C4l4ZvvsqujF0WpQTpqqHJ+9xt4174R7ueQOUrBR4yakJpAIPCA==",
+            "resolved": "https://registry.npmjs.org/nouislider/-/nouislider-15.4.0.tgz",
+            "version": "15.4.0"
+        },
         "npm-run-all": {
             "dev": true,
             "integrity": "sha512-Oo82gJDAVcaMdi3nuoKFavkIHBRVqQ1qvMb+9LHk/cF4P6B2m8aP04hGf7oL6wZ9BuGwX1onlLhpuoofSyoQDQ==",
             "requires": {
                 "ansi-styles": "^3.2.1",
                 "chalk": "^2.4.1",
                 "cross-spawn": "^6.0.5",
@@ -7906,17 +8172,20 @@
         }
     },
     "lockfileVersion": 2,
     "name": "@widgetti/solara-widget-manager",
     "packages": {
         "": {
             "dependencies": {
-                "@jupyter-widgets/base": "^4.1.0",
-                "@jupyter-widgets/controls": "^3.1.0",
+                "@jupyter-widgets/base": "^4.1.2",
+                "@jupyter-widgets/base8": "npm:@jupyter-widgets/base@^6.0.1",
+                "@jupyter-widgets/controls": "^3.1.2",
+                "@jupyter-widgets/controls8": "npm:@jupyter-widgets/controls@^5.0.1",
                 "@jupyter-widgets/jupyterlab-manager": "^3.1.0",
+                "@jupyter-widgets/jupyterlab-manager8": "npm:@jupyter-widgets/jupyterlab-manager@^5.0.3",
                 "@jupyterlab/application": "^3.0.0",
                 "@jupyterlab/apputils": "^3.0.0",
                 "@jupyterlab/coreutils": "^5.0.0",
                 "@jupyterlab/docregistry": "^3.0.0",
                 "@jupyterlab/javascript-extension": "~3.0.0",
                 "@jupyterlab/notebook": "^3.0.0",
                 "@jupyterlab/outputarea": "^3.0.0",
@@ -7943,15 +8212,15 @@
                 "typescript": "~4.1.3",
                 "url-loader": "^1.0.0",
                 "webpack": "^4.29.3",
                 "webpack-cli": "^3.2.3"
             },
             "license": "MIT",
             "name": "@widgetti/solara-widget-manager",
-            "version": "0.3.4"
+            "version": "0.4.0"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.1.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
@@ -9684,34 +9953,172 @@
                 "@types/backbone": "^1.4.1",
                 "@types/lodash": "^4.14.134",
                 "backbone": "1.2.3",
                 "base64-js": "^1.2.1",
                 "jquery": "^3.1.1",
                 "lodash": "^4.17.4"
             },
-            "integrity": "sha512-bw3Qib1FbUaRXjXol0HcjzYnKzEvmevGXyXjxIiVXGIG43cwMipFLwL9mPa7RWUim/5u1H+XzGdWpfyNj4zdDA==",
-            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-4.1.1.tgz",
-            "version": "4.1.1"
+            "integrity": "sha512-URaQ6rUR0ZC1G1g0pSZHcV8W9x5pK/FnC/zSF5/i2QHmjLVfwVRBFt7a8VL88xZG8V4G8tOIDZTTg1NZcHfB0A==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-4.1.2.tgz",
+            "version": "4.1.2"
+        },
+        "node_modules/@jupyter-widgets/base-manager": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "base64-js": "^1.2.1",
+                "sanitize-html": "^2.3"
+            },
+            "integrity": "sha512-u/SfuOGc1Z3OUOj/hCNXzS/OWfk6jrrrqRYAhVXiIEJqvql0Nd6fGW/zHxZB+FpqG5I5DzZzBNI20H+4mB+TGQ==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base-manager/-/base-manager-1.0.3.tgz",
+            "version": "1.0.3"
+        },
+        "node_modules/@jupyter-widgets/base-manager/node_modules/@jupyter-widgets/base": {
+            "dependencies": {
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "@types/lodash": "^4.14.134",
+                "backbone": "1.4.0",
+                "jquery": "^3.1.1",
+                "lodash": "^4.17.4"
+            },
+            "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+            "version": "6.0.2"
+        },
+        "node_modules/@jupyter-widgets/base-manager/node_modules/@types/backbone": {
+            "dependencies": {
+                "@types/jquery": "*",
+                "@types/underscore": "*"
+            },
+            "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+            "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+            "version": "1.4.14"
+        },
+        "node_modules/@jupyter-widgets/base-manager/node_modules/backbone": {
+            "dependencies": {
+                "underscore": ">=1.8.3"
+            },
+            "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+            "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+            "version": "1.4.0"
+        },
+        "node_modules/@jupyter-widgets/base8": {
+            "dependencies": {
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "@types/lodash": "^4.14.134",
+                "backbone": "1.4.0",
+                "jquery": "^3.1.1",
+                "lodash": "^4.17.4"
+            },
+            "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+            "name": "@jupyter-widgets/base",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+            "version": "6.0.2"
+        },
+        "node_modules/@jupyter-widgets/base8/node_modules/@types/backbone": {
+            "dependencies": {
+                "@types/jquery": "*",
+                "@types/underscore": "*"
+            },
+            "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+            "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+            "version": "1.4.14"
+        },
+        "node_modules/@jupyter-widgets/base8/node_modules/backbone": {
+            "dependencies": {
+                "underscore": ">=1.8.3"
+            },
+            "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+            "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+            "version": "1.4.0"
         },
         "node_modules/@jupyter-widgets/controls": {
             "dependencies": {
-                "@jupyter-widgets/base": "^4.1.1",
+                "@jupyter-widgets/base": "^4.1.2",
                 "@lumino/algorithm": "^1.1.0",
                 "@lumino/domutils": "^1.1.0",
                 "@lumino/messaging": "^1.2.1",
                 "@lumino/signaling": "^1.2.0",
                 "@lumino/widgets": "^1.3.0",
                 "d3-format": "^1.3.0",
                 "jquery": "^3.1.1",
                 "jquery-ui": "^1.12.1",
                 "underscore": "^1.8.3"
             },
-            "integrity": "sha512-zo+LZYqn/rIQc9o9TiPO5WX8n7g/jN8eFCwP0tjg6tRfv5Tl/uvdcByv1pIyFm/qB5fsn6k01NKrAc6NlKh2SQ==",
-            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-3.1.1.tgz",
-            "version": "3.1.1"
+            "integrity": "sha512-uxRfsuS5F2IJgG4o+jJqqrVtRuOItS1vTExK8GBXr/iljTyQ57qSGcCKZ67qXYi6L/t/RYDr9Fohyu0eWV3Zyg==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-3.1.2.tgz",
+            "version": "3.1.2"
+        },
+        "node_modules/@jupyter-widgets/controls8": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@lumino/algorithm": "^1.9.1",
+                "@lumino/domutils": "^1.8.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/signaling": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "d3-color": "^3.0.1",
+                "d3-format": "^3.0.1",
+                "jquery": "^3.1.1",
+                "nouislider": "15.4.0"
+            },
+            "integrity": "sha512-IVPGC+yLDEiFD7YzdSrn/dLNlpQJ4fcsikT2ksw3Vemc7d+CJ9N/uPM6yNMSVcsMCuMuC8LB6T/ecl2STcXaQQ==",
+            "name": "@jupyter-widgets/controls",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-5.0.3.tgz",
+            "version": "5.0.3"
+        },
+        "node_modules/@jupyter-widgets/controls8/node_modules/@jupyter-widgets/base": {
+            "dependencies": {
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "@types/lodash": "^4.14.134",
+                "backbone": "1.4.0",
+                "jquery": "^3.1.1",
+                "lodash": "^4.17.4"
+            },
+            "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+            "version": "6.0.2"
+        },
+        "node_modules/@jupyter-widgets/controls8/node_modules/@types/backbone": {
+            "dependencies": {
+                "@types/jquery": "*",
+                "@types/underscore": "*"
+            },
+            "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+            "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+            "version": "1.4.14"
+        },
+        "node_modules/@jupyter-widgets/controls8/node_modules/backbone": {
+            "dependencies": {
+                "underscore": ">=1.8.3"
+            },
+            "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+            "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+            "version": "1.4.0"
+        },
+        "node_modules/@jupyter-widgets/controls8/node_modules/d3-format": {
+            "engines": {
+                "node": ">=12"
+            },
+            "integrity": "sha512-YyUI6AEuY/Wpt8KWLgZHsIU86atmikuoOmCfommt0LYHiQSPjvX2AcFc38PX0CBpr2RCyZhjex+NS/LPOv6YqA==",
+            "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-3.1.0.tgz",
+            "version": "3.1.0"
         },
         "node_modules/@jupyter-widgets/jupyterlab-manager": {
             "dependencies": {
                 "@jupyter-widgets/base": "^4.1.1",
                 "@jupyter-widgets/controls": "^3.1.1",
                 "@jupyter-widgets/output": "^4.1.1",
                 "@jupyterlab/application": "^3.0.0",
@@ -9736,14 +10143,143 @@
                 "jquery": "^3.1.1",
                 "semver": "^6.1.1"
             },
             "integrity": "sha512-whjFC46lteMtF5l2f6nmOArUYiFHTgB7Ymtod2+zwBYRIjG4eN0euEqJvqvrfDy2IQaclddhIYXCem3NxeNUwA==",
             "resolved": "https://registry.npmjs.org/@jupyter-widgets/jupyterlab-manager/-/jupyterlab-manager-3.1.1.tgz",
             "version": "3.1.1"
         },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@jupyter-widgets/base-manager": "^1.0.3",
+                "@jupyter-widgets/controls": "^5.0.3",
+                "@jupyter-widgets/output": "^6.0.2",
+                "@jupyterlab/application": "^3.0.0",
+                "@jupyterlab/docregistry": "^3.0.0",
+                "@jupyterlab/logconsole": "^3.0.0",
+                "@jupyterlab/mainmenu": "^3.0.0",
+                "@jupyterlab/nbformat": "^3.0.0",
+                "@jupyterlab/notebook": "^3.0.0",
+                "@jupyterlab/outputarea": "^3.0.0",
+                "@jupyterlab/rendermime": "^3.0.0",
+                "@jupyterlab/rendermime-interfaces": "^3.0.0",
+                "@jupyterlab/services": "^6.0.0",
+                "@jupyterlab/settingregistry": "^3.0.0",
+                "@jupyterlab/translation": "^3.0.0",
+                "@lumino/algorithm": "^1.9.1",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/disposable": "^1.10.1",
+                "@lumino/properties": "^1.8.1",
+                "@lumino/signaling": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "jquery": "^3.1.1",
+                "semver": "^7.3.5"
+            },
+            "integrity": "sha512-EJMcF/GedUkhVzonQJqSnenOiL8UahXede62mO79pqVlZuzVez6wJRgP3Zlkia8mqiuuF560dtI7Y0Txy4MEGQ==",
+            "name": "@jupyter-widgets/jupyterlab-manager",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/jupyterlab-manager/-/jupyterlab-manager-5.0.5.tgz",
+            "version": "5.0.5"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/@jupyter-widgets/base": {
+            "dependencies": {
+                "@jupyterlab/services": "^6.0.0",
+                "@lumino/coreutils": "^1.11.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "@types/backbone": "1.4.14",
+                "@types/lodash": "^4.14.134",
+                "backbone": "1.4.0",
+                "jquery": "^3.1.1",
+                "lodash": "^4.17.4"
+            },
+            "integrity": "sha512-CIVjSTrqQFzkg9VCdDjrjDqwbba3eZfNigCPFSuKmMVXc+ATAOFczOv9/9uaCPzQ+E+0g6SOLhJ25SpKB0cl9g==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/base/-/base-6.0.2.tgz",
+            "version": "6.0.2"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/@jupyter-widgets/controls": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.2",
+                "@lumino/algorithm": "^1.9.1",
+                "@lumino/domutils": "^1.8.1",
+                "@lumino/messaging": "^1.10.1",
+                "@lumino/signaling": "^1.10.1",
+                "@lumino/widgets": "^1.30.0",
+                "d3-color": "^3.0.1",
+                "d3-format": "^3.0.1",
+                "jquery": "^3.1.1",
+                "nouislider": "15.4.0"
+            },
+            "integrity": "sha512-IVPGC+yLDEiFD7YzdSrn/dLNlpQJ4fcsikT2ksw3Vemc7d+CJ9N/uPM6yNMSVcsMCuMuC8LB6T/ecl2STcXaQQ==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/controls/-/controls-5.0.3.tgz",
+            "version": "5.0.3"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/@jupyter-widgets/output": {
+            "dependencies": {
+                "@jupyter-widgets/base": "^6.0.2"
+            },
+            "integrity": "sha512-S2AP3ffJTOo1j8oXAa/NPg1uH3GXw6i8GbsQVPiQcolOnBG+M6mDJWQFUpMblu7FdfXy9K9Qdf2cpv8m67krRA==",
+            "resolved": "https://registry.npmjs.org/@jupyter-widgets/output/-/output-6.0.2.tgz",
+            "version": "6.0.2"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/@types/backbone": {
+            "dependencies": {
+                "@types/jquery": "*",
+                "@types/underscore": "*"
+            },
+            "integrity": "sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==",
+            "resolved": "https://registry.npmjs.org/@types/backbone/-/backbone-1.4.14.tgz",
+            "version": "1.4.14"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/backbone": {
+            "dependencies": {
+                "underscore": ">=1.8.3"
+            },
+            "integrity": "sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==",
+            "resolved": "https://registry.npmjs.org/backbone/-/backbone-1.4.0.tgz",
+            "version": "1.4.0"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/d3-format": {
+            "engines": {
+                "node": ">=12"
+            },
+            "integrity": "sha512-YyUI6AEuY/Wpt8KWLgZHsIU86atmikuoOmCfommt0LYHiQSPjvX2AcFc38PX0CBpr2RCyZhjex+NS/LPOv6YqA==",
+            "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-3.1.0.tgz",
+            "version": "3.1.0"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/lru-cache": {
+            "dependencies": {
+                "yallist": "^4.0.0"
+            },
+            "engines": {
+                "node": ">=10"
+            },
+            "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
+            "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
+            "version": "6.0.0"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/semver": {
+            "bin": {
+                "semver": "bin/semver.js"
+            },
+            "dependencies": {
+                "lru-cache": "^6.0.0"
+            },
+            "engines": {
+                "node": ">=10"
+            },
+            "integrity": "sha512-NB1ctGL5rlHrPJtFDVIVzTyQylMLu9N9VICA6HSFJo8MCGVTMW6gfpicwKmmK/dAjTOrqu5l63JJOpDSrAis3A==",
+            "resolved": "https://registry.npmjs.org/semver/-/semver-7.3.8.tgz",
+            "version": "7.3.8"
+        },
+        "node_modules/@jupyter-widgets/jupyterlab-manager8/node_modules/yallist": {
+            "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
+            "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
+            "version": "4.0.0"
+        },
         "node_modules/@jupyter-widgets/output": {
             "dependencies": {
                 "@jupyter-widgets/base": "^4.1.1"
             },
             "integrity": "sha512-XYNabDT3MtPGNAx1yLFYHn9mJTqGWqRRsejyJkv1KrAlUhJJQTJwvoBInP2OdaGAUMk8n6pE16qzzQcCS1+Qog==",
             "resolved": "https://registry.npmjs.org/@jupyter-widgets/output/-/output-4.1.1.tgz",
             "version": "4.1.1"
@@ -11383,15 +11919,14 @@
             "resolved": "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz",
             "version": "2.4.2"
         },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
-                "fsevents": "~2.3.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
                 "is-glob": "~4.0.1",
                 "normalize-path": "~3.0.0",
                 "readdirp": "~3.6.0"
             },
             "dev": true,
@@ -11973,14 +12508,22 @@
         },
         "node_modules/cyclist": {
             "dev": true,
             "integrity": "sha512-NJGVKPS81XejHcLhaLJS7plab0fK3slPh11mESeeDq2W4ZI5kUKK/LRRdVDvjJseojbPB7ZwjnyOybg3Igea/A==",
             "resolved": "https://registry.npmjs.org/cyclist/-/cyclist-1.0.1.tgz",
             "version": "1.0.1"
         },
+        "node_modules/d3-color": {
+            "engines": {
+                "node": ">=12"
+            },
+            "integrity": "sha512-zg/chbXyeBtMQ1LbD/WSoW2DpC3I0mpmPdW+ynRTj/x2DAWYrIY7qeZIHidozwV24m4iavr15lNwIwLxRmOxhA==",
+            "resolved": "https://registry.npmjs.org/d3-color/-/d3-color-3.1.0.tgz",
+            "version": "3.1.0"
+        },
         "node_modules/d3-format": {
             "integrity": "sha512-J0piedu6Z8iB6TbIGfZgDzfXxUFN3qQRMofy2oPdXzQibYGqPB/9iMcxr/TGalU+2RsyDO+U4f33id8tbnSRMQ==",
             "resolved": "https://registry.npmjs.org/d3-format/-/d3-format-1.4.5.tgz",
             "version": "1.4.5"
         },
         "node_modules/debug": {
             "dependencies": {
@@ -14661,14 +15204,19 @@
             "version": "3.0.0"
         },
         "node_modules/normalize.css": {
             "integrity": "sha512-qizSNPO93t1YUuUhP22btGOo3chcvDFqFaj2TRybP0DMxkHOCTYwp3n34fel4a31ORXy4m1Xq0Gyqpb5m33qIg==",
             "resolved": "https://registry.npmjs.org/normalize.css/-/normalize.css-8.0.1.tgz",
             "version": "8.0.1"
         },
+        "node_modules/nouislider": {
+            "integrity": "sha512-AV7UMhGhZ4Mj6ToMT812Ib8OJ4tAXR2/Um7C4l4ZvvsqujF0WpQTpqqHJ+9xt4174R7ueQOUrBR4yakJpAIPCA==",
+            "resolved": "https://registry.npmjs.org/nouislider/-/nouislider-15.4.0.tgz",
+            "version": "15.4.0"
+        },
         "node_modules/npm-run-all": {
             "bin": {
                 "npm-run-all": "bin/npm-run-all/index.js",
                 "run-p": "bin/run-p/index.js",
                 "run-s": "bin/run-s/index.js"
             },
             "dependencies": {
@@ -17288,18 +17836,16 @@
             },
             "integrity": "sha512-rpJyN222KWIvHJ/F53XSZv0Zl/accqHR8et1kpaMTD/fLCRxtV8iX8czMzY7sVZupTI3zcUTg8eycS2kNF9l6w==",
             "resolved": "https://registry.npmjs.org/warning/-/warning-4.0.3.tgz",
             "version": "4.0.3"
         },
         "node_modules/watchpack": {
             "dependencies": {
-                "chokidar": "^3.4.1",
                 "graceful-fs": "^4.1.2",
-                "neo-async": "^2.5.0",
-                "watchpack-chokidar2": "^2.0.1"
+                "neo-async": "^2.5.0"
             },
             "dev": true,
             "integrity": "sha512-9P3MWk6SrKjHsGkLT2KHXdQ/9SNkyoJbabxnKOoJepsvJjJG8uYTR3yTPxPQvNDI3w4Nz1xnE0TLHK4RIVe/MQ==",
             "optionalDependencies": {
                 "chokidar": "^3.4.1",
                 "watchpack-chokidar2": "^2.0.1"
             },
@@ -17351,15 +17897,14 @@
             "version": "1.13.1"
         },
         "node_modules/watchpack-chokidar2/node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "^2.0.0",
                 "async-each": "^1.0.1",
                 "braces": "^2.3.2",
-                "fsevents": "^1.2.7",
                 "glob-parent": "^3.1.0",
                 "inherits": "^2.0.3",
                 "is-binary-path": "^1.0.0",
                 "is-glob": "^4.0.0",
                 "normalize-path": "^3.0.0",
                 "path-is-absolute": "^1.0.0",
                 "readdirp": "^2.2.1",
@@ -17788,16 +18333,14 @@
             "bin": {
                 "y-websocket": "bin/server.js",
                 "y-websocket-server": "bin/server.js"
             },
             "dependencies": {
                 "lib0": "^0.2.42",
                 "lodash.debounce": "^4.0.8",
-                "ws": "^6.2.1",
-                "y-leveldb": "^0.1.0",
                 "y-protocols": "^1.0.5"
             },
             "funding": {
                 "type": "GitHub Sponsors \u2764",
                 "url": "https://github.com/sponsors/dmonad"
             },
             "integrity": "sha512-VobyJaAoyWIETETNZragnTpL7kcJr8a/CIUQP6DfXcQ4v0UmZUuANdsPsbmMjDsEeUECVFRhHauxpDtRhYqkaQ==",
@@ -17916,9 +18459,9 @@
             },
             "integrity": "sha512-4eSTrrs8OeI0heXKKioRY4ag7V5Bk85Z4MeniUyown3o3y0G7G4JpAZWrZWfTp7pzw2b53GkAQWKqHsHi9j9JA==",
             "resolved": "https://registry.npmjs.org/yjs/-/yjs-13.5.41.tgz",
             "version": "13.5.41"
         }
     },
     "requires": true,
-    "version": "0.3.4"
+    "version": "0.4.0"
 }
```

### Comparing `solara-1.8.2/packages/solara-widget-manager/package.json` & `solara-1.9.0/packages/solara-widget-manager/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.992094861660079%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^4.1.2', '@jupyter-widgets/controls': '^3.1.2', "*

 * *                   "'@jupyter-widgets/base8': 'npm:@jupyter-widgets/base@^6.0.1', "*

 * *                   "'@jupyter-widgets/controls8': 'npm:@jupyter-widgets/controls@^5.0.1', "*

 * *                   "'@jupyter-widgets/jupyterlab-manager8': "*

 * *                   "'npm:@jupyter-widgets/jupyterlab-manager@^5.0.3'}"}*

```diff
@@ -1,13 +1,16 @@
 {
     "browserslist": ">0.8%, not ie 11, not op_mini all, not dead",
     "dependencies": {
-        "@jupyter-widgets/base": "^4.1.0",
-        "@jupyter-widgets/controls": "^3.1.0",
+        "@jupyter-widgets/base": "^4.1.2",
+        "@jupyter-widgets/base8": "npm:@jupyter-widgets/base@^6.0.1",
+        "@jupyter-widgets/controls": "^3.1.2",
+        "@jupyter-widgets/controls8": "npm:@jupyter-widgets/controls@^5.0.1",
         "@jupyter-widgets/jupyterlab-manager": "^3.1.0",
+        "@jupyter-widgets/jupyterlab-manager8": "npm:@jupyter-widgets/jupyterlab-manager@^5.0.3",
         "@jupyterlab/application": "^3.0.0",
         "@jupyterlab/apputils": "^3.0.0",
         "@jupyterlab/coreutils": "^5.0.0",
         "@jupyterlab/docregistry": "^3.0.0",
         "@jupyterlab/javascript-extension": "~3.0.0",
         "@jupyterlab/notebook": "^3.0.0",
         "@jupyterlab/outputarea": "^3.0.0",
```

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/index.ts` & `solara-1.9.0/packages/solara-widget-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/kernel.ts` & `solara-1.9.0/packages/solara-widget-manager/src/kernel.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/loader.ts` & `solara-1.9.0/packages/solara-widget-manager/src/loader.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/manager.ts` & `solara-1.9.0/packages/solara-widget-manager/src/manager.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/mathjax.ts` & `solara-1.9.0/packages/solara-widget-manager/src/mathjax.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/src/rendermime.ts` & `solara-1.9.0/packages/solara-widget-manager/src/rendermime.ts`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/packages/solara-widget-manager/style/index.css` & `solara-1.9.0/packages/solara-widget-manager/style/index.css`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/pyproject.toml` & `solara-1.9.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 packages = [
     { include = "solara" }
 ]
 dependencies = [
-    "reacton>=1.2.0",
-    "ipywidgets<8",
+    "reacton>=1.4.0",
+    "ipywidgets",
     "cachetools",
     "filelock",
     "markdown",
     "pygments",
     "pymdown-extensions",
     "markdown-it-py",
     "mdit-py-plugins",
     "humanize",
     "ipyvuetify",
-    "ipyvue>=1.8.2",
+    "ipyvue>=1.9.0",
     "numpy",
     "pillow",
     "jinja2",
     "MarkupSafe<2.1",
     "pydantic",
     "click>=7.1.0",
     "rich_click",
@@ -39,14 +39,16 @@
     "starlette",
     "nbconvert",
     "jupyter_server",
     "jupyter_client>=7.0.0",
     "watchdog",
     "requests",
     "pygments==2.10; python_version < '3.7'",
+    "nbformat",
+    "ipykernel",
 ]
 
 [tool.flit.external-data]
 directory = "prefix"
 
 [tool.flit.module]
 name = "solara"
@@ -74,15 +76,15 @@
     "pre-commit",
     "bump2version",
     "dask[dataframe]; python_version < '3.7'",
     "playwright; python_version > '3.6'",
     "pytest-playwright; python_version > '3.6'",
 ]
 assets = [
-    "solara-assets==1.8.2"
+    "solara-assets==1.9.0"
 ]
 flask = [
     "flask",
     "flask-sock",
 ]
 documentation = [
     "numpy",
```

### Comparing `solara-1.8.2/solara/__init__.py` & `solara-1.9.0/solara/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Build webapps using IPywidgets"""
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 github_url = "https://github.com/widgetti/solara"
 git_branch = "master"
 
 
+from . import comm  # noqa: F401
+
+
 def _using_solara_server():
     import sys
 
     if "solara.server" in sys.modules:
         return True
     if sys.argv[0].split("/")[-1] == "solara":
         return True
@@ -17,14 +20,15 @@
 # isort: skip_file
 from reacton import (
     component,
     component_interactive,
     value_component,
     create_context,
     get_widget,
+    get_context,
     make,
     provide_context,
     render,
     render_fixed,
     use_context,
     use_effect,
     use_exception,
@@ -90,15 +94,15 @@
             # children
             display(button)
     ```
     Note that this is a dispatch call to the
     [IPython display function](https://ipython.readthedocs.io/en/stable/api/generated/IPython.display.html#IPython.display.display),
     with a slimmer API. The main purpose of this function is the have type safety, since tools like mypy do now know about
     the existance of the IPython display function, and will complain if you use it without importing it.
-    Since solara is always important, this saves you from having to import IPython in your code.
+    Since solara is always imported, this saves you from having to import IPython in your code.
 
     ## Arguments
 
      * `objs`: The objects to display.
      * `kwargs`: Keyword arguments to pass to the IPython display function.
 
     """
```

### Comparing `solara-1.8.2/solara/__main__.py` & `solara-1.9.0/solara/__main__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/autorouting.py` & `solara-1.9.0/solara/autorouting.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,17 @@
     return results
 
 
 @solara.component
 def RoutingProvider(children: List[reacton.core.Element] = [], routes: List[solara.Route] = [], pathname: str = ""):
     """Wraps the app, adds extra context, like navigation/routing."""
     path, set_path = solara.use_state(pathname, key="solara-context-path")
+    # TODO: since we provide a cross filter context here, I don't think name `RoutingProvider` is a good name
+    # we might want to change/refactor this.
+    solara.provide_cross_filter()
     nav = solara.Navigator(location=path, on_location=set_path)
     solara.routing._location_context.provide(solara.routing._Location(path, set_path))
     solara.routing.router_context.provide(solara.routing.Router(path, routes=routes, set_path=set_path))
 
     main = solara.VBox(
         children=[
             nav,
```

### Comparing `solara-1.8.2/solara/cache.py` & `solara-1.9.0/solara/cache.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/checks.html` & `solara-1.9.0/solara/checks.html`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/checks.py` & `solara-1.9.0/solara/checks.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/__init__.py` & `solara-1.9.0/solara/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     SliderRangeFloat,  # noqa: F401 F403
 )  # noqa: F401 F403
 from .sql_code import SqlCode  # noqa: #F401 F403
 from .togglebuttons import (  # noqa: #F401 F403
     ToggleButtonsMultiple,
     ToggleButtonsSingle,
 )
-from .input import InputText, InputFloat  # noqa: #F401 F403
+from .input import InputText, InputFloat, InputInt  # noqa: #F401 F403
 from .pivot_table import PivotTableView, PivotTable, PivotTableCard  # noqa: #F401 F403
 from .head import Head  # noqa: #F401 F403
 from .title import Title  # noqa: #F401 F403
 from .link import Link  # noqa: #F401 F403
 from .applayout import AppLayout, Sidebar, AppBar  # noqa: #F401 F403
 from .tab_navigation import TabNavigation  # noqa: #F401 F403
 from .markdown_editor import MarkdownEditor  # noqa: #F401 F403
@@ -45,12 +45,12 @@
 from .echarts import FigureEcharts  # noqa: #F401 F403
 from .figure_altair import FigureAltair, AltairChart  # noqa: #F401 F403
 from .meta import Meta  # noqa: #F401 F403
 from .columns import Columns, ColumnsResponsive  # noqa: #F401 F403
 from .file_drop import FileDrop  # noqa: #F401 F403
 from .file_download import FileDownload  # noqa: #F401 F403
 from .tooltip import Tooltip  # noqa: #F401 F403
-
+from .card import Card, CardActions  # noqa: #F401 F403
 
 import reacton.core
 
 reacton.core._default_container = Column  # noqa: F405
```

### Comparing `solara-1.8.2/solara/components/alert.py` & `solara-1.9.0/solara/components/alert.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/applayout.py` & `solara-1.9.0/solara/components/applayout.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/button.py` & `solara-1.9.0/solara/components/button.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/checkbox.py` & `solara-1.9.0/solara/components/checkbox.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/code_highlight_css.vue` & `solara-1.9.0/solara/components/code_highlight_css.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/columns.py` & `solara-1.9.0/solara/components/columns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import itertools
-from typing import List, Union
+from typing import List, Optional, Union
 
 import reacton.ipyvuetify as rv
 
 import solara
+from solara.util import _combine_classes
 
 
 def cycle(value):
     if value is None:
         return itertools.cycle([None])
     elif isinstance(value, int):
         return itertools.cycle([value])
@@ -70,15 +71,27 @@
             for child, width in zip(children, cycle(widths)):
                 with rv.Col(children=[child], style_=f"flex-grow: {width}; overflow: auto" if width != 0 else "flex-grow: 0;"):
                     pass
     return main
 
 
 @solara.component
-def ColumnsResponsive(default=None, small=None, medium=None, large=None, xlarge=None, children=[], wrap=True, gutters=True, gutters_dense=False):
+def ColumnsResponsive(
+    default=None,
+    small=None,
+    medium=None,
+    large=None,
+    xlarge=None,
+    children=[],
+    wrap=True,
+    gutters=True,
+    gutters_dense=False,
+    classes: List[str] = [],
+    style: Optional[str] = None,
+):
     """Lay our children in columns, on a 12 point grid system that is responsive to screen size.
 
     If a single number is specified, or less values than children, the values will be cycled.
     The total width of this system is 12, so if you want to have 3 columns, each taking up 4 points, you would specify [4, 4, 4] or 4.
 
 
     ```python
@@ -118,15 +131,15 @@
         elif isinstance(value, int):
             return itertools.cycle([value])
         elif isinstance(value, (list, tuple)):
             return itertools.cycle(value)
         else:
             raise ValueError(f"Invalid value for columns: {value}, should be None, int, or list/tuple.")
 
-    with rv.Container() as main:
+    with rv.Container(class_=_combine_classes(classes), style_=style) as main:
         with rv.Row(class_="flex-nowrap" if not wrap else "", no_gutters=not gutters, dense=gutters_dense):
             for child, xsmall, small, medium, large, xlarge in zip(children, cycle(default), cycle(small), cycle(medium), cycle(large), cycle(xlarge)):
                 with rv.Col(
                     cols=xsmall,
                     sm=small,
                     md=medium,
                     lg=large,
```

### Comparing `solara-1.8.2/solara/components/cross_filter.py` & `solara-1.9.0/solara/components/cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/dataframe.py` & `solara-1.9.0/solara/components/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/datatable.py` & `solara-1.9.0/solara/components/datatable.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/datatable.vue` & `solara-1.9.0/solara/components/datatable.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/details.py` & `solara-1.9.0/solara/components/details.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/download.vue` & `solara-1.9.0/solara/components/download.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/echarts.py` & `solara-1.9.0/solara/components/echarts.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/echarts.vue` & `solara-1.9.0/solara/components/echarts.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/figure_altair.py` & `solara-1.9.0/solara/components/figure_altair.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/file_browser.py` & `solara-1.9.0/solara/components/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/file_download.py` & `solara-1.9.0/solara/components/file_download.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/file_drop.py` & `solara-1.9.0/solara/components/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/file_drop.vue` & `solara-1.9.0/solara/components/file_drop.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/file_list_widget.vue` & `solara-1.9.0/solara/components/file_list_widget.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/head.py` & `solara-1.9.0/solara/components/head.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/head_tag.py` & `solara-1.9.0/solara/components/head_tag.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/head_tag.vue` & `solara-1.9.0/solara/components/head_tag.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/image.py` & `solara-1.9.0/solara/components/image.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/link.py` & `solara-1.9.0/solara/components/link.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/markdown.py` & `solara-1.9.0/solara/components/markdown.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/markdown_editor.py` & `solara-1.9.0/solara/components/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/markdown_editor.vue` & `solara-1.9.0/solara/components/markdown_editor.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/matplotlib.py` & `solara-1.9.0/solara/components/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/meta.py` & `solara-1.9.0/solara/components/meta.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/misc.py` & `solara-1.9.0/solara/components/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,35 +74,16 @@
         disabled=disabled,
         **kwargs,
     )
     return value
 
 
 @solara.component
-def Card(title: str = None, subtitle: str = None, elevation: int = 2, margin=2, children: List[reacton.core.Element] = [], classes: List[str] = []):
-    class_ = _combine_classes([f"ma-{margin}", *classes])
-    with v.Card(elevation=elevation, class_=class_) as main:
-        if title:
-            with v.CardTitle(
-                children=[title],
-            ):
-                pass
-        if subtitle:
-            with v.CardSubtitle(
-                children=[subtitle],
-            ):
-                pass
-        with v.CardText(children=children):
-            pass
-    return main
-
-
-@solara.component
-def Text(text):
-    return v.Html(tag="span", children=[text])
+def Text(text, style: str = None, classes: List[str] = []):
+    return v.Html(tag="span", class_=_combine_classes(classes), style_=style, children=[text])
 
 
 @solara.component
 def Div(children=[], **kwargs):
     return v.Html(tag="div", children=children, **kwargs)
```

### Comparing `solara-1.8.2/solara/components/pivot_table.py` & `solara-1.9.0/solara/components/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/pivot_table.vue` & `solara-1.9.0/solara/components/pivot_table.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/select.py` & `solara-1.9.0/solara/components/select.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/select.vue` & `solara-1.9.0/solara/components/select.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/slider.py` & `solara-1.9.0/solara/components/slider.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/slider_date.vue` & `solara-1.9.0/solara/components/slider_date.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/sql_code.py` & `solara-1.9.0/solara/components/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/sql_code.vue` & `solara-1.9.0/solara/components/sql_code.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/style.py` & `solara-1.9.0/solara/components/style.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/tab_navigation.py` & `solara-1.9.0/solara/components/tab_navigation.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/title.py` & `solara-1.9.0/solara/components/title.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/title.vue` & `solara-1.9.0/solara/components/title.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/togglebuttons.py` & `solara-1.9.0/solara/components/togglebuttons.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/components/tooltip.py` & `solara-1.9.0/solara/components/tooltip.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/datatypes.py` & `solara-1.9.0/solara/datatypes.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/express.py` & `solara-1.9.0/solara/express.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/hooks/dataframe.py` & `solara-1.9.0/solara/hooks/dataframe.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         def on_change():
             set_filter(data_filters.get(key))
             # even if we don't change our own filter, the other may change
             updater()
 
         def connect():
             self.listeners.append(on_change)
+            # we need to force an extra render after the first render
+            # to make sure we have the correct filter, since others components
+            # may set a filter after we have rendered, *or* mounted
+            on_change()
 
             def cleanup():
                 self.listeners.remove(on_change)
                 # also remove our filter, and notify the rest
                 data_filters.pop(key, None)  # remove, ignoring key error
                 for listener in self.listeners:
                     listener()
```

### Comparing `solara-1.8.2/solara/hooks/misc.py` & `solara-1.9.0/solara/hooks/misc.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/lab/__init__.py` & `solara-1.9.0/solara/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/lab/toestand.py` & `solara-1.9.0/solara/lab/toestand.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 import dataclasses
 import sys
 import threading
+from collections import defaultdict
 from operator import getitem
-from typing import Any, Callable, Dict, Generic, Set, Tuple, TypeVar, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import react_ipywidgets as react
+import reacton.core
 from reacton.utils import equals
 
+import solara
 from solara import _using_solara_server
 
 T = TypeVar("T")
 TS = TypeVar("TS")
 S = TypeVar("S")  # used for state
 
-local = threading.local()
 _DEBUG = False
 
 
+class ThreadLocal(threading.local):
+    reactive_used: Optional[Set["ValueBase"]] = None
+
+
+thread_local = ThreadLocal()
+
+
 # these hooks should go into react-ipywidgets
 def use_sync_external_store(subscribe: Callable[[Callable[[], None]], Callable[[], None]], get_snapshot: Callable[[], Any]):
     _, set_counter = react.use_state(0)
 
     def force_update():
         set_counter(lambda x: x + 1)
 
@@ -53,16 +74,16 @@
         return type(d1)(**{**d1.dict(), **kwargs})  # type: ignore
     return cast(S, {**cast(dict, d1), **kwargs})
 
 
 class ValueBase(Generic[T]):
     def __init__(self, merge: Callable = merge_state):
         self.merge = merge
-        self.listeners: Set[Callable[[T], None]] = set()
-        self.listeners2: Set[Callable[[T, T], None]] = set()
+        self.listeners: Dict[str, Set[Callable[[T], None]]] = defaultdict(set)
+        self.listeners2: Dict[str, Set[Callable[[T, T], None]]] = defaultdict(set)
 
     @property
     def lock(self):
         raise NotImplementedError
 
     @property
     def value(self) -> T:
@@ -74,68 +95,69 @@
 
     def set(self, value: T):
         raise NotImplementedError
 
     def get(self) -> T:
         raise NotImplementedError
 
+    def _get_scope_key(self):
+        raise NotImplementedError
+
     def subscribe(self, listener: Callable[[T], None]):
-        self.listeners.add(listener)
+        scope_id = self._get_scope_key()
+        self.listeners[scope_id].add(listener)
 
         def cleanup():
-            self.listeners.remove(listener)
+            self.listeners[scope_id].remove(listener)
 
         return cleanup
 
     def subscribe_change(self, listener: Callable[[T, T], None]):
-        self.listeners2.add(listener)
+        scope_id = self._get_scope_key()
+        self.listeners2[scope_id].add(listener)
 
         def cleanup():
-            self.listeners2.remove(listener)
+            self.listeners2[scope_id].remove(listener)
 
         return cleanup
 
+    def fire(self, new: T, old: T):
+        scope_id = self._get_scope_key()
+        for listener in self.listeners[scope_id].copy():
+            listener(new)
+        for listener2 in self.listeners2[scope_id].copy():
+            listener2(new, old)
+
     def update(self, _f=None, **kwargs):
         if _f is not None:
             assert not kwargs
             with self.lock:
                 kwargs = _f(self.get())
         with self.lock:
             # important to have this part thread-safe
             new = self.merge(self.get(), **kwargs)
             self.set(new)
 
-    def fire(self, new: T, old: T):
-        for listener in self.listeners.copy():
-            listener(new)
-        for listener2 in self.listeners2.copy():
-            listener2(new, old)
-
     def use_value(self) -> T:
         # .use with the default argument doesn't give good type inference
         return self.use()
 
     def use(self, selector: Callable[[T], TS] = lambda x: x) -> TS:  # type: ignore
-        slice = use_sync_external_store_with_selector(
-            self.subscribe,
-            self.get,
-            selector,
-        )
-        return slice
+        return selector(self.value)
 
     def use_state(self) -> Tuple[T, Callable[[T], None]]:
         setter = self.set
         value = self.use()  # type: ignore
         return value, setter
 
     @property
-    def fields(self) -> T:
+    def fields(self) -> Type[T]:
         # we lie about the return type, but in combination with
         # setter we can make type safe setters (see docs/tests)
-        return cast(T, Fields(self))
+        return cast(Type[T], Fields(self))
 
     def setter(self, field: TS) -> Callable[[TS], None]:
         _field = cast(FieldBase, field)
 
         def setter(new_value: TS):
             _field.set(new_value)
 
@@ -154,43 +176,50 @@
         super().__init__()
         self.default_value = default_value
         cls = type(default_value)
         self.storage_key = key or (cls.__module__ + ":" + cls.__name__ + "-" + str(id(default_value)))
         self._global_dict = {}
         # since a set can trigger events, which can trigger new updates, we need a recursive lock
         self._lock = threading.RLock()
+        self.local = threading.local()
 
     @property
     def lock(self):
         return self._lock
 
+    def _get_scope_key(self):
+        scope_dict, scope_id = self._get_dict()
+        return scope_id
+
     def _get_dict(self):
         scope_dict = self._global_dict
+        scope_id = "global"
         if _using_solara_server():
             import solara.server.app
 
             try:
                 context = solara.server.app.get_current_context()
             except:  # noqa
                 pass  # do we need to be more strict?
             else:
                 scope_dict = cast(Dict[str, S], context.user_dicts)
-        return scope_dict
+                scope_id = context.id
+        return cast(Dict[str, S], scope_dict), scope_id
 
     def get(self):
-        scope_dict = self._get_dict()
+        scope_dict, scope_id = self._get_dict()
         if self.storage_key not in scope_dict:
             with self.scope_lock:
                 if self.storage_key not in scope_dict:
                     # we assume immutable, so don't make a copy
                     scope_dict[self.storage_key] = self.default_value
         return scope_dict[self.storage_key]
 
     def set(self, value: S):
-        scope_dict = self._get_dict()
+        scope_dict, scope_id = self._get_dict()
         old = self.get()
         if equals(old, value):
             return
         scope_dict[self.storage_key] = value
 
         if _DEBUG:
             import traceback
@@ -209,29 +238,49 @@
     def __init__(self, default_value: Union[S, ValueBase[S]]):
         super().__init__()
         if not isinstance(default_value, ValueBase):
             self._storage = ConnectionStore(default_value, key=id(self))
         else:
             self._storage = default_value
         self.__post__init__()
+        self._name = None
+        self._owner = None
+
+    def __set_name__(self, owner, name):
+        self._name = name
+        self._owner = owner
+
+    def __repr__(self):
+        if self._name:
+            return f"<Reactive {self._owner.__name__}.{self._name} value={self.value!r} id={hex(id(self))}>"
+        else:
+            return f"<Reactive {self.value!r} id={hex(id(self))}>"
+
+    def __str__(self):
+        if self._name:
+            return f"{self._owner.__name__}.{self._name}={self.value!r}"
+        else:
+            return f"{self.value!r}"
 
     @property
     def lock(self):
         return self._storage.lock
 
     def __post__init__(self):
         pass
 
     def update(self, **kwargs):
         self._storage.update(**kwargs)
 
     def set(self, value: S):
         self._storage.set(value)
 
-    def get(self) -> S:
+    def get(self, add_watch=True) -> S:
+        if add_watch and thread_local.reactive_used is not None:
+            thread_local.reactive_used.add(self)
         return self._storage.get()
 
     def subscribe(self, listener: Callable[[S], None]):
         return self._storage.subscribe(listener)
 
     def subscribe_change(self, listener: Callable[[S, S], None]):
         return self._storage.subscribe_change(listener)
@@ -266,28 +315,45 @@
         self._field = field
         field = field
         while not isinstance(field, ValueBase):
             field = field._parent
         self._root = field
         assert isinstance(self._root, ValueBase)
 
+    def __str__(self):
+        return str(self._field)
+
+    def __repr__(self):
+        return f"<Reactive subfield {self._field}>"
+
     @property
     def lock(self):
         return self._root.lock
 
     def subscribe(self, listener: Callable[[T], None]):
         def on_change(new, old):
             new_value = self._field.get(new)
             old_value = self._field.get(old)
             if not equals(new_value, old_value):
                 listener(new_value)
 
         return self._root.subscribe_change(on_change)
 
-    def get(self, obj=None) -> T:
+    def subscribe_change(self, listener: Callable[[T, T], None]):
+        def on_change(new, old):
+            new_value = self._field.get(new)
+            old_value = self._field.get(old)
+            if not equals(new_value, old_value):
+                listener(new_value, old_value)
+
+        return self._root.subscribe_change(on_change)
+
+    def get(self, obj=None, add_watch=True) -> T:
+        if add_watch and thread_local.reactive_used is not None:
+            thread_local.reactive_used.add(self)
         return self._field.get(obj)
 
     def set(self, value: T):
         self._field.set(value)
 
 
 def Ref(field: T) -> ValueSubField[T]:
@@ -319,19 +385,22 @@
         self._lock = state.lock
 
     def get(self, obj=None):
         # we are at the root, so override the object
         # so we can get the 'old' value
         if obj is not None:
             return obj
-        return self._parent.get()
+        return self._parent.get(add_watch=False)
 
     def set(self, value):
         self._parent.set(value)
 
+    def __repr__(self):
+        return repr(self._parent)
+
 
 class FieldAttr(FieldBase):
     def __init__(self, parent, key: str):
         self._parent = parent
         self.key = key
         self._lock = parent._lock
 
@@ -344,14 +413,20 @@
             parent_value = self._parent.get()
             if isinstance(self.key, str):
                 parent_value = merge_state(parent_value, **{self.key: value})
                 self._parent.set(parent_value)
             else:
                 raise TypeError(f"Type of key {self.key!r} is not supported")
 
+    def __str__(self):
+        return f".{self.key}"
+
+    def __repr__(self):
+        return f"<Field {self._parent}{self}>"
+
 
 class FieldItem(FieldBase):
     def __init__(self, parent, key: str):
         self._parent = parent
         self.key = key
         self._lock = parent._lock
 
@@ -368,9 +443,73 @@
                 parent_value[self.key] = value
                 self._parent.set(parent_type(parent_value))
             else:
                 parent_value = merge_state(parent_value, **{self.key: value})
                 self._parent.set(parent_value)
 
 
+class AutoSubscribeContextManager:
+    # a render loop might trigger a new render loop of a differtent render context
+    # so we want to save, and restore the current reactive_used
+    reactive_used_before: Optional[Set[ValueBase]] = None
+    reactive_used: Optional[Set[ValueBase]] = None
+    reactive_added_previous_run: Optional[Set[ValueBase]] = None
+    subscribed: Dict[ValueBase, Callable]
+
+    def __init__(self, element: solara.Element):
+        self.element = element
+        self.subscribed = {}
+
+    def __enter__(self):
+        self.reactive_used_before = thread_local.reactive_used
+        self.reactive_used = thread_local.reactive_used = set()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        assert thread_local.reactive_used is self.reactive_used, f"{hex(id(thread_local.reactive_used))} vs {hex(id(self.reactive_used))}"
+        _, set_counter = solara.use_state(0)
+
+        def update_listeners():
+            assert self.reactive_used is not None
+            reactive_used = self.reactive_used
+            # remove subfields for which we already listen to it's root reactive value
+            reactive_used_subfields = {k for k in reactive_used if isinstance(k, ValueSubField)}
+            reactive_used = reactive_used - reactive_used_subfields
+            # only add subfield for which we don't listen to it's parent
+            for reactive_used_subfield in reactive_used_subfields:
+                if reactive_used_subfield._root not in reactive_used:
+                    reactive_used.add(reactive_used_subfield)
+            added = reactive_used - (self.reactive_added_previous_run or set())
+
+            removed = (self.reactive_added_previous_run or set()) - added
+
+            for reactive in added:
+                if reactive not in self.subscribed:
+
+                    def force_update(new_value, old_value, _reactive=reactive):
+                        # can we do just x+1 to collapse multiple updates into one?
+                        set_counter(lambda x: x + 1)
+
+                    unsubscribe = reactive.subscribe_change(force_update)
+                    self.subscribed[reactive] = unsubscribe
+            for reactive in removed:
+                unsubscribe = self.subscribed[reactive]
+                unsubscribe()
+                del self.subscribed[reactive]
+            self.reactive_added_previous_run = added
+
+            def cleanup():
+                assert self.reactive_added_previous_run is not None
+                for reactive in self.reactive_added_previous_run:
+                    unsubscribe = self.subscribed[reactive]
+                    unsubscribe()
+
+            return cleanup
+
+        solara.use_effect(update_listeners, [])
+        thread_local.reactive_used = self.reactive_used_before
+
+
 # alias for compatibility
 State = Reactive
+
+auto_subscribe_context_manager = AutoSubscribeContextManager
+reacton.core._component_context_manager_classes.append(auto_subscribe_context_manager)
```

### Comparing `solara-1.8.2/solara/lab/utils/dataframe.py` & `solara-1.9.0/solara/lab/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/layout.py` & `solara-1.9.0/solara/layout.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/routing.py` & `solara-1.9.0/solara/routing.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,16 +110,16 @@
     if route_level < len(router.path_routes):
         return router.path_routes[route_level], router.path_routes_siblings[route_level]
     else:
         return None, []
 
 
 def find_route(path: str) -> Optional[solara.Route]:
-    router = solara.use_context(router_context)
-    route_level = min(solara.use_context(route_level_context), len(router.path_routes_siblings) - 1)
+    router = solara.get_context(router_context)
+    route_level = min(solara.get_context(route_level_context), len(router.path_routes_siblings) - 1)
     for route in router.path_routes_siblings[route_level]:
         if path.startswith(route.path) or (not path and route.path == "/"):
             return route
     return None
 
 
 def use_pathname():
@@ -157,20 +157,20 @@
     ## See also
 
      * [Multipage](/docs/howto/multipage).
      * [Understanding Routing](/docs/understanding/routing).
 
 
     """
-    router = solara.use_context(router_context)
+    router = solara.get_context(router_context)
     if isinstance(path_or_route, str):
         path = path_or_route
         if path.startswith("/"):
             return path
-        route_level = solara.use_context(route_level_context) + level - 1
+        route_level = solara.get_context(route_level_context) + level
         parts = [*router.parts[:route_level], path]
         path = "/" + "/".join(parts)
         if path.startswith("//"):
             path = path[1:]
         return path
     elif isinstance(path_or_route, solara.Route):
         route: solara.Route = path_or_route
```

### Comparing `solara-1.8.2/solara/scope/__init__.py` & `solara-1.9.0/solara/scope/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/scope/types.py` & `solara-1.9.0/solara/scope/types.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/app.py` & `solara-1.9.0/solara/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,18 +345,14 @@
             if self.app_object is not None:
                 if isinstance(self.app_object, reacton.core._RenderContext):
                     try:
                         self.app_object.close()
                     except Exception as e:
                         logger.exception("Could not close render context: %s", e)
                         # we want to continue, so we at least close all widgets
-            import solara.server.patch
-
-            assert isinstance(widgets.Widget.widgets, solara.server.patch.context_dict_widgets), f"Unexpected widget dict type: {type(widgets.Widget.widgets)}"
-            assert widgets.Widget.widgets._get_context_dict() is self.widgets
             widgets.Widget.close_all()
             # what if we reference eachother
             # import gc
             # gc.collect()
         if self.id in contexts:
             del contexts[self.id]
 
@@ -492,40 +488,39 @@
     # load the app, and set it at the child of the context's container
     app_state_initial = app_state
     context = get_current_context()
     container = context.container
     assert container is not None
     try:
         render_context = context.app_object
-        with context:
-            app_state = app_state_initial
-            with pdb_guard():
-                widget, render_context = _run_app(
-                    app_state,
-                    app_script,
-                    pathname,
-                    render_context=render_context,
-                )
-                if render_context is None:
-                    assert context.container is not None
-                    context.container.children = [widget]
+        app_state = app_state_initial
+        with pdb_guard():
+            widget, render_context = _run_app(
+                app_state,
+                app_script,
+                pathname,
+                render_context=render_context,
+            )
+            if render_context is None:
+                assert context.container is not None
+                context.container.children = [widget]
 
-            if render_context:
-                context.app_object = render_context
+        if render_context:
+            context.app_object = render_context
 
     except BaseException as e:
         error = ""
         error = "".join(traceback.format_exception(None, e, e.__traceback__))
         print(error, file=sys.stdout, flush=True)  # noqa
         # widget = widgets.Label(value="Error, see server logs")
         import html
 
         error = html.escape(error)
         with context:
-            widget = widgets.HTML(f"<pre>{error}</pre>")
+            widget = widgets.HTML(f"<pre>{error}</pre>", layout=widgets.Layout(overflow="auto"))
             container.children = [widget]
 
 
 def solara_comm_target(comm, msg_first):
     app: Optional[AppScript] = None
 
     def on_msg(msg):
```

### Comparing `solara-1.8.2/solara/server/assets/favicon.png` & `solara-1.9.0/solara/server/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/assets/favicon.svg` & `solara-1.9.0/solara/server/assets/favicon.svg`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/assets/style.css` & `solara-1.9.0/solara/server/assets/style.css`

 * *Files 5% similar despite different names*

```diff
@@ -77,19 +77,10 @@
     padding: 0 !important;
 }
 
 .solara-markdown pre {
     background-color: unset !important
 }
 
-
-/* See https://github.com/jupyter-widgets/ipywidgets/issues/3692
-  TODO: this fixes the cursor in Solara, but not in the notebook
-*/
-.solara-image {
-    cursor: unset !important;
-}
-
-
 .jp-OutputArea-prompt {
     display: none;
 }
```

### Comparing `solara-1.8.2/solara/server/cdn_helper.py` & `solara-1.9.0/solara/server/cdn_helper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import pathlib
+import shutil
 
 import requests
 
 from . import settings
 
 logger = logging.getLogger("Solara.cdn")
 
@@ -55,15 +56,21 @@
 def get_path(base_cache_dir: pathlib.Path, path) -> pathlib.Path:
 
     parts = path.replace("\\", "/").split("/")
     store_path = path if len(parts) != 1 else pathlib.Path(path) / "__main.js"
     cache_path = base_cache_dir / store_path
 
     if cache_path.exists():
-        return cache_path
+        # before d7eba856f100d5c3c64f4eec22c62390f084cb40 on windows, we could
+        # accidentally write to the cache directory, so we need to check if we still
+        # have an old directory layout, and remove that first.
+        if cache_path.is_dir():
+            shutil.rmtree(cache_path)
+        else:
+            return cache_path
     url = get_cdn_url(path)
     response = requests.get(url)
     if response.ok:
         put_in_cache(base_cache_dir, store_path, response.content)
         assert cache_path.exists(), f"Could not write to {cache_path}"
         return cache_path
     else:
```

### Comparing `solara-1.8.2/solara/server/flask.py` & `solara-1.9.0/solara/server/flask.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/jupyter/cdn_handler.py` & `solara-1.9.0/solara/server/jupyter/cdn_handler.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/jupyter/server_extension.py` & `solara-1.9.0/solara/server/jupyter/server_extension.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/kernel.py` & `solara-1.9.0/solara/server/kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,23 @@
 
 ipykernel_version = tuple(map(int, ipykernel.__version__.split(".")))
 if ipykernel_version >= (6, 18, 0):
     import comm.base_comm
 
     class Comm(comm.base_comm.BaseComm):
         def __init__(self, **kwargs) -> None:
-            self.kernel = ipykernel.kernelbase.Kernel.instance()
+            if ipykernel.kernelbase.Kernel.initialized():
+                self.kernel = ipykernel.kernelbase.Kernel.instance()
+            else:
+                self.kernel = None
             super().__init__(**kwargs)
 
         def publish_msg(self, msg_type, data=None, metadata=None, buffers=None, **keys):
+            if self.kernel is None:
+                return
             data = {} if data is None else data
             metadata = {} if metadata is None else metadata
             content = dict(data=data, comm_id=self.comm_id, **keys)
             self.kernel.session.send(
                 self.kernel.iopub_socket,
                 msg_type,
                 content,
```

### Comparing `solara-1.8.2/solara/server/patch.py` & `solara-1.9.0/solara/server/patch.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 logger = logging.getLogger("solara.server.app")
 try:
     from reacton.patch_display import patch as patch_display
 except:  # noqa
     patch_display = None  # type: ignore
 if patch_display is not None:
     patch_display()
+ipywidget_version_major = int(ipywidgets.__version__.split(".")[0])
 
 
 class FakeIPython:
     def __init__(self, context: app.AppContext):
         self.context = context
         self.kernel = context.kernel
         self.display_pub = mock.MagicMock()
@@ -239,15 +240,23 @@
     template_mod_vue = sys.modules["ipyvue.VueTemplateWidget"]
     template_mod_vue.get_template = template_mod.get_template  # type: ignore
 
     component_mod_vue = sys.modules["ipyvue.VueComponentRegistry"]
     component_mod_vue.vue_component_registry = context_dict_user("vue_component_registry")  # type: ignore
     component_mod_vue.vue_component_files = context_dict_user("vue_component_files")  # type: ignore
 
-    ipywidgets.widget.Widget.widgets = context_dict_widgets()  # type: ignore
+    if ipywidget_version_major < 8:
+        ipywidgets.widget.Widget.widgets = context_dict_widgets()  # type: ignore
+    else:
+        if hasattr(ipywidgets.widgets.widget, "_instances"):  # since 8.0.3
+            ipywidgets.widgets.widget._instances = context_dict_widgets()  # type: ignore
+        elif hasattr(ipywidgets.widget.Widget, "_instances"):
+            ipywidgets.widget.Widget._instances = context_dict_widgets()  # type: ignore
+        else:
+            raise RuntimeError("Could not find _instances on ipywidgets version %r" % ipywidgets.__version__)
     threading.Thread.__init__ = WidgetContextAwareThread__init__  # type: ignore
     threading.Thread.run = Thread_debug_run  # type: ignore
     # on CI we get a mypy error:
     # solara/server/patch.py:210: error: Cannot assign to a method
     #  solara/server/patch.py:210: error: Incompatible types in assignment (expression has type "classmethod[Any]",\
     #                                     variable has type "Callable[[VarArg(Any), KwArg(Any)], Any]")
     # not sure why we cannot reproduce that locally
@@ -255,7 +264,25 @@
     # on CI we get a mypy error:
     # solara/server/patch.py:211: error: Cannot assign to a method
     # solara/server/patch.py:211: error: Incompatible types in assignment (expression has type "classmethod[Any]", variable has type "Callable[[], Any]")
     # not sure why we cannot reproduce that locally
     ipykernel.kernelbase.Kernel.initialized = classmethod(kernel_initialized_dispatch)  # type: ignore
     ipywidgets.widgets.widget.get_ipython = get_ipython
     IPython.get_ipython = get_ipython
+
+    def model_id_debug(self: ipywidgets.widgets.widget.Widget):
+        from ipyvue.ForceLoad import force_load_instance
+
+        import solara.comm
+
+        if self.comm is None or isinstance(self.comm, solara.comm.DummyComm) and force_load_instance.comm is not self.comm:
+            stack = solara.comm.orphan_comm_stacks.get(self.comm)
+            if stack:
+                raise RuntimeError(
+                    "Widget has no comm, you are probably using a widget that was created at app startup, the stacktrace when the widget was created is:\n"
+                    + stack
+                )
+            else:
+                raise RuntimeError("Widget has no comm, you are probably using a widget that was closed. The widget is:\n" + repr(self))
+        return self.comm.comm_id
+
+    ipywidgets.widget.Widget.model_id = property(model_id_debug)
```

### Comparing `solara-1.8.2/solara/server/pyodide.py` & `solara-1.9.0/solara/server/pyodide.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/reload.py` & `solara-1.9.0/solara/server/reload.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import errno
 import importlib
 import inspect
 import logging
 import os
 import sys
 import threading
-from typing import Callable, Dict, List, Optional, Set, Type
+from typing import Any, Callable, Dict, List, Optional, Set, Type
 
 NO_WATCHDOG = False
 try:
     from watchdog.events import FileSystemEventHandler
     from watchdog.observers import Observer
 except ImportError:
     pass
@@ -44,15 +44,15 @@
     WatcherType: Type[Watcher] = WatcherDummy  # type: ignore
 
 else:
 
     class WatcherWatchdog(FileSystemEventHandler):
         def __init__(self, files, on_change: Callable[[str], None]):
             self.on_change = on_change
-            self.observers: List[Observer] = []
+            self.observers: List[Any] = []
             self.directories: Set[str] = set()
             self.files: List[str] = []
             self.mtimes: Dict[str, float] = dict()
             for file in files:
                 self.add_file(file)
 
         def close(self):
```

### Comparing `solara-1.8.2/solara/server/server.py` & `solara-1.9.0/solara/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import sys
 import time
 from pathlib import Path
 from typing import Dict, List, Optional, TypeVar
 
 import ipykernel
+import ipywidgets
 import jinja2
 import requests
 
 import solara
 import solara.routing
 
 from . import app, settings, websocket
@@ -22,14 +23,15 @@
 
 T = TypeVar("T")
 
 
 directory = Path(__file__).parent
 template_name = "index.html.j2"
 ipykernel_major = int(ipykernel.__version__.split(".")[0])
+ipywidgets_major = int(ipywidgets.__version__.split(".")[0])
 cache_memory = solara.cache.Memory(max_items=128)
 
 # first look at the project directory, then the builtin solara directory
 
 
 def get_jinja_env(app_name: str) -> jinja2.Environment:
     jinja_loader = jinja2.FileSystemLoader(
@@ -248,14 +250,15 @@
         "theme": settings.theme.dict(),
         "production": settings.main.mode == "production",
         "pre_rendered_html": pre_rendered_html,
         "pre_rendered_css": pre_rendered_css,
         "pre_rendered_metas": pre_rendered_metas,
         "assets": settings.assets.dict(),
         "cdn": cdn,
+        "ipywidget_major_version": ipywidgets_major,
         **render_kwargs,
     }
     response = template.render(**render_settings)
     return response
 
 
 def find_prefixed_directory(path):
```

### Comparing `solara-1.8.2/solara/server/settings.py` & `solara-1.9.0/solara/server/settings.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/starlette.py` & `solara-1.9.0/solara/server/starlette.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/ansi.js` & `solara-1.9.0/solara/server/static/ansi.js`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/highlight-dark.css` & `solara-1.9.0/solara/server/static/highlight-dark.css`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/highlight.css` & `solara-1.9.0/solara/server/static/highlight.css`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/main-vuetify.js` & `solara-1.9.0/solara/server/static/main-vuetify.js`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/main.js` & `solara-1.9.0/solara/server/static/main.js`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/solara_bootstrap.py` & `solara-1.9.0/solara/server/static/solara_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         "altair",
         "vega_datasets",
         "plotly",
         "ipycanvas",
     ]
     for dep in requirements:
         await micropip.install(dep, keep_going=True)
-    await micropip.install("/wheels/solara-1.8.2-py2.py3-none-any.whl", keep_going=True)
+    await micropip.install("/wheels/solara-1.9.0-py2.py3-none-any.whl", keep_going=True)
     import solara
 
     el = solara.Warning("lala")
     import solara
 
     solara.render_fixed(el)
     return el
```

### Comparing `solara-1.8.2/solara/server/static/sun.svg` & `solara-1.9.0/solara/server/static/sun.svg`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/static/webworker.js` & `solara-1.9.0/solara/server/static/webworker.js`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/telemetry.py` & `solara-1.9.0/solara/server/telemetry.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/templates/loader-plain.html` & `solara-1.9.0/solara/server/templates/loader-plain.html`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/templates/loader-solara.css` & `solara-1.9.0/solara/server/templates/loader-solara.css`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/templates/loader-solara.html` & `solara-1.9.0/solara/server/templates/loader-solara.html`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/templates/plain.html` & `solara-1.9.0/solara/server/templates/plain.html`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/templates/solara.html.j2` & `solara-1.9.0/solara/server/templates/solara.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <link rel="icon" type="image/svg+xml" href="{{root_path}}/static/assets/favicon.svg">
 
     {% block header %}
 
 
     {{ pre_rendered_css | safe }}
 
-    <link href="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@3.0.1/dist/main.css" rel="stylesheet"></link>
+    <link href="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@4.0.0/dist/main.css" rel="stylesheet"></link>
 
 
     {% if assets.fontawesome_enabled == True %}
     <link rel="stylesheet" href="{{cdn}}{{assets.fontawesome_path}}" type="text/css">
     {% endif %}
     <link href="{{root_path}}/static/highlight.css" rel="stylesheet">
     <link href="{{root_path}}/static/highlight-dark.css" rel="stylesheet">
@@ -202,18 +202,18 @@
     <div id="app" class="v-application v-application--is-ltr theme--dark" data-app="true">
     {% endif %}
         {{ pre_rendered_html|safe }}
         {# next div is used in ssg code to see if vue took over rendering #}
         <div id="pre-rendered-html-present" style="display: none"></div>
     </div>
     {% if production %}
-    <script src="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@3.0.1/dist/solara-vuetify-app.min.js"></script>
+    <script src="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@4.0.0/dist/solara-vuetify-app{{ipywidget_major_version}}.min.js"></script>
     <script src="{{root_path}}/_solara/cdn/mermaid@9.1.7/dist/mermaid.min.js"></script>
     {% else %}
-    <script src="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@3.0.1/dist/solara-vuetify-app.js"></script>
+    <script src="{{root_path}}/_solara/cdn/@widgetti/solara-vuetify-app@4.0.0/dist/solara-vuetify-app{{ipywidget_major_version}}.js"></script>
     <script src="{{root_path}}/_solara/cdn/mermaid@9.1.7/dist/mermaid.js"></script>
     {% endif %}
     <script>
         solara.rootPath = {{ root_path | tojson | safe}};
         console.log("rootPath", solara.rootPath);
     </script>
```

### Comparing `solara-1.8.2/solara/server/threaded.py` & `solara-1.9.0/solara/server/threaded.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/utils.py` & `solara-1.9.0/solara/server/utils.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/server/websocket.py` & `solara-1.9.0/solara/server/websocket.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/settings.py` & `solara-1.9.0/solara/settings.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/markdown.py` & `solara-1.9.0/solara/template/markdown.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/.pre-commit-config.yaml` & `solara-1.9.0/solara/template/portal/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/LICENSE` & `solara-1.9.0/solara/template/portal/LICENSE`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/components/article.py` & `solara-1.9.0/solara/template/portal/solara_portal/components/article.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/components/data.py` & `solara-1.9.0/solara/template/portal/solara_portal/components/data.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md` & `solara-1.9.0/solara/template/portal/solara_portal/content/articles/equis-in-vidi.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/content/articles/substiterat-vati.md` & `solara-1.9.0/solara/template/portal/solara_portal/content/articles/substiterat-vati.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/data.py` & `solara-1.9.0/solara/template/portal/solara_portal/data.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/pages/__init__.py` & `solara-1.9.0/solara/template/portal/solara_portal/pages/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/pages/article/__init__.py` & `solara-1.9.0/solara/template/portal/solara_portal/pages/article/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/pages/tabular.py` & `solara-1.9.0/solara/template/portal/solara_portal/pages/tabular.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/template/portal/solara_portal/pages/viz/__init__.py` & `solara-1.9.0/solara/template/portal/solara_portal/pages/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/util.py` & `solara-1.9.0/solara/util.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/assets/custom.css` & `solara-1.9.0/solara/website/assets/custom.css`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/assets/images/logo-small.png` & `solara-1.9.0/solara/website/assets/images/logo-small.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/assets/images/logo.svg` & `solara-1.9.0/solara/website/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/components/header.py` & `solara-1.9.0/solara/website/components/header.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/components/hero.py` & `solara-1.9.0/solara/website/components/hero.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/README.md` & `solara-1.9.0/solara/website/pages/README.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/__init__.py` & `solara-1.9.0/solara/website/pages/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pathlib import Path
 
 import solara
 from solara.alias import rv
 from solara.components.title import Title
-from solara.routing import route_level_context
 
 from ..components import Header, Hero
 
 directory = Path(__file__).parent
 
 # md file
 md = open(directory / "README.md").read()
@@ -65,18 +64,15 @@
     return main
 
 
 @solara.component
 def Layout(children=[]):
     router = solara.use_router()
     route_current, all_routes = solara.use_route()
-    # get child routes, and restore router level, so we can also render the route of the sidebar for the mobile view
-    route_level = solara.use_context(route_level_context)
-    route_sidebar_current, all_routes_sidebar = solara.use_route()
-    route_level_context.provide(route_level)
+    route_sidebar_current, all_routes_sidebar = solara.use_route(1)
 
     show_left_menu, set_show_left_menu = solara.use_state(False)
     show_right_menu, set_show_right_menu = solara.use_state(False)
 
     if route_current and route_current.path == "apps":
         return children[0]
     with solara.VBox(grow=False) as main:
```

### Comparing `solara-1.8.2/solara/website/pages/api/__init__.py` & `solara-1.9.0/solara/website/pages/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
                     add("echarts")
                     add("matplotlib")
                     add("plotly")
                     add("plotly_express")
                 #     ListItem("AltairChart")
             with ListItem("Layout", icon_name="mdi-page-layout-sidebar-left"):
                 with List():
+                    add("card")
+                    add("card_actions")
                     add("columns")
                     add("columns_responsive")
                     add("column")
                     add("row")
                     add("hbox")
                     add("vbox")
                     add("griddraggable")
```

### Comparing `solara-1.8.2/solara/website/pages/api/altair.py` & `solara-1.9.0/solara/website/pages/api/altair.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/checkbox.py` & `solara-1.9.0/solara/website/pages/api/checkbox.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/column.py` & `solara-1.9.0/solara/website/pages/api/column.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from .common import ColorCard
 
 gap_size = solara.lab.Reactive[str]("12px")
 
 
 @solara.component
 def Page():
-    gap_size.use()
-
     with solara.Card("Column demo") as main:
         with solara.Column():
             solara.Select(
                 label="Gap size",
                 values=["0px", "4px", "8px", "12px", "16px", "20px", "24px"],
             ).connect(gap_size)
         with solara.Column(gap=gap_size.value):
```

### Comparing `solara-1.8.2/solara/website/pages/api/columns.py` & `solara-1.9.0/solara/website/pages/api/columns.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 gutters = solara.lab.Reactive[bool](True)
 gutters_dense = solara.lab.Reactive[bool](True)
 
 
 @solara.component
 def Page():
-    gutters.use()
-    gutters_dense.use()
-
     with solara.Columns([1, 2, 1], gutters=gutters.value, gutters_dense=gutters_dense.value) as main:
         with solara.Card("Left", margin=0):
             solara.Checkbox(label="Gutters").connect(gutters)
             solara.Checkbox(label="Dense gutters").connect(gutters_dense)
         with solara.Card("Middle", margin=0):
             solara.Markdown("This column has a relative width of 2, the columns to the left and right have a relative width of 1.")
         with solara.Card("Right", margin=0):
```

### Comparing `solara-1.8.2/solara/website/pages/api/columns_responsive.py` & `solara-1.9.0/solara/website/pages/api/columns_responsive.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,14 @@
 columns_medium = solara.lab.Reactive[int](3)
 columns_large = solara.lab.Reactive[int](2)
 columns_xlarge = solara.lab.Reactive[int](1)
 
 
 @solara.component
 def Page():
-    gutters.use()
-    gutters_dense.use()
-    children_count.use()
-    columns_default.use()
-    columns_small.use()
-    columns_medium.use()
-    columns_large.use()
-    columns_xlarge.use()
-    wrap.use()
-
     with solara.VBox() as main:
         with solara.Card("Controls"):
             solara.Checkbox(label="Wrap").connect(wrap)
             solara.Checkbox(label="Gutters").connect(gutters)
             solara.Checkbox(label="Dense gutters").connect(gutters_dense)
             solara.IntSlider("Children", max=20).connect(children_count)
```

### Comparing `solara-1.8.2/solara/website/pages/api/dataframe.py` & `solara-1.9.0/solara/website/pages/api/dataframe.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/echarts.py` & `solara-1.9.0/solara/website/pages/api/echarts.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/error.py` & `solara-1.9.0/solara/website/pages/api/error.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/file_browser.py` & `solara-1.9.0/solara/website/pages/api/file_browser.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/file_drop.py` & `solara-1.9.0/solara/website/pages/api/file_drop.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/griddraggable.py` & `solara-1.9.0/solara/website/pages/api/griddraggable.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/image.py` & `solara-1.9.0/solara/website/pages/api/image.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/info.py` & `solara-1.9.0/solara/website/pages/api/info.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/input.py` & `solara-1.9.0/solara/website/pages/api/input.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 @solara.component
 def Page():
     text, set_text = solara.use_state("Hello world")
     password, set_password = solara.use_state("Super secret")
     number, set_number = solara.use_state(42.0)
+    number_int, set_number_int = solara.use_state(42)
 
     continuous_update, set_continuous_update = solara.use_state(False)
 
     with solara.VBox() as main:
         with solara.Card("Settings"):
             solara.Checkbox(label="Continuous update", value=continuous_update, on_value=set_continuous_update)
 
@@ -33,17 +34,23 @@
                 solara.Button("Clear", on_click=lambda: set_password(""))
                 solara.Button("Reset", on_click=lambda: set_password("Super secret"))
             solara.Markdown(f"**You entered**: {password}")
 
         with solara.Card("Number (float)"):
             solara.InputFloat("Enter some number", value=number, on_value=set_number, continuous_update=continuous_update)
             with solara.HBox():
-                solara.Button("Reset", on_click=lambda: set_number(42))
+                solara.Button("Reset", on_click=lambda: set_number(42.0))
             solara.Markdown(f"**You entered**: {number}")
 
+        with solara.Card("Number (int)"):
+            solara.InputInt("Enter some number", value=number_int, on_value=set_number_int, continuous_update=continuous_update)
+            with solara.HBox():
+                solara.Button("Reset", on_click=lambda: set_number_int(42))
+            solara.Markdown(f"**You entered**: {number_int}")
+
     return main
 
 
 __doc__ += apidoc(solara.InputText.f)  # type: ignore
 
 __doc__ += "# InputFloat"
 __doc__ += apidoc(solara.InputFloat.f)  # type: ignore
```

### Comparing `solara-1.8.2/solara/website/pages/api/link.py` & `solara-1.9.0/solara/website/pages/api/link.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/markdown.py` & `solara-1.9.0/solara/website/pages/api/markdown.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/markdown_editor.py` & `solara-1.9.0/solara/website/pages/api/markdown_editor.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/matplotlib.py` & `solara-1.9.0/solara/website/pages/api/matplotlib.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/memoize.py` & `solara-1.9.0/solara/website/pages/api/memoize.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/meta.py` & `solara-1.9.0/solara/website/pages/api/meta.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/pivot_table.py` & `solara-1.9.0/solara/website/pages/api/pivot_table.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/plotly.py` & `solara-1.9.0/solara/website/pages/api/plotly.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/plotly_express.py` & `solara-1.9.0/solara/website/pages/api/plotly_express.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/resolve_path.py` & `solara-1.9.0/solara/website/pages/api/resolve_path.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/route.py` & `solara-1.9.0/solara/website/pages/api/route.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/row.py` & `solara-1.9.0/solara/website/pages/api/row.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from .common import ColorCard
 
 gap_size = solara.lab.Reactive[str]("12px")
 
 
 @solara.component
 def Page():
-    gap_size.use()
-
     with solara.Card("Row demo") as main:
         with solara.Row():
             solara.Select(
                 label="Gap size",
                 values=["0px", "4px", "8px", "12px", "16px", "20px", "24px"],
             ).connect(gap_size)
         with solara.Row(gap=gap_size.value):
```

### Comparing `solara-1.8.2/solara/website/pages/api/select.py` & `solara-1.9.0/solara/website/pages/api/select.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/slider.py` & `solara-1.9.0/solara/website/pages/api/slider.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/sql_code.py` & `solara-1.9.0/solara/website/pages/api/sql_code.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/style.py` & `solara-1.9.0/solara/website/pages/api/style.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/success.py` & `solara-1.9.0/solara/website/pages/api/success.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/title.py` & `solara-1.9.0/solara/website/pages/api/title.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/togglebuttons.py` & `solara-1.9.0/solara/website/pages/api/togglebuttons.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_cross_filter.py` & `solara-1.9.0/solara/website/pages/api/use_cross_filter.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_exception.py` & `solara-1.9.0/solara/website/pages/api/use_exception.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_previous.py` & `solara-1.9.0/solara/website/pages/api/use_previous.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_route.py` & `solara-1.9.0/solara/website/pages/api/use_route.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_state_or_update.py` & `solara-1.9.0/solara/website/pages/api/use_state_or_update.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_thread.md` & `solara-1.9.0/solara/website/pages/api/use_thread.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/use_thread.py` & `solara-1.9.0/solara/website/pages/api/use_thread.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/warning.py` & `solara-1.9.0/solara/website/pages/api/warning.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/api/widget.py` & `solara-1.9.0/solara/website/pages/api/widget.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/apps/layout-demo.py` & `solara-1.9.0/solara/website/pages/apps/layout-demo.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/apps/multipage/__init__.py` & `solara-1.9.0/solara/website/pages/apps/multipage/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/apps/multipage/page1.py` & `solara-1.9.0/solara/website/pages/apps/multipage/page1.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/apps/scatter.py` & `solara-1.9.0/solara/website/pages/apps/scatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,15 @@
     @staticmethod
     def reset():
         State.df.value = None
 
 
 @solara.component
 def Page():
-    # TODO: .use can be removed in the future if we wire this up automatically
-    State.size.use()
-    State.color.use()
-    State.size_max.use()
-    State.x.use()
-    State.y.use()
-    State.logx.use()
-    State.logy.use()
-    df = State.df.use_value()
+    df = State.df.value
 
     # the .scatter will set this cross filter
     filter, _set_filter = solara.use_cross_filter(id(df))
 
     # only apply the filter if the filter or dataframe changes
     def filter_df():
         if filter is not None and df is not None:
@@ -81,15 +73,15 @@
                     solara.Checkbox(label="Log y").connect(State.logy)
                     columns = list(map(str, df.columns))
                     solara.Select("Column x", values=columns).connect(State.x)  # type: ignore
                     solara.Select("Column y", values=columns).connect(State.y)  # type: ignore
                     solara.Select("Size", values=columns).connect(State.size)  # type: ignore
                     solara.Select("Color", values=columns).connect(State.color)  # type: ignore
                     if filter is None:
-                        solara.Info("I you select points in the scatter plot, you can download the points here.")
+                        solara.Info("If you select points in the scatter plot, you can download the points here.")
                     else:
 
                         def get_data():
                             return dff.to_csv(index=False)
 
                         solara.FileDownload(get_data, label=f"Download {len(dff):,} selected points", filename="selected.csv")
```

### Comparing `solara-1.8.2/solara/website/pages/doc_use_download.py` & `solara-1.9.0/solara/website/pages/doc_use_download.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/00-introduction.md` & `solara-1.9.0/solara/website/pages/docs/content/00-introduction.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/02-installing.md` & `solara-1.9.0/solara/website/pages/docs/content/02-installing.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/03-quickstart.md` & `solara-1.9.0/solara/website/pages/docs/content/03-quickstart.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/00-overview.md` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/00-overview.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/10_data_science.py` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/10_data_science.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/20-web-app.md` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/20-web-app.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/30-ipywidgets.md` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/30-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/40-streamlit.md` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/40-streamlit.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 If you add the above code snippet to your notebook, and include `Page()` at the end of your notebook cell, you should see:
 ![app screenshot](/static/public/docs/app-squared-notebook.png)
 
 Again, slightly different for a different environment.
 
 ## Hot reloading
 
-If you are using [Solara server](docs/understanding/solara-server), try editing `sol.py`, and watch the page reload automatically after you save your file. Notebook users can simply edit and re-run.
+If you are using [Solara server](/docs/understanding/solara-server), try editing `sol.py`, and watch the page reload automatically after you save your file. Notebook users can simply edit and re-run.
 
 ## How are streamlit and Solara different?
 
 ### Execution model
 As the introduction says, Solara does not re-execute your whole script after user interactions.
 The main script is executed only once. With Solara you can use your main script to read large dataframes, or do some pre-calculations without the need for [caching](/docs/reference/caching).
```

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/50-dash.md` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/50-dash.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/04-tutorial/_data_science.ipynb` & `solara-1.9.0/solara/website/pages/docs/content/04-tutorial/_data_science.ipynb`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/10-howto/20-multipage.md` & `solara-1.9.0/solara/website/pages/docs/content/10-howto/20-multipage.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/10-howto/30-layout.md` & `solara-1.9.0/solara/website/pages/docs/content/10-howto/30-layout.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,13 +108,13 @@
 
 ## Components
 
 The following [Container components](/docs/understanding/containers) can be used to define the layout of you app.
 
  * [Row](/api/row)
  * [Column](/api/column)
- * [ColumnsResponsive](/api/ColumnsResponsive)
+ * [ColumnsResponsive](/api/columns_responsive)
  * [GridFixed](/api/gridfixed)
  * [GridDraggable](/api/griddraggable)
  * [VBox](/api/vbox) (kept for ipywidgets compatibility, please use Column)
  * [HBox](/api/hbox) (kept for ipywidgets compatibility, please use Row)
- * [AppLayout](/api/applayout) Not often used directly, since Solara will already wrap your page in it. Sometimes re-used in a new `Layout` component.
+ * [AppLayout](/api/app_layout) Not often used directly, since Solara will already wrap your page in it. Sometimes re-used in a new `Layout` component.
```

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/40-static_files.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/40-static_files.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/41-asset-files.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/41-asset-files.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/60-static-site-generation.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/60-static-site-generation.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/70-search.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/70-search.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/80-reloading.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/80-reloading.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/15-reference/95-caching.md` & `solara-1.9.0/solara/website/pages/docs/content/15-reference/95-caching.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/05-ipywidgets.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/05-ipywidgets.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/06-ipyvuetify.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/06-ipyvuetify.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/10-reacton.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/10-reacton.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/12-reacton-basics.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/12-reacton-basics.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/15-anatomy.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/15-anatomy.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/18-containers.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/18-containers.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/40-routing.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/40-routing.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/50-solara-server.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/50-solara-server.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/20-understanding/60-voila.md` & `solara-1.9.0/solara/website/pages/docs/content/20-understanding/60-voila.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/30-deploying/10-self-hosted.md` & `solara-1.9.0/solara/website/pages/docs/content/30-deploying/10-self-hosted.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/30-deploying/20-cloud-hosted.md` & `solara-1.9.0/solara/website/pages/docs/content/30-deploying/20-cloud-hosted.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/90-development/10-setup.md` & `solara-1.9.0/solara/website/pages/docs/content/90-development/10-setup.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/90-troubleshoot.md` & `solara-1.9.0/solara/website/pages/docs/content/90-troubleshoot.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/99-faq.md` & `solara-1.9.0/solara/website/pages/docs/content/99-faq.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docs/content/lab/toestand.md` & `solara-1.9.0/solara/website/pages/docs/content/lab/toestand.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/docutils.py` & `solara-1.9.0/solara/website/pages/docutils.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/__init__.py` & `solara-1.9.0/solara/website/pages/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/basics/sine.py` & `solara-1.9.0/solara/website/pages/examples/basics/sine.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/general/pokemon_search.py` & `solara-1.9.0/solara/website/pages/examples/general/pokemon_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     with solara.Div() as main:
         if json.error:
             solara.Error(f"Error {json.error}")
             solara.Button("Retry", on_click=data.retry)
         else:
             if json.value:
-                solara.InputText(label="Filter pokemons by name", value=filter, on_value=set_filter)
+                solara.InputText(label="Filter pokemons by name", value=filter, on_value=set_filter, continuous_update=True)
                 pokemons = json.value
                 if filter:
                     pokemons = [k for k in pokemons if filter.lower() in k["name"].lower()]
                     if len(pokemons) == 0:
                         solara.Warning("No pokemons found, try a different filter")
                     else:
                         solara.Info(f"{len(pokemons)} pokemons found")
```

### Comparing `solara-1.8.2/solara/website/pages/examples/ipycanvas.py` & `solara-1.9.0/solara/website/pages/examples/ipycanvas.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/utilities/calculator.py` & `solara-1.9.0/solara/website/pages/examples/utilities/calculator.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/utilities/countdown_timer.py` & `solara-1.9.0/solara/website/pages/examples/utilities/countdown_timer.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/visualization/bqplot.py` & `solara-1.9.0/solara/website/pages/examples/visualization/bqplot.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/visualization/linked_views.py` & `solara-1.9.0/solara/website/pages/examples/visualization/linked_views.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/pages/examples/visualization/plotly.py` & `solara-1.9.0/solara/website/pages/examples/visualization/plotly.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/beach.jpeg` & `solara-1.9.0/solara/website/public/beach.jpeg`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/docs/anatomy.png` & `solara-1.9.0/solara/website/public/docs/anatomy.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/docs/reacton-basics.png` & `solara-1.9.0/solara/website/public/docs/reacton-basics.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/docs/solara-stack.png` & `solara-1.9.0/solara/website/public/docs/solara-stack.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/hero.png` & `solara-1.9.0/solara/website/public/hero.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/landing/complexity.png` & `solara-1.9.0/solara/website/public/landing/complexity.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/landing/python-love-react.png` & `solara-1.9.0/solara/website/public/landing/python-love-react.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/landing/what.png` & `solara-1.9.0/solara/website/public/landing/what.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/public/quickstart-notebook.png` & `solara-1.9.0/solara/website/public/quickstart-notebook.png`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/templates/index.html.j2` & `solara-1.9.0/solara/website/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/website/utils.py` & `solara-1.9.0/solara/website/utils.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/widgets/vue/gridlayout.vue` & `solara-1.9.0/solara/widgets/vue/gridlayout.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/widgets/vue/navigator.vue` & `solara-1.9.0/solara/widgets/vue/navigator.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/widgets/vue/vegalite.vue` & `solara-1.9.0/solara/widgets/vue/vegalite.vue`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/solara/widgets/widgets.py` & `solara-1.9.0/solara/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/api_test.py` & `solara-1.9.0/tests/integration/api_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/cmdline_test.py` & `solara-1.9.0/tests/integration/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/conftest.py` & `solara-1.9.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/create_test.py` & `solara-1.9.0/tests/integration/create_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/file_download_test.py` & `solara-1.9.0/tests/integration/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/markdown_test.py` & `solara-1.9.0/tests/integration/markdown_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/reload_test.py` & `solara-1.9.0/tests/integration/reload_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/router_test.py` & `solara-1.9.0/tests/integration/router_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/server_test.py` & `solara-1.9.0/tests/integration/server_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/ssg_test.py` & `solara-1.9.0/tests/integration/ssg_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/integration/testapp.py` & `solara-1.9.0/tests/integration/testapp.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/app_test.py` & `solara-1.9.0/tests/unit/app_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/applayout_test.py` & `solara-1.9.0/tests/unit/applayout_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/autorouting_test.py` & `solara-1.9.0/tests/unit/autorouting_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/cache_test.py` & `solara-1.9.0/tests/unit/cache_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/cdn_helper_test.py` & `solara-1.9.0/tests/unit/cdn_helper_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/common.py` & `solara-1.9.0/tests/unit/common.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/conftest.py` & `solara-1.9.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/cross_filter_component_test.py` & `solara-1.9.0/tests/unit/cross_filter_component_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/cross_filter_test.py` & `solara-1.9.0/tests/unit/cross_filter_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/dataframe_test.py` & `solara-1.9.0/tests/unit/dataframe_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/express_test.py` & `solara-1.9.0/tests/unit/express_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/file_browser_test.py` & `solara-1.9.0/tests/unit/file_browser_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/file_download_test.py` & `solara-1.9.0/tests/unit/file_download_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/hooks_test.py` & `solara-1.9.0/tests/unit/hooks_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/kernel_test.py` & `solara-1.9.0/tests/unit/kernel_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/lab/toestand_test.py` & `solara-1.9.0/tests/unit/lab/toestand_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import dataclasses
+import threading
 import unittest.mock
-from typing import Callable, Dict, List, Optional, TypeVar
+from typing import Callable, Dict, List, Optional, Set, TypeVar
 
 import ipyvuetify as v
 import react_ipywidgets as react
 from typing_extensions import TypedDict
 
 import solara
 import solara as sol
+import solara.lab
 from solara.lab import State
 from solara.lab.toestand import Reactive, Ref, use_sync_external_store
 from solara.server import app, kernel
 
 from ..common import click
 
 
@@ -69,14 +71,59 @@
     mock.assert_called_with(Bears(type="purple", count=3))
     mock_type.assert_not_called()
     mock_count.assert_called_with(3)
     for u in unsub:
         u()
 
 
+def test_scopes(no_app_context):
+    bear_store = BearReactive(bears)
+    mock_global = unittest.mock.Mock()
+    unsub = []
+    unsub += [bear_store.subscribe(mock_global)]
+
+    kernel_shared = kernel.Kernel()
+    assert app.current_context[app.get_current_thread_key()] is None
+
+    context1 = app.AppContext(id="toestand-1", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
+    context2 = app.AppContext(id="toestand-2", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
+
+    with context1:
+        mock1 = unittest.mock.Mock()
+        unsub += [bear_store.subscribe(mock1)]
+    with context2:
+        mock2 = unittest.mock.Mock()
+        unsub += [bear_store.subscribe(mock2)]
+
+    mock_global.assert_not_called()
+
+    with context2:
+        bear_store.update(type="purple")
+    mock_global.assert_not_called()
+    mock1.assert_not_called()
+    mock2.assert_called_with(Bears(type="purple", count=1))
+    mock2.reset_mock()
+
+    with context1:
+        bear_store.update(count=3)
+    mock_global.assert_not_called()
+    mock1.assert_called_with(Bears(type="brown", count=3))
+    mock2.assert_not_called()
+    mock1.reset_mock()
+
+    bear_store.update(type="yellow")
+    mock_global.assert_called_with(Bears(type="yellow", count=1))
+    mock1.assert_not_called()
+    mock2.assert_not_called()
+
+    mock_global.reset_mock()
+    for u in unsub:
+        u()
+
+
 def test_nested_update():
     # this effectively test the RLock vs Lock
     bear_store = BearReactive(bears)
 
     mock = unittest.mock.Mock()
     mock_type = unittest.mock.Mock()
     mock_count = unittest.mock.Mock()
@@ -290,46 +337,64 @@
     box, rc = react.render(el, handle_error=False)
     assert rc._find(v.Alert).widget.children[0] == "1 bears around here"
     click(rc._find(v.Btn).widget)
     assert rc._find(v.Alert).widget.children[0] == "2 bears around here"
 
     # the storage should live in the app context to support multiple users/connections
     kernel_shared = kernel.Kernel()
-    context1 = app.AppContext(id="1", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
-    context2 = app.AppContext(id="2", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
+    context1 = app.AppContext(id="bear-1", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
+    context2 = app.AppContext(id="bear-2", kernel=kernel_shared, control_sockets=[], widgets={}, templates={})
+    rcs = []
     for context in [context1, context2]:
         with context:
-            rc.render(el)
+            el = App()
+            box, rc = react.render(el, handle_error=False)
+            rcs.append(rc)
             # el = App()
             # box, rc = react.render(el, handle_error=False)
             assert rc._find(v.Alert).widget.children[0] == "1 bears around here"
+            assert Ref(bear_store.fields.count).value == 1
             click(rc._find(v.Btn).widget)
             assert rc._find(v.Alert).widget.children[0] == "2 bears around here"
+            assert Ref(bear_store.fields.count).value == 2
 
+    rc = rcs[1]
     with context2:
         rc.render(el)
+        assert Ref(bear_store.fields.count).value == 2
         assert rc._find(v.Alert).widget.children[0] == "2 bears around here"
         click(rc._find(v.Btn).widget)
+        assert Ref(bear_store.fields.count).value == 3
         assert rc._find(v.Alert).widget.children[0] == "3 bears around here"
 
+    rc = rcs[0]
     with context1:
         rc.render(el)
+        assert Ref(bear_store.fields.count).value == 2
         assert rc._find(v.Alert).widget.children[0] == "2 bears around here"
         click(rc._find(v.Btn).widget)
+        assert Ref(bear_store.fields.count).value == 3
         assert rc._find(v.Alert).widget.children[0] == "3 bears around here"
         click(rc._find(v.Btn).widget)
+        assert Ref(bear_store.fields.count).value == 4
         assert rc._find(v.Alert).widget.children[0] == "4 bears around here"
         click(rc._find(v.Btn).widget)
+        assert Ref(bear_store.fields.count).value == 5
         assert rc._find(v.Alert).widget.children[0] == "5 bears around here"
 
+    rc = rcs[1]
     with context2:
         rc.render(el)
+        assert Ref(bear_store.fields.count).value == 3
         assert rc._find(v.Alert).widget.children[0] == "3 bears around here"
         click(rc._find(v.Btn).widget)
+        assert Ref(bear_store.fields.count).value == 4
         assert rc._find(v.Alert).widget.children[0] == "4 bears around here"
+        Ref(bear_store.fields.count).value = 10
+        assert rc._find(v.Alert).widget.children[0] == "10 bears around here"
 
 
 def test_simplest():
 
     settings = State({"bears": 2, "theme": "dark"})
     unsub = settings.subscribe(print)  # noqa
 
@@ -465,15 +530,15 @@
 
     mock.assert_not_called()
     app_store.eat()
     assert app_store.get().fish.fishes == 3
     assert mock.call_count == 1
     mock.assert_called_with(AppStateComposite(bear=Bears(type="brown", count=1), fish=Fish(fishes=3)))
 
-    app_store.bears.increase_population()
+    app_store.bears.increase_population()  # type: ignore
     mock.assert_called_with(AppStateComposite(bear=Bears(type="brown", count=2), fish=Fish(fishes=3)))
     assert mock.call_count == 2
     assert app_store.get().bear.count == 2
     assert app_store.bears.get().count == 2
     assert app_store.get().fish.fishes == 3
 
     app_store.eat()
@@ -648,7 +713,173 @@
     mock.assert_not_called()
     df_store.set(DataFrame(df=df2))
     mock.assert_called_once()
     mock.reset_mock()
     Ref(df_store.fields.df).set(df)
     mock.assert_called_once()
     unsub()
+
+
+def test_thread_local():
+    def test1():
+        assert solara.lab.thread_local.reactive_used is None
+
+    t = threading.Thread(target=test1)
+    t.start()
+    t.join()
+
+    def test2():
+        myset: Set[solara.lab.ValueBase] = set()
+        solara.lab.local.reactive_used = myset
+        assert solara.lab.thread_local.reactive_used is myset
+
+    t = threading.Thread(target=test2)
+    t.start()
+    t.join()
+
+    def test3():
+        assert solara.lab.thread_local.reactive_used is None
+
+    t = threading.Thread(target=test3)
+    t.start()
+    t.join()
+
+
+def test_reactive_auto_subscribe(app_context):
+    x = Reactive(1)
+    y = Reactive("hi")
+    extra = Reactive("extra")
+    count = Reactive(1)
+
+    @solara.component
+    def Test():
+        if x.value == 0:
+            _ = extra.value  # access conditional
+        _ = x.value  # access twice
+        return solara.IntSlider(label=y.value, value=x.value)
+
+    @solara.component
+    def Main():
+        for i in range(count.value):
+            Test()
+        if count.value == 0:
+            return solara.Info("no slider")
+
+    box, rc = solara.render(Main(), handle_error=False)
+    assert rc.find(v.Slider).widget.v_model == 1
+    x.value = 2
+    assert rc.find(v.Slider).widget.v_model == 2
+    y.value = "hello"
+    assert rc.find(v.Slider).widget.label == "hello"
+    assert len(x._storage.listeners2) == 1
+    # force an extra listener
+    x.value = 0
+    # and remove it
+    x.value = 1
+
+    count.value = 2
+    assert len(rc.find(v.Slider)) == 2
+    assert len(x._storage.listeners2[app_context.id]) == 2
+    x.value = 3
+    assert rc.find(v.Slider)[0].widget.v_model == 3
+    assert len(x._storage.listeners2[app_context.id]) == 2
+
+    count.value = 1
+    assert len(rc.find(v.Slider)) == 1
+    count.value = 0
+    assert len(rc.find(v.Slider)) == 0
+
+    rc.close()
+    assert not x._storage.listeners[app_context.id]
+    assert not x._storage.listeners2[app_context.id]
+
+
+def test_reactive_auto_subscribe_sub():
+    bears = Reactive(Bears(type="brown", count=1))
+    renders = 0
+
+    @solara.component
+    def Test():
+        nonlocal renders
+        renders += 1
+        count = Ref(bears.fields.count).value
+        return solara.Info(f"{count} bears around here")
+
+    box, rc = solara.render(Test(), handle_error=False)
+    assert rc.find(v.Alert).widget.children[0] == "1 bears around here"
+    Ref(bears.fields.count).value += 1
+    assert rc.find(v.Alert).widget.children[0] == "2 bears around here"
+    # now check that we didn't listen to the while object, just count changes
+    renders_before = renders
+    Ref(bears.fields.type).value = "pink"
+    assert renders == renders_before
+
+
+def test_reactive_auto_subscribe_cleanup(app_context):
+    x = Reactive(1)
+    y = Reactive("hi")
+    renders = 0
+
+    @solara.component
+    def Test():
+        nonlocal renders
+        renders += 1
+        if x.value == 0:
+            _ = y.value  # access conditional
+            x.value = 100
+        return solara.IntSlider("test", value=x.value)
+
+    box, rc = solara.render(Test(), handle_error=False)
+    assert rc.find(v.Slider).widget.v_model == 1
+    assert len(x._storage.listeners2) == 1
+    assert len(y._storage.listeners2) == 0
+    # this triggers two renders, where during the first one we use y, but the seconds we don't
+    x.value = 0
+    assert rc.find(v.Slider).widget.v_model == 100
+    assert len(x._storage.listeners2[app_context.id]) == 1
+    # which means we shouldn't have a listener on y
+    assert len(y._storage.listeners2[app_context.id]) == 0
+
+    rc.close()
+    assert not x._storage.listeners[app_context.id]
+    assert not y._storage.listeners2[app_context.id]
+
+
+def test_reactive_auto_subscribe_subfield_limit(app_context):
+    bears = Reactive(Bears(type="brown", count=1))
+    renders = 0
+
+    @solara.component
+    def Test():
+        nonlocal renders
+        renders += 1
+        _ = bears.value  # access it to trigger the subscription
+        return solara.IntSlider("test", value=Ref(bears.fields.count).value)
+
+    box, rc = solara.render(Test(), handle_error=False)
+    assert rc.find(v.Slider).widget.v_model == 1
+    assert renders == 1
+    Ref(bears.fields.count).value = 2
+    assert renders == 2
+    rc.close()
+    assert not bears._storage.listeners[app_context.id]
+    assert not bears._storage.listeners2[app_context.id]
+
+
+def test_repr():
+    x = Reactive(1)
+    assert repr(x).startswith("<Reactive 1")
+    assert str(x) == "1"
+    y = Reactive("hi")
+    assert repr(y).startswith("<Reactive 'hi'")
+    assert str(y) == "'hi'"
+
+    class Foo:
+        bar = Reactive(1)
+
+    assert repr(Foo.bar).startswith("<Reactive Foo.bar value=1")
+    assert str(Foo.bar) == "Foo.bar=1"
+
+    bears = Reactive(Bears(type="brown", count=1))
+    s = repr(bears.fields.count)
+    assert s.startswith("<Field <Reactive Bears(type='brown', count=1)")
+    assert s.endswith(".count>")
```

### Comparing `solara-1.8.2/tests/unit/pivottable_test.py` & `solara-1.9.0/tests/unit/pivottable_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/router_test.py` & `solara-1.9.0/tests/unit/router_test.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb` & `solara-1.9.0/tests/unit/solara_test_apps/multipage-widgets/04-color.ipynb`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/solara_test_apps/multipage/03-some-markdown.md` & `solara-1.9.0/tests/unit/solara_test_apps/multipage/03-some-markdown.md`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/solara_test_apps/notebookapp_component.ipynb` & `solara-1.9.0/tests/unit/solara_test_apps/notebookapp_component.ipynb`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/solara_test_apps/notebookapp_element.ipynb` & `solara-1.9.0/tests/unit/solara_test_apps/notebookapp_element.ipynb`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/solara_test_apps/notebookapp_widget.ipynb` & `solara-1.9.0/tests/unit/solara_test_apps/notebookapp_widget.ipynb`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tests/unit/telemetry_tests.py` & `solara-1.9.0/tests/unit/telemetry_tests.py`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/tsconfigbase.json` & `solara-1.9.0/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `solara-1.8.2/PKG-INFO` & `solara-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: solara
-Version: 1.8.2
+Version: 1.9.0
 Summary: Build webapps using IPywidgets
 Author-email: "Maarten A. Breddels" <maartenbreddels@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: reacton>=1.2.0
-Requires-Dist: ipywidgets<8
+Requires-Dist: reacton>=1.4.0
+Requires-Dist: ipywidgets
 Requires-Dist: cachetools
 Requires-Dist: filelock
 Requires-Dist: markdown
 Requires-Dist: pygments
 Requires-Dist: pymdown-extensions
 Requires-Dist: markdown-it-py
 Requires-Dist: mdit-py-plugins
 Requires-Dist: humanize
 Requires-Dist: ipyvuetify
-Requires-Dist: ipyvue>=1.8.2
+Requires-Dist: ipyvue>=1.9.0
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: jinja2
 Requires-Dist: MarkupSafe<2.1
 Requires-Dist: pydantic
 Requires-Dist: click>=7.1.0
 Requires-Dist: rich_click
@@ -29,15 +29,17 @@
 Requires-Dist: starlette
 Requires-Dist: nbconvert
 Requires-Dist: jupyter_server
 Requires-Dist: jupyter_client>=7.0.0
 Requires-Dist: watchdog
 Requires-Dist: requests
 Requires-Dist: pygments==2.10; python_version < '3.7'
-Requires-Dist: solara-assets==1.8.2 ; extra == "assets"
+Requires-Dist: nbformat
+Requires-Dist: ipykernel
+Requires-Dist: solara-assets==1.9.0 ; extra == "assets"
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: bqplot ; extra == "dev"
 Requires-Dist: bqplot-image-gl ; extra == "dev"
 Requires-Dist: vaex-core ; extra == "dev"
 Requires-Dist: vaex-hdf5 ; extra == "dev"
 Requires-Dist: vaex-jupyter ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
```

