# Comparing `tmp/openstackdocstheme-3.1.0.tar.gz` & `tmp/openstackdocstheme-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstackdocstheme-3.1.0.tar", last modified: Thu Mar  2 13:37:05 2023, max compression
+gzip compressed data, was "openstackdocstheme-3.1.1.tar", last modified: Tue May 23 08:59:21 2023, max compression
```

## Comparing `openstackdocstheme-3.1.0.tar` & `openstackdocstheme-3.1.1.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17824 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6782 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.753982 openstackdocstheme-3.1.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/api-ref/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.753982 openstackdocstheme-3.1.0/api-ref/source/_static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/api-ref/source/_static/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/_static/css/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/image.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/service.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/api-ref/source/update-server-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/bin/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1160 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/bin/docstheme-build-pdf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7937 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/bin/docstheme-build-translated.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      813 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/bin/docstheme-lang-display-name.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.753982 openstackdocstheme-3.1.0/doc/source/_static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.761984 openstackdocstheme-3.1.0/doc/source/_static/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/_static/css/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.765985 openstackdocstheme-3.1.0/doc/source/demo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7146 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/configure_access_and_security_for_instances.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4896 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/create_and_manage_databases.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3317 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/create_and_manage_networks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6490 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/dashboard_demo.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.765985 openstackdocstheme-3.1.0/doc/source/demo/figures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74714 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/figures/dashboard-project-tab.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    72705 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/figures/dashboard_admin_project_tab.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42821 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/figures/doc-logo-fox.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5254 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/launch-instance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6987 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/demo/section_dashboard_access_and_security.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9089 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.765985 openstackdocstheme-3.1.0/openstackdocstheme/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18703 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/ext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/page_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/paths.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.757983 openstackdocstheme-3.1.0/openstackdocstheme/theme/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.773986 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/css.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/footer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9359 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/header.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3661 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/layout.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/license_cc.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/localtoc.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/os_search.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/os_search_install.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/os_search_mobile.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/script_footer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/script_search.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/search.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc_menu.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5730 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc_menu_apiref.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.773986 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.773986 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   146010 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   121200 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.min.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20236 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/combined.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37414 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31000 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.min.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/search.css
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/favicon.ico
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.777987 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/.gitkeep
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   124988 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/FontAwesome.otf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76518 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   391621 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   152796 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90412 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71896 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20127 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108737 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18028 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff2
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.781988 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.781988 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4739 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/license.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18616 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14372 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12403 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser3.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11727 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser4.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook-hover.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin-hover.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter-hover.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube-hover.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/loading.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-full.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-full.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/search-icon.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.785989 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69707 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37045 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4203 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/docs.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   268039 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    86659 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.min.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/navigation.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/theme.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/titlerow.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.785989 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs_pdf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs_pdf/logo-full.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs_pdf/pdftheme.sty
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.785989 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/footer.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/header.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      570 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu_apiref.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.757983 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.785989 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20236 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/css/combined.css
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.789990 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15123 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15123 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/stx_search.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/stx_search_install.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/stx_search_mobile.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/theme.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/titlerow.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.789990 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/pdftheme.sty
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/openstackdocstheme/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.769986 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9924 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-03-02 13:37:05.000000 openstackdocstheme-3.1.0/openstackdocstheme.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.757983 openstackdocstheme-3.1.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/add-openstackdocs_auto_name-option-efbd1cf9a171f079.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/add-openstackdocs_auto_version-option-fd03f20373eede39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/add-reno-8da9bd3ccb7bbeab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/add-starlingxdocs-10a33318f8630486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/add-translations-9238b0f56b677a6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/allow-disabling-toc-in-body-d98d3a6e633fa28e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/autoconfigure-settings-7083fdeeb121da89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/badge-6f8713da36a7e570.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/bug-project-e9ff50f6149d2be1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/bug-title-fdbefea0408e2cbf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/bug_project-d26160cfe5324694.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/css-cleanup-7fb30a2d1208bb4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/custom-bug-link-ec64bdf9ce357d16.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/disable_analytics-45d98d6fab71d2b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/do-not-display-local-toc-title-without-subtitles-4e1fc48705d66289.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/doc-bug-template-7234e7f00e0ff599.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/double-backticks-not-red-5ce6dbc828221929.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/get_openstack_logo_path-6cdb6538bc5893c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/last-updated-via-git-245fb14be3770a19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/latex_engine-cc35cb3a4ad2fa00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/local-project-search-e6f00a84f2eed0a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/lp1516819-b4bb7b0f10004cef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/merge-latex-options-242f10c932f0e6af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/norelease-ccd7722c078a73a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/opendev-5c528b2b4c737d59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/pdf-version-56c223128dff8357.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/pdf_link-c6b0ed36dd12b0ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/renamed-opts-bbf5d1390ed6ba71.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/side-bar-config-d7e66388e252cadf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/sidebar-top-page-link-252532ddf42a5acf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/sidebar_dropdown_apiref-993b4dba4c0369f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/sidebarlinks-db0a8463f32ab95d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/source_date_epoch-1078730ca0b29a4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/storyboard-5f67da8941aec6ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/storyboard-string-643a47e957b64557.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/storyboard-url-cee60d9449ec2980.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/strip-html-tags-from-navigation-titles-929c92a339413015.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/notes/version-dropdown-1aa39974f524dd75.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9081 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/current.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/historic.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-03-02 13:37:05.797991 openstackdocstheme-3.1.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2758 2023-03-02 13:36:37.000000 openstackdocstheme-3.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2885 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18000 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6782 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1569 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.806409 openstackdocstheme-3.1.1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.814409 openstackdocstheme-3.1.1/api-ref/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.810409 openstackdocstheme-3.1.1/api-ref/source/_static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.814409 openstackdocstheme-3.1.1/api-ref/source/_static/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/_static/css/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3095 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2384 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/image.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/service.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/api-ref/source/update-server-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.814409 openstackdocstheme-3.1.1/bin/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1160 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/bin/docstheme-build-pdf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7937 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/bin/docstheme-build-translated.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      813 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/bin/docstheme-lang-display-name.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.810409 openstackdocstheme-3.1.1/doc/source/_static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/doc/source/_static/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/_static/css/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/doc/source/demo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7146 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/configure_access_and_security_for_instances.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4896 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/create_and_manage_databases.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3317 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/create_and_manage_networks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6490 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/dashboard_demo.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/doc/source/demo/figures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74714 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/figures/dashboard-project-tab.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    72705 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/figures/dashboard_admin_project_tab.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42821 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/figures/doc-logo-fox.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5254 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2788 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/launch-instance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6987 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/demo/section_dashboard_access_and_security.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9089 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.818410 openstackdocstheme-3.1.1/openstackdocstheme/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18703 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/ext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/page_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/paths.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.810409 openstackdocstheme-3.1.1/openstackdocstheme/theme/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.826410 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/css.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/footer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9305 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/header.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3638 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/layout.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/license_cc.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/localtoc.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/os_search.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/os_search_install.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/os_search_mobile.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/script_footer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/script_search.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/search.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2405 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc_menu.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5540 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc_menu_apiref.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.826410 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.826410 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   146010 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   121200 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.min.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20236 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/combined.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37414 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31000 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.min.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/search.css
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/favicon.ico
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.830410 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/.gitkeep
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   124988 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/FontAwesome.otf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76518 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   391621 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   152796 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90412 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71896 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20127 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108737 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18028 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.834411 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.838411 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4739 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/license.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18616 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14372 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12403 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser3.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11727 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser4.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook-hover.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin-hover.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter-hover.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1280 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube-hover.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/loading.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-full.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-full.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/search-icon.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.842411 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69707 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37045 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4203 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/docs.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   268039 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    86659 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.min.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1887 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/navigation.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/theme.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/titlerow.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.842411 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs_pdf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs_pdf/logo-full.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs_pdf/pdftheme.sty
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.842411 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/footer.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/header.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu_apiref.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.810409 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.842411 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20236 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/css/combined.css
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.846411 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15123 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15123 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/stx_search.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/stx_search_install.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/stx_search_mobile.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/theme.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/titlerow.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.846411 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7853 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1807 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/pdftheme.sty
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/openstackdocstheme/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.822410 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2833 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9924 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-05-23 08:59:21.000000 openstackdocstheme-3.1.1/openstackdocstheme.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.810409 openstackdocstheme-3.1.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/add-openstackdocs_auto_name-option-efbd1cf9a171f079.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/add-openstackdocs_auto_version-option-fd03f20373eede39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/add-reno-8da9bd3ccb7bbeab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/add-starlingxdocs-10a33318f8630486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/add-translations-9238b0f56b677a6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/allow-disabling-toc-in-body-d98d3a6e633fa28e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/autoconfigure-settings-7083fdeeb121da89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/badge-6f8713da36a7e570.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/bug-project-e9ff50f6149d2be1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/bug-title-fdbefea0408e2cbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/bug_project-d26160cfe5324694.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/css-cleanup-7fb30a2d1208bb4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/custom-bug-link-ec64bdf9ce357d16.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/disable_analytics-45d98d6fab71d2b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/do-not-display-local-toc-title-without-subtitles-4e1fc48705d66289.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/doc-bug-template-7234e7f00e0ff599.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/double-backticks-not-red-5ce6dbc828221929.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/get_openstack_logo_path-6cdb6538bc5893c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/last-updated-via-git-245fb14be3770a19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/latex_engine-cc35cb3a4ad2fa00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/local-project-search-e6f00a84f2eed0a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/lp1516819-b4bb7b0f10004cef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/merge-latex-options-242f10c932f0e6af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/norelease-ccd7722c078a73a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/opendev-5c528b2b4c737d59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/pdf-version-56c223128dff8357.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/pdf_link-c6b0ed36dd12b0ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/renamed-opts-bbf5d1390ed6ba71.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/side-bar-config-d7e66388e252cadf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/sidebar-top-page-link-252532ddf42a5acf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/sidebar_dropdown_apiref-993b4dba4c0369f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/sidebarlinks-db0a8463f32ab95d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/source_date_epoch-1078730ca0b29a4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/storyboard-5f67da8941aec6ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/storyboard-string-643a47e957b64557.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/storyboard-url-cee60d9449ec2980.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/strip-html-tags-from-navigation-titles-929c92a339413015.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/notes/version-dropdown-1aa39974f524dd75.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:59:21.854412 openstackdocstheme-3.1.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9081 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/current.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3239 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/historic.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-05-23 08:59:21.858412 openstackdocstheme-3.1.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2758 2023-05-23 08:58:29.000000 openstackdocstheme-3.1.1/tox.ini
```

### Comparing `openstackdocstheme-3.1.0/.pre-commit-config.yaml` & `openstackdocstheme-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/.zuul.yaml` & `openstackdocstheme-3.1.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/AUTHORS` & `openstackdocstheme-3.1.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/ChangeLog` & `openstackdocstheme-3.1.1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,1114 +1,1125 @@
 00000000: 4348 414e 4745 530a 3d3d 3d3d 3d3d 3d0a  CHANGES.=======.
-00000010: 0a33 2e31 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .3.1.0.-----..* 
-00000020: 4f6e 6c79 2068 6964 6520 746f 702d 6c65  Only hide top-le
-00000030: 7665 6c20 6475 706c 6963 6174 6564 2074  vel duplicated t
-00000040: 6974 6c65 0a0a 332e 302e 310a 2d2d 2d2d  itle..3.0.1.----
-00000050: 2d0a 0a2a 2055 7064 6174 6520 696e 636c  -..* Update incl
-00000060: 7564 6564 2070 6167 6520 666f 6f74 6572  uded page footer
-00000070: 7320 746f 2075 7365 2063 7572 7265 6e74  s to use current
-00000080: 2055 524c 730a 0a33 2e30 2e30 0a2d 2d2d   URLs..3.0.0.---
-00000090: 2d2d 0a0a 2a20 4472 6f70 2070 7974 686f  --..* Drop pytho
-000000a0: 6e33 2e36 2f33 2e37 2073 7570 706f 7274  n3.6/3.7 support
-000000b0: 2069 6e20 7465 7374 696e 6720 7275 6e74   in testing runt
-000000c0: 696d 650a 2a20 4669 7820 6272 6f6b 656e  ime.* Fix broken
-000000d0: 206c 696e 6b20 666f 7220 4d61 726b 6574   link for Market
-000000e0: 706c 6163 6520 696e 2068 6561 6465 720a  place in header.
-000000f0: 0a32 2e34 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .2.4.0.-----..* 
-00000100: 4669 7820 4f70 656e 5374 6163 6b20 7072  Fix OpenStack pr
-00000110: 6f6a 6563 7420 2253 6561 7263 6822 2070  oject "Search" p
-00000120: 6167 6573 0a0a 322e 332e 310a 2d2d 2d2d  ages..2.3.1.----
-00000130: 2d0a 0a2a 2050 6167 6520 6865 6164 6572  -..* Page header
-00000140: 2066 6978 2077 6974 6820 5370 6869 6e78   fix with Sphinx
-00000150: 340a 0a32 2e33 2e30 0a2d 2d2d 2d2d 0a0a  4..2.3.0.-----..
-00000160: 2a20 496e 6865 7269 7420 6672 6f6d 2062  * Inherit from b
-00000170: 6173 6520 2262 6173 6963 2220 7465 6d70  ase "basic" temp
-00000180: 6c61 7465 0a2a 2073 7068 696e 7820 342e  late.* sphinx 4.
-00000190: 303a 2048 616e 646c 6520 4854 4d4c 2035  0: Handle HTML 5
-000001a0: 2063 6861 6e67 6573 0a2a 2073 7068 696e   changes.* sphin
-000001b0: 7820 342e 303a 2046 6978 2073 7068 696e  x 4.0: Fix sphin
-000001c0: 782e 6578 742e 6578 746c 696e 6b73 2e6d  x.ext.extlinks.m
-000001d0: 616b 655c 5f6c 696e 6b5c 5f72 6f6c 6520  ake\_link\_role 
-000001e0: 6361 6c6c 0a2a 2074 6f78 3a20 546f 6767  call.* tox: Togg
-000001f0: 6c65 2027 7573 6564 6576 656c 6f70 270a  le 'usedevelop'.
-00000200: 2a20 7472 6976 6961 6c3a 2046 6978 2069  * trivial: Fix i
-00000210: 6e64 656e 7461 7469 6f6e 0a2a 2043 6861  ndentation.* Cha
-00000220: 6e67 6520 746f 204f 4654 430a 2a20 7365  nge to OFTC.* se
-00000230: 7475 702e 6366 673a 2052 6570 6c61 6365  tup.cfg: Replace
-00000240: 2064 6173 6865 7320 7769 7468 2075 6e64   dashes with und
-00000250: 6572 7363 6f72 6573 0a2a 204d 6f76 6520  erscores.* Move 
-00000260: 666c 616b 6538 2061 7320 6120 7072 652d  flake8 as a pre-
-00000270: 636f 6d6d 6974 206c 6f63 616c 2074 6172  commit local tar
-00000280: 6765 740a 2a20 5570 6461 7465 6420 4e61  get.* Updated Na
-00000290: 7620 4d65 6e75 0a2a 2055 7365 2054 4f58  v Menu.* Use TOX
-000002a0: 5c5f 434f 4e53 5452 4149 4e54 535c 5f46  \_CONSTRAINTS\_F
-000002b0: 494c 450a 0a32 2e32 2e37 0a2d 2d2d 2d2d  ILE..2.2.7.-----
-000002c0: 0a0a 2a20 4164 6465 6420 7374 796c 696e  ..* Added stylin
-000002d0: 6720 666f 7220 7253 5420 7275 6272 6963  g for rST rubric
-000002e0: 2064 6972 6563 7469 7665 0a0a 322e 322e   directive..2.2.
-000002f0: 360a 2d2d 2d2d 2d0a 0a2a 2043 6861 6e67  6.-----..* Chang
-00000300: 6520 6e61 6d65 206f 6620 4f70 656e 5374  e name of OpenSt
-00000310: 6163 6b20 466f 756e 6461 7469 6f6e 0a2a  ack Foundation.*
-00000320: 2074 7269 7669 616c 3a20 4164 6472 6573   trivial: Addres
-00000330: 7320 736f 6d65 2069 6e64 656e 7461 7469  s some indentati
-00000340: 6f6e 206e 6974 730a 2a20 6a73 3a20 446f  on nits.* js: Do
-00000350: 6e27 7420 6174 7465 6d70 7420 746f 2073  n't attempt to s
-00000360: 6574 2062 7567 2c20 5044 4620 6c69 6e6b  et bug, PDF link
-00000370: 7320 7769 7468 6f75 7420 636f 6e66 6967  s without config
-00000380: 7572 6174 696f 6e0a 2a20 5374 6f72 6520  uration.* Store 
-00000390: 656d 7074 7920 7374 7269 6e67 2066 6f72  empty string for
-000003a0: 2072 656c 6561 7365 0a2a 206a 733a 2053   release.* js: S
-000003b0: 6574 2027 4c49 4e4b 5c5f 5355 4646 4958  et 'LINK\_SUFFIX
-000003c0: 270a 2a20 4164 6469 6e67 2070 7265 2d63  '.* Adding pre-c
-000003d0: 6f6d 6d69 740a 2a20 5265 6d6f 7665 2061  ommit.* Remove a
-000003e0: 736b 2e6f 2e6f 0a0a 322e 322e 350a 2d2d  sk.o.o..2.2.5.--
-000003f0: 2d2d 2d0a 0a2a 2041 6464 2076 6572 7369  ---..* Add versi
-00000400: 6f6e 2064 726f 7064 6f77 6e20 6f6e 2064  on dropdown on d
-00000410: 6f63 732e 7374 6172 6c69 6e67 782e 696f  ocs.starlingx.io
-00000420: 0a0a 322e 322e 340a 2d2d 2d2d 2d0a 0a2a  ..2.2.4.-----..*
-00000430: 2043 6861 6e67 696e 6720 7468 6520 7363   Changing the sc
-00000440: 6f70 6520 6f66 2074 6865 2073 6561 7263  ope of the searc
-00000450: 6820 6261 7220 6f6e 2064 6f63 732e 7374  h bar on docs.st
-00000460: 6172 6c69 6e67 782e 696f 0a0a 322e 322e  arlingx.io..2.2.
-00000470: 330a 2d2d 2d2d 2d0a 0a2a 2041 6464 2070  3.-----..* Add p
-00000480: 7933 3820 7061 636b 6167 6520 6d65 7461  y38 package meta
-00000490: 6461 7461 0a0a 322e 322e 320a 2d2d 2d2d  data..2.2.2.----
-000004a0: 2d0a 0a2a 204c 6f77 6572 206c 6f67 6769  -..* Lower loggi
-000004b0: 6e67 206c 6576 656c 206f 6620 7064 662d  ng level of pdf-
-000004c0: 7265 6c61 7465 6420 6c6f 6773 0a2a 2049  related logs.* I
-000004d0: 676e 6f72 6520 276c 6173 745c 5f75 7064  gnore 'last\_upd
-000004e0: 6174 6564 2720 666f 7220 6175 746f 2d67  ated' for auto-g
-000004f0: 656e 6572 6174 6564 2070 6167 6573 0a2a  enerated pages.*
-00000500: 2046 6978 2068 6163 6b69 6e67 206d 696e   Fix hacking min
-00000510: 2076 6572 7369 6f6e 2074 6f20 332e 302e   version to 3.0.
-00000520: 310a 0a32 2e32 2e31 0a2d 2d2d 2d2d 0a0a  1..2.2.1.-----..
-00000530: 2a20 5368 6f77 2076 6572 7369 6f6e 2069  * Show version i
-00000540: 6e20 5044 4673 0a2a 2041 6464 206f 6374  n PDFs.* Add oct
-00000550: 6176 6961 636c 6965 6e74 2063 726f 7373  aviaclient cross
-00000560: 206a 6f62 0a2a 2046 6978 2061 7574 6f5c   job.* Fix auto\
-00000570: 5f6e 616d 6520 6c6f 6769 630a 0a32 2e32  _name logic..2.2
-00000580: 2e30 0a2d 2d2d 2d2d 0a0a 2a20 4164 6420  .0.-----..* Add 
-00000590: 6c69 6e6b 2074 6f20 5044 4620 6669 6c65  link to PDF file
-000005a0: 0a2a 2043 6c65 616e 7570 2062 696e 6465  .* Cleanup binde
-000005b0: 700a 2a20 4164 6420 6372 6f73 732d 7465  p.* Add cross-te
-000005c0: 7374 7320 666f 7220 6e6f 7661 0a2a 2045  sts for nova.* E
-000005d0: 6e61 626c 6520 7061 7261 6c6c 656c 2062  nable parallel b
-000005e0: 7569 6c64 696e 670a 2a20 5573 6520 636f  uilding.* Use co
-000005f0: 6e73 6973 7465 6e74 206c 6f67 6769 6e67  nsistent logging
-00000600: 0a2a 2074 7269 7669 616c 3a20 5265 6d6f  .* trivial: Remo
-00000610: 7665 206c 6566 746f 7665 7220 5079 7468  ve leftover Pyth
-00000620: 6f6e 2032 2063 6f64 650a 2a20 5072 6f76  on 2 code.* Prov
-00000630: 6964 6520 6578 7465 6e73 696f 6e20 7665  ide extension ve
-00000640: 7273 696f 6e0a 0a32 2e31 2e32 0a2d 2d2d  rsion..2.1.2.---
-00000650: 2d2d 0a0a 2a20 5570 6461 7465 2064 6f63  --..* Update doc
-00000660: 7374 6865 6d65 0a2a 2055 7365 2078 656c  stheme.* Use xel
-00000670: 6174 6578 2061 7320 6c61 7465 785c 5f65  atex as latex\_e
-00000680: 6e67 696e 650a 0a32 2e31 2e31 0a2d 2d2d  ngine..2.1.1.---
-00000690: 2d2d 0a0a 2a20 5265 7374 6f72 6520 636f  --..* Restore co
-000006a0: 6e66 6967 7572 6174 696f 6e20 6f66 2027  nfiguration of '
-000006b0: 6c61 7465 785c 5f65 6e67 696e 6527 0a0a  latex\_engine'..
-000006c0: 322e 312e 300a 2d2d 2d2d 2d0a 0a2a 2074  2.1.0.-----..* t
-000006d0: 7269 7669 616c 3a20 4164 6420 7768 6974  rivial: Add whit
-000006e0: 6573 7061 6365 0a2a 2041 6464 2070 6163  espace.* Add pac
-000006f0: 6b61 6765 2070 7265 6669 7865 7320 666f  kage prefixes fo
-00000700: 7220 616c 6c20 636f 6e66 6967 206f 7074  r all config opt
-00000710: 696f 6e73 0a2a 2052 656d 6f76 6520 7665  ions.* Remove ve
-00000720: 6e64 6f72 6564 2027 6e61 7469 7665 2720  ndored 'native' 
-00000730: 5079 676d 656e 7473 2074 6865 6d65 0a2a  Pygments theme.*
-00000740: 2063 7373 3a20 4e61 6d65 7370 6163 6520   css: Namespace 
-00000750: 5079 676d 656e 7473 2073 7479 6c65 7368  Pygments stylesh
-00000760: 6565 740a 2a20 4d65 7267 652c 2072 6174  eet.* Merge, rat
-00000770: 6865 7220 7468 616e 206f 7665 7277 7269  her than overwri
-00000780: 7465 2c20 4c61 5465 5820 7365 7474 696e  te, LaTeX settin
-00000790: 6773 0a2a 2041 6464 2027 6f70 656e 7374  gs.* Add 'openst
-000007a0: 6163 6b64 6f63 735c 5f61 7574 6f5c 5f6e  ackdocs\_auto\_n
-000007b0: 616d 6527 2063 6f6e 6669 6720 6f70 7469  ame' config opti
-000007c0: 6f6e 0a2a 2041 6464 2027 6f70 656e 7374  on.* Add 'openst
-000007d0: 6163 6b64 6f63 735c 5f61 7574 6f5c 5f76  ackdocs\_auto\_v
-000007e0: 6572 7369 6f6e 2720 636f 6e66 6967 206f  ersion' config o
-000007f0: 7074 696f 6e2c 2070 6174 6820 6368 6563  ption, path chec
-00000800: 6b69 6e67 0a2a 204d 6172 6b20 7370 6869  king.* Mark sphi
-00000810: 6e78 2065 7874 656e 7369 6f6e 7320 7468  nx extensions th
-00000820: 7265 6164 2073 6166 650a 0a32 2e30 2e32  read safe..2.0.2
-00000830: 0a2d 2d2d 2d2d 0a0a 2a20 5570 6461 7465  .-----..* Update
-00000840: 2068 6163 6b69 6e67 2066 6f72 2050 7974   hacking for Pyt
-00000850: 686f 6e33 0a0a 322e 302e 310a 2d2d 2d2d  hon3..2.0.1.----
-00000860: 2d0a 0a2a 2055 7064 6174 6520 7365 7665  -..* Update seve
-00000870: 7261 6c20 6c69 6e6b 730a 2a20 446f 206e  ral links.* Do n
-00000880: 6f74 2073 6574 2068 746d 6c5c 5f6c 6173  ot set html\_las
-00000890: 745c 5f75 7064 6174 6564 5c5f 666d 740a  t\_updated\_fmt.
-000008a0: 0a32 2e30 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .2.0.0.-----..* 
-000008b0: 4669 7820 6272 6f6b 656e 2055 524c 730a  Fix broken URLs.
-000008c0: 2a20 5b75 7373 7572 695d 5b67 6f61 6c5d  * [ussuri][goal]
-000008d0: 2044 726f 7020 7079 7468 6f6e 2032 2e37   Drop python 2.7
-000008e0: 2073 7570 706f 7274 2061 6e64 2074 6573   support and tes
-000008f0: 7469 6e67 0a0a 312e 3331 2e32 0a2d 2d2d  ting..1.31.2.---
-00000900: 2d2d 2d0a 0a2a 204d 6f76 6520 7665 7273  ---..* Move vers
-00000910: 696f 6e20 6472 6f70 646f 776e 2074 6f20  ion dropdown to 
-00000920: 7469 746c 6520 6c69 6e65 0a2a 2049 6d70  title line.* Imp
-00000930: 726f 7665 2064 6f63 7320 7469 746c 6520  rove docs title 
-00000940: 7374 796c 650a 2a20 4665 7463 6820 6765  style.* Fetch ge
-00000950: 6e65 7261 7465 6420 5044 4620 6669 6c65  nerated PDF file
-00000960: 7320 636f 7272 6563 746c 790a 2a20 4361  s correctly.* Ca
-00000970: 7463 6820 616e 7920 6578 6365 7074 696f  tch any exceptio
-00000980: 6e20 7768 656e 2074 7279 696e 6720 746f  n when trying to
-00000990: 2063 616c 6c20 2267 6974 220a 0a31 2e33   call "git"..1.3
-000009a0: 312e 310a 2d2d 2d2d 2d2d 0a0a 2a20 4669  1.1.------..* Fi
-000009b0: 7820 7665 7273 696f 6e20 6472 6f70 646f  x version dropdo
-000009c0: 776e 0a0a 312e 3331 2e30 0a2d 2d2d 2d2d  wn..1.31.0.-----
-000009d0: 2d0a 0a2a 2055 7064 6174 6520 4150 4920  -..* Update API 
-000009e0: 7369 6465 6261 720a 2a20 5570 6461 7465  sidebar.* Update
-000009f0: 2061 7069 2d72 6566 206c 6f63 6174 696f   api-ref locatio
-00000a00: 6e0a 2a20 4d61 6b65 2027 646f 6373 7468  n.* Make 'docsth
-00000a10: 656d 652d 6275 696c 642d 7064 6627 2065  eme-build-pdf' e
-00000a20: 7865 6375 7461 626c 650a 2a20 4164 6420  xecutable.* Add 
-00000a30: 2764 6f63 7374 6865 6d65 2d62 7569 6c64  'docstheme-build
-00000a40: 2d70 6466 2720 7363 7269 7074 0a2a 2073  -pdf' script.* s
-00000a50: 6574 7570 2e63 6667 3a20 5265 6d6f 7665  etup.cfg: Remove
-00000a60: 2072 656d 616e 656e 7473 206f 6620 2762   remanents of 'b
-00000a70: 7569 6c64 5c5f 7370 6869 6e78 2720 7573  uild\_sphinx' us
-00000a80: 6167 650a 2a20 4164 6420 6d69 7373 696e  age.* Add missin
-00000a90: 6720 2772 6f6c 653d 226d 6169 6e22 2720  g 'role="main"' 
-00000aa0: 6174 7472 6962 7574 650a 2a20 6373 733a  attribute.* css:
-00000ab0: 2047 656e 6572 616c 2063 6c65 616e 7570   General cleanup
-00000ac0: 0a2a 206a 733a 2046 6978 2073 6f6d 6520  .* js: Fix some 
-00000ad0: 636f 6d6d 656e 7473 0a2a 206a 733a 2052  comments.* js: R
-00000ae0: 656d 6f76 6520 6465 6164 206f 7220 756e  emove dead or un
-00000af0: 7573 6564 204a 530a 2a20 4164 6420 7265  used JS.* Add re
-00000b00: 6e6f 2066 6f72 2072 6563 656e 7420 4353  no for recent CS
-00000b10: 5320 636c 6561 6e75 7073 0a2a 204e 6f74  S cleanups.* Not
-00000b20: 6520 4578 7465 726e 616c 204c 696e 6b20  e External Link 
-00000b30: 4865 6c70 6572 2069 7320 6e6f 7420 636f  Helper is not co
-00000b40: 6d70 6174 6962 6c65 2077 6974 6820 7072  mpatible with pr
-00000b50: 6f6a 6563 7420 6f6e 6c79 206d 6173 7465  oject only maste
-00000b60: 7220 6272 6163 680a 2a20 5265 6d6f 7665  r brach.* Remove
-00000b70: 2061 2068 6561 7020 6f66 2064 6561 6420   a heap of dead 
-00000b80: 4353 5320 7275 6c65 730a 2a20 5265 6d6f  CSS rules.* Remo
-00000b90: 7665 6420 2763 6f6d 6269 6e65 642e 6373  ved 'combined.cs
-00000ba0: 7327 2066 6f72 2027 7374 6172 6c69 6e67  s' for 'starling
-00000bb0: 7864 6f63 7327 2074 6865 6d65 0a2a 2063  xdocs' theme.* c
-00000bc0: 7373 3a20 4164 6420 7379 6d6c 696e 6b73  ss: Add symlinks
-00000bd0: 2066 6f72 206f 7065 6e73 7461 636b 206c   for openstack l
-00000be0: 6f67 6f73 0a2a 2063 7373 3a20 4d6f 7665  ogos.* css: Move
-00000bf0: 2062 6f6f 7473 7472 6170 206d 6f64 6966   bootstrap modif
-00000c00: 6963 6174 696f 6e73 2074 6f20 2763 6f6d  ications to 'com
-00000c10: 6269 6e65 642e 6373 7327 2028 5374 6172  bined.css' (Star
-00000c20: 6c69 6e67 5829 0a2a 2063 7373 3a20 5573  lingX).* css: Us
-00000c30: 6520 656c 6c69 7073 6973 2066 6f72 206c  e ellipsis for l
-00000c40: 6f6e 6720 7469 746c 6573 2069 6e20 7369  ong titles in si
-00000c50: 6465 6261 7220 2853 7461 726c 696e 6758  debar (StarlingX
-00000c60: 290a 2a20 6373 733a 2055 7365 2068 7474  ).* css: Use htt
-00000c70: 7073 206c 696e 6b73 2028 5374 6172 6c69  ps links (Starli
-00000c80: 6e67 5829 0a2a 2063 7373 3a20 446f 6e27  ngX).* css: Don'
-00000c90: 7420 7573 6520 626f 6c64 2074 6578 7420  t use bold text 
-00000ca0: 696e 2074 6974 6c65 7320 2853 7461 726c  in titles (Starl
-00000cb0: 696e 6758 290a 0a31 2e33 302e 300a 2d2d  ingX)..1.30.0.--
-00000cc0: 2d2d 2d2d 0a0a 2a20 4164 6420 7461 626c  ----..* Add tabl
-00000cd0: 6520 7374 796c 696e 670a 2a20 416c 6c6f  e styling.* Allo
-00000ce0: 7720 746f 206f 7665 7272 6964 6520 6275  w to override bu
-00000cf0: 696c 6420 6461 7465 2077 6974 6820 534f  ild date with SO
-00000d00: 5552 4345 5c5f 4441 5445 5c5f 4550 4f43  URCE\_DATE\_EPOC
-00000d10: 480a 2a20 5265 6665 7265 6e63 6520 4f70  H.* Reference Op
-00000d20: 656e 5374 6163 6b20 6c6f 676f 2069 6e20  enStack logo in 
-00000d30: 6f70 656e 7374 6163 6b64 6f63 7374 6865  openstackdocsthe
-00000d40: 6d65 0a0a 312e 3239 2e33 0a2d 2d2d 2d2d  me..1.29.3.-----
-00000d50: 2d0a 0a2a 2055 7064 6174 6520 666f 7220  -..* Update for 
-00000d60: 4f70 656e 4465 7620 6368 616e 6765 0a2a  OpenDev change.*
-00000d70: 2050 7265 7665 6e74 2049 6e76 6f63 6174   Prevent Invocat
-00000d80: 696f 6e45 7272 6f72 206f 6e20 6e6f 6e2d  ionError on non-
-00000d90: 6578 6973 7465 6e74 2066 696c 6573 0a2a  existent files.*
-00000da0: 204f 7065 6e44 6576 204d 6967 7261 7469   OpenDev Migrati
-00000db0: 6f6e 2050 6174 6368 0a2a 2041 6464 206d  on Patch.* Add m
-00000dc0: 6973 7369 6e67 2066 6f6e 7473 2066 6f72  issing fonts for
-00000dd0: 2070 6466 2062 7569 6c64 2069 6e20 5370   pdf build in Sp
-00000de0: 6869 6e78 2032 2e30 0a0a 312e 3239 2e32  hinx 2.0..1.29.2
-00000df0: 0a2d 2d2d 2d2d 2d0a 0a2a 204d 6f76 6520  .------..* Move 
-00000e00: 626f 6f74 7374 7261 7020 6d6f 6469 6669  bootstrap modifi
-00000e10: 6361 7469 6f6e 7320 746f 2027 636f 6d62  cations to 'comb
-00000e20: 696e 6564 2e63 7373 270a 2a20 6373 733a  ined.css'.* css:
-00000e30: 2044 6f6e 2774 2075 7365 2062 6f6c 6420   Don't use bold 
-00000e40: 7465 7874 2069 6e20 7469 746c 6573 0a2a  text in titles.*
-00000e50: 2063 7373 3a20 5573 6520 656c 6c69 7073   css: Use ellips
-00000e60: 6973 2066 6f72 206c 6f6e 6720 7469 746c  is for long titl
-00000e70: 6573 2069 6e20 7369 6465 6261 720a 2a20  es in sidebar.* 
-00000e80: 5369 6c65 6e63 6521 2041 2073 6571 7565  Silence! A seque
-00000e90: 6c0a 2a20 5369 6c65 6e63 6521 0a0a 312e  l.* Silence!..1.
-00000ea0: 3239 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 2046  29.1.------..* F
-00000eb0: 6978 2077 726f 6e67 2076 6172 6961 626c  ix wrong variabl
-00000ec0: 6520 696e 2062 7569 6c64 2d74 7261 6e73  e in build-trans
-00000ed0: 6c61 7465 640a 2a20 4578 6974 2074 7261  lated.* Exit tra
-00000ee0: 7020 636c 6561 6e75 7020 696e 2064 6f63  p cleanup in doc
-00000ef0: 7374 6865 6d65 2d62 7569 6c64 2d74 7261  stheme-build-tra
-00000f00: 6e73 6c61 7465 642e 7368 0a0a 312e 3239  nslated.sh..1.29
-00000f10: 2e30 0a2d 2d2d 2d2d 2d0a 0a0a 312e 3238  .0.------...1.28
-00000f20: 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 2043 6174  .1.------..* Cat
-00000f30: 6368 204f 5345 7272 6f72 2077 6865 6e20  ch OSError when 
-00000f40: 7472 7969 6e67 2074 6f20 6765 7420 7468  trying to get th
-00000f50: 6520 6c61 7374 5c5f 7570 6461 7465 2066  e last\_update f
-00000f60: 726f 6d20 6769 740a 2a20 4164 6420 6f70  rom git.* Add op
-00000f70: 7469 6f6e 7320 666f 7220 7370 6869 6e78  tions for sphinx
-00000f80: 2d62 7569 6c64 202d 5720 696e 2064 6f63  -build -W in doc
-00000f90: 7374 6865 6d65 2d62 7569 6c64 2d74 7261  stheme-build-tra
-00000fa0: 6e73 6c61 7465 642e 7368 0a2a 2054 7261  nslated.sh.* Tra
-00000fb0: 6e73 6c61 7469 6f6e 733a 2048 616e 646c  nslations: Handl
-00000fc0: 6520 6469 7265 6374 6f72 6965 730a 2a20  e directories.* 
-00000fd0: 5570 6461 7465 2068 6163 6b69 6e67 2076  Update hacking v
-00000fe0: 6572 7369 6f6e 0a0a 312e 3238 2e30 0a2d  ersion..1.28.0.-
-00000ff0: 2d2d 2d2d 2d0a 0a2a 2043 6861 6e67 6520  -----..* Change 
-00001000: 6f70 656e 7374 6163 6b2d 6465 7620 746f  openstack-dev to
-00001010: 206f 7065 6e73 7461 636b 2d64 6973 6375   openstack-discu
-00001020: 7373 0a2a 2075 7365 2067 6974 206d 6f64  ss.* use git mod
-00001030: 6966 6963 6174 696f 6e20 7469 6d65 7374  ification timest
-00001040: 616d 7073 2061 7320 6c61 7374 2d75 7064  amps as last-upd
-00001050: 6174 6564 2074 696d 6520 666f 7220 6561  ated time for ea
-00001060: 6368 2070 6167 650a 2a20 496d 706f 7274  ch page.* Import
-00001070: 2074 6f6f 6c73 2066 6f72 2062 7569 6c64   tools for build
-00001080: 696e 6720 7472 616e 736c 6174 6564 2064  ing translated d
-00001090: 6f63 756d 656e 7473 0a2a 2046 6978 2074  ocuments.* Fix t
-000010a0: 7970 6f0a 2a20 5265 6d6f 7665 2073 6574  ypo.* Remove set
-000010b0: 7570 2e70 7920 6368 6563 6b20 6672 6f6d  up.py check from
-000010c0: 2070 6570 3820 6a6f 620a 2a20 5374 6172   pep8 job.* Star
-000010d0: 6c69 6e67 5820 6e61 7620 6669 7820 746f  lingX nav fix to
-000010e0: 2072 656d 6f76 6520 2253 6f66 7477 6172   remove "Softwar
-000010f0: 6520 5570 6461 7465 2220 6c69 6e6b 730a  e Update" links.
-00001100: 0a31 2e32 372e 310a 2d2d 2d2d 2d2d 0a0a  .1.27.1.------..
-00001110: 2a20 5468 6520 7468 656d 6520 6973 206f  * The theme is o
-00001120: 7065 6e73 7461 636b 646f 6373 0a0a 312e  penstackdocs..1.
-00001130: 3237 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2052  27.0.------..* R
-00001140: 6561 6464 2067 6574 5c5f 6f70 656e 7374  eadd get\_openst
-00001150: 6163 6b5c 5f6c 6f67 6f5c 5f70 6174 680a  ack\_logo\_path.
-00001160: 2a20 5365 7420 6465 6661 756c 7420 7061  * Set default pa
-00001170: 7468 7320 666f 7220 4f70 656e 5374 6163  ths for OpenStac
-00001180: 6b0a 0a31 2e32 362e 300a 2d2d 2d2d 2d2d  k..1.26.0.------
-00001190: 0a0a 2a20 4d61 6b65 2061 2062 6172 652d  ..* Make a bare-
-000011a0: 626f 6e65 7320 7374 6172 6c69 6e67 7864  bones starlingxd
-000011b0: 6f63 7320 7468 656d 650a 2a20 4164 6420  ocs theme.* Add 
-000011c0: 7363 7269 7074 7320 746f 2074 6865 2068  scripts to the h
-000011d0: 6561 6420 7365 6374 696f 6e0a 2a20 5265  ead section.* Re
-000011e0: 6d6f 7665 2065 7861 6d70 6c65 206f 6620  move example of 
-000011f0: 6465 7072 6563 6174 6564 2061 7070 2e69  deprecated app.i
-00001200: 6e66 6f0a 2a20 4164 6420 7374 6172 6c69  nfo.* Add starli
-00001210: 6e67 7864 6f63 7320 7468 656d 6520 7375  ngxdocs theme su
-00001220: 7070 6f72 740a 0a31 2e32 352e 310a 2d2d  pport..1.25.1.--
-00001230: 2d2d 2d2d 0a0a 2a20 4669 7820 7265 6772  ----..* Fix regr
-00001240: 6573 7369 6f6e 7320 696e 7472 6f64 7563  essions introduc
-00001250: 6564 2069 6e20 312e 3235 2e30 0a0a 312e  ed in 1.25.0..1.
-00001260: 3235 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2041  25.0.------..* A
-00001270: 6464 2061 6e20 6f70 7469 6f6e 2074 6f20  dd an option to 
-00001280: 6469 7361 626c 6520 676c 6f62 616c 2054  disable global T
-00001290: 4f43 2073 6563 7469 6f6e 0a2a 204d 616b  OC section.* Mak
-000012a0: 6520 726f 6f74 2074 6974 6c65 2063 7573  e root title cus
-000012b0: 746f 6d69 7a61 626c 650a 2a20 496d 706f  tomizable.* Impo
-000012c0: 7274 2062 7569 6c64 2d6f 7065 6e73 7461  rt build-opensta
-000012d0: 636b 2d61 7069 2d72 6566 0a0a 312e 3234  ck-api-ref..1.24
-000012e0: 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 206c 6f67  .1.------..* log
-000012f0: 2064 6574 6169 6c73 206f 6620 6874 6d6c   details of html
-00001300: 2063 6f6e 7465 7874 0a2a 2070 6173 7320   context.* pass 
-00001310: 7573 6553 746f 7279 626f 6172 6420 746f  useStoryboard to
-00001320: 206c 6f67 4142 7567 0a2a 2065 6e73 7572   logABug.* ensur
-00001330: 6520 7265 706f 7369 746f 7279 5c5f 6e61  e repository\_na
-00001340: 6d65 2069 7320 616c 7761 7973 2073 6574  me is always set
-00001350: 0a0a 312e 3234 2e30 0a2d 2d2d 2d2d 2d0a  ..1.24.0.------.
-00001360: 0a2a 2046 6978 2074 6865 2069 6e63 6f72  .* Fix the incor
-00001370: 7265 6374 2073 746f 7279 626f 6172 6420  rect storyboard 
-00001380: 7572 6c0a 2a20 4669 7820 7072 6f6a 6563  url.* Fix projec
-00001390: 742d 6e61 7669 6761 746f 7220 6c69 6e6b  t-navigator link
-000013a0: 0a0a 312e 3233 2e32 0a2d 2d2d 2d2d 2d0a  ..1.23.2.------.
-000013b0: 0a2a 2046 6978 2075 7365 5c5f 7374 6f72  .* Fix use\_stor
-000013c0: 7962 6f61 7264 0a0a 312e 3233 2e31 0a2d  yboard..1.23.1.-
-000013d0: 2d2d 2d2d 2d0a 0a2a 2048 616e 646c 6520  -----..* Handle 
-000013e0: 5374 6f72 7942 6f61 7264 2070 726f 6a65  StoryBoard proje
-000013f0: 6374 2067 726f 7570 730a 2a20 446f 206e  ct groups.* Do n
-00001400: 6f74 2073 686f 7720 6261 6467 6520 666f  ot show badge fo
-00001410: 7220 6d61 7374 6572 206f 6e6c 7920 7265  r master only re
-00001420: 706f 730a 0a31 2e32 332e 300a 2d2d 2d2d  pos..1.23.0.----
-00001430: 2d2d 0a0a 2a20 4669 7820 6275 696c 6420  --..* Fix build 
-00001440: 6a6f 6273 0a2a 2044 6f20 6e6f 7420 6469  jobs.* Do not di
-00001450: 7370 6c61 7920 226c 6174 6573 7422 2062  splay "latest" b
-00001460: 6164 6765 2069 6620 7265 706f 2069 7320  adge if repo is 
-00001470: 6e6f 7420 7665 7273 696f 6e65 640a 2a20  not versioned.* 
-00001480: 5573 6520 7370 6869 6e78 2d62 7569 6c64  Use sphinx-build
-00001490: 2065 7665 7279 7768 6572 650a 2a20 7377   everywhere.* sw
-000014a0: 6974 6368 2064 6f63 756d 656e 7461 7469  itch documentati
-000014b0: 6f6e 206a 6f62 2074 6f20 6e65 7720 5054  on job to new PT
-000014c0: 490a 2a20 696d 706f 7274 207a 7575 6c20  I.* import zuul 
-000014d0: 6a6f 6220 7365 7474 696e 6773 2066 726f  job settings fro
-000014e0: 6d20 7072 6f6a 6563 742d 636f 6e66 6967  m project-config
-000014f0: 0a0a 312e 3232 2e30 0a2d 2d2d 2d2d 2d0a  ..1.22.0.------.
-00001500: 0a0a 312e 3231 2e32 0a2d 2d2d 2d2d 2d0a  ..1.21.2.------.
-00001510: 0a2a 204d 616b 6520 6267 2063 6f6c 6f72  .* Make bg color
-00001520: 2066 6f72 2068 6967 686c 6967 6874 6564   for highlighted
-00001530: 2074 6578 7420 6c65 7373 2062 7269 6768   text less brigh
-00001540: 740a 2a20 6967 6e6f 7265 2066 696c 6573  t.* ignore files
-00001550: 2063 7265 6174 6564 2064 7572 696e 6720   created during 
-00001560: 7061 636b 6167 696e 670a 2a20 4164 6465  packaging.* Adde
-00001570: 6420 6465 7072 6563 6174 696f 6e20 6261  d deprecation ba
-00001580: 6467 650a 0a31 2e32 312e 310a 2d2d 2d2d  dge..1.21.1.----
-00001590: 2d2d 0a0a 2a20 4d61 6b65 2065 6d70 6861  --..* Make empha
-000015a0: 7369 7a65 2d6c 696e 6573 206d 6f72 6520  size-lines more 
-000015b0: 6869 6768 6c69 6768 7465 640a 2a20 5570  highlighted.* Up
-000015c0: 6461 7465 6420 5365 6172 6368 2077 6964  dated Search wid
-000015d0: 6765 740a 2a20 6669 7820 746f 7820 7079  get.* fix tox py
-000015e0: 7468 6f6e 3320 6f76 6572 7269 6465 730a  thon3 overrides.
-000015f0: 2a20 6164 6420 7468 6520 7365 7269 6573  * add the series
-00001600: 206e 616d 6520 746f 2074 6865 2074 656d   name to the tem
-00001610: 706c 6174 6520 636f 6e74 6578 740a 2a20  plate context.* 
-00001620: 616c 7761 7973 206c 6f6f 6b20 666f 7220  always look for 
-00001630: 7468 6520 2e67 6974 7265 7669 6577 2066  the .gitreview f
-00001640: 696c 6520 696e 2072 6f6f 7420 6f66 2072  ile in root of r
-00001650: 6570 6f0a 2a20 5374 7269 7020 7461 6773  epo.* Strip tags
-00001660: 2066 726f 6d20 7469 746c 6573 2069 6e20   from titles in 
-00001670: 6275 6754 6974 6c65 2061 6e64 206d 6574  bugTitle and met
-00001680: 610a 2a20 4368 6563 6b20 5253 5420 6173  a.* Check RST as
-00001690: 2070 6172 7420 6f66 206c 696e 7469 6e67   part of linting
-000016a0: 0a0a 312e 3231 2e30 0a2d 2d2d 2d2d 2d0a  ..1.21.0.------.
-000016b0: 0a2a 2055 7365 206d 6574 6164 6174 6120  .* Use metadata 
-000016c0: 7375 6d6d 6172 7920 696e 7374 6561 6420  summary instead 
-000016d0: 6e61 6d65 2066 6f72 2064 6f63 2074 6974  name for doc tit
-000016e0: 6c65 0a2a 2052 656c 6f63 6174 6520 6275  le.* Relocate bu
-000016f0: 675c 5f74 6167 2069 6e20 6c6f 6741 4275  g\_tag in logABu
-00001700: 6720 6765 6e65 7261 7465 6420 5552 4c0a  g generated URL.
-00001710: 0a31 2e32 302e 310a 2d2d 2d2d 2d2d 0a0a  .1.20.1.------..
-00001720: 2a20 4861 6e64 6c65 2070 6f73 7369 626c  * Handle possibl
-00001730: 6520 6578 6365 7074 696f 6e73 2077 6865  e exceptions whe
-00001740: 6e20 6665 7463 6869 6e67 2076 6572 7369  n fetching versi
-00001750: 6f6e 206e 756d 6265 7273 0a0a 312e 3230  on numbers..1.20
-00001760: 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2055 7064  .0.------..* Upd
-00001770: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
-00001780: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
-00001790: 436f 6e66 6967 7572 6520 6164 6469 7469  Configure additi
-000017a0: 6f6e 616c 2070 726f 7065 7274 6965 730a  onal properties.
-000017b0: 2a20 436f 6e66 6967 7572 6520 7072 6f6a  * Configure proj
-000017c0: 6563 7420 6e61 6d65 2c20 7665 7273 696f  ect name, versio
-000017d0: 6e2c 2072 656c 6561 7365 0a2a 2074 7269  n, release.* tri
-000017e0: 7669 616c 3a20 5265 6d6f 7665 2063 7275  vial: Remove cru
-000017f0: 6674 2066 726f 6d20 2763 6f6e 662e 7079  ft from 'conf.py
-00001800: 270a 2a20 7472 6976 6961 6c3a 2055 7365  '.* trivial: Use
-00001810: 2074 6865 2027 6765 745c 5f68 746d 6c5c   the 'get\_html\
-00001820: 5f74 6865 6d65 5c5f 7061 7468 2720 6675  _theme\_path' fu
-00001830: 6e63 7469 6f6e 0a2a 204d 6f76 6520 636f  nction.* Move co
-00001840: 6465 206f 7574 206f 6620 275c 5f5c 5f69  de out of '\_\_i
-00001850: 6e69 745c 5f5c 5f27 0a2a 204d 6172 6b20  nit\_\_'.* Mark 
-00001860: 736f 6d65 2066 756e 6374 696f 6e73 2061  some functions a
-00001870: 7320 7072 6976 6174 650a 0a31 2e31 392e  s private..1.19.
-00001880: 300a 2d2d 2d2d 2d2d 0a0a 2a20 7472 6976  0.------..* triv
-00001890: 6961 6c3a 2047 656e 6572 6174 6520 277b  ial: Generate '{
-000018a0: 7072 6f6a 6563 747d 2d64 6f63 2720 726f  project}-doc' ro
-000018b0: 6c65 732c 206e 6f74 2027 7b70 726f 6a65  les, not '{proje
-000018c0: 6374 7d2d 646f 632d 6c69 6e6b 270a 2a20  ct}-doc-link'.* 
-000018d0: 4176 6f69 6420 7465 7874 206f 7665 7266  Avoid text overf
-000018e0: 6c6f 7720 696e 2074 6f63 0a2a 2046 6978  low in toc.* Fix
-000018f0: 2074 7970 6f20 696e 206c 6f67 6765 722e   typo in logger.
-00001900: 7761 726e 696e 6728 2920 6361 6c6c 0a2a  warning() call.*
-00001910: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
-00001920: 7265 6174 6520 7072 6f6a 6563 7420 646f  reate project do
-00001930: 632d 6c69 6e6b 2072 6f6c 6573 0a2a 2052  c-link roles.* R
-00001940: 656d 6f76 6520 6e61 6d65 2066 726f 6d20  emove name from 
-00001950: 7072 6f6a 6563 7420 7374 616e 7a61 0a2a  project stanza.*
-00001960: 2055 7064 6174 6564 2066 726f 6d20 676c   Updated from gl
-00001970: 6f62 616c 2072 6571 7569 7265 6d65 6e74  obal requirement
-00001980: 730a 2a20 5570 6461 7465 2074 6865 2064  s.* Update the d
-00001990: 6573 6372 6970 7469 6f6e 206f 6620 2267  escription of "g
-000019a0: 6974 7572 6c22 0a0a 312e 3138 2e31 0a2d  iturl"..1.18.1.-
-000019b0: 2d2d 2d2d 2d0a 0a2a 2046 6978 2067 6974  -----..* Fix git
-000019c0: 7572 6c20 7061 7273 696e 670a 0a31 2e31  url parsing..1.1
-000019d0: 382e 300a 2d2d 2d2d 2d2d 0a0a 2a20 5265  8.0.------..* Re
-000019e0: 706c 6163 6520 7468 6520 6874 7470 206c  place the http l
-000019f0: 696e 6b73 2077 6974 6820 7468 6520 7269  inks with the ri
-00001a00: 6768 7420 6f6e 6573 2069 6e20 646f 6373  ght ones in docs
-00001a10: 0a2a 2041 7474 656d 7074 2074 6f20 6775  .* Attempt to gu
-00001a20: 6573 7320 7661 6c69 6420 4769 7420 5552  ess valid Git UR
-00001a30: 4c73 0a2a 2052 6576 6572 7420 2246 6978  Ls.* Revert "Fix
-00001a40: 2074 6865 2069 6e63 6f72 7265 6374 2067   the incorrect g
-00001a50: 6974 2073 6f75 7263 6520 7572 6c22 0a2a  it source url".*
-00001a60: 2074 7269 7669 616c 3a20 5265 6d6f 7665   trivial: Remove
-00001a70: 2075 7365 206f 6620 2741 7070 6c69 6361   use of 'Applica
-00001a80: 7469 6f6e 2e7b 7761 726e 2c69 6e66 6f7d  tion.{warn,info}
-00001a90: 270a 2a20 4669 7820 7468 6520 696e 636f  '.* Fix the inco
-00001aa0: 7272 6563 7420 6769 7420 736f 7572 6365  rrect git source
-00001ab0: 2075 726c 0a2a 2044 6f20 6e6f 7420 7072   url.* Do not pr
-00001ac0: 696e 7420 7468 6520 7265 6c65 6173 6520  int the release 
-00001ad0: 6966 2065 6d70 7479 0a2a 2041 6464 7320  if empty.* Adds 
-00001ae0: 2d70 206f 7074 696f 6e20 696e 206d 6b64  -p option in mkd
-00001af0: 6972 2066 6f72 2062 7569 6c64 7064 6620  ir for buildpdf 
-00001b00: 746f 7820 656e 760a 2a20 6269 6e64 6570  tox env.* bindep
-00001b10: 3a20 4164 6420 6465 7065 6e64 656e 6369  : Add dependenci
-00001b20: 6573 2066 6f72 2050 4446 7320 6f6e 2046  es for PDFs on F
-00001b30: 6564 6f72 610a 2a20 6769 7469 676e 6f72  edora.* gitignor
-00001b40: 653a 2049 676e 6f72 6520 6d6f 7265 2066  e: Ignore more f
-00001b50: 696c 6573 0a2a 2055 7064 6174 6564 2066  iles.* Updated f
-00001b60: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
-00001b70: 7265 6d65 6e74 730a 2a20 5265 6d6f 7665  rements.* Remove
-00001b80: 202d 5520 6672 6f6d 2070 6970 2069 6e73   -U from pip ins
-00001b90: 7461 6c6c 0a2a 2041 766f 6964 2074 6f78  tall.* Avoid tox
-00001ba0: 5c5f 696e 7374 616c 6c2e 7368 2066 6f72  \_install.sh for
-00001bb0: 2063 6f6e 7374 7261 696e 7473 2073 7570   constraints sup
-00001bc0: 706f 7274 0a2a 2052 656d 6f76 6520 7365  port.* Remove se
-00001bd0: 7474 696e 6720 6f66 2076 6572 7369 6f6e  tting of version
-00001be0: 2f72 656c 6561 7365 2066 726f 6d20 7265  /release from re
-00001bf0: 6c65 6173 656e 6f74 6573 0a2a 2041 6464  leasenotes.* Add
-00001c00: 207a 7575 6c76 3320 6e61 7469 7665 206a   zuulv3 native j
-00001c10: 6f62 0a2a 2041 6464 7320 5475 726b 6973  ob.* Adds Turkis
-00001c20: 6820 6c61 6e64 696e 6720 7061 6765 2074  h landing page t
-00001c30: 6f20 7369 6465 6261 7274 6f63 5c5f 6d65  o sidebartoc\_me
-00001c40: 6e75 0a2a 204e 6f20 7265 6420 7769 7468  nu.* No red with
-00001c50: 2064 6f75 626c 6520 6261 636b 7469 636b   double backtick
-00001c60: 7320 6d61 726b 7570 0a0a 312e 3137 2e30  s markup..1.17.0
-00001c70: 0a2d 2d2d 2d2d 2d0a 0a2a 2055 7064 6174  .------..* Updat
-00001c80: 6564 2066 726f 6d20 676c 6f62 616c 2072  ed from global r
-00001c90: 6571 7569 7265 6d65 6e74 730a 2a20 4669  equirements.* Fi
-00001ca0: 7820 6c69 6e6b 2074 6f20 6f70 656e 7374  x link to openst
-00001cb0: 6163 6b64 6179 730a 2a20 5b77 7777 5d20  ackdays.* [www] 
-00001cc0: 4669 7820 6c69 6e6b 2074 6f20 434f 410a  Fix link to COA.
-00001cd0: 2a20 4164 6420 7375 7070 6f72 7420 666f  * Add support fo
-00001ce0: 7220 7370 6869 6e78 2073 6964 6562 6172  r sphinx sidebar
-00001cf0: 2072 6f6c 650a 2a20 5265 6d6f 7665 2073   role.* Remove s
-00001d00: 7472 6179 2063 6861 7261 6374 6572 7320  tray characters 
-00001d10: 6672 6f6d 2064 656d 6f0a 2a20 5570 6461  from demo.* Upda
-00001d20: 7465 2074 6865 2063 6f6e 6669 6775 7261  te the configura
-00001d30: 7469 6f6e 206f 6620 6765 6e65 7261 7469  tion of generati
-00001d40: 6e67 2061 2050 4446 2064 6f63 756d 656e  ng a PDF documen
-00001d50: 740a 2a20 5570 6461 7465 6420 6672 6f6d  t.* Updated from
-00001d60: 2067 6c6f 6261 6c20 7265 7175 6972 656d   global requirem
-00001d70: 656e 7473 0a2a 2053 796e 6320 6c61 6e67  ents.* Sync lang
-00001d80: 7561 6765 206c 6973 7420 7769 7468 206f  uage list with o
-00001d90: 7065 6e73 7461 636b 2d6d 616e 7561 6c73  penstack-manuals
-00001da0: 2072 6570 6f0a 2a20 4272 696e 6720 6261   repo.* Bring ba
-00001db0: 636b 206c 6f63 616c 2073 6561 7263 680a  ck local search.
-00001dc0: 2a20 436c 6561 6e75 7020 7365 7475 702e  * Cleanup setup.
-00001dd0: 6366 670a 2a20 5570 6461 7465 6420 6672  cfg.* Updated fr
-00001de0: 6f6d 2067 6c6f 6261 6c20 7265 7175 6972  om global requir
-00001df0: 656d 656e 7473 0a2a 2042 7265 616b 2063  ements.* Break c
-00001e00: 7963 6c65 2064 6570 656e 6465 6e63 7920  ycle dependency 
-00001e10: 7769 7468 2072 656e 6f0a 2a20 5570 6461  with reno.* Upda
-00001e20: 7465 6420 6672 6f6d 2067 6c6f 6261 6c20  ted from global 
-00001e30: 7265 7175 6972 656d 656e 7473 0a2a 2042  requirements.* B
-00001e40: 7265 616b 2063 7963 6c65 2064 6570 656e  reak cycle depen
-00001e50: 6465 6e63 7920 7769 7468 206f 732d 6170  dency with os-ap
-00001e60: 692d 7265 660a 2a20 5265 6d6f 7665 206e  i-ref.* Remove n
-00001e70: 6176 6967 6174 696f 6e2e 6874 6d6c 0a2a  avigation.html.*
-00001e80: 2055 7064 6174 6520 6c69 6e6b 7320 696e   Update links in
-00001e90: 2052 4541 444d 450a 2a20 5570 6461 7465   README.* Update
-00001ea0: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
-00001eb0: 7175 6972 656d 656e 7473 0a2a 2044 6f63  quirements.* Doc
-00001ec0: 756d 656e 7473 2068 6f77 2074 6f20 7365  uments how to se
-00001ed0: 7420 636f 6e66 2e70 7920 666f 7220 5044  t conf.py for PD
-00001ee0: 4620 6765 6e65 7261 7469 6f6e 0a2a 2073  F generation.* s
-00001ef0: 686f 7720 7265 6c65 6173 6520 7365 7269  how release seri
-00001f00: 6573 206e 616d 6573 206e 6f74 2076 6572  es names not ver
-00001f10: 7369 6f6e 2074 6167 730a 2a20 4c69 6e6b  sion tags.* Link
-00001f20: 2074 6f20 6c61 7465 7374 2076 6572 7369   to latest versi
-00001f30: 6f6e 0a0a 312e 3136 2e31 0a2d 2d2d 2d2d  on..1.16.1.-----
-00001f40: 2d0a 0a2a 2066 6978 2061 6c69 676e 6d65  -..* fix alignme
-00001f50: 6e74 206f 6620 746f 6320 7472 6565 2069  nt of toc tree i
-00001f60: 7465 6d73 2069 6e20 7369 6465 6261 720a  tems in sidebar.
-00001f70: 0a31 2e31 362e 300a 2d2d 2d2d 2d2d 0a0a  .1.16.0.------..
-00001f80: 2a20 4669 7820 6120 6c6f 6769 6320 6973  * Fix a logic is
-00001f90: 7375 6520 696e 2074 6865 204a 530a 2a20  sue in the JS.* 
-00001fa0: 6d6f 7665 2074 6865 206c 6f63 616c 746f  move the localto
-00001fb0: 6320 666f 7220 7468 6520 7061 6765 2069  c for the page i
-00001fc0: 6e74 6f20 7468 6520 7369 6465 6261 720a  nto the sidebar.
-00001fd0: 2a20 5365 7276 6520 6d69 6e69 6669 6564  * Serve minified
-00001fe0: 2043 5353 0a0a 312e 3135 2e30 0a2d 2d2d   CSS..1.15.0.---
-00001ff0: 2d2d 2d0a 0a2a 2052 656d 6f76 6520 7275  ---..* Remove ru
-00002000: 6c65 7320 6c69 6e6b 6564 2074 6f20 6120  les linked to a 
-00002010: 2253 7461 7475 7322 2049 440a 2a20 5570  "Status" ID.* Up
-00002020: 6461 7465 2032 2064 6f63 756d 656e 7461  date 2 documenta
-00002030: 7469 6f6e 2055 524c 7320 6163 636f 7264  tion URLs accord
-00002040: 696e 6720 746f 2064 6f63 206d 6967 7261  ing to doc migra
-00002050: 7469 6f6e 0a2a 204d 6f76 6520 6672 6f6d  tion.* Move from
-00002060: 2033 7264 2070 6172 7479 2066 6f6e 7473   3rd party fonts
-00002070: 2074 6f20 6e61 7469 7665 2066 6f6e 7420   to native font 
-00002080: 7374 6163 6b0a 2a20 4669 7820 4164 6465  stack.* Fix Adde
-00002090: 6420 2f20 4368 616e 6765 6420 2f20 4465  d / Changed / De
-000020a0: 7072 6563 6174 6564 206e 6f74 6963 6573  precated notices
-000020b0: 0a2a 2053 7461 6e64 6172 6469 7365 2068  .* Standardise h
-000020c0: 6561 6465 7220 7374 796c 696e 670a 2a20  eader styling.* 
-000020d0: 4164 6420 7370 6163 6573 2069 6e20 6465  Add spaces in de
-000020e0: 6d6f 2066 6f72 2064 6570 7265 6361 7469  mo for deprecati
-000020f0: 6f6e 206e 6f74 6963 6573 0a2a 2072 656d  on notices.* rem
-00002100: 6f76 6520 736d 6f6f 7468 2073 6372 6f6c  ove smooth scrol
-00002110: 6c69 6e67 0a0a 312e 3134 2e30 0a2d 2d2d  ling..1.14.0.---
-00002120: 2d2d 2d0a 0a2a 2061 6464 2061 2063 6f6d  ---..* add a com
-00002130: 6d65 6e74 2074 6f20 616c 6c20 6f75 7470  ment to all outp
-00002140: 7574 2048 544d 4c20 7061 6765 7320 7368  ut HTML pages sh
-00002150: 6f77 696e 6720 7468 6520 696e 7075 7420  owing the input 
-00002160: 6669 6c65 0a2a 2043 5353 3a20 4164 6420  file.* CSS: Add 
-00002170: 6d61 7267 696e 2d6c 6566 7420 746f 203c  margin-left to <
-00002180: 6464 3e0a 2a20 4164 6420 7375 7070 6f72  dd>.* Add suppor
-00002190: 7420 666f 7220 7665 7273 696f 6e61 6464  t for versionadd
-000021a0: 6564 2061 6e64 2064 6570 7265 6361 7465  ed and deprecate
-000021b0: 640a 2a20 7368 6f77 2074 6865 2063 7572  d.* show the cur
-000021c0: 7265 6e74 2070 726f 6a65 6374 206e 616d  rent project nam
-000021d0: 6520 616e 6420 7665 7273 696f 6e20 696e  e and version in
-000021e0: 206e 6176 6967 6174 696f 6e20 6c69 6e6b   navigation link
-000021f0: 0a2a 2044 6563 6c61 7265 2070 6172 616c  .* Declare paral
-00002200: 6c65 6c20 7265 6164 696e 6720 7361 6665  lel reading safe
-00002210: 0a0a 312e 3133 2e30 0a2d 2d2d 2d2d 2d0a  ..1.13.0.------.
-00002220: 0a2a 2053 7472 6970 2074 6167 7320 6672  .* Strip tags fr
-00002230: 6f6d 206e 6176 6967 6174 696f 6e20 7072  om navigation pr
-00002240: 6576 2c20 6e65 7874 2074 6974 6c65 730a  ev, next titles.
-00002250: 2a20 436c 6561 6e75 7020 636f 6e66 2e70  * Cleanup conf.p
-00002260: 790a 2a20 416c 6c6f 7720 7573 696e 6720  y.* Allow using 
-00002270: 6f70 656e 7374 6163 6b64 6f63 7374 6865  openstackdocsthe
-00002280: 6d65 2077 6974 686f 7574 2067 6974 2069  me without git i
-00002290: 6e73 7461 6c6c 6564 0a2a 2046 6978 2073  nstalled.* Fix s
-000022a0: 6f72 7469 6e67 206f 6620 6769 7420 7665  orting of git ve
-000022b0: 7273 696f 6e73 0a2a 2041 6464 206e 6f74  rsions.* Add not
-000022c0: 6520 666f 7220 7368 6f77 5c5f 6f74 6865  e for show\_othe
-000022d0: 725c 5f76 6572 7369 6f6e 730a 2a20 446f  r\_versions.* Do
-000022e0: 206e 6f74 2064 6973 706c 6179 2074 6974   not display tit
-000022f0: 6c65 2073 7472 696e 6720 6f66 2070 6167  le string of pag
-00002300: 6520 6c6f 6361 6c20 544f 430a 0a31 2e31  e local TOC..1.1
-00002310: 322e 300a 2d2d 2d2d 2d2d 0a0a 2a20 496e  2.0.------..* In
-00002320: 6372 6561 7365 2061 646d 6f6e 6974 696f  crease admonitio
-00002330: 6e2e 696d 706f 7274 616e 7420 636f 6e74  n.important cont
-00002340: 7261 7374 0a2a 2041 6464 7320 646f 6373  rast.* Adds docs
-00002350: 2066 6f72 2072 656c 6561 7365 2076 6572   for release ver
-00002360: 7369 6f6e 7320 6472 6f70 646f 776e 206d  sions dropdown m
-00002370: 656e 750a 2a20 4164 6473 206c 6973 7420  enu.* Adds list 
-00002380: 6f66 2076 6572 7369 6f6e 7320 696e 2074  of versions in t
-00002390: 6865 2022 5570 6461 7465 6422 2062 6172  he "Updated" bar
-000023a0: 0a2a 2055 7064 6174 6520 646f 6373 0a2a  .* Update docs.*
-000023b0: 2043 6861 6e67 6520 6e61 6d65 206f 6620   Change name of 
-000023c0: 6368 6563 6b62 7569 6c64 2074 6573 7465  checkbuild teste
-000023d0: 6e76 2074 6f20 6275 696c 6470 6466 2066  nv to buildpdf f
-000023e0: 6f72 2063 6c61 7269 7479 0a2a 2052 6571  or clarity.* Req
-000023f0: 7569 7265 2062 7567 5c5f 7072 6f6a 6563  uire bug\_projec
-00002400: 7420 7365 7474 696e 670a 2a20 4164 6469  t setting.* Addi
-00002410: 6e67 206f 6374 6176 6961 2061 7069 2d72  ng octavia api-r
-00002420: 6566 0a2a 204d 696e 696d 616c 2073 7570  ef.* Minimal sup
-00002430: 706f 7274 2066 6f72 2073 746f 7279 626f  port for storybo
-00002440: 6172 640a 2a20 6d6f 7665 2064 6f63 756d  ard.* move docum
-00002450: 656e 7461 7469 6f6e 2066 726f 6d20 7265  entation from re
-00002460: 6164 6d65 2074 6f20 7370 6869 6e78 2074  adme to sphinx t
-00002470: 7265 650a 2a20 5570 6461 7465 6420 6672  ree.* Updated fr
-00002480: 6f6d 2067 6c6f 6261 6c20 7265 7175 6972  om global requir
-00002490: 656d 656e 7473 0a2a 2055 7064 6174 6573  ements.* Updates
-000024a0: 2022 436f 6e74 656e 7473 2220 746f 2022   "Contents" to "
-000024b0: 5072 6f6a 6563 7420 686f 6d65 2070 6167  Project home pag
-000024c0: 6522 2074 6f20 6265 7474 6572 206d 6174  e" to better mat
-000024d0: 6368 2065 7869 7374 696e 670a 2a20 576f  ch existing.* Wo
-000024e0: 726b 696e 6720 6f6e 2069 6e74 6567 7261  rking on integra
-000024f0: 7469 6e67 206f 7074 696f 6e73 2066 726f  ting options fro
-00002500: 6d20 6f73 6c6f 7370 6869 6e78 2074 6865  m oslosphinx the
-00002510: 6d65 0a0a 312e 3131 2e30 0a2d 2d2d 2d2d  me..1.11.0.-----
-00002520: 2d0a 0a2a 2073 7769 7463 6820 7265 6c65  -..* switch rele
-00002530: 6173 6520 6e6f 7465 7320 6275 696c 6420  ase notes build 
-00002540: 746f 2075 7365 206f 7065 6e73 7461 636b  to use openstack
-00002550: 646f 6373 2069 6e73 7465 6164 206f 6620  docs instead of 
-00002560: 6f73 6c6f 7370 6869 6e78 0a2a 2061 7574  oslosphinx.* aut
-00002570: 6f6d 6174 6520 736f 6d65 206f 6620 7468  omate some of th
-00002580: 6520 6578 7465 6e73 696f 6e20 7365 7475  e extension setu
-00002590: 700a 2a20 456e 6162 6c65 2073 6f6d 6520  p.* Enable some 
-000025a0: 6f66 662d 6279 2d64 6566 6175 6c74 2063  off-by-default c
-000025b0: 6865 636b 730a 0a31 2e31 302e 300a 2d2d  hecks..1.10.0.--
-000025c0: 2d2d 2d2d 0a0a 2a20 5570 6461 7465 2053  ----..* Update S
-000025d0: 6974 6520 5365 6172 6368 0a2a 2055 7064  ite Search.* Upd
-000025e0: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
-000025f0: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
-00002600: 5044 4620 6275 696c 6420 7375 7070 6f72  PDF build suppor
-00002610: 7420 3e3d 2053 7068 696e 7820 312e 362e  t >= Sphinx 1.6.
-00002620: 310a 2a20 5245 4144 4d45 3a20 5570 6461  1.* README: Upda
-00002630: 7465 2063 6f6e 6669 6775 7261 7469 6f6e  te configuration
-00002640: 206f 6620 6f70 656e 7374 6163 6b64 6f63   of openstackdoc
-00002650: 7374 6865 6d65 0a0a 312e 392e 300a 2d2d  stheme..1.9.0.--
-00002660: 2d2d 2d0a 0a2a 2055 7064 6174 6564 2066  ---..* Updated f
-00002670: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
-00002680: 7265 6d65 6e74 730a 2a20 4669 7820 6c69  rements.* Fix li
-00002690: 6e6b 7320 696e 2064 726f 702d 646f 776e  nks in drop-down
-000026a0: 206d 656e 7520 756e 6465 7220 4a6f 696e   menu under Join
-000026b0: 3b20 6164 6420 6874 7470 730a 0a31 2e38  ; add https..1.8
-000026c0: 2e30 0a2d 2d2d 2d2d 0a0a 2a20 5573 6520  .0.-----..* Use 
-000026d0: 6e65 7720 4f70 656e 5374 6163 6b20 6c6f  new OpenStack lo
-000026e0: 676f 2061 6e64 2068 6561 6465 720a 2a20  go and header.* 
-000026f0: 5570 6461 7465 6420 6672 6f6d 2067 6c6f  Updated from glo
-00002700: 6261 6c20 7265 7175 6972 656d 656e 7473  bal requirements
-00002710: 0a0a 312e 372e 300a 2d2d 2d2d 2d0a 0a2a  ..1.7.0.-----..*
-00002720: 2043 6c61 7269 6679 2073 6561 7263 6820   Clarify search 
-00002730: 7469 746c 650a 2a20 4669 7820 7365 6172  title.* Fix sear
-00002740: 6368 2e68 746d 6c20 7061 6765 2073 6372  ch.html page scr
-00002750: 6970 7420 6572 726f 7273 0a2a 2041 6464  ipt errors.* Add
-00002760: 2061 6c69 676e 6d65 6e74 2073 7479 6c69   alignment styli
-00002770: 6e67 2066 6f72 2066 6967 7572 6573 2061  ng for figures a
-00002780: 6e64 2069 6d61 6765 730a 2a20 5044 4620  nd images.* PDF 
-00002790: 7375 7070 6f72 7420 666f 7220 7361 6d70  support for samp
-000027a0: 6c65 2064 6f63 756d 656e 7420 7769 7468  le document with
-000027b0: 2066 6f6e 740a 2a20 4164 6420 746f 7820   font.* Add tox 
-000027c0: 656e 7620 666f 7220 5044 4620 6275 696c  env for PDF buil
-000027d0: 6469 6e67 0a2a 2055 7064 6174 6520 6373  ding.* Update cs
-000027e0: 7320 6d61 726b 7570 7320 666f 7220 6e65  s markups for ne
-000027f0: 7765 7220 5370 6869 6e78 0a2a 2041 6464  wer Sphinx.* Add
-00002800: 7320 4c61 5465 5820 7374 796c 6520 6669  s LaTeX style fi
-00002810: 6c65 2066 6f72 2062 7569 6c64 696e 6720  le for building 
-00002820: 5044 4620 646f 6375 6d65 6e74 730a 2a20  PDF documents.* 
-00002830: 4164 6420 7761 726e 696e 672d 6973 2d65  Add warning-is-e
-00002840: 7272 6f72 0a2a 2055 7064 6174 6564 2066  rror.* Updated f
-00002850: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
-00002860: 7265 6d65 6e74 730a 2a20 5570 6461 7465  rements.* Update
-00002870: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
-00002880: 7175 6972 656d 656e 7473 0a2a 2055 7064  quirements.* Upd
-00002890: 6174 6520 6861 636b 696e 6720 746f 2063  ate hacking to c
-000028a0: 7572 7265 6e74 2076 6572 7369 6f6e 0a2a  urrent version.*
-000028b0: 2041 646a 7573 7420 2764 6f63 732d 746f   Adjust 'docs-to
-000028c0: 6320 6127 2064 6973 706c 6179 2076 616c  c a' display val
-000028d0: 7565 0a2a 2052 656d 6f76 6520 6765 744a  ue.* Remove getJ
-000028e0: 534f 4e20 6675 6e63 7469 6f6e 2061 6e64  SON function and
-000028f0: 2064 6f63 2d63 6861 7261 6374 6572 7320   doc-characters 
-00002900: 6669 6c65 0a2a 2055 7064 6174 6520 4c61  file.* Update La
-00002910: 756e 6368 7061 6420 696e 666f 0a2a 2055  unchpad info.* U
-00002920: 7064 6174 6564 2066 726f 6d20 676c 6f62  pdated from glob
-00002930: 616c 2072 6571 7569 7265 6d65 6e74 730a  al requirements.
-00002940: 2a20 5573 6520 6874 7470 7320 696e 7374  * Use https inst
-00002950: 6561 6420 6f66 2068 7474 7020 666f 7220  ead of http for 
-00002960: 6769 742e 6f70 656e 7374 6163 6b2e 6f72  git.openstack.or
-00002970: 670a 2a20 5570 6461 7465 2062 6f6f 7473  g.* Update boots
-00002980: 7472 6170 2061 6e64 206a 7175 6572 7920  trap and jquery 
-00002990: 6669 6c65 730a 2a20 5265 6d6f 7665 2064  files.* Remove d
-000029a0: 7570 6c69 6361 7465 2073 6561 7263 6820  uplicate search 
-000029b0: 6669 656c 6420 6672 6f6d 2074 6865 206c  field from the l
-000029c0: 6566 7420 7369 6465 6261 720a 2a20 4164  eft sidebar.* Ad
-000029d0: 6420 6e6f 7465 2069 6e20 5245 4144 4d45  d note in README
-000029e0: 2061 626f 7574 2050 7974 686f 6e20 3320   about Python 3 
-000029f0: 6368 616e 6765 730a 2a20 4669 7820 6d69  changes.* Fix mi
-00002a00: 7373 696e 6720 726f 6c65 5c5f 6964 0a0a  ssing role\_id..
-00002a10: 312e 362e 310a 2d2d 2d2d 2d0a 0a2a 2049  1.6.1.-----..* I
-00002a20: 6e63 6c75 6465 7320 6368 6563 6b6c 6973  ncludes checklis
-00002a30: 7420 7768 656e 2066 696c 696e 6720 6120  t when filing a 
-00002a40: 6275 6720 666f 7220 6f73 6d61 6e75 616c  bug for osmanual
-00002a50: 730a 2a20 4164 6420 7472 6f76 6520 636c  s.* Add trove cl
-00002a60: 6173 7369 6669 6572 7320 666f 7220 5079  assifiers for Py
-00002a70: 7468 6f6e 0a0a 312e 362e 300a 2d2d 2d2d  thon..1.6.0.----
-00002a80: 2d0a 0a2a 2041 6464 2043 6f6e 7374 7261  -..* Add Constra
-00002a90: 696e 7473 2073 7570 706f 7274 0a2a 2053  ints support.* S
-00002aa0: 686f 7720 7465 616d 2061 6e64 2072 6570  how team and rep
-00002ab0: 6f20 6261 6467 6573 206f 6e20 5245 4144  o badges on READ
-00002ac0: 4d45 0a2a 2052 656d 6f76 6564 206d 696e  ME.* Removed min
-00002ad0: 696d 697a 6564 2066 696c 6573 0a2a 2041  imized files.* A
-00002ae0: 6c6c 6f77 2074 6f20 6275 696c 6420 646f  llow to build do
-00002af0: 6373 2077 6974 686f 7574 2067 6974 2063  cs without git c
-00002b00: 6f6d 6d61 6e64 0a2a 205b 7777 775d 2075  ommand.* [www] u
-00002b10: 7064 6174 6520 7061 6765 2068 6561 6465  pdate page heade
-00002b20: 7220 6c69 6e6b 730a 2a20 5570 6461 7465  r links.* Update
-00002b30: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
-00002b40: 7175 6972 656d 656e 7473 0a2a 2055 7064  quirements.* Upd
-00002b50: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
-00002b60: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
-00002b70: 456e 6162 6c65 2072 656c 6561 7365 206e  Enable release n
-00002b80: 6f74 6573 2074 7261 6e73 6c61 7469 6f6e  otes translation
-00002b90: 0a2a 2055 7064 6174 6520 7465 7374 2041  .* Update test A
-00002ba0: 5049 2052 6566 0a2a 2046 6978 2074 7970  PI Ref.* Fix typ
-00002bb0: 6f3a 2072 656d 6f76 6520 7265 6475 6e64  o: remove redund
-00002bc0: 616e 7420 2774 6865 270a 2a20 5570 6461  ant 'the'.* Upda
-00002bd0: 7465 6420 6672 6f6d 2067 6c6f 6261 6c20  ted from global 
-00002be0: 7265 7175 6972 656d 656e 7473 0a2a 2055  requirements.* U
-00002bf0: 7064 6174 6564 2066 726f 6d20 676c 6f62  pdated from glob
-00002c00: 616c 2072 6571 7569 7265 6d65 6e74 730a  al requirements.
-00002c10: 2a20 5570 6461 7465 2072 6571 7569 7265  * Update require
-00002c20: 6d65 6e74 730a 2a20 4669 7820 746f 7820  ments.* Fix tox 
-00002c30: 7365 7475 700a 2a20 496e 7374 616c 6c20  setup.* Install 
-00002c40: 7265 7175 6972 6564 2070 6163 6b61 6765  required package
-00002c50: 730a 2a20 5570 6461 7465 6420 6672 6f6d  s.* Updated from
-00002c60: 2067 6c6f 6261 6c20 7265 7175 6972 656d   global requirem
-00002c70: 656e 7473 0a0a 312e 352e 300a 2d2d 2d2d  ents..1.5.0.----
-00002c80: 2d0a 0a2a 2041 5049 2052 6566 6572 656e  -..* API Referen
-00002c90: 6365 7320 6472 6f70 646f 776e 206d 656e  ces dropdown men
-00002ca0: 750a 2a20 416c 6c6f 7720 6175 746f 6d61  u.* Allow automa
-00002cb0: 7469 6320 746f 6320 746f 2062 6520 6469  tic toc to be di
-00002cc0: 7361 626c 6564 0a0a 312e 342e 300a 2d2d  sabled..1.4.0.--
-00002cd0: 2d2d 2d0a 0a2a 2055 7064 6174 6520 5265  ---..* Update Re
-00002ce0: 6c65 6173 6520 4e6f 7465 730a 2a20 4164  lease Notes.* Ad
-00002cf0: 6473 2072 656c 6561 7365 206e 6f74 6573  ds release notes
-00002d00: 2069 7465 6d73 2066 6f72 206e 6578 7420   items for next 
-00002d10: 7265 6c65 6173 650a 2a20 4d61 6b65 205c  release.* Make \
-00002d20: 605c 6073 6f6d 6574 6869 6e67 5c60 5c60  `\`something\`\`
-00002d30: 206d 6f72 6520 6869 6768 6c69 6768 7465   more highlighte
-00002d40: 640a 2a20 416c 6c6f 7720 7468 6520 6275  d.* Allow the bu
-00002d50: 6720 7469 746c 6520 746f 2062 6520 6375  g title to be cu
-00002d60: 7374 6f6d 6973 6162 6c65 0a2a 2042 726f  stomisable.* Bro
-00002d70: 6b65 6e20 4c69 6e6b 0a2a 2055 7064 6174  ken Link.* Updat
-00002d80: 6564 2066 726f 6d20 676c 6f62 616c 2072  ed from global r
-00002d90: 6571 7569 7265 6d65 6e74 730a 2a20 496e  equirements.* In
-00002da0: 6372 6561 7365 2069 6e64 656e 7420 6c65  crease indent le
-00002db0: 7665 6c20 6f66 2064 6f63 2074 6f70 2063  vel of doc top c
-00002dc0: 6f6e 7465 6e74 730a 2a20 5570 6461 7465  ontents.* Update
-00002dd0: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
-00002de0: 7175 6972 656d 656e 7473 0a2a 2041 6374  quirements.* Act
-00002df0: 7561 6c6c 7920 696e 636c 7564 6520 6375  ually include cu
-00002e00: 7374 6f6d 204a 5320 6669 6c65 730a 2a20  stom JS files.* 
-00002e10: 5265 6c65 6173 6520 6e6f 7465 2066 6f72  Release note for
-00002e20: 206e 6577 2073 6964 6562 6172 2066 6561   new sidebar fea
-00002e30: 7475 7265 0a2a 2055 7365 2048 5454 5053  ture.* Use HTTPS
-00002e40: 2066 6f72 2065 7874 6572 6e61 6c20 6465   for external de
-00002e50: 7073 0a2a 2053 6574 2073 6964 6520 6261  ps.* Set side ba
-00002e60: 7220 636f 6e74 656e 7420 746f 2062 6520  r content to be 
-00002e70: 636f 6e66 6967 7572 6162 6c65 0a2a 2043  configurable.* C
-00002e80: 7265 6174 6520 656d 7074 7920 666f 6c64  reate empty fold
-00002e90: 6572 2066 6f72 2063 7573 746f 6d20 666f  er for custom fo
-00002ea0: 6e74 2066 696c 6573 0a2a 2046 6978 2074  nt files.* Fix t
-00002eb0: 6578 7420 666f 6e74 2d66 616d 696c 7920  ext font-family 
-00002ec0: 6f66 2061 646d 6f6e 6974 696f 6e73 0a2a  of admonitions.*
-00002ed0: 2041 6c6c 6f77 2066 6f72 2069 6e63 6c75   Allow for inclu
-00002ee0: 7369 6f6e 206f 6620 6375 7374 6f6d 204a  sion of custom J
-00002ef0: 5320 6669 6c65 730a 2a20 5570 6461 7465  S files.* Update
-00002f00: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
-00002f10: 7175 6972 656d 656e 7473 0a2a 2043 6861  quirements.* Cha
-00002f20: 6e67 6520 7375 6d6d 6974 2076 6964 656f  nge summit video
-00002f30: 2055 524c 0a2a 2055 7064 6174 6564 2066   URL.* Updated f
-00002f40: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
-00002f50: 7265 6d65 6e74 730a 2a20 5570 6461 7465  rements.* Update
-00002f60: 2074 6865 2041 646d 696e 6973 7472 6174   the Administrat
-00002f70: 6f72 2047 7569 6465 206c 696e 6b0a 2a20  or Guide link.* 
-00002f80: 436c 6172 6966 7920 7573 6573 2066 6f72  Clarify uses for
-00002f90: 2074 6869 7320 7468 656d 650a 2a20 416c   this theme.* Al
-00002fa0: 6c6f 7720 6373 7366 696c 6573 2061 6464  low cssfiles add
-00002fb0: 6564 2062 7920 7370 6869 6e78 2065 7874  ed by sphinx ext
-00002fc0: 656e 7369 6f6e 730a 0a31 2e33 2e30 0a2d  ensions..1.3.0.-
-00002fd0: 2d2d 2d2d 0a0a 2a20 4d61 6b65 2074 6865  ----..* Make the
-00002fe0: 6d65 2076 6572 7369 6f6e 2069 6e64 6570  me version indep
-00002ff0: 656e 6465 6e74 0a2a 2041 6464 2061 7070  endent.* Add app
-00003000: 726f 7072 6961 7465 206f 7264 6572 206c  ropriate order l
-00003010: 6973 7420 7374 796c 6573 0a2a 2053 686f  ist styles.* Sho
-00003020: 7274 6564 206d 6172 6769 6e20 616e 6420  rted margin and 
-00003030: 7061 6464 696e 6720 666f 7220 746f 7020  padding for top 
-00003040: 7061 6765 206d 656e 750a 2a20 5573 6520  page menu.* Use 
-00003050: 7065 7038 2069 6e73 7465 6164 206f 6620  pep8 instead of 
-00003060: 6c69 6e74 6572 730a 2a20 4669 7820 6120  linters.* Fix a 
-00003070: 7370 656c 6c20 7479 706f 730a 2a20 5265  spell typos.* Re
-00003080: 6e61 6d65 2070 6570 3820 746f 206c 696e  name pep8 to lin
-00003090: 7465 7273 2074 6573 740a 0a31 2e32 2e37  ters test..1.2.7
-000030a0: 0a2d 2d2d 2d2d 0a0a 2a20 5570 6461 7465  .-----..* Update
-000030b0: 2074 6865 2063 6f6e 7472 6962 7574 6520   the contribute 
-000030c0: 6c69 6e6b 2061 7420 7468 6520 666f 6f74  link at the foot
-000030d0: 6572 0a2a 2055 7064 6174 6520 6c69 6e6b  er.* Update link
-000030e0: 7320 696e 2074 6865 204f 7065 6e53 7461  s in the OpenSta
-000030f0: 636b 2063 6f6c 756d 6e20 696e 2074 6865  ck column in the
-00003100: 2066 6f6f 7465 720a 2a20 5265 6d6f 7665   footer.* Remove
-00003110: 2066 6565 6462 6163 6b20 666f 726d 756c   feedback formul
-00003120: 6172 2066 726f 6d20 7468 6520 666f 6f74  ar from the foot
-00003130: 6572 0a2a 2048 6964 6520 6475 706c 6963  er.* Hide duplic
-00003140: 6174 6520 7469 746c 6573 2061 6e64 2065  ate titles and e
-00003150: 6d70 7479 2074 6f63 7320 696e 2067 656e  mpty tocs in gen
-00003160: 6572 6174 6564 2063 6f6e 7465 6e74 0a2a  erated content.*
-00003170: 2055 7064 6174 6564 2066 726f 6d20 676c   Updated from gl
-00003180: 6f62 616c 2072 6571 7569 7265 6d65 6e74  obal requirement
-00003190: 730a 2a20 5379 6e63 2068 6561 6465 7220  s.* Sync header 
-000031a0: 7769 7468 2077 7777 2e6f 7065 6e73 7461  with www.opensta
-000031b0: 636b 2e6f 7267 0a2a 2052 6570 6c61 6365  ck.org.* Replace
-000031c0: 2064 6570 7265 6361 7465 6420 6c69 6272   deprecated libr
-000031d0: 6172 7920 6675 6e63 7469 6f6e 206f 732e  ary function os.
-000031e0: 706f 7065 6e28 2920 7769 7468 2073 7562  popen() with sub
-000031f0: 7072 6f63 6573 730a 2a20 4472 6f70 2070  process.* Drop p
-00003200: 7974 686f 6e20 636c 6173 7369 6669 6572  ython classifier
-00003210: 7320 6672 6f6d 2073 6574 7570 2e63 6667  s from setup.cfg
-00003220: 2066 696c 650a 2a20 5570 6461 7465 6420   file.* Updated 
-00003230: 6672 6f6d 2067 6c6f 6261 6c20 7265 7175  from global requ
-00003240: 6972 656d 656e 7473 0a2a 2046 6978 2073  irements.* Fix s
-00003250: 6964 6562 6172 2066 6f72 2064 6576 656c  idebar for devel
-00003260: 6f70 6572 2e6f 7065 6e73 7461 636b 2e6f  oper.openstack.o
-00003270: 7267 0a2a 2044 6570 7265 6361 7465 6420  rg.* Deprecated 
-00003280: 746f 7820 2d64 6f77 6e6c 6f61 6463 6163  tox -downloadcac
-00003290: 6865 206f 7074 696f 6e20 7265 6d6f 7665  he option remove
-000032a0: 640a 2a20 4472 6f70 2070 7932 3620 6672  d.* Drop py26 fr
-000032b0: 6f6d 2073 6574 7570 2e63 6667 0a0a 312e  om setup.cfg..1.
-000032c0: 322e 360a 2d2d 2d2d 2d0a 0a2a 204d 616b  2.6.-----..* Mak
-000032d0: 6520 476f 6f67 6c65 2041 6e61 6c79 7469  e Google Analyti
-000032e0: 6373 2074 7261 636b 696e 6720 6f70 7469  cs tracking opti
-000032f0: 6f6e 616c 0a2a 2041 6464 2062 7567 2072  onal.* Add bug r
-00003300: 6570 6f72 7420 7072 6f6a 6563 7420 6465  eport project de
-00003310: 6669 6e69 7469 6f6e 2066 6561 7475 7265  finition feature
-00003320: 0a2a 2046 6978 2074 6865 2075 726c 206f  .* Fix the url o
-00003330: 6620 2248 6f77 2074 6f20 636f 6e74 7269  f "How to contri
-00003340: 6275 7465 220a 0a31 2e32 2e35 0a2d 2d2d  bute"..1.2.5.---
-00003350: 2d2d 0a0a 2a20 4164 6420 2d57 2074 6f20  --..* Add -W to 
-00003360: 7370 6869 6e78 2069 6e76 6f63 6174 696f  sphinx invocatio
-00003370: 6e20 666f 7220 7265 6c65 6173 652d 6e6f  n for release-no
-00003380: 7465 7320 6275 696c 640a 2a20 5461 626c  tes build.* Tabl
-00003390: 6520 6361 7074 696f 6e3a 2075 7365 2061  e caption: use a
-000033a0: 2062 6f6c 6420 666f 6e74 0a2a 2072 656c   bold font.* rel
-000033b0: 6561 7365 206e 6f74 6520 656e 7472 7920  ease note entry 
-000033c0: 666f 7220 7369 6465 6261 7220 6c69 6e6b  for sidebar link
-000033d0: 2074 6f20 6120 746f 7020 7061 6765 0a2a   to a top page.*
-000033e0: 2041 6464 206c 696e 6b20 666f 7220 6120   Add link for a 
-000033f0: 746f 7020 7061 6765 206f 6620 646f 6375  top page of docu
-00003400: 6d65 6e74 2074 6f20 2243 6f6e 7465 6e74  ment to "Content
-00003410: 7322 2069 6e20 7369 6465 6261 720a 2a20  s" in sidebar.* 
-00003420: 4164 6420 476f 6f67 6c65 2041 6e61 6c79  Add Google Analy
-00003430: 7469 6373 204a 6176 6153 6372 6970 7420  tics JavaScript 
-00003440: 7472 6163 6b69 6e67 2073 6e69 7070 6574  tracking snippet
-00003450: 2063 6f64 650a 2a20 4164 6420 7265 6e6f   code.* Add reno
-00003460: 2066 6f72 2072 656c 6561 7365 2d6e 6f74   for release-not
-00003470: 6573 0a2a 2041 6464 2070 6164 6469 6e67  es.* Add padding
-00003480: 2063 7373 2070 726f 7065 7274 7920 666f   css property fo
-00003490: 7220 7464 2061 6e64 2074 680a 2a20 5265  r td and th.* Re
-000034a0: 6d6f 7665 2074 6865 206f 7269 6769 6e61  move the origina
-000034b0: 6c2d 6465 7369 676e 2064 6972 6563 746f  l-design directo
-000034c0: 7279 0a0a 312e 322e 340a 2d2d 2d2d 2d0a  ry..1.2.4.-----.
-000034d0: 0a2a 2055 7064 6174 6520 5245 4c45 4153  .* Update RELEAS
-000034e0: 454e 4f54 4553 2066 6f72 2031 2e32 2e34  ENOTES for 1.2.4
-000034f0: 2072 656c 6561 7365 0a2a 2046 6978 2074   release.* Fix t
-00003500: 6865 2062 726f 6b65 6e20 616e 6368 6f72  he broken anchor
-00003510: 2074 6167 730a 2a20 5265 6d6f 7665 2075   tags.* Remove u
-00003520: 6e75 7365 6420 6669 6c65 730a 2a20 4164  nused files.* Ad
-00003530: 6420 7461 626c 6520 7061 6464 696e 6720  d table padding 
-00003540: 746f 206f 7065 6e73 7461 636b 646f 6373  to openstackdocs
-00003550: 7468 656d 6520 4353 530a 2a20 5570 6461  theme CSS.* Upda
-00003560: 7465 2072 656c 6561 7365 7320 696e 2074  te releases in t
-00003570: 6865 206c 6566 7420 7369 6465 6261 720a  he left sidebar.
-00003580: 0a31 2e32 2e33 0a2d 2d2d 2d2d 0a0a 2a20  .1.2.3.-----..* 
-00003590: 5570 6461 7465 206c 6f67 2d61 2d62 7567  Update log-a-bug
-000035a0: 2063 6f6d 6d65 6e74 730a 2a20 4578 7465   comments.* Exte
-000035b0: 6e64 2072 656c 6561 7365 206e 6f74 6573  nd release notes
-000035c0: 2066 6f72 2031 2e32 2e33 0a2a 2044 6563   for 1.2.3.* Dec
-000035d0: 7265 6173 6520 7468 6520 696e 6465 6e74  rease the indent
-000035e0: 206f 6620 544f 4320 656e 7472 6965 7320   of TOC entries 
-000035f0: 6f6e 2074 6865 2032 6e64 206c 6576 656c  on the 2nd level
-00003600: 0a2a 2053 6574 2074 6865 2077 6964 7468  .* Set the width
-00003610: 206f 6620 7468 6520 6869 6768 6c69 6768   of the highligh
-00003620: 7420 7461 626c 6520 746f 2031 3030 250a  t table to 100%.
-00003630: 2a20 4164 6420 7061 6464 696e 6720 746f  * Add padding to
-00003640: 2074 6865 206c 6566 7420 7461 626c 6520   the left table 
-00003650: 6f66 2063 6f6e 7465 6e74 730a 2a20 5265  of contents.* Re
-00003660: 6d6f 7665 2065 7865 6375 7461 626c 6520  move executable 
-00003670: 666c 6167 7320 6672 6f6d 206a 732f 6373  flags from js/cs
-00003680: 7320 6669 6c65 730a 2a20 4164 6420 5245  s files.* Add RE
-00003690: 4c45 4153 454e 4f54 4553 2066 6f72 2031  LEASENOTES for 1
-000036a0: 2e32 2e33 0a2a 2041 6464 2073 7570 706f  .2.3.* Add suppo
-000036b0: 7274 2066 6f72 2046 6972 7374 6170 700a  rt for Firstapp.
-000036c0: 0a31 2e32 2e32 0a2d 2d2d 2d2d 0a0a 2a20  .1.2.2.-----..* 
-000036d0: 4164 6420 7265 6c65 6173 6520 6e6f 7465  Add release note
-000036e0: 7320 666f 7220 7665 7273 696f 6e20 312e  s for version 1.
-000036f0: 322e 320a 2a20 4669 7820 7379 6e74 6178  2.2.* Fix syntax
-00003700: 206f 6620 5245 4c45 4153 454e 4f54 4553   of RELEASENOTES
-00003710: 0a2a 2043 6c65 616e 7570 2048 544d 4c20  .* Cleanup HTML 
-00003720: 6669 6c65 730a 2a20 5265 6d6f 7665 206c  files.* Remove l
-00003730: 6173 7420 7265 6c65 6173 6520 6465 7461  ast release deta
-00003740: 696c 7320 6672 6f6d 2068 6561 6465 722f  ils from header/
-00003750: 666f 6f74 6572 0a2a 2046 6978 206c 696e  footer.* Fix lin
-00003760: 6b73 2f74 6578 7473 2069 6e20 7468 6520  ks/texts in the 
-00003770: 6c69 6365 6e73 6520 666f 6f74 6572 0a2a  license footer.*
-00003780: 204d 6f76 6520 6c69 7374 6564 2067 7569   Move listed gui
-00003790: 6465 7320 696e 2074 6865 2073 6964 6562  des in the sideb
-000037a0: 6172 2069 6e74 6f20 7468 6520 6472 6f70  ar into the drop
-000037b0: 646f 776e 206d 656e 750a 2a20 5265 6d6f  down menu.* Remo
-000037c0: 7665 2074 6865 2027 5369 676e 2069 6e27  ve the 'Sign in'
-000037d0: 206c 696e 6b20 696e 2074 6865 2074 6f70   link in the top
-000037e0: 2062 6172 0a2a 2046 6978 206c 696e 6b73   bar.* Fix links
-000037f0: 2f61 6464 206d 6973 7369 6e67 206c 696e  /add missing lin
-00003800: 6b73 2069 6e20 7468 6520 746f 7020 6261  ks in the top ba
-00003810: 720a 2a20 4669 7820 6c69 6e6b 2074 6f20  r.* Fix link to 
-00003820: 7468 6520 4f70 656e 5374 6163 6b20 7375  the OpenStack su
-00003830: 6d6d 6974 2061 6e64 2072 656d 6f76 6520  mmit and remove 
-00003840: 5061 7269 7320 7265 6c61 7465 6420 4353  Paris related CS
-00003850: 530a 2a20 4c69 6e6b 2074 6865 2041 7061  S.* Link the Apa
-00003860: 6368 6520 322e 3020 6c69 6365 6e73 6520  che 2.0 license 
-00003870: 6e6f 7465 2069 6e20 7468 6520 666f 6f74  note in the foot
-00003880: 6572 0a2a 2052 656d 6f76 6520 2773 7567  er.* Remove 'sug
-00003890: 6765 7374 2065 6469 7473 2720 6c69 6e6b  gest edits' link
-000038a0: 2066 726f 6d20 6c61 796f 7574 0a2a 2052   from layout.* R
-000038b0: 656d 6f76 6520 6475 706c 6963 6174 6520  emove duplicate 
-000038c0: 6173 6b2e 6f70 656e 7374 6163 6b2e 6f72  ask.openstack.or
-000038d0: 6720 6c69 6e6b 2066 726f 6d20 7468 6520  g link from the 
-000038e0: 666f 6f74 6572 0a0a 312e 322e 310a 2d2d  footer..1.2.1.--
-000038f0: 2d2d 2d0a 0a2a 2046 6978 2022 446f 6373  ---..* Fix "Docs
-00003900: 2048 6f6d 6522 206c 696e 6b0a 2a20 4f6e   Home" link.* On
-00003910: 2068 6f76 6572 2064 6f6e 2774 2063 6861   hover don't cha
-00003920: 6e67 6520 7468 6520 6261 636b 6772 6f75  nge the backgrou
-00003930: 6e64 2063 6f6c 6f72 206f 6620 7468 6520  nd color of the 
-00003940: 7369 6465 6261 7220 544f 430a 2a20 4669  sidebar TOC.* Fi
-00003950: 7820 6c69 6e6b 2074 6f20 436c 6f75 6420  x link to Cloud 
-00003960: 4164 6d69 6e20 4775 6964 650a 2a20 5265  Admin Guide.* Re
-00003970: 6d6f 7665 206a 7175 6572 7920 7375 6264  move jquery subd
-00003980: 6972 0a2a 204a 6176 6173 6372 6970 7420  ir.* Javascript 
-00003990: 636c 6561 6e75 700a 2a20 5265 6d6f 7665  cleanup.* Remove
-000039a0: 2075 6e75 7365 6420 696d 6167 6573 0a2a   unused images.*
-000039b0: 2046 6978 2069 6e63 6c75 7369 6f6e 206f   Fix inclusion o
-000039c0: 6620 6d65 7461 7461 6773 0a0a 312e 322e  f metatags..1.2.
-000039d0: 300a 2d2d 2d2d 2d0a 0a2a 204e 6578 7420  0.-----..* Next 
-000039e0: 7265 6c65 6173 6520 6973 2031 2e32 2e30  release is 1.2.0
-000039f0: 0a2a 2055 7064 6174 6520 5245 4c45 4153  .* Update RELEAS
-00003a00: 454e 4f54 4553 2e72 7374 0a2a 2041 6464  ENOTES.rst.* Add
-00003a10: 206e 6578 742c 2070 7265 7669 6f75 732c   next, previous,
-00003a20: 2072 6570 6f72 7420 6120 6275 6720 6275   report a bug bu
-00003a30: 7474 6f6e 7320 6174 2062 6f74 746f 6d0a  ttons at bottom.
-00003a40: 2a20 4669 7820 666f 7220 5253 5420 656e  * Fix for RST en
-00003a50: 756d 6572 6174 6564 206c 6973 742c 206c  umerated list, l
-00003a60: 6f77 6572 616c 7068 610a 2a20 4164 6420  oweralpha.* Add 
-00003a70: 7369 6465 6261 7220 6479 6e61 6d69 6320  sidebar dynamic 
-00003a80: 544f 4320 6f66 2063 6f6e 7465 6e74 0a2a  TOC of content.*
-00003a90: 2046 6978 6564 204b 6f72 6561 6e20 7479   Fixed Korean ty
-00003aa0: 706f 206f 6e20 7369 6465 6261 7274 6f63  po on sidebartoc
-00003ab0: 0a0a 312e 312e 300a 2d2d 2d2d 2d0a 0a2a  ..1.1.0.-----..*
-00003ac0: 204e 6578 7420 7265 6c65 6173 6520 6973   Next release is
-00003ad0: 2031 2e31 2e30 0a2a 2041 6464 7320 7265   1.1.0.* Adds re
-00003ae0: 6c65 6173 6520 6e6f 7465 7320 656e 7472  lease notes entr
-00003af0: 6965 7320 666f 7220 312e 302e 3820 616e  ies for 1.0.8 an
-00003b00: 6420 312e 302e 390a 2a20 4164 6473 206f  d 1.0.9.* Adds o
-00003b10: 7269 6769 6e61 6c20 6465 7369 676e 2066  riginal design f
-00003b20: 696c 6573 2069 6e63 6c75 6469 6e67 2043  iles including C
-00003b30: 5353 2061 6e64 204a 530a 2a20 4d6f 7665  SS and JS.* Move
-00003b40: 2f69 6d70 726f 7665 2074 6865 2070 7265  /improve the pre
-00003b50: 7669 6f75 732f 6e65 7874 206c 696e 6b73  vious/next links
-00003b60: 2069 6e20 7468 6520 6c65 6674 2073 6964   in the left sid
-00003b70: 6562 6172 0a2a 2043 6c65 616e 7570 2063  ebar.* Cleanup c
-00003b80: 7373 2f73 7479 6c65 732e 6373 730a 2a20  ss/styles.css.* 
-00003b90: 4c6f 6741 4275 673a 2050 7562 6c69 7368  LogABug: Publish
-00003ba0: 2055 524c 206f 6620 6375 7272 656e 7420   URL of current 
-00003bb0: 7061 6765 0a2a 2055 7365 206f 732e 6765  page.* Use os.ge
-00003bc0: 7463 7764 2829 2069 6e73 7465 6164 206f  tcwd() instead o
-00003bd0: 6620 7368 656c 6c69 6e67 206f 7574 2074  f shelling out t
-00003be0: 6f20 7275 6e20 7077 640a 2a20 2252 6570  o run pwd.* "Rep
-00003bf0: 6f72 7420 6120 6275 6722 206c 696e 6b20  ort a bug" link 
-00003c00: 696e 2048 544d 4c20 6d61 6e75 616c 7320  in HTML manuals 
-00003c10: 6175 746f 6d61 7469 6361 6c6c 7920 6669  automatically fi
-00003c20: 6c6c 7320 696e 2062 7567 2773 2074 6167  lls in bug's tag
-00003c30: 0a2a 2041 6464 7320 4353 5320 666f 7220  .* Adds CSS for 
-00003c40: 676c 6f73 7361 7279 2064 6566 696e 6974  glossary definit
-00003c50: 696f 6e73 2074 6f20 6265 2069 6e64 656e  ions to be inden
-00003c60: 7465 640a 2a20 5570 6461 7465 2068 6163  ted.* Update hac
-00003c70: 6b69 6e67 2074 6f20 6669 7820 7065 7038  king to fix pep8
-00003c80: 2066 6169 6c75 7265 0a0a 312e 302e 380a   failure..1.0.8.
-00003c90: 2d2d 2d2d 2d0a 0a2a 204d 616b 6520 7468  -----..* Make th
-00003ca0: 6520 6e61 7669 6761 7469 6f6e 206c 696e  e navigation lin
-00003cb0: 6b73 2062 6967 6765 720a 2a20 5265 6d6f  ks bigger.* Remo
-00003cc0: 7665 202f 7472 756e 6b2c 2069 7420 646f  ve /trunk, it do
-00003cd0: 6573 206e 6f74 2065 7869 7374 2061 6e79  es not exist any
-00003ce0: 6d6f 7265 0a2a 204b 696c 6f20 6973 2063  more.* Kilo is c
-00003cf0: 7572 7265 6e74 2072 656c 6561 7365 0a2a  urrent release.*
-00003d00: 2044 6f63 756d 656e 7420 636f 6e66 2e70   Document conf.p
-00003d10: 7920 7661 7269 6162 6c65 730a 2a20 4f70  y variables.* Op
-00003d20: 656e 7374 6163 6b64 6f63 7374 6865 6d65  enstackdocstheme
-00003d30: 3a20 6c6f 672d 612d 6275 6720 7072 6566  : log-a-bug pref
-00003d40: 696c 6c73 2077 726f 6e67 2073 6f75 7263  ills wrong sourc
-00003d50: 6520 6669 6c65 0a2a 2049 676e 6f72 6520  e file.* Ignore 
-00003d60: 746f 7820 6469 7265 6374 6f72 790a 0a31  tox directory..1
-00003d70: 2e30 2e37 0a2d 2d2d 2d2d 0a0a 2a20 4164  .0.7.-----..* Ad
-00003d80: 6473 2072 656c 6561 7365 206e 6f74 6573  ds release notes
-00003d90: 2066 6f72 2031 2e30 2e37 0a2a 2022 6c6f   for 1.0.7.* "lo
-00003da0: 6720 6120 6275 6722 206c 696e 6b20 6164  g a bug" link ad
-00003db0: 6465 6420 746f 2053 7068 696e 782d 6261  ded to Sphinx-ba
-00003dc0: 7365 6420 646f 6375 6d65 6e74 6174 696f  sed documentatio
-00003dd0: 6e0a 2a20 4669 7820 7479 706f 2069 6e20  n.* Fix typo in 
-00003de0: 696e 6920 626c 6f63 6b20 7365 6374 696f  ini block sectio
-00003df0: 6e0a 0a31 2e30 2e36 0a2d 2d2d 2d2d 0a0a  n..1.0.6.-----..
-00003e00: 2a20 4164 6473 2072 656c 6561 7365 206e  * Adds release n
-00003e10: 6f74 6573 2066 6f72 2031 2e30 2e36 0a2a  otes for 1.0.6.*
-00003e20: 2041 6464 2074 6865 206f 7574 7075 7420   Add the output 
-00003e30: 6672 6f6d 2070 7967 6d65 6e74 697a 650a  from pygmentize.
-00003e40: 2a20 4164 6473 206c 696e 6b73 2069 6e20  * Adds links in 
-00003e50: 7369 6465 6261 7220 6e61 7620 7468 6174  sidebar nav that
-00003e60: 2067 6f20 746f 2064 6f63 7320 6c61 6e64   go to docs land
-00003e70: 696e 6720 7061 6765 0a0a 312e 302e 350a  ing page..1.0.5.
-00003e80: 2d2d 2d2d 2d0a 0a2a 2041 6464 7320 7265  -----..* Adds re
-00003e90: 6c65 6173 6520 6e6f 7465 7320 666f 7220  lease notes for 
-00003ea0: 312e 302e 350a 2a20 4164 6473 2061 206e  1.0.5.* Adds a n
-00003eb0: 6f6e 2d62 7265 616b 696e 6720 7370 6163  on-breaking spac
-00003ec0: 6520 6265 666f 7265 204e 4558 5420 666f  e before NEXT fo
-00003ed0: 7220 6265 7474 6572 2073 7061 6369 6e67  r better spacing
-00003ee0: 2061 726f 756e 6420 7069 7065 0a2a 2041   around pipe.* A
-00003ef0: 6464 7320 476f 6f67 6c65 2043 7573 746f  dds Google Custo
-00003f00: 6d20 5365 6172 6368 2045 6e67 696e 6520  m Search Engine 
-00003f10: 7261 7468 6572 2074 6861 6e20 6765 6e65  rather than gene
-00003f20: 7269 6320 666f 726d 0a2a 2055 7064 6174  ric form.* Updat
-00003f30: 6573 2066 6f72 2063 632d 6279 206c 6963  es for cc-by lic
-00003f40: 656e 7369 6e67 0a2a 2041 6464 7320 6e65  ensing.* Adds ne
-00003f50: 7874 2061 6e64 2070 7265 7669 6f75 7320  xt and previous 
-00003f60: 6c69 6e6b 730a 0a31 2e30 2e34 0a2d 2d2d  links..1.0.4.---
-00003f70: 2d2d 0a0a 2a20 4164 6473 2072 656c 6561  --..* Adds relea
-00003f80: 7365 206e 6f74 6573 2066 6f72 2031 2e30  se notes for 1.0
-00003f90: 2e33 2061 6e64 2031 2e30 2e34 0a2a 2052  .3 and 1.0.4.* R
-00003fa0: 656e 6465 7269 6e67 2061 646d 6f6e 6974  endering admonit
-00003fb0: 696f 6e73 2077 6974 6820 466f 6e74 2041  ions with Font A
-00003fc0: 7765 736f 6d65 2069 636f 6e73 0a2a 2046  wesome icons.* F
-00003fd0: 6978 2066 6f72 2075 6e77 616e 7465 6420  ix for unwanted 
-00003fe0: 706c 7573 2073 6967 6e20 696e 2073 7562  plus sign in sub
-00003ff0: 6c69 7374 730a 2a20 436f 6d6d 656e 7473  lists.* Comments
-00004000: 206f 7574 206e 6f6e 2d77 6f72 6b69 6e67   out non-working
-00004010: 2064 6f63 7320 6163 7469 6f6e 7320 666f   docs actions fo
-00004020: 7220 6e6f 770a 0a31 2e30 2e33 0a2d 2d2d  r now..1.0.3.---
-00004030: 2d2d 0a0a 2a20 4164 6420 696e 7374 7275  --..* Add instru
-00004040: 6374 696f 6e73 2074 6f20 7468 6520 5245  ctions to the RE
-00004050: 4144 4d45 0a2a 2052 656d 6f76 6564 206c  ADME.* Removed l
-00004060: 6974 6572 616c 2063 6172 7269 6167 6520  iteral carriage 
-00004070: 7265 7475 726e 7320 6672 6f6d 206c 6963  returns from lic
-00004080: 656e 7365 2e74 7874 0a2a 204d 6f76 6520  ense.txt.* Move 
-00004090: 7468 6520 6c69 6365 6e73 6520 696e 666f  the license info
-000040a0: 726d 6174 696f 6e20 696e 746f 2061 2073  rmation into a s
-000040b0: 6570 6172 6174 6520 6669 6c65 0a2a 2041  eparate file.* A
-000040c0: 6464 7320 5265 6c65 6173 6520 4e6f 7465  dds Release Note
-000040d0: 730a 2a20 5570 6461 7465 7320 7361 6d70  s.* Updates samp
-000040e0: 6c65 2074 6f20 696e 636c 7564 6520 6c69  le to include li
-000040f0: 6e65 6e6f 7320 666f 7220 5370 6869 6e78  nenos for Sphinx
-00004100: 206c 696e 6520 6e75 6d62 6572 696e 670a   line numbering.
-00004110: 2a20 6164 6420 6120 2e67 6974 7265 7669  * add a .gitrevi
-00004120: 6577 2066 696c 650a 0a31 2e30 2e31 0a2d  ew file..1.0.1.-
-00004130: 2d2d 2d2d 0a0a 2a20 5468 656d 6520 6e65  ----..* Theme ne
-00004140: 6564 7320 6120 7365 7475 7020 6675 6e63  eds a setup func
-00004150: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00004160: 6672 6f6d 2070 6163 6b61 6765 0a0a 312e  from package..1.
-00004170: 302e 320a 2d2d 2d2d 2d0a 0a2a 204d 6f64  0.2.-----..* Mod
-00004180: 6966 6965 7320 636f 6d62 696e 6564 2e63  ifies combined.c
-00004190: 7373 2074 6f20 6d61 7463 6820 636c 6173  ss to match clas
-000041a0: 7365 7320 666f 7220 6164 6d6f 6e69 7469  ses for admoniti
-000041b0: 6f6e 0a2a 2041 6464 7320 636f 7272 6563  on.* Adds correc
-000041c0: 7420 3a72 6566 3a20 666f 7220 6372 6f73  t :ref: for cros
-000041d0: 7320 6c69 6e6b 696e 670a 2a20 4164 6473  s linking.* Adds
-000041e0: 2063 6f72 7265 6374 2072 7374 206d 6172   correct rst mar
-000041f0: 6b75 7020 666f 7220 696d 6167 6520 696e  kup for image in
-00004200: 7365 7274 696f 6e0a 2a20 4164 6473 206d  sertion.* Adds m
-00004210: 6f72 6520 7273 7420 666f 7220 7465 7374  ore rst for test
-00004220: 696e 670a 2a20 5570 6461 7465 7320 636f  ing.* Updates co
-00004230: 6d62 696e 6564 2e63 7373 2074 6f20 6869  mbined.css to hi
-00004240: 6465 2070 6172 6120 7379 6d62 6f6c 2075  de para symbol u
-00004250: 6e74 696c 2075 7365 7220 686f 7665 7273  ntil user hovers
-00004260: 206f 7665 7220 6974 0a2a 204d 6f76 6573   over it.* Moves
-00004270: 2043 5353 2063 6861 6e67 6520 6672 6f6d   CSS change from
-00004280: 2062 6f6f 7473 7472 6170 2074 6f20 636f   bootstrap to co
-00004290: 6d62 696e 6564 2e63 7373 0a2a 2055 7064  mbined.css.* Upd
-000042a0: 6174 6573 203c 7072 653e 2073 6f20 7468  ates <pre> so th
-000042b0: 6174 2079 6f75 2063 616e 2073 6565 2077  at you can see w
-000042c0: 6869 7465 2074 6578 7420 6f6e 2064 6172  hite text on dar
-000042d0: 6b20 6772 6579 2062 6163 6b67 726f 756e  k grey backgroun
-000042e0: 640a 2a20 4164 6473 2061 6e6f 7468 6572  d.* Adds another
-000042f0: 2073 616d 706c 6520 5253 5420 6669 6c65   sample RST file
-00004300: 2066 6f72 2074 6573 7469 6e67 0a2a 2041   for testing.* A
-00004310: 6464 7320 7365 6374 696f 6e20 666f 7220  dds section for 
-00004320: 7465 7374 696e 6720 7075 7270 6f73 6573  testing purposes
-00004330: 0a2a 2066 6978 2070 6174 6820 746f 206a  .* fix path to j
-00004340: 7175 6572 790a 2a20 6669 7820 7273 7420  query.* fix rst 
-00004350: 7379 6e74 6178 0a2a 2055 7365 2070 6174  syntax.* Use pat
-00004360: 6874 6f28 2920 746f 2063 6f6d 7075 7465  hto() to compute
-00004370: 2072 656c 6174 6976 6520 7061 7468 7320   relative paths 
-00004380: 746f 2073 7461 7469 6320 6669 6c65 730a  to static files.
-00004390: 2a20 5265 6e61 6d65 205c 5f73 7461 7469  * Rename \_stati
-000043a0: 6320 746f 2073 7461 7469 630a 2a20 436c  c to static.* Cl
-000043b0: 6561 6e20 7570 2067 6574 5c5f 6874 6d6c  ean up get\_html
-000043c0: 5c5f 7468 656d 655c 5f70 6174 680a 2a20  \_theme\_path.* 
-000043d0: 446f 6e27 7420 666f 7263 652d 696e 6a65  Don't force-inje
-000043e0: 6374 2074 6865 2074 6865 6d65 0a2a 204d  ct the theme.* M
-000043f0: 6f76 6520 7468 656d 6520 6669 6c65 7320  ove theme files 
-00004400: 696e 746f 2063 6f72 7265 6374 2066 6f72  into correct for
-00004410: 6d61 7469 6f6e 0a2a 2055 7064 6174 6520  mation.* Update 
-00004420: 666c 616b 6538 2063 6f6d 6d61 6e64 730a  flake8 commands.
-00004430: 2a20 5570 6461 7465 202e 6769 7469 676e  * Update .gitign
-00004440: 6f72 650a 2a20 5265 6d6f 7665 7320 7265  ore.* Removes re
-00004450: 6475 6e64 616e 7420 7374 6174 6963 2066  dundant static f
-00004460: 696c 6573 2061 6e64 2074 656d 706c 6174  iles and templat
-00004470: 6520 6669 6c65 730a 2a20 5265 6d6f 7665  e files.* Remove
-00004480: 7320 756e 6565 6465 6420 6669 6c65 730a  s uneeded files.
-00004490: 2a20 4164 6473 2072 6561 7272 616e 6765  * Adds rearrange
-000044a0: 6420 6669 6c65 7320 666f 7220 7265 6e61  d files for rena
-000044b0: 6d65 2074 6f20 6f70 656e 7374 6163 6b64  me to openstackd
-000044c0: 6f63 7374 6865 6d65 0a2a 2041 6464 7320  ocstheme.* Adds 
-000044d0: 776f 726b 696e 6720 6c69 6e6b 7320 746f  working links to
-000044e0: 206e 6176 6967 6174 696f 6e20 6472 6f70   navigation drop
-000044f0: 646f 776e 2061 6e64 2063 6f6c 756d 6e0a  down and column.
-00004500: 2a20 5465 6d70 6c61 7465 7320 6e6f 7720  * Templates now 
-00004510: 7375 7070 6f72 7420 6469 7673 2063 6f72  support divs cor
-00004520: 7265 6374 6c79 0a2a 2041 6464 7320 7469  rectly.* Adds ti
-00004530: 746c 6520 726f 772c 2062 7574 746f 6e20  tle row, button 
-00004540: 726f 772c 2075 7064 6174 6564 2072 6f77  row, updated row
-00004550: 732c 2061 6e64 2073 6964 6562 6172 0a2a  s, and sidebar.*
-00004560: 2053 7461 7274 696e 6720 706f 696e 7420   Starting point 
-00004570: 666f 7220 5370 6869 6e78 2074 6865 6d65  for Sphinx theme
-00004580: 2066 6f72 2064 6f63 732e 6f70 656e 7374   for docs.openst
-00004590: 6163 6b2e 6f72 6720 636f 6e74 656e 740a  ack.org content.
+00000010: 0a33 2e31 2e31 0a2d 2d2d 2d2d 0a0a 2a20  .3.1.1.-----..* 
+00000020: 5265 6d6f 7665 2027 7479 7065 2720 6174  Remove 'type' at
+00000030: 7472 6962 7574 6520 6f66 203c 7363 7269  tribute of <scri
+00000040: 7074 3e20 656c 656d 656e 740a 2a20 5265  pt> element.* Re
+00000050: 6d6f 7665 2069 6e76 616c 6964 2061 7474  move invalid att
+00000060: 7269 6275 7465 730a 2a20 5265 6d6f 7665  ributes.* Remove
+00000070: 2065 7272 616e 7420 6368 6172 6163 7465   errant characte
+00000080: 720a 2a20 5265 6d6f 7665 206e 6573 7465  r.* Remove neste
+00000090: 6420 276c 6927 0a2a 2052 6570 6c61 6365  d 'li'.* Replace
+000000a0: 2061 6d70 6572 7361 6e64 2077 6974 6820   ampersand with 
+000000b0: 4854 4d4c 2063 6861 7261 6374 6572 730a  HTML characters.
+000000c0: 0a33 2e31 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .3.1.0.-----..* 
+000000d0: 4f6e 6c79 2068 6964 6520 746f 702d 6c65  Only hide top-le
+000000e0: 7665 6c20 6475 706c 6963 6174 6564 2074  vel duplicated t
+000000f0: 6974 6c65 0a0a 332e 302e 310a 2d2d 2d2d  itle..3.0.1.----
+00000100: 2d0a 0a2a 2055 7064 6174 6520 696e 636c  -..* Update incl
+00000110: 7564 6564 2070 6167 6520 666f 6f74 6572  uded page footer
+00000120: 7320 746f 2075 7365 2063 7572 7265 6e74  s to use current
+00000130: 2055 524c 730a 0a33 2e30 2e30 0a2d 2d2d   URLs..3.0.0.---
+00000140: 2d2d 0a0a 2a20 4472 6f70 2070 7974 686f  --..* Drop pytho
+00000150: 6e33 2e36 2f33 2e37 2073 7570 706f 7274  n3.6/3.7 support
+00000160: 2069 6e20 7465 7374 696e 6720 7275 6e74   in testing runt
+00000170: 696d 650a 2a20 4669 7820 6272 6f6b 656e  ime.* Fix broken
+00000180: 206c 696e 6b20 666f 7220 4d61 726b 6574   link for Market
+00000190: 706c 6163 6520 696e 2068 6561 6465 720a  place in header.
+000001a0: 0a32 2e34 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .2.4.0.-----..* 
+000001b0: 4669 7820 4f70 656e 5374 6163 6b20 7072  Fix OpenStack pr
+000001c0: 6f6a 6563 7420 2253 6561 7263 6822 2070  oject "Search" p
+000001d0: 6167 6573 0a0a 322e 332e 310a 2d2d 2d2d  ages..2.3.1.----
+000001e0: 2d0a 0a2a 2050 6167 6520 6865 6164 6572  -..* Page header
+000001f0: 2066 6978 2077 6974 6820 5370 6869 6e78   fix with Sphinx
+00000200: 340a 0a32 2e33 2e30 0a2d 2d2d 2d2d 0a0a  4..2.3.0.-----..
+00000210: 2a20 496e 6865 7269 7420 6672 6f6d 2062  * Inherit from b
+00000220: 6173 6520 2262 6173 6963 2220 7465 6d70  ase "basic" temp
+00000230: 6c61 7465 0a2a 2073 7068 696e 7820 342e  late.* sphinx 4.
+00000240: 303a 2048 616e 646c 6520 4854 4d4c 2035  0: Handle HTML 5
+00000250: 2063 6861 6e67 6573 0a2a 2073 7068 696e   changes.* sphin
+00000260: 7820 342e 303a 2046 6978 2073 7068 696e  x 4.0: Fix sphin
+00000270: 782e 6578 742e 6578 746c 696e 6b73 2e6d  x.ext.extlinks.m
+00000280: 616b 655c 5f6c 696e 6b5c 5f72 6f6c 6520  ake\_link\_role 
+00000290: 6361 6c6c 0a2a 2074 6f78 3a20 546f 6767  call.* tox: Togg
+000002a0: 6c65 2027 7573 6564 6576 656c 6f70 270a  le 'usedevelop'.
+000002b0: 2a20 7472 6976 6961 6c3a 2046 6978 2069  * trivial: Fix i
+000002c0: 6e64 656e 7461 7469 6f6e 0a2a 2043 6861  ndentation.* Cha
+000002d0: 6e67 6520 746f 204f 4654 430a 2a20 7365  nge to OFTC.* se
+000002e0: 7475 702e 6366 673a 2052 6570 6c61 6365  tup.cfg: Replace
+000002f0: 2064 6173 6865 7320 7769 7468 2075 6e64   dashes with und
+00000300: 6572 7363 6f72 6573 0a2a 204d 6f76 6520  erscores.* Move 
+00000310: 666c 616b 6538 2061 7320 6120 7072 652d  flake8 as a pre-
+00000320: 636f 6d6d 6974 206c 6f63 616c 2074 6172  commit local tar
+00000330: 6765 740a 2a20 5570 6461 7465 6420 4e61  get.* Updated Na
+00000340: 7620 4d65 6e75 0a2a 2055 7365 2054 4f58  v Menu.* Use TOX
+00000350: 5c5f 434f 4e53 5452 4149 4e54 535c 5f46  \_CONSTRAINTS\_F
+00000360: 494c 450a 0a32 2e32 2e37 0a2d 2d2d 2d2d  ILE..2.2.7.-----
+00000370: 0a0a 2a20 4164 6465 6420 7374 796c 696e  ..* Added stylin
+00000380: 6720 666f 7220 7253 5420 7275 6272 6963  g for rST rubric
+00000390: 2064 6972 6563 7469 7665 0a0a 322e 322e   directive..2.2.
+000003a0: 360a 2d2d 2d2d 2d0a 0a2a 2043 6861 6e67  6.-----..* Chang
+000003b0: 6520 6e61 6d65 206f 6620 4f70 656e 5374  e name of OpenSt
+000003c0: 6163 6b20 466f 756e 6461 7469 6f6e 0a2a  ack Foundation.*
+000003d0: 2074 7269 7669 616c 3a20 4164 6472 6573   trivial: Addres
+000003e0: 7320 736f 6d65 2069 6e64 656e 7461 7469  s some indentati
+000003f0: 6f6e 206e 6974 730a 2a20 6a73 3a20 446f  on nits.* js: Do
+00000400: 6e27 7420 6174 7465 6d70 7420 746f 2073  n't attempt to s
+00000410: 6574 2062 7567 2c20 5044 4620 6c69 6e6b  et bug, PDF link
+00000420: 7320 7769 7468 6f75 7420 636f 6e66 6967  s without config
+00000430: 7572 6174 696f 6e0a 2a20 5374 6f72 6520  uration.* Store 
+00000440: 656d 7074 7920 7374 7269 6e67 2066 6f72  empty string for
+00000450: 2072 656c 6561 7365 0a2a 206a 733a 2053   release.* js: S
+00000460: 6574 2027 4c49 4e4b 5c5f 5355 4646 4958  et 'LINK\_SUFFIX
+00000470: 270a 2a20 4164 6469 6e67 2070 7265 2d63  '.* Adding pre-c
+00000480: 6f6d 6d69 740a 2a20 5265 6d6f 7665 2061  ommit.* Remove a
+00000490: 736b 2e6f 2e6f 0a0a 322e 322e 350a 2d2d  sk.o.o..2.2.5.--
+000004a0: 2d2d 2d0a 0a2a 2041 6464 2076 6572 7369  ---..* Add versi
+000004b0: 6f6e 2064 726f 7064 6f77 6e20 6f6e 2064  on dropdown on d
+000004c0: 6f63 732e 7374 6172 6c69 6e67 782e 696f  ocs.starlingx.io
+000004d0: 0a0a 322e 322e 340a 2d2d 2d2d 2d0a 0a2a  ..2.2.4.-----..*
+000004e0: 2043 6861 6e67 696e 6720 7468 6520 7363   Changing the sc
+000004f0: 6f70 6520 6f66 2074 6865 2073 6561 7263  ope of the searc
+00000500: 6820 6261 7220 6f6e 2064 6f63 732e 7374  h bar on docs.st
+00000510: 6172 6c69 6e67 782e 696f 0a0a 322e 322e  arlingx.io..2.2.
+00000520: 330a 2d2d 2d2d 2d0a 0a2a 2041 6464 2070  3.-----..* Add p
+00000530: 7933 3820 7061 636b 6167 6520 6d65 7461  y38 package meta
+00000540: 6461 7461 0a0a 322e 322e 320a 2d2d 2d2d  data..2.2.2.----
+00000550: 2d0a 0a2a 204c 6f77 6572 206c 6f67 6769  -..* Lower loggi
+00000560: 6e67 206c 6576 656c 206f 6620 7064 662d  ng level of pdf-
+00000570: 7265 6c61 7465 6420 6c6f 6773 0a2a 2049  related logs.* I
+00000580: 676e 6f72 6520 276c 6173 745c 5f75 7064  gnore 'last\_upd
+00000590: 6174 6564 2720 666f 7220 6175 746f 2d67  ated' for auto-g
+000005a0: 656e 6572 6174 6564 2070 6167 6573 0a2a  enerated pages.*
+000005b0: 2046 6978 2068 6163 6b69 6e67 206d 696e   Fix hacking min
+000005c0: 2076 6572 7369 6f6e 2074 6f20 332e 302e   version to 3.0.
+000005d0: 310a 0a32 2e32 2e31 0a2d 2d2d 2d2d 0a0a  1..2.2.1.-----..
+000005e0: 2a20 5368 6f77 2076 6572 7369 6f6e 2069  * Show version i
+000005f0: 6e20 5044 4673 0a2a 2041 6464 206f 6374  n PDFs.* Add oct
+00000600: 6176 6961 636c 6965 6e74 2063 726f 7373  aviaclient cross
+00000610: 206a 6f62 0a2a 2046 6978 2061 7574 6f5c   job.* Fix auto\
+00000620: 5f6e 616d 6520 6c6f 6769 630a 0a32 2e32  _name logic..2.2
+00000630: 2e30 0a2d 2d2d 2d2d 0a0a 2a20 4164 6420  .0.-----..* Add 
+00000640: 6c69 6e6b 2074 6f20 5044 4620 6669 6c65  link to PDF file
+00000650: 0a2a 2043 6c65 616e 7570 2062 696e 6465  .* Cleanup binde
+00000660: 700a 2a20 4164 6420 6372 6f73 732d 7465  p.* Add cross-te
+00000670: 7374 7320 666f 7220 6e6f 7661 0a2a 2045  sts for nova.* E
+00000680: 6e61 626c 6520 7061 7261 6c6c 656c 2062  nable parallel b
+00000690: 7569 6c64 696e 670a 2a20 5573 6520 636f  uilding.* Use co
+000006a0: 6e73 6973 7465 6e74 206c 6f67 6769 6e67  nsistent logging
+000006b0: 0a2a 2074 7269 7669 616c 3a20 5265 6d6f  .* trivial: Remo
+000006c0: 7665 206c 6566 746f 7665 7220 5079 7468  ve leftover Pyth
+000006d0: 6f6e 2032 2063 6f64 650a 2a20 5072 6f76  on 2 code.* Prov
+000006e0: 6964 6520 6578 7465 6e73 696f 6e20 7665  ide extension ve
+000006f0: 7273 696f 6e0a 0a32 2e31 2e32 0a2d 2d2d  rsion..2.1.2.---
+00000700: 2d2d 0a0a 2a20 5570 6461 7465 2064 6f63  --..* Update doc
+00000710: 7374 6865 6d65 0a2a 2055 7365 2078 656c  stheme.* Use xel
+00000720: 6174 6578 2061 7320 6c61 7465 785c 5f65  atex as latex\_e
+00000730: 6e67 696e 650a 0a32 2e31 2e31 0a2d 2d2d  ngine..2.1.1.---
+00000740: 2d2d 0a0a 2a20 5265 7374 6f72 6520 636f  --..* Restore co
+00000750: 6e66 6967 7572 6174 696f 6e20 6f66 2027  nfiguration of '
+00000760: 6c61 7465 785c 5f65 6e67 696e 6527 0a0a  latex\_engine'..
+00000770: 322e 312e 300a 2d2d 2d2d 2d0a 0a2a 2074  2.1.0.-----..* t
+00000780: 7269 7669 616c 3a20 4164 6420 7768 6974  rivial: Add whit
+00000790: 6573 7061 6365 0a2a 2041 6464 2070 6163  espace.* Add pac
+000007a0: 6b61 6765 2070 7265 6669 7865 7320 666f  kage prefixes fo
+000007b0: 7220 616c 6c20 636f 6e66 6967 206f 7074  r all config opt
+000007c0: 696f 6e73 0a2a 2052 656d 6f76 6520 7665  ions.* Remove ve
+000007d0: 6e64 6f72 6564 2027 6e61 7469 7665 2720  ndored 'native' 
+000007e0: 5079 676d 656e 7473 2074 6865 6d65 0a2a  Pygments theme.*
+000007f0: 2063 7373 3a20 4e61 6d65 7370 6163 6520   css: Namespace 
+00000800: 5079 676d 656e 7473 2073 7479 6c65 7368  Pygments stylesh
+00000810: 6565 740a 2a20 4d65 7267 652c 2072 6174  eet.* Merge, rat
+00000820: 6865 7220 7468 616e 206f 7665 7277 7269  her than overwri
+00000830: 7465 2c20 4c61 5465 5820 7365 7474 696e  te, LaTeX settin
+00000840: 6773 0a2a 2041 6464 2027 6f70 656e 7374  gs.* Add 'openst
+00000850: 6163 6b64 6f63 735c 5f61 7574 6f5c 5f6e  ackdocs\_auto\_n
+00000860: 616d 6527 2063 6f6e 6669 6720 6f70 7469  ame' config opti
+00000870: 6f6e 0a2a 2041 6464 2027 6f70 656e 7374  on.* Add 'openst
+00000880: 6163 6b64 6f63 735c 5f61 7574 6f5c 5f76  ackdocs\_auto\_v
+00000890: 6572 7369 6f6e 2720 636f 6e66 6967 206f  ersion' config o
+000008a0: 7074 696f 6e2c 2070 6174 6820 6368 6563  ption, path chec
+000008b0: 6b69 6e67 0a2a 204d 6172 6b20 7370 6869  king.* Mark sphi
+000008c0: 6e78 2065 7874 656e 7369 6f6e 7320 7468  nx extensions th
+000008d0: 7265 6164 2073 6166 650a 0a32 2e30 2e32  read safe..2.0.2
+000008e0: 0a2d 2d2d 2d2d 0a0a 2a20 5570 6461 7465  .-----..* Update
+000008f0: 2068 6163 6b69 6e67 2066 6f72 2050 7974   hacking for Pyt
+00000900: 686f 6e33 0a0a 322e 302e 310a 2d2d 2d2d  hon3..2.0.1.----
+00000910: 2d0a 0a2a 2055 7064 6174 6520 7365 7665  -..* Update seve
+00000920: 7261 6c20 6c69 6e6b 730a 2a20 446f 206e  ral links.* Do n
+00000930: 6f74 2073 6574 2068 746d 6c5c 5f6c 6173  ot set html\_las
+00000940: 745c 5f75 7064 6174 6564 5c5f 666d 740a  t\_updated\_fmt.
+00000950: 0a32 2e30 2e30 0a2d 2d2d 2d2d 0a0a 2a20  .2.0.0.-----..* 
+00000960: 4669 7820 6272 6f6b 656e 2055 524c 730a  Fix broken URLs.
+00000970: 2a20 5b75 7373 7572 695d 5b67 6f61 6c5d  * [ussuri][goal]
+00000980: 2044 726f 7020 7079 7468 6f6e 2032 2e37   Drop python 2.7
+00000990: 2073 7570 706f 7274 2061 6e64 2074 6573   support and tes
+000009a0: 7469 6e67 0a0a 312e 3331 2e32 0a2d 2d2d  ting..1.31.2.---
+000009b0: 2d2d 2d0a 0a2a 204d 6f76 6520 7665 7273  ---..* Move vers
+000009c0: 696f 6e20 6472 6f70 646f 776e 2074 6f20  ion dropdown to 
+000009d0: 7469 746c 6520 6c69 6e65 0a2a 2049 6d70  title line.* Imp
+000009e0: 726f 7665 2064 6f63 7320 7469 746c 6520  rove docs title 
+000009f0: 7374 796c 650a 2a20 4665 7463 6820 6765  style.* Fetch ge
+00000a00: 6e65 7261 7465 6420 5044 4620 6669 6c65  nerated PDF file
+00000a10: 7320 636f 7272 6563 746c 790a 2a20 4361  s correctly.* Ca
+00000a20: 7463 6820 616e 7920 6578 6365 7074 696f  tch any exceptio
+00000a30: 6e20 7768 656e 2074 7279 696e 6720 746f  n when trying to
+00000a40: 2063 616c 6c20 2267 6974 220a 0a31 2e33   call "git"..1.3
+00000a50: 312e 310a 2d2d 2d2d 2d2d 0a0a 2a20 4669  1.1.------..* Fi
+00000a60: 7820 7665 7273 696f 6e20 6472 6f70 646f  x version dropdo
+00000a70: 776e 0a0a 312e 3331 2e30 0a2d 2d2d 2d2d  wn..1.31.0.-----
+00000a80: 2d0a 0a2a 2055 7064 6174 6520 4150 4920  -..* Update API 
+00000a90: 7369 6465 6261 720a 2a20 5570 6461 7465  sidebar.* Update
+00000aa0: 2061 7069 2d72 6566 206c 6f63 6174 696f   api-ref locatio
+00000ab0: 6e0a 2a20 4d61 6b65 2027 646f 6373 7468  n.* Make 'docsth
+00000ac0: 656d 652d 6275 696c 642d 7064 6627 2065  eme-build-pdf' e
+00000ad0: 7865 6375 7461 626c 650a 2a20 4164 6420  xecutable.* Add 
+00000ae0: 2764 6f63 7374 6865 6d65 2d62 7569 6c64  'docstheme-build
+00000af0: 2d70 6466 2720 7363 7269 7074 0a2a 2073  -pdf' script.* s
+00000b00: 6574 7570 2e63 6667 3a20 5265 6d6f 7665  etup.cfg: Remove
+00000b10: 2072 656d 616e 656e 7473 206f 6620 2762   remanents of 'b
+00000b20: 7569 6c64 5c5f 7370 6869 6e78 2720 7573  uild\_sphinx' us
+00000b30: 6167 650a 2a20 4164 6420 6d69 7373 696e  age.* Add missin
+00000b40: 6720 2772 6f6c 653d 226d 6169 6e22 2720  g 'role="main"' 
+00000b50: 6174 7472 6962 7574 650a 2a20 6373 733a  attribute.* css:
+00000b60: 2047 656e 6572 616c 2063 6c65 616e 7570   General cleanup
+00000b70: 0a2a 206a 733a 2046 6978 2073 6f6d 6520  .* js: Fix some 
+00000b80: 636f 6d6d 656e 7473 0a2a 206a 733a 2052  comments.* js: R
+00000b90: 656d 6f76 6520 6465 6164 206f 7220 756e  emove dead or un
+00000ba0: 7573 6564 204a 530a 2a20 4164 6420 7265  used JS.* Add re
+00000bb0: 6e6f 2066 6f72 2072 6563 656e 7420 4353  no for recent CS
+00000bc0: 5320 636c 6561 6e75 7073 0a2a 204e 6f74  S cleanups.* Not
+00000bd0: 6520 4578 7465 726e 616c 204c 696e 6b20  e External Link 
+00000be0: 4865 6c70 6572 2069 7320 6e6f 7420 636f  Helper is not co
+00000bf0: 6d70 6174 6962 6c65 2077 6974 6820 7072  mpatible with pr
+00000c00: 6f6a 6563 7420 6f6e 6c79 206d 6173 7465  oject only maste
+00000c10: 7220 6272 6163 680a 2a20 5265 6d6f 7665  r brach.* Remove
+00000c20: 2061 2068 6561 7020 6f66 2064 6561 6420   a heap of dead 
+00000c30: 4353 5320 7275 6c65 730a 2a20 5265 6d6f  CSS rules.* Remo
+00000c40: 7665 6420 2763 6f6d 6269 6e65 642e 6373  ved 'combined.cs
+00000c50: 7327 2066 6f72 2027 7374 6172 6c69 6e67  s' for 'starling
+00000c60: 7864 6f63 7327 2074 6865 6d65 0a2a 2063  xdocs' theme.* c
+00000c70: 7373 3a20 4164 6420 7379 6d6c 696e 6b73  ss: Add symlinks
+00000c80: 2066 6f72 206f 7065 6e73 7461 636b 206c   for openstack l
+00000c90: 6f67 6f73 0a2a 2063 7373 3a20 4d6f 7665  ogos.* css: Move
+00000ca0: 2062 6f6f 7473 7472 6170 206d 6f64 6966   bootstrap modif
+00000cb0: 6963 6174 696f 6e73 2074 6f20 2763 6f6d  ications to 'com
+00000cc0: 6269 6e65 642e 6373 7327 2028 5374 6172  bined.css' (Star
+00000cd0: 6c69 6e67 5829 0a2a 2063 7373 3a20 5573  lingX).* css: Us
+00000ce0: 6520 656c 6c69 7073 6973 2066 6f72 206c  e ellipsis for l
+00000cf0: 6f6e 6720 7469 746c 6573 2069 6e20 7369  ong titles in si
+00000d00: 6465 6261 7220 2853 7461 726c 696e 6758  debar (StarlingX
+00000d10: 290a 2a20 6373 733a 2055 7365 2068 7474  ).* css: Use htt
+00000d20: 7073 206c 696e 6b73 2028 5374 6172 6c69  ps links (Starli
+00000d30: 6e67 5829 0a2a 2063 7373 3a20 446f 6e27  ngX).* css: Don'
+00000d40: 7420 7573 6520 626f 6c64 2074 6578 7420  t use bold text 
+00000d50: 696e 2074 6974 6c65 7320 2853 7461 726c  in titles (Starl
+00000d60: 696e 6758 290a 0a31 2e33 302e 300a 2d2d  ingX)..1.30.0.--
+00000d70: 2d2d 2d2d 0a0a 2a20 4164 6420 7461 626c  ----..* Add tabl
+00000d80: 6520 7374 796c 696e 670a 2a20 416c 6c6f  e styling.* Allo
+00000d90: 7720 746f 206f 7665 7272 6964 6520 6275  w to override bu
+00000da0: 696c 6420 6461 7465 2077 6974 6820 534f  ild date with SO
+00000db0: 5552 4345 5c5f 4441 5445 5c5f 4550 4f43  URCE\_DATE\_EPOC
+00000dc0: 480a 2a20 5265 6665 7265 6e63 6520 4f70  H.* Reference Op
+00000dd0: 656e 5374 6163 6b20 6c6f 676f 2069 6e20  enStack logo in 
+00000de0: 6f70 656e 7374 6163 6b64 6f63 7374 6865  openstackdocsthe
+00000df0: 6d65 0a0a 312e 3239 2e33 0a2d 2d2d 2d2d  me..1.29.3.-----
+00000e00: 2d0a 0a2a 2055 7064 6174 6520 666f 7220  -..* Update for 
+00000e10: 4f70 656e 4465 7620 6368 616e 6765 0a2a  OpenDev change.*
+00000e20: 2050 7265 7665 6e74 2049 6e76 6f63 6174   Prevent Invocat
+00000e30: 696f 6e45 7272 6f72 206f 6e20 6e6f 6e2d  ionError on non-
+00000e40: 6578 6973 7465 6e74 2066 696c 6573 0a2a  existent files.*
+00000e50: 204f 7065 6e44 6576 204d 6967 7261 7469   OpenDev Migrati
+00000e60: 6f6e 2050 6174 6368 0a2a 2041 6464 206d  on Patch.* Add m
+00000e70: 6973 7369 6e67 2066 6f6e 7473 2066 6f72  issing fonts for
+00000e80: 2070 6466 2062 7569 6c64 2069 6e20 5370   pdf build in Sp
+00000e90: 6869 6e78 2032 2e30 0a0a 312e 3239 2e32  hinx 2.0..1.29.2
+00000ea0: 0a2d 2d2d 2d2d 2d0a 0a2a 204d 6f76 6520  .------..* Move 
+00000eb0: 626f 6f74 7374 7261 7020 6d6f 6469 6669  bootstrap modifi
+00000ec0: 6361 7469 6f6e 7320 746f 2027 636f 6d62  cations to 'comb
+00000ed0: 696e 6564 2e63 7373 270a 2a20 6373 733a  ined.css'.* css:
+00000ee0: 2044 6f6e 2774 2075 7365 2062 6f6c 6420   Don't use bold 
+00000ef0: 7465 7874 2069 6e20 7469 746c 6573 0a2a  text in titles.*
+00000f00: 2063 7373 3a20 5573 6520 656c 6c69 7073   css: Use ellips
+00000f10: 6973 2066 6f72 206c 6f6e 6720 7469 746c  is for long titl
+00000f20: 6573 2069 6e20 7369 6465 6261 720a 2a20  es in sidebar.* 
+00000f30: 5369 6c65 6e63 6521 2041 2073 6571 7565  Silence! A seque
+00000f40: 6c0a 2a20 5369 6c65 6e63 6521 0a0a 312e  l.* Silence!..1.
+00000f50: 3239 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 2046  29.1.------..* F
+00000f60: 6978 2077 726f 6e67 2076 6172 6961 626c  ix wrong variabl
+00000f70: 6520 696e 2062 7569 6c64 2d74 7261 6e73  e in build-trans
+00000f80: 6c61 7465 640a 2a20 4578 6974 2074 7261  lated.* Exit tra
+00000f90: 7020 636c 6561 6e75 7020 696e 2064 6f63  p cleanup in doc
+00000fa0: 7374 6865 6d65 2d62 7569 6c64 2d74 7261  stheme-build-tra
+00000fb0: 6e73 6c61 7465 642e 7368 0a0a 312e 3239  nslated.sh..1.29
+00000fc0: 2e30 0a2d 2d2d 2d2d 2d0a 0a0a 312e 3238  .0.------...1.28
+00000fd0: 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 2043 6174  .1.------..* Cat
+00000fe0: 6368 204f 5345 7272 6f72 2077 6865 6e20  ch OSError when 
+00000ff0: 7472 7969 6e67 2074 6f20 6765 7420 7468  trying to get th
+00001000: 6520 6c61 7374 5c5f 7570 6461 7465 2066  e last\_update f
+00001010: 726f 6d20 6769 740a 2a20 4164 6420 6f70  rom git.* Add op
+00001020: 7469 6f6e 7320 666f 7220 7370 6869 6e78  tions for sphinx
+00001030: 2d62 7569 6c64 202d 5720 696e 2064 6f63  -build -W in doc
+00001040: 7374 6865 6d65 2d62 7569 6c64 2d74 7261  stheme-build-tra
+00001050: 6e73 6c61 7465 642e 7368 0a2a 2054 7261  nslated.sh.* Tra
+00001060: 6e73 6c61 7469 6f6e 733a 2048 616e 646c  nslations: Handl
+00001070: 6520 6469 7265 6374 6f72 6965 730a 2a20  e directories.* 
+00001080: 5570 6461 7465 2068 6163 6b69 6e67 2076  Update hacking v
+00001090: 6572 7369 6f6e 0a0a 312e 3238 2e30 0a2d  ersion..1.28.0.-
+000010a0: 2d2d 2d2d 2d0a 0a2a 2043 6861 6e67 6520  -----..* Change 
+000010b0: 6f70 656e 7374 6163 6b2d 6465 7620 746f  openstack-dev to
+000010c0: 206f 7065 6e73 7461 636b 2d64 6973 6375   openstack-discu
+000010d0: 7373 0a2a 2075 7365 2067 6974 206d 6f64  ss.* use git mod
+000010e0: 6966 6963 6174 696f 6e20 7469 6d65 7374  ification timest
+000010f0: 616d 7073 2061 7320 6c61 7374 2d75 7064  amps as last-upd
+00001100: 6174 6564 2074 696d 6520 666f 7220 6561  ated time for ea
+00001110: 6368 2070 6167 650a 2a20 496d 706f 7274  ch page.* Import
+00001120: 2074 6f6f 6c73 2066 6f72 2062 7569 6c64   tools for build
+00001130: 696e 6720 7472 616e 736c 6174 6564 2064  ing translated d
+00001140: 6f63 756d 656e 7473 0a2a 2046 6978 2074  ocuments.* Fix t
+00001150: 7970 6f0a 2a20 5265 6d6f 7665 2073 6574  ypo.* Remove set
+00001160: 7570 2e70 7920 6368 6563 6b20 6672 6f6d  up.py check from
+00001170: 2070 6570 3820 6a6f 620a 2a20 5374 6172   pep8 job.* Star
+00001180: 6c69 6e67 5820 6e61 7620 6669 7820 746f  lingX nav fix to
+00001190: 2072 656d 6f76 6520 2253 6f66 7477 6172   remove "Softwar
+000011a0: 6520 5570 6461 7465 2220 6c69 6e6b 730a  e Update" links.
+000011b0: 0a31 2e32 372e 310a 2d2d 2d2d 2d2d 0a0a  .1.27.1.------..
+000011c0: 2a20 5468 6520 7468 656d 6520 6973 206f  * The theme is o
+000011d0: 7065 6e73 7461 636b 646f 6373 0a0a 312e  penstackdocs..1.
+000011e0: 3237 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2052  27.0.------..* R
+000011f0: 6561 6464 2067 6574 5c5f 6f70 656e 7374  eadd get\_openst
+00001200: 6163 6b5c 5f6c 6f67 6f5c 5f70 6174 680a  ack\_logo\_path.
+00001210: 2a20 5365 7420 6465 6661 756c 7420 7061  * Set default pa
+00001220: 7468 7320 666f 7220 4f70 656e 5374 6163  ths for OpenStac
+00001230: 6b0a 0a31 2e32 362e 300a 2d2d 2d2d 2d2d  k..1.26.0.------
+00001240: 0a0a 2a20 4d61 6b65 2061 2062 6172 652d  ..* Make a bare-
+00001250: 626f 6e65 7320 7374 6172 6c69 6e67 7864  bones starlingxd
+00001260: 6f63 7320 7468 656d 650a 2a20 4164 6420  ocs theme.* Add 
+00001270: 7363 7269 7074 7320 746f 2074 6865 2068  scripts to the h
+00001280: 6561 6420 7365 6374 696f 6e0a 2a20 5265  ead section.* Re
+00001290: 6d6f 7665 2065 7861 6d70 6c65 206f 6620  move example of 
+000012a0: 6465 7072 6563 6174 6564 2061 7070 2e69  deprecated app.i
+000012b0: 6e66 6f0a 2a20 4164 6420 7374 6172 6c69  nfo.* Add starli
+000012c0: 6e67 7864 6f63 7320 7468 656d 6520 7375  ngxdocs theme su
+000012d0: 7070 6f72 740a 0a31 2e32 352e 310a 2d2d  pport..1.25.1.--
+000012e0: 2d2d 2d2d 0a0a 2a20 4669 7820 7265 6772  ----..* Fix regr
+000012f0: 6573 7369 6f6e 7320 696e 7472 6f64 7563  essions introduc
+00001300: 6564 2069 6e20 312e 3235 2e30 0a0a 312e  ed in 1.25.0..1.
+00001310: 3235 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2041  25.0.------..* A
+00001320: 6464 2061 6e20 6f70 7469 6f6e 2074 6f20  dd an option to 
+00001330: 6469 7361 626c 6520 676c 6f62 616c 2054  disable global T
+00001340: 4f43 2073 6563 7469 6f6e 0a2a 204d 616b  OC section.* Mak
+00001350: 6520 726f 6f74 2074 6974 6c65 2063 7573  e root title cus
+00001360: 746f 6d69 7a61 626c 650a 2a20 496d 706f  tomizable.* Impo
+00001370: 7274 2062 7569 6c64 2d6f 7065 6e73 7461  rt build-opensta
+00001380: 636b 2d61 7069 2d72 6566 0a0a 312e 3234  ck-api-ref..1.24
+00001390: 2e31 0a2d 2d2d 2d2d 2d0a 0a2a 206c 6f67  .1.------..* log
+000013a0: 2064 6574 6169 6c73 206f 6620 6874 6d6c   details of html
+000013b0: 2063 6f6e 7465 7874 0a2a 2070 6173 7320   context.* pass 
+000013c0: 7573 6553 746f 7279 626f 6172 6420 746f  useStoryboard to
+000013d0: 206c 6f67 4142 7567 0a2a 2065 6e73 7572   logABug.* ensur
+000013e0: 6520 7265 706f 7369 746f 7279 5c5f 6e61  e repository\_na
+000013f0: 6d65 2069 7320 616c 7761 7973 2073 6574  me is always set
+00001400: 0a0a 312e 3234 2e30 0a2d 2d2d 2d2d 2d0a  ..1.24.0.------.
+00001410: 0a2a 2046 6978 2074 6865 2069 6e63 6f72  .* Fix the incor
+00001420: 7265 6374 2073 746f 7279 626f 6172 6420  rect storyboard 
+00001430: 7572 6c0a 2a20 4669 7820 7072 6f6a 6563  url.* Fix projec
+00001440: 742d 6e61 7669 6761 746f 7220 6c69 6e6b  t-navigator link
+00001450: 0a0a 312e 3233 2e32 0a2d 2d2d 2d2d 2d0a  ..1.23.2.------.
+00001460: 0a2a 2046 6978 2075 7365 5c5f 7374 6f72  .* Fix use\_stor
+00001470: 7962 6f61 7264 0a0a 312e 3233 2e31 0a2d  yboard..1.23.1.-
+00001480: 2d2d 2d2d 2d0a 0a2a 2048 616e 646c 6520  -----..* Handle 
+00001490: 5374 6f72 7942 6f61 7264 2070 726f 6a65  StoryBoard proje
+000014a0: 6374 2067 726f 7570 730a 2a20 446f 206e  ct groups.* Do n
+000014b0: 6f74 2073 686f 7720 6261 6467 6520 666f  ot show badge fo
+000014c0: 7220 6d61 7374 6572 206f 6e6c 7920 7265  r master only re
+000014d0: 706f 730a 0a31 2e32 332e 300a 2d2d 2d2d  pos..1.23.0.----
+000014e0: 2d2d 0a0a 2a20 4669 7820 6275 696c 6420  --..* Fix build 
+000014f0: 6a6f 6273 0a2a 2044 6f20 6e6f 7420 6469  jobs.* Do not di
+00001500: 7370 6c61 7920 226c 6174 6573 7422 2062  splay "latest" b
+00001510: 6164 6765 2069 6620 7265 706f 2069 7320  adge if repo is 
+00001520: 6e6f 7420 7665 7273 696f 6e65 640a 2a20  not versioned.* 
+00001530: 5573 6520 7370 6869 6e78 2d62 7569 6c64  Use sphinx-build
+00001540: 2065 7665 7279 7768 6572 650a 2a20 7377   everywhere.* sw
+00001550: 6974 6368 2064 6f63 756d 656e 7461 7469  itch documentati
+00001560: 6f6e 206a 6f62 2074 6f20 6e65 7720 5054  on job to new PT
+00001570: 490a 2a20 696d 706f 7274 207a 7575 6c20  I.* import zuul 
+00001580: 6a6f 6220 7365 7474 696e 6773 2066 726f  job settings fro
+00001590: 6d20 7072 6f6a 6563 742d 636f 6e66 6967  m project-config
+000015a0: 0a0a 312e 3232 2e30 0a2d 2d2d 2d2d 2d0a  ..1.22.0.------.
+000015b0: 0a0a 312e 3231 2e32 0a2d 2d2d 2d2d 2d0a  ..1.21.2.------.
+000015c0: 0a2a 204d 616b 6520 6267 2063 6f6c 6f72  .* Make bg color
+000015d0: 2066 6f72 2068 6967 686c 6967 6874 6564   for highlighted
+000015e0: 2074 6578 7420 6c65 7373 2062 7269 6768   text less brigh
+000015f0: 740a 2a20 6967 6e6f 7265 2066 696c 6573  t.* ignore files
+00001600: 2063 7265 6174 6564 2064 7572 696e 6720   created during 
+00001610: 7061 636b 6167 696e 670a 2a20 4164 6465  packaging.* Adde
+00001620: 6420 6465 7072 6563 6174 696f 6e20 6261  d deprecation ba
+00001630: 6467 650a 0a31 2e32 312e 310a 2d2d 2d2d  dge..1.21.1.----
+00001640: 2d2d 0a0a 2a20 4d61 6b65 2065 6d70 6861  --..* Make empha
+00001650: 7369 7a65 2d6c 696e 6573 206d 6f72 6520  size-lines more 
+00001660: 6869 6768 6c69 6768 7465 640a 2a20 5570  highlighted.* Up
+00001670: 6461 7465 6420 5365 6172 6368 2077 6964  dated Search wid
+00001680: 6765 740a 2a20 6669 7820 746f 7820 7079  get.* fix tox py
+00001690: 7468 6f6e 3320 6f76 6572 7269 6465 730a  thon3 overrides.
+000016a0: 2a20 6164 6420 7468 6520 7365 7269 6573  * add the series
+000016b0: 206e 616d 6520 746f 2074 6865 2074 656d   name to the tem
+000016c0: 706c 6174 6520 636f 6e74 6578 740a 2a20  plate context.* 
+000016d0: 616c 7761 7973 206c 6f6f 6b20 666f 7220  always look for 
+000016e0: 7468 6520 2e67 6974 7265 7669 6577 2066  the .gitreview f
+000016f0: 696c 6520 696e 2072 6f6f 7420 6f66 2072  ile in root of r
+00001700: 6570 6f0a 2a20 5374 7269 7020 7461 6773  epo.* Strip tags
+00001710: 2066 726f 6d20 7469 746c 6573 2069 6e20   from titles in 
+00001720: 6275 6754 6974 6c65 2061 6e64 206d 6574  bugTitle and met
+00001730: 610a 2a20 4368 6563 6b20 5253 5420 6173  a.* Check RST as
+00001740: 2070 6172 7420 6f66 206c 696e 7469 6e67   part of linting
+00001750: 0a0a 312e 3231 2e30 0a2d 2d2d 2d2d 2d0a  ..1.21.0.------.
+00001760: 0a2a 2055 7365 206d 6574 6164 6174 6120  .* Use metadata 
+00001770: 7375 6d6d 6172 7920 696e 7374 6561 6420  summary instead 
+00001780: 6e61 6d65 2066 6f72 2064 6f63 2074 6974  name for doc tit
+00001790: 6c65 0a2a 2052 656c 6f63 6174 6520 6275  le.* Relocate bu
+000017a0: 675c 5f74 6167 2069 6e20 6c6f 6741 4275  g\_tag in logABu
+000017b0: 6720 6765 6e65 7261 7465 6420 5552 4c0a  g generated URL.
+000017c0: 0a31 2e32 302e 310a 2d2d 2d2d 2d2d 0a0a  .1.20.1.------..
+000017d0: 2a20 4861 6e64 6c65 2070 6f73 7369 626c  * Handle possibl
+000017e0: 6520 6578 6365 7074 696f 6e73 2077 6865  e exceptions whe
+000017f0: 6e20 6665 7463 6869 6e67 2076 6572 7369  n fetching versi
+00001800: 6f6e 206e 756d 6265 7273 0a0a 312e 3230  on numbers..1.20
+00001810: 2e30 0a2d 2d2d 2d2d 2d0a 0a2a 2055 7064  .0.------..* Upd
+00001820: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
+00001830: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
+00001840: 436f 6e66 6967 7572 6520 6164 6469 7469  Configure additi
+00001850: 6f6e 616c 2070 726f 7065 7274 6965 730a  onal properties.
+00001860: 2a20 436f 6e66 6967 7572 6520 7072 6f6a  * Configure proj
+00001870: 6563 7420 6e61 6d65 2c20 7665 7273 696f  ect name, versio
+00001880: 6e2c 2072 656c 6561 7365 0a2a 2074 7269  n, release.* tri
+00001890: 7669 616c 3a20 5265 6d6f 7665 2063 7275  vial: Remove cru
+000018a0: 6674 2066 726f 6d20 2763 6f6e 662e 7079  ft from 'conf.py
+000018b0: 270a 2a20 7472 6976 6961 6c3a 2055 7365  '.* trivial: Use
+000018c0: 2074 6865 2027 6765 745c 5f68 746d 6c5c   the 'get\_html\
+000018d0: 5f74 6865 6d65 5c5f 7061 7468 2720 6675  _theme\_path' fu
+000018e0: 6e63 7469 6f6e 0a2a 204d 6f76 6520 636f  nction.* Move co
+000018f0: 6465 206f 7574 206f 6620 275c 5f5c 5f69  de out of '\_\_i
+00001900: 6e69 745c 5f5c 5f27 0a2a 204d 6172 6b20  nit\_\_'.* Mark 
+00001910: 736f 6d65 2066 756e 6374 696f 6e73 2061  some functions a
+00001920: 7320 7072 6976 6174 650a 0a31 2e31 392e  s private..1.19.
+00001930: 300a 2d2d 2d2d 2d2d 0a0a 2a20 7472 6976  0.------..* triv
+00001940: 6961 6c3a 2047 656e 6572 6174 6520 277b  ial: Generate '{
+00001950: 7072 6f6a 6563 747d 2d64 6f63 2720 726f  project}-doc' ro
+00001960: 6c65 732c 206e 6f74 2027 7b70 726f 6a65  les, not '{proje
+00001970: 6374 7d2d 646f 632d 6c69 6e6b 270a 2a20  ct}-doc-link'.* 
+00001980: 4176 6f69 6420 7465 7874 206f 7665 7266  Avoid text overf
+00001990: 6c6f 7720 696e 2074 6f63 0a2a 2046 6978  low in toc.* Fix
+000019a0: 2074 7970 6f20 696e 206c 6f67 6765 722e   typo in logger.
+000019b0: 7761 726e 696e 6728 2920 6361 6c6c 0a2a  warning() call.*
+000019c0: 2061 7574 6f6d 6174 6963 616c 6c79 2063   automatically c
+000019d0: 7265 6174 6520 7072 6f6a 6563 7420 646f  reate project do
+000019e0: 632d 6c69 6e6b 2072 6f6c 6573 0a2a 2052  c-link roles.* R
+000019f0: 656d 6f76 6520 6e61 6d65 2066 726f 6d20  emove name from 
+00001a00: 7072 6f6a 6563 7420 7374 616e 7a61 0a2a  project stanza.*
+00001a10: 2055 7064 6174 6564 2066 726f 6d20 676c   Updated from gl
+00001a20: 6f62 616c 2072 6571 7569 7265 6d65 6e74  obal requirement
+00001a30: 730a 2a20 5570 6461 7465 2074 6865 2064  s.* Update the d
+00001a40: 6573 6372 6970 7469 6f6e 206f 6620 2267  escription of "g
+00001a50: 6974 7572 6c22 0a0a 312e 3138 2e31 0a2d  iturl"..1.18.1.-
+00001a60: 2d2d 2d2d 2d0a 0a2a 2046 6978 2067 6974  -----..* Fix git
+00001a70: 7572 6c20 7061 7273 696e 670a 0a31 2e31  url parsing..1.1
+00001a80: 382e 300a 2d2d 2d2d 2d2d 0a0a 2a20 5265  8.0.------..* Re
+00001a90: 706c 6163 6520 7468 6520 6874 7470 206c  place the http l
+00001aa0: 696e 6b73 2077 6974 6820 7468 6520 7269  inks with the ri
+00001ab0: 6768 7420 6f6e 6573 2069 6e20 646f 6373  ght ones in docs
+00001ac0: 0a2a 2041 7474 656d 7074 2074 6f20 6775  .* Attempt to gu
+00001ad0: 6573 7320 7661 6c69 6420 4769 7420 5552  ess valid Git UR
+00001ae0: 4c73 0a2a 2052 6576 6572 7420 2246 6978  Ls.* Revert "Fix
+00001af0: 2074 6865 2069 6e63 6f72 7265 6374 2067   the incorrect g
+00001b00: 6974 2073 6f75 7263 6520 7572 6c22 0a2a  it source url".*
+00001b10: 2074 7269 7669 616c 3a20 5265 6d6f 7665   trivial: Remove
+00001b20: 2075 7365 206f 6620 2741 7070 6c69 6361   use of 'Applica
+00001b30: 7469 6f6e 2e7b 7761 726e 2c69 6e66 6f7d  tion.{warn,info}
+00001b40: 270a 2a20 4669 7820 7468 6520 696e 636f  '.* Fix the inco
+00001b50: 7272 6563 7420 6769 7420 736f 7572 6365  rrect git source
+00001b60: 2075 726c 0a2a 2044 6f20 6e6f 7420 7072   url.* Do not pr
+00001b70: 696e 7420 7468 6520 7265 6c65 6173 6520  int the release 
+00001b80: 6966 2065 6d70 7479 0a2a 2041 6464 7320  if empty.* Adds 
+00001b90: 2d70 206f 7074 696f 6e20 696e 206d 6b64  -p option in mkd
+00001ba0: 6972 2066 6f72 2062 7569 6c64 7064 6620  ir for buildpdf 
+00001bb0: 746f 7820 656e 760a 2a20 6269 6e64 6570  tox env.* bindep
+00001bc0: 3a20 4164 6420 6465 7065 6e64 656e 6369  : Add dependenci
+00001bd0: 6573 2066 6f72 2050 4446 7320 6f6e 2046  es for PDFs on F
+00001be0: 6564 6f72 610a 2a20 6769 7469 676e 6f72  edora.* gitignor
+00001bf0: 653a 2049 676e 6f72 6520 6d6f 7265 2066  e: Ignore more f
+00001c00: 696c 6573 0a2a 2055 7064 6174 6564 2066  iles.* Updated f
+00001c10: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
+00001c20: 7265 6d65 6e74 730a 2a20 5265 6d6f 7665  rements.* Remove
+00001c30: 202d 5520 6672 6f6d 2070 6970 2069 6e73   -U from pip ins
+00001c40: 7461 6c6c 0a2a 2041 766f 6964 2074 6f78  tall.* Avoid tox
+00001c50: 5c5f 696e 7374 616c 6c2e 7368 2066 6f72  \_install.sh for
+00001c60: 2063 6f6e 7374 7261 696e 7473 2073 7570   constraints sup
+00001c70: 706f 7274 0a2a 2052 656d 6f76 6520 7365  port.* Remove se
+00001c80: 7474 696e 6720 6f66 2076 6572 7369 6f6e  tting of version
+00001c90: 2f72 656c 6561 7365 2066 726f 6d20 7265  /release from re
+00001ca0: 6c65 6173 656e 6f74 6573 0a2a 2041 6464  leasenotes.* Add
+00001cb0: 207a 7575 6c76 3320 6e61 7469 7665 206a   zuulv3 native j
+00001cc0: 6f62 0a2a 2041 6464 7320 5475 726b 6973  ob.* Adds Turkis
+00001cd0: 6820 6c61 6e64 696e 6720 7061 6765 2074  h landing page t
+00001ce0: 6f20 7369 6465 6261 7274 6f63 5c5f 6d65  o sidebartoc\_me
+00001cf0: 6e75 0a2a 204e 6f20 7265 6420 7769 7468  nu.* No red with
+00001d00: 2064 6f75 626c 6520 6261 636b 7469 636b   double backtick
+00001d10: 7320 6d61 726b 7570 0a0a 312e 3137 2e30  s markup..1.17.0
+00001d20: 0a2d 2d2d 2d2d 2d0a 0a2a 2055 7064 6174  .------..* Updat
+00001d30: 6564 2066 726f 6d20 676c 6f62 616c 2072  ed from global r
+00001d40: 6571 7569 7265 6d65 6e74 730a 2a20 4669  equirements.* Fi
+00001d50: 7820 6c69 6e6b 2074 6f20 6f70 656e 7374  x link to openst
+00001d60: 6163 6b64 6179 730a 2a20 5b77 7777 5d20  ackdays.* [www] 
+00001d70: 4669 7820 6c69 6e6b 2074 6f20 434f 410a  Fix link to COA.
+00001d80: 2a20 4164 6420 7375 7070 6f72 7420 666f  * Add support fo
+00001d90: 7220 7370 6869 6e78 2073 6964 6562 6172  r sphinx sidebar
+00001da0: 2072 6f6c 650a 2a20 5265 6d6f 7665 2073   role.* Remove s
+00001db0: 7472 6179 2063 6861 7261 6374 6572 7320  tray characters 
+00001dc0: 6672 6f6d 2064 656d 6f0a 2a20 5570 6461  from demo.* Upda
+00001dd0: 7465 2074 6865 2063 6f6e 6669 6775 7261  te the configura
+00001de0: 7469 6f6e 206f 6620 6765 6e65 7261 7469  tion of generati
+00001df0: 6e67 2061 2050 4446 2064 6f63 756d 656e  ng a PDF documen
+00001e00: 740a 2a20 5570 6461 7465 6420 6672 6f6d  t.* Updated from
+00001e10: 2067 6c6f 6261 6c20 7265 7175 6972 656d   global requirem
+00001e20: 656e 7473 0a2a 2053 796e 6320 6c61 6e67  ents.* Sync lang
+00001e30: 7561 6765 206c 6973 7420 7769 7468 206f  uage list with o
+00001e40: 7065 6e73 7461 636b 2d6d 616e 7561 6c73  penstack-manuals
+00001e50: 2072 6570 6f0a 2a20 4272 696e 6720 6261   repo.* Bring ba
+00001e60: 636b 206c 6f63 616c 2073 6561 7263 680a  ck local search.
+00001e70: 2a20 436c 6561 6e75 7020 7365 7475 702e  * Cleanup setup.
+00001e80: 6366 670a 2a20 5570 6461 7465 6420 6672  cfg.* Updated fr
+00001e90: 6f6d 2067 6c6f 6261 6c20 7265 7175 6972  om global requir
+00001ea0: 656d 656e 7473 0a2a 2042 7265 616b 2063  ements.* Break c
+00001eb0: 7963 6c65 2064 6570 656e 6465 6e63 7920  ycle dependency 
+00001ec0: 7769 7468 2072 656e 6f0a 2a20 5570 6461  with reno.* Upda
+00001ed0: 7465 6420 6672 6f6d 2067 6c6f 6261 6c20  ted from global 
+00001ee0: 7265 7175 6972 656d 656e 7473 0a2a 2042  requirements.* B
+00001ef0: 7265 616b 2063 7963 6c65 2064 6570 656e  reak cycle depen
+00001f00: 6465 6e63 7920 7769 7468 206f 732d 6170  dency with os-ap
+00001f10: 692d 7265 660a 2a20 5265 6d6f 7665 206e  i-ref.* Remove n
+00001f20: 6176 6967 6174 696f 6e2e 6874 6d6c 0a2a  avigation.html.*
+00001f30: 2055 7064 6174 6520 6c69 6e6b 7320 696e   Update links in
+00001f40: 2052 4541 444d 450a 2a20 5570 6461 7465   README.* Update
+00001f50: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
+00001f60: 7175 6972 656d 656e 7473 0a2a 2044 6f63  quirements.* Doc
+00001f70: 756d 656e 7473 2068 6f77 2074 6f20 7365  uments how to se
+00001f80: 7420 636f 6e66 2e70 7920 666f 7220 5044  t conf.py for PD
+00001f90: 4620 6765 6e65 7261 7469 6f6e 0a2a 2073  F generation.* s
+00001fa0: 686f 7720 7265 6c65 6173 6520 7365 7269  how release seri
+00001fb0: 6573 206e 616d 6573 206e 6f74 2076 6572  es names not ver
+00001fc0: 7369 6f6e 2074 6167 730a 2a20 4c69 6e6b  sion tags.* Link
+00001fd0: 2074 6f20 6c61 7465 7374 2076 6572 7369   to latest versi
+00001fe0: 6f6e 0a0a 312e 3136 2e31 0a2d 2d2d 2d2d  on..1.16.1.-----
+00001ff0: 2d0a 0a2a 2066 6978 2061 6c69 676e 6d65  -..* fix alignme
+00002000: 6e74 206f 6620 746f 6320 7472 6565 2069  nt of toc tree i
+00002010: 7465 6d73 2069 6e20 7369 6465 6261 720a  tems in sidebar.
+00002020: 0a31 2e31 362e 300a 2d2d 2d2d 2d2d 0a0a  .1.16.0.------..
+00002030: 2a20 4669 7820 6120 6c6f 6769 6320 6973  * Fix a logic is
+00002040: 7375 6520 696e 2074 6865 204a 530a 2a20  sue in the JS.* 
+00002050: 6d6f 7665 2074 6865 206c 6f63 616c 746f  move the localto
+00002060: 6320 666f 7220 7468 6520 7061 6765 2069  c for the page i
+00002070: 6e74 6f20 7468 6520 7369 6465 6261 720a  nto the sidebar.
+00002080: 2a20 5365 7276 6520 6d69 6e69 6669 6564  * Serve minified
+00002090: 2043 5353 0a0a 312e 3135 2e30 0a2d 2d2d   CSS..1.15.0.---
+000020a0: 2d2d 2d0a 0a2a 2052 656d 6f76 6520 7275  ---..* Remove ru
+000020b0: 6c65 7320 6c69 6e6b 6564 2074 6f20 6120  les linked to a 
+000020c0: 2253 7461 7475 7322 2049 440a 2a20 5570  "Status" ID.* Up
+000020d0: 6461 7465 2032 2064 6f63 756d 656e 7461  date 2 documenta
+000020e0: 7469 6f6e 2055 524c 7320 6163 636f 7264  tion URLs accord
+000020f0: 696e 6720 746f 2064 6f63 206d 6967 7261  ing to doc migra
+00002100: 7469 6f6e 0a2a 204d 6f76 6520 6672 6f6d  tion.* Move from
+00002110: 2033 7264 2070 6172 7479 2066 6f6e 7473   3rd party fonts
+00002120: 2074 6f20 6e61 7469 7665 2066 6f6e 7420   to native font 
+00002130: 7374 6163 6b0a 2a20 4669 7820 4164 6465  stack.* Fix Adde
+00002140: 6420 2f20 4368 616e 6765 6420 2f20 4465  d / Changed / De
+00002150: 7072 6563 6174 6564 206e 6f74 6963 6573  precated notices
+00002160: 0a2a 2053 7461 6e64 6172 6469 7365 2068  .* Standardise h
+00002170: 6561 6465 7220 7374 796c 696e 670a 2a20  eader styling.* 
+00002180: 4164 6420 7370 6163 6573 2069 6e20 6465  Add spaces in de
+00002190: 6d6f 2066 6f72 2064 6570 7265 6361 7469  mo for deprecati
+000021a0: 6f6e 206e 6f74 6963 6573 0a2a 2072 656d  on notices.* rem
+000021b0: 6f76 6520 736d 6f6f 7468 2073 6372 6f6c  ove smooth scrol
+000021c0: 6c69 6e67 0a0a 312e 3134 2e30 0a2d 2d2d  ling..1.14.0.---
+000021d0: 2d2d 2d0a 0a2a 2061 6464 2061 2063 6f6d  ---..* add a com
+000021e0: 6d65 6e74 2074 6f20 616c 6c20 6f75 7470  ment to all outp
+000021f0: 7574 2048 544d 4c20 7061 6765 7320 7368  ut HTML pages sh
+00002200: 6f77 696e 6720 7468 6520 696e 7075 7420  owing the input 
+00002210: 6669 6c65 0a2a 2043 5353 3a20 4164 6420  file.* CSS: Add 
+00002220: 6d61 7267 696e 2d6c 6566 7420 746f 203c  margin-left to <
+00002230: 6464 3e0a 2a20 4164 6420 7375 7070 6f72  dd>.* Add suppor
+00002240: 7420 666f 7220 7665 7273 696f 6e61 6464  t for versionadd
+00002250: 6564 2061 6e64 2064 6570 7265 6361 7465  ed and deprecate
+00002260: 640a 2a20 7368 6f77 2074 6865 2063 7572  d.* show the cur
+00002270: 7265 6e74 2070 726f 6a65 6374 206e 616d  rent project nam
+00002280: 6520 616e 6420 7665 7273 696f 6e20 696e  e and version in
+00002290: 206e 6176 6967 6174 696f 6e20 6c69 6e6b   navigation link
+000022a0: 0a2a 2044 6563 6c61 7265 2070 6172 616c  .* Declare paral
+000022b0: 6c65 6c20 7265 6164 696e 6720 7361 6665  lel reading safe
+000022c0: 0a0a 312e 3133 2e30 0a2d 2d2d 2d2d 2d0a  ..1.13.0.------.
+000022d0: 0a2a 2053 7472 6970 2074 6167 7320 6672  .* Strip tags fr
+000022e0: 6f6d 206e 6176 6967 6174 696f 6e20 7072  om navigation pr
+000022f0: 6576 2c20 6e65 7874 2074 6974 6c65 730a  ev, next titles.
+00002300: 2a20 436c 6561 6e75 7020 636f 6e66 2e70  * Cleanup conf.p
+00002310: 790a 2a20 416c 6c6f 7720 7573 696e 6720  y.* Allow using 
+00002320: 6f70 656e 7374 6163 6b64 6f63 7374 6865  openstackdocsthe
+00002330: 6d65 2077 6974 686f 7574 2067 6974 2069  me without git i
+00002340: 6e73 7461 6c6c 6564 0a2a 2046 6978 2073  nstalled.* Fix s
+00002350: 6f72 7469 6e67 206f 6620 6769 7420 7665  orting of git ve
+00002360: 7273 696f 6e73 0a2a 2041 6464 206e 6f74  rsions.* Add not
+00002370: 6520 666f 7220 7368 6f77 5c5f 6f74 6865  e for show\_othe
+00002380: 725c 5f76 6572 7369 6f6e 730a 2a20 446f  r\_versions.* Do
+00002390: 206e 6f74 2064 6973 706c 6179 2074 6974   not display tit
+000023a0: 6c65 2073 7472 696e 6720 6f66 2070 6167  le string of pag
+000023b0: 6520 6c6f 6361 6c20 544f 430a 0a31 2e31  e local TOC..1.1
+000023c0: 322e 300a 2d2d 2d2d 2d2d 0a0a 2a20 496e  2.0.------..* In
+000023d0: 6372 6561 7365 2061 646d 6f6e 6974 696f  crease admonitio
+000023e0: 6e2e 696d 706f 7274 616e 7420 636f 6e74  n.important cont
+000023f0: 7261 7374 0a2a 2041 6464 7320 646f 6373  rast.* Adds docs
+00002400: 2066 6f72 2072 656c 6561 7365 2076 6572   for release ver
+00002410: 7369 6f6e 7320 6472 6f70 646f 776e 206d  sions dropdown m
+00002420: 656e 750a 2a20 4164 6473 206c 6973 7420  enu.* Adds list 
+00002430: 6f66 2076 6572 7369 6f6e 7320 696e 2074  of versions in t
+00002440: 6865 2022 5570 6461 7465 6422 2062 6172  he "Updated" bar
+00002450: 0a2a 2055 7064 6174 6520 646f 6373 0a2a  .* Update docs.*
+00002460: 2043 6861 6e67 6520 6e61 6d65 206f 6620   Change name of 
+00002470: 6368 6563 6b62 7569 6c64 2074 6573 7465  checkbuild teste
+00002480: 6e76 2074 6f20 6275 696c 6470 6466 2066  nv to buildpdf f
+00002490: 6f72 2063 6c61 7269 7479 0a2a 2052 6571  or clarity.* Req
+000024a0: 7569 7265 2062 7567 5c5f 7072 6f6a 6563  uire bug\_projec
+000024b0: 7420 7365 7474 696e 670a 2a20 4164 6469  t setting.* Addi
+000024c0: 6e67 206f 6374 6176 6961 2061 7069 2d72  ng octavia api-r
+000024d0: 6566 0a2a 204d 696e 696d 616c 2073 7570  ef.* Minimal sup
+000024e0: 706f 7274 2066 6f72 2073 746f 7279 626f  port for storybo
+000024f0: 6172 640a 2a20 6d6f 7665 2064 6f63 756d  ard.* move docum
+00002500: 656e 7461 7469 6f6e 2066 726f 6d20 7265  entation from re
+00002510: 6164 6d65 2074 6f20 7370 6869 6e78 2074  adme to sphinx t
+00002520: 7265 650a 2a20 5570 6461 7465 6420 6672  ree.* Updated fr
+00002530: 6f6d 2067 6c6f 6261 6c20 7265 7175 6972  om global requir
+00002540: 656d 656e 7473 0a2a 2055 7064 6174 6573  ements.* Updates
+00002550: 2022 436f 6e74 656e 7473 2220 746f 2022   "Contents" to "
+00002560: 5072 6f6a 6563 7420 686f 6d65 2070 6167  Project home pag
+00002570: 6522 2074 6f20 6265 7474 6572 206d 6174  e" to better mat
+00002580: 6368 2065 7869 7374 696e 670a 2a20 576f  ch existing.* Wo
+00002590: 726b 696e 6720 6f6e 2069 6e74 6567 7261  rking on integra
+000025a0: 7469 6e67 206f 7074 696f 6e73 2066 726f  ting options fro
+000025b0: 6d20 6f73 6c6f 7370 6869 6e78 2074 6865  m oslosphinx the
+000025c0: 6d65 0a0a 312e 3131 2e30 0a2d 2d2d 2d2d  me..1.11.0.-----
+000025d0: 2d0a 0a2a 2073 7769 7463 6820 7265 6c65  -..* switch rele
+000025e0: 6173 6520 6e6f 7465 7320 6275 696c 6420  ase notes build 
+000025f0: 746f 2075 7365 206f 7065 6e73 7461 636b  to use openstack
+00002600: 646f 6373 2069 6e73 7465 6164 206f 6620  docs instead of 
+00002610: 6f73 6c6f 7370 6869 6e78 0a2a 2061 7574  oslosphinx.* aut
+00002620: 6f6d 6174 6520 736f 6d65 206f 6620 7468  omate some of th
+00002630: 6520 6578 7465 6e73 696f 6e20 7365 7475  e extension setu
+00002640: 700a 2a20 456e 6162 6c65 2073 6f6d 6520  p.* Enable some 
+00002650: 6f66 662d 6279 2d64 6566 6175 6c74 2063  off-by-default c
+00002660: 6865 636b 730a 0a31 2e31 302e 300a 2d2d  hecks..1.10.0.--
+00002670: 2d2d 2d2d 0a0a 2a20 5570 6461 7465 2053  ----..* Update S
+00002680: 6974 6520 5365 6172 6368 0a2a 2055 7064  ite Search.* Upd
+00002690: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
+000026a0: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
+000026b0: 5044 4620 6275 696c 6420 7375 7070 6f72  PDF build suppor
+000026c0: 7420 3e3d 2053 7068 696e 7820 312e 362e  t >= Sphinx 1.6.
+000026d0: 310a 2a20 5245 4144 4d45 3a20 5570 6461  1.* README: Upda
+000026e0: 7465 2063 6f6e 6669 6775 7261 7469 6f6e  te configuration
+000026f0: 206f 6620 6f70 656e 7374 6163 6b64 6f63   of openstackdoc
+00002700: 7374 6865 6d65 0a0a 312e 392e 300a 2d2d  stheme..1.9.0.--
+00002710: 2d2d 2d0a 0a2a 2055 7064 6174 6564 2066  ---..* Updated f
+00002720: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
+00002730: 7265 6d65 6e74 730a 2a20 4669 7820 6c69  rements.* Fix li
+00002740: 6e6b 7320 696e 2064 726f 702d 646f 776e  nks in drop-down
+00002750: 206d 656e 7520 756e 6465 7220 4a6f 696e   menu under Join
+00002760: 3b20 6164 6420 6874 7470 730a 0a31 2e38  ; add https..1.8
+00002770: 2e30 0a2d 2d2d 2d2d 0a0a 2a20 5573 6520  .0.-----..* Use 
+00002780: 6e65 7720 4f70 656e 5374 6163 6b20 6c6f  new OpenStack lo
+00002790: 676f 2061 6e64 2068 6561 6465 720a 2a20  go and header.* 
+000027a0: 5570 6461 7465 6420 6672 6f6d 2067 6c6f  Updated from glo
+000027b0: 6261 6c20 7265 7175 6972 656d 656e 7473  bal requirements
+000027c0: 0a0a 312e 372e 300a 2d2d 2d2d 2d0a 0a2a  ..1.7.0.-----..*
+000027d0: 2043 6c61 7269 6679 2073 6561 7263 6820   Clarify search 
+000027e0: 7469 746c 650a 2a20 4669 7820 7365 6172  title.* Fix sear
+000027f0: 6368 2e68 746d 6c20 7061 6765 2073 6372  ch.html page scr
+00002800: 6970 7420 6572 726f 7273 0a2a 2041 6464  ipt errors.* Add
+00002810: 2061 6c69 676e 6d65 6e74 2073 7479 6c69   alignment styli
+00002820: 6e67 2066 6f72 2066 6967 7572 6573 2061  ng for figures a
+00002830: 6e64 2069 6d61 6765 730a 2a20 5044 4620  nd images.* PDF 
+00002840: 7375 7070 6f72 7420 666f 7220 7361 6d70  support for samp
+00002850: 6c65 2064 6f63 756d 656e 7420 7769 7468  le document with
+00002860: 2066 6f6e 740a 2a20 4164 6420 746f 7820   font.* Add tox 
+00002870: 656e 7620 666f 7220 5044 4620 6275 696c  env for PDF buil
+00002880: 6469 6e67 0a2a 2055 7064 6174 6520 6373  ding.* Update cs
+00002890: 7320 6d61 726b 7570 7320 666f 7220 6e65  s markups for ne
+000028a0: 7765 7220 5370 6869 6e78 0a2a 2041 6464  wer Sphinx.* Add
+000028b0: 7320 4c61 5465 5820 7374 796c 6520 6669  s LaTeX style fi
+000028c0: 6c65 2066 6f72 2062 7569 6c64 696e 6720  le for building 
+000028d0: 5044 4620 646f 6375 6d65 6e74 730a 2a20  PDF documents.* 
+000028e0: 4164 6420 7761 726e 696e 672d 6973 2d65  Add warning-is-e
+000028f0: 7272 6f72 0a2a 2055 7064 6174 6564 2066  rror.* Updated f
+00002900: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
+00002910: 7265 6d65 6e74 730a 2a20 5570 6461 7465  rements.* Update
+00002920: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
+00002930: 7175 6972 656d 656e 7473 0a2a 2055 7064  quirements.* Upd
+00002940: 6174 6520 6861 636b 696e 6720 746f 2063  ate hacking to c
+00002950: 7572 7265 6e74 2076 6572 7369 6f6e 0a2a  urrent version.*
+00002960: 2041 646a 7573 7420 2764 6f63 732d 746f   Adjust 'docs-to
+00002970: 6320 6127 2064 6973 706c 6179 2076 616c  c a' display val
+00002980: 7565 0a2a 2052 656d 6f76 6520 6765 744a  ue.* Remove getJ
+00002990: 534f 4e20 6675 6e63 7469 6f6e 2061 6e64  SON function and
+000029a0: 2064 6f63 2d63 6861 7261 6374 6572 7320   doc-characters 
+000029b0: 6669 6c65 0a2a 2055 7064 6174 6520 4c61  file.* Update La
+000029c0: 756e 6368 7061 6420 696e 666f 0a2a 2055  unchpad info.* U
+000029d0: 7064 6174 6564 2066 726f 6d20 676c 6f62  pdated from glob
+000029e0: 616c 2072 6571 7569 7265 6d65 6e74 730a  al requirements.
+000029f0: 2a20 5573 6520 6874 7470 7320 696e 7374  * Use https inst
+00002a00: 6561 6420 6f66 2068 7474 7020 666f 7220  ead of http for 
+00002a10: 6769 742e 6f70 656e 7374 6163 6b2e 6f72  git.openstack.or
+00002a20: 670a 2a20 5570 6461 7465 2062 6f6f 7473  g.* Update boots
+00002a30: 7472 6170 2061 6e64 206a 7175 6572 7920  trap and jquery 
+00002a40: 6669 6c65 730a 2a20 5265 6d6f 7665 2064  files.* Remove d
+00002a50: 7570 6c69 6361 7465 2073 6561 7263 6820  uplicate search 
+00002a60: 6669 656c 6420 6672 6f6d 2074 6865 206c  field from the l
+00002a70: 6566 7420 7369 6465 6261 720a 2a20 4164  eft sidebar.* Ad
+00002a80: 6420 6e6f 7465 2069 6e20 5245 4144 4d45  d note in README
+00002a90: 2061 626f 7574 2050 7974 686f 6e20 3320   about Python 3 
+00002aa0: 6368 616e 6765 730a 2a20 4669 7820 6d69  changes.* Fix mi
+00002ab0: 7373 696e 6720 726f 6c65 5c5f 6964 0a0a  ssing role\_id..
+00002ac0: 312e 362e 310a 2d2d 2d2d 2d0a 0a2a 2049  1.6.1.-----..* I
+00002ad0: 6e63 6c75 6465 7320 6368 6563 6b6c 6973  ncludes checklis
+00002ae0: 7420 7768 656e 2066 696c 696e 6720 6120  t when filing a 
+00002af0: 6275 6720 666f 7220 6f73 6d61 6e75 616c  bug for osmanual
+00002b00: 730a 2a20 4164 6420 7472 6f76 6520 636c  s.* Add trove cl
+00002b10: 6173 7369 6669 6572 7320 666f 7220 5079  assifiers for Py
+00002b20: 7468 6f6e 0a0a 312e 362e 300a 2d2d 2d2d  thon..1.6.0.----
+00002b30: 2d0a 0a2a 2041 6464 2043 6f6e 7374 7261  -..* Add Constra
+00002b40: 696e 7473 2073 7570 706f 7274 0a2a 2053  ints support.* S
+00002b50: 686f 7720 7465 616d 2061 6e64 2072 6570  how team and rep
+00002b60: 6f20 6261 6467 6573 206f 6e20 5245 4144  o badges on READ
+00002b70: 4d45 0a2a 2052 656d 6f76 6564 206d 696e  ME.* Removed min
+00002b80: 696d 697a 6564 2066 696c 6573 0a2a 2041  imized files.* A
+00002b90: 6c6c 6f77 2074 6f20 6275 696c 6420 646f  llow to build do
+00002ba0: 6373 2077 6974 686f 7574 2067 6974 2063  cs without git c
+00002bb0: 6f6d 6d61 6e64 0a2a 205b 7777 775d 2075  ommand.* [www] u
+00002bc0: 7064 6174 6520 7061 6765 2068 6561 6465  pdate page heade
+00002bd0: 7220 6c69 6e6b 730a 2a20 5570 6461 7465  r links.* Update
+00002be0: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
+00002bf0: 7175 6972 656d 656e 7473 0a2a 2055 7064  quirements.* Upd
+00002c00: 6174 6564 2066 726f 6d20 676c 6f62 616c  ated from global
+00002c10: 2072 6571 7569 7265 6d65 6e74 730a 2a20   requirements.* 
+00002c20: 456e 6162 6c65 2072 656c 6561 7365 206e  Enable release n
+00002c30: 6f74 6573 2074 7261 6e73 6c61 7469 6f6e  otes translation
+00002c40: 0a2a 2055 7064 6174 6520 7465 7374 2041  .* Update test A
+00002c50: 5049 2052 6566 0a2a 2046 6978 2074 7970  PI Ref.* Fix typ
+00002c60: 6f3a 2072 656d 6f76 6520 7265 6475 6e64  o: remove redund
+00002c70: 616e 7420 2774 6865 270a 2a20 5570 6461  ant 'the'.* Upda
+00002c80: 7465 6420 6672 6f6d 2067 6c6f 6261 6c20  ted from global 
+00002c90: 7265 7175 6972 656d 656e 7473 0a2a 2055  requirements.* U
+00002ca0: 7064 6174 6564 2066 726f 6d20 676c 6f62  pdated from glob
+00002cb0: 616c 2072 6571 7569 7265 6d65 6e74 730a  al requirements.
+00002cc0: 2a20 5570 6461 7465 2072 6571 7569 7265  * Update require
+00002cd0: 6d65 6e74 730a 2a20 4669 7820 746f 7820  ments.* Fix tox 
+00002ce0: 7365 7475 700a 2a20 496e 7374 616c 6c20  setup.* Install 
+00002cf0: 7265 7175 6972 6564 2070 6163 6b61 6765  required package
+00002d00: 730a 2a20 5570 6461 7465 6420 6672 6f6d  s.* Updated from
+00002d10: 2067 6c6f 6261 6c20 7265 7175 6972 656d   global requirem
+00002d20: 656e 7473 0a0a 312e 352e 300a 2d2d 2d2d  ents..1.5.0.----
+00002d30: 2d0a 0a2a 2041 5049 2052 6566 6572 656e  -..* API Referen
+00002d40: 6365 7320 6472 6f70 646f 776e 206d 656e  ces dropdown men
+00002d50: 750a 2a20 416c 6c6f 7720 6175 746f 6d61  u.* Allow automa
+00002d60: 7469 6320 746f 6320 746f 2062 6520 6469  tic toc to be di
+00002d70: 7361 626c 6564 0a0a 312e 342e 300a 2d2d  sabled..1.4.0.--
+00002d80: 2d2d 2d0a 0a2a 2055 7064 6174 6520 5265  ---..* Update Re
+00002d90: 6c65 6173 6520 4e6f 7465 730a 2a20 4164  lease Notes.* Ad
+00002da0: 6473 2072 656c 6561 7365 206e 6f74 6573  ds release notes
+00002db0: 2069 7465 6d73 2066 6f72 206e 6578 7420   items for next 
+00002dc0: 7265 6c65 6173 650a 2a20 4d61 6b65 205c  release.* Make \
+00002dd0: 605c 6073 6f6d 6574 6869 6e67 5c60 5c60  `\`something\`\`
+00002de0: 206d 6f72 6520 6869 6768 6c69 6768 7465   more highlighte
+00002df0: 640a 2a20 416c 6c6f 7720 7468 6520 6275  d.* Allow the bu
+00002e00: 6720 7469 746c 6520 746f 2062 6520 6375  g title to be cu
+00002e10: 7374 6f6d 6973 6162 6c65 0a2a 2042 726f  stomisable.* Bro
+00002e20: 6b65 6e20 4c69 6e6b 0a2a 2055 7064 6174  ken Link.* Updat
+00002e30: 6564 2066 726f 6d20 676c 6f62 616c 2072  ed from global r
+00002e40: 6571 7569 7265 6d65 6e74 730a 2a20 496e  equirements.* In
+00002e50: 6372 6561 7365 2069 6e64 656e 7420 6c65  crease indent le
+00002e60: 7665 6c20 6f66 2064 6f63 2074 6f70 2063  vel of doc top c
+00002e70: 6f6e 7465 6e74 730a 2a20 5570 6461 7465  ontents.* Update
+00002e80: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
+00002e90: 7175 6972 656d 656e 7473 0a2a 2041 6374  quirements.* Act
+00002ea0: 7561 6c6c 7920 696e 636c 7564 6520 6375  ually include cu
+00002eb0: 7374 6f6d 204a 5320 6669 6c65 730a 2a20  stom JS files.* 
+00002ec0: 5265 6c65 6173 6520 6e6f 7465 2066 6f72  Release note for
+00002ed0: 206e 6577 2073 6964 6562 6172 2066 6561   new sidebar fea
+00002ee0: 7475 7265 0a2a 2055 7365 2048 5454 5053  ture.* Use HTTPS
+00002ef0: 2066 6f72 2065 7874 6572 6e61 6c20 6465   for external de
+00002f00: 7073 0a2a 2053 6574 2073 6964 6520 6261  ps.* Set side ba
+00002f10: 7220 636f 6e74 656e 7420 746f 2062 6520  r content to be 
+00002f20: 636f 6e66 6967 7572 6162 6c65 0a2a 2043  configurable.* C
+00002f30: 7265 6174 6520 656d 7074 7920 666f 6c64  reate empty fold
+00002f40: 6572 2066 6f72 2063 7573 746f 6d20 666f  er for custom fo
+00002f50: 6e74 2066 696c 6573 0a2a 2046 6978 2074  nt files.* Fix t
+00002f60: 6578 7420 666f 6e74 2d66 616d 696c 7920  ext font-family 
+00002f70: 6f66 2061 646d 6f6e 6974 696f 6e73 0a2a  of admonitions.*
+00002f80: 2041 6c6c 6f77 2066 6f72 2069 6e63 6c75   Allow for inclu
+00002f90: 7369 6f6e 206f 6620 6375 7374 6f6d 204a  sion of custom J
+00002fa0: 5320 6669 6c65 730a 2a20 5570 6461 7465  S files.* Update
+00002fb0: 6420 6672 6f6d 2067 6c6f 6261 6c20 7265  d from global re
+00002fc0: 7175 6972 656d 656e 7473 0a2a 2043 6861  quirements.* Cha
+00002fd0: 6e67 6520 7375 6d6d 6974 2076 6964 656f  nge summit video
+00002fe0: 2055 524c 0a2a 2055 7064 6174 6564 2066   URL.* Updated f
+00002ff0: 726f 6d20 676c 6f62 616c 2072 6571 7569  rom global requi
+00003000: 7265 6d65 6e74 730a 2a20 5570 6461 7465  rements.* Update
+00003010: 2074 6865 2041 646d 696e 6973 7472 6174   the Administrat
+00003020: 6f72 2047 7569 6465 206c 696e 6b0a 2a20  or Guide link.* 
+00003030: 436c 6172 6966 7920 7573 6573 2066 6f72  Clarify uses for
+00003040: 2074 6869 7320 7468 656d 650a 2a20 416c   this theme.* Al
+00003050: 6c6f 7720 6373 7366 696c 6573 2061 6464  low cssfiles add
+00003060: 6564 2062 7920 7370 6869 6e78 2065 7874  ed by sphinx ext
+00003070: 656e 7369 6f6e 730a 0a31 2e33 2e30 0a2d  ensions..1.3.0.-
+00003080: 2d2d 2d2d 0a0a 2a20 4d61 6b65 2074 6865  ----..* Make the
+00003090: 6d65 2076 6572 7369 6f6e 2069 6e64 6570  me version indep
+000030a0: 656e 6465 6e74 0a2a 2041 6464 2061 7070  endent.* Add app
+000030b0: 726f 7072 6961 7465 206f 7264 6572 206c  ropriate order l
+000030c0: 6973 7420 7374 796c 6573 0a2a 2053 686f  ist styles.* Sho
+000030d0: 7274 6564 206d 6172 6769 6e20 616e 6420  rted margin and 
+000030e0: 7061 6464 696e 6720 666f 7220 746f 7020  padding for top 
+000030f0: 7061 6765 206d 656e 750a 2a20 5573 6520  page menu.* Use 
+00003100: 7065 7038 2069 6e73 7465 6164 206f 6620  pep8 instead of 
+00003110: 6c69 6e74 6572 730a 2a20 4669 7820 6120  linters.* Fix a 
+00003120: 7370 656c 6c20 7479 706f 730a 2a20 5265  spell typos.* Re
+00003130: 6e61 6d65 2070 6570 3820 746f 206c 696e  name pep8 to lin
+00003140: 7465 7273 2074 6573 740a 0a31 2e32 2e37  ters test..1.2.7
+00003150: 0a2d 2d2d 2d2d 0a0a 2a20 5570 6461 7465  .-----..* Update
+00003160: 2074 6865 2063 6f6e 7472 6962 7574 6520   the contribute 
+00003170: 6c69 6e6b 2061 7420 7468 6520 666f 6f74  link at the foot
+00003180: 6572 0a2a 2055 7064 6174 6520 6c69 6e6b  er.* Update link
+00003190: 7320 696e 2074 6865 204f 7065 6e53 7461  s in the OpenSta
+000031a0: 636b 2063 6f6c 756d 6e20 696e 2074 6865  ck column in the
+000031b0: 2066 6f6f 7465 720a 2a20 5265 6d6f 7665   footer.* Remove
+000031c0: 2066 6565 6462 6163 6b20 666f 726d 756c   feedback formul
+000031d0: 6172 2066 726f 6d20 7468 6520 666f 6f74  ar from the foot
+000031e0: 6572 0a2a 2048 6964 6520 6475 706c 6963  er.* Hide duplic
+000031f0: 6174 6520 7469 746c 6573 2061 6e64 2065  ate titles and e
+00003200: 6d70 7479 2074 6f63 7320 696e 2067 656e  mpty tocs in gen
+00003210: 6572 6174 6564 2063 6f6e 7465 6e74 0a2a  erated content.*
+00003220: 2055 7064 6174 6564 2066 726f 6d20 676c   Updated from gl
+00003230: 6f62 616c 2072 6571 7569 7265 6d65 6e74  obal requirement
+00003240: 730a 2a20 5379 6e63 2068 6561 6465 7220  s.* Sync header 
+00003250: 7769 7468 2077 7777 2e6f 7065 6e73 7461  with www.opensta
+00003260: 636b 2e6f 7267 0a2a 2052 6570 6c61 6365  ck.org.* Replace
+00003270: 2064 6570 7265 6361 7465 6420 6c69 6272   deprecated libr
+00003280: 6172 7920 6675 6e63 7469 6f6e 206f 732e  ary function os.
+00003290: 706f 7065 6e28 2920 7769 7468 2073 7562  popen() with sub
+000032a0: 7072 6f63 6573 730a 2a20 4472 6f70 2070  process.* Drop p
+000032b0: 7974 686f 6e20 636c 6173 7369 6669 6572  ython classifier
+000032c0: 7320 6672 6f6d 2073 6574 7570 2e63 6667  s from setup.cfg
+000032d0: 2066 696c 650a 2a20 5570 6461 7465 6420   file.* Updated 
+000032e0: 6672 6f6d 2067 6c6f 6261 6c20 7265 7175  from global requ
+000032f0: 6972 656d 656e 7473 0a2a 2046 6978 2073  irements.* Fix s
+00003300: 6964 6562 6172 2066 6f72 2064 6576 656c  idebar for devel
+00003310: 6f70 6572 2e6f 7065 6e73 7461 636b 2e6f  oper.openstack.o
+00003320: 7267 0a2a 2044 6570 7265 6361 7465 6420  rg.* Deprecated 
+00003330: 746f 7820 2d64 6f77 6e6c 6f61 6463 6163  tox -downloadcac
+00003340: 6865 206f 7074 696f 6e20 7265 6d6f 7665  he option remove
+00003350: 640a 2a20 4472 6f70 2070 7932 3620 6672  d.* Drop py26 fr
+00003360: 6f6d 2073 6574 7570 2e63 6667 0a0a 312e  om setup.cfg..1.
+00003370: 322e 360a 2d2d 2d2d 2d0a 0a2a 204d 616b  2.6.-----..* Mak
+00003380: 6520 476f 6f67 6c65 2041 6e61 6c79 7469  e Google Analyti
+00003390: 6373 2074 7261 636b 696e 6720 6f70 7469  cs tracking opti
+000033a0: 6f6e 616c 0a2a 2041 6464 2062 7567 2072  onal.* Add bug r
+000033b0: 6570 6f72 7420 7072 6f6a 6563 7420 6465  eport project de
+000033c0: 6669 6e69 7469 6f6e 2066 6561 7475 7265  finition feature
+000033d0: 0a2a 2046 6978 2074 6865 2075 726c 206f  .* Fix the url o
+000033e0: 6620 2248 6f77 2074 6f20 636f 6e74 7269  f "How to contri
+000033f0: 6275 7465 220a 0a31 2e32 2e35 0a2d 2d2d  bute"..1.2.5.---
+00003400: 2d2d 0a0a 2a20 4164 6420 2d57 2074 6f20  --..* Add -W to 
+00003410: 7370 6869 6e78 2069 6e76 6f63 6174 696f  sphinx invocatio
+00003420: 6e20 666f 7220 7265 6c65 6173 652d 6e6f  n for release-no
+00003430: 7465 7320 6275 696c 640a 2a20 5461 626c  tes build.* Tabl
+00003440: 6520 6361 7074 696f 6e3a 2075 7365 2061  e caption: use a
+00003450: 2062 6f6c 6420 666f 6e74 0a2a 2072 656c   bold font.* rel
+00003460: 6561 7365 206e 6f74 6520 656e 7472 7920  ease note entry 
+00003470: 666f 7220 7369 6465 6261 7220 6c69 6e6b  for sidebar link
+00003480: 2074 6f20 6120 746f 7020 7061 6765 0a2a   to a top page.*
+00003490: 2041 6464 206c 696e 6b20 666f 7220 6120   Add link for a 
+000034a0: 746f 7020 7061 6765 206f 6620 646f 6375  top page of docu
+000034b0: 6d65 6e74 2074 6f20 2243 6f6e 7465 6e74  ment to "Content
+000034c0: 7322 2069 6e20 7369 6465 6261 720a 2a20  s" in sidebar.* 
+000034d0: 4164 6420 476f 6f67 6c65 2041 6e61 6c79  Add Google Analy
+000034e0: 7469 6373 204a 6176 6153 6372 6970 7420  tics JavaScript 
+000034f0: 7472 6163 6b69 6e67 2073 6e69 7070 6574  tracking snippet
+00003500: 2063 6f64 650a 2a20 4164 6420 7265 6e6f   code.* Add reno
+00003510: 2066 6f72 2072 656c 6561 7365 2d6e 6f74   for release-not
+00003520: 6573 0a2a 2041 6464 2070 6164 6469 6e67  es.* Add padding
+00003530: 2063 7373 2070 726f 7065 7274 7920 666f   css property fo
+00003540: 7220 7464 2061 6e64 2074 680a 2a20 5265  r td and th.* Re
+00003550: 6d6f 7665 2074 6865 206f 7269 6769 6e61  move the origina
+00003560: 6c2d 6465 7369 676e 2064 6972 6563 746f  l-design directo
+00003570: 7279 0a0a 312e 322e 340a 2d2d 2d2d 2d0a  ry..1.2.4.-----.
+00003580: 0a2a 2055 7064 6174 6520 5245 4c45 4153  .* Update RELEAS
+00003590: 454e 4f54 4553 2066 6f72 2031 2e32 2e34  ENOTES for 1.2.4
+000035a0: 2072 656c 6561 7365 0a2a 2046 6978 2074   release.* Fix t
+000035b0: 6865 2062 726f 6b65 6e20 616e 6368 6f72  he broken anchor
+000035c0: 2074 6167 730a 2a20 5265 6d6f 7665 2075   tags.* Remove u
+000035d0: 6e75 7365 6420 6669 6c65 730a 2a20 4164  nused files.* Ad
+000035e0: 6420 7461 626c 6520 7061 6464 696e 6720  d table padding 
+000035f0: 746f 206f 7065 6e73 7461 636b 646f 6373  to openstackdocs
+00003600: 7468 656d 6520 4353 530a 2a20 5570 6461  theme CSS.* Upda
+00003610: 7465 2072 656c 6561 7365 7320 696e 2074  te releases in t
+00003620: 6865 206c 6566 7420 7369 6465 6261 720a  he left sidebar.
+00003630: 0a31 2e32 2e33 0a2d 2d2d 2d2d 0a0a 2a20  .1.2.3.-----..* 
+00003640: 5570 6461 7465 206c 6f67 2d61 2d62 7567  Update log-a-bug
+00003650: 2063 6f6d 6d65 6e74 730a 2a20 4578 7465   comments.* Exte
+00003660: 6e64 2072 656c 6561 7365 206e 6f74 6573  nd release notes
+00003670: 2066 6f72 2031 2e32 2e33 0a2a 2044 6563   for 1.2.3.* Dec
+00003680: 7265 6173 6520 7468 6520 696e 6465 6e74  rease the indent
+00003690: 206f 6620 544f 4320 656e 7472 6965 7320   of TOC entries 
+000036a0: 6f6e 2074 6865 2032 6e64 206c 6576 656c  on the 2nd level
+000036b0: 0a2a 2053 6574 2074 6865 2077 6964 7468  .* Set the width
+000036c0: 206f 6620 7468 6520 6869 6768 6c69 6768   of the highligh
+000036d0: 7420 7461 626c 6520 746f 2031 3030 250a  t table to 100%.
+000036e0: 2a20 4164 6420 7061 6464 696e 6720 746f  * Add padding to
+000036f0: 2074 6865 206c 6566 7420 7461 626c 6520   the left table 
+00003700: 6f66 2063 6f6e 7465 6e74 730a 2a20 5265  of contents.* Re
+00003710: 6d6f 7665 2065 7865 6375 7461 626c 6520  move executable 
+00003720: 666c 6167 7320 6672 6f6d 206a 732f 6373  flags from js/cs
+00003730: 7320 6669 6c65 730a 2a20 4164 6420 5245  s files.* Add RE
+00003740: 4c45 4153 454e 4f54 4553 2066 6f72 2031  LEASENOTES for 1
+00003750: 2e32 2e33 0a2a 2041 6464 2073 7570 706f  .2.3.* Add suppo
+00003760: 7274 2066 6f72 2046 6972 7374 6170 700a  rt for Firstapp.
+00003770: 0a31 2e32 2e32 0a2d 2d2d 2d2d 0a0a 2a20  .1.2.2.-----..* 
+00003780: 4164 6420 7265 6c65 6173 6520 6e6f 7465  Add release note
+00003790: 7320 666f 7220 7665 7273 696f 6e20 312e  s for version 1.
+000037a0: 322e 320a 2a20 4669 7820 7379 6e74 6178  2.2.* Fix syntax
+000037b0: 206f 6620 5245 4c45 4153 454e 4f54 4553   of RELEASENOTES
+000037c0: 0a2a 2043 6c65 616e 7570 2048 544d 4c20  .* Cleanup HTML 
+000037d0: 6669 6c65 730a 2a20 5265 6d6f 7665 206c  files.* Remove l
+000037e0: 6173 7420 7265 6c65 6173 6520 6465 7461  ast release deta
+000037f0: 696c 7320 6672 6f6d 2068 6561 6465 722f  ils from header/
+00003800: 666f 6f74 6572 0a2a 2046 6978 206c 696e  footer.* Fix lin
+00003810: 6b73 2f74 6578 7473 2069 6e20 7468 6520  ks/texts in the 
+00003820: 6c69 6365 6e73 6520 666f 6f74 6572 0a2a  license footer.*
+00003830: 204d 6f76 6520 6c69 7374 6564 2067 7569   Move listed gui
+00003840: 6465 7320 696e 2074 6865 2073 6964 6562  des in the sideb
+00003850: 6172 2069 6e74 6f20 7468 6520 6472 6f70  ar into the drop
+00003860: 646f 776e 206d 656e 750a 2a20 5265 6d6f  down menu.* Remo
+00003870: 7665 2074 6865 2027 5369 676e 2069 6e27  ve the 'Sign in'
+00003880: 206c 696e 6b20 696e 2074 6865 2074 6f70   link in the top
+00003890: 2062 6172 0a2a 2046 6978 206c 696e 6b73   bar.* Fix links
+000038a0: 2f61 6464 206d 6973 7369 6e67 206c 696e  /add missing lin
+000038b0: 6b73 2069 6e20 7468 6520 746f 7020 6261  ks in the top ba
+000038c0: 720a 2a20 4669 7820 6c69 6e6b 2074 6f20  r.* Fix link to 
+000038d0: 7468 6520 4f70 656e 5374 6163 6b20 7375  the OpenStack su
+000038e0: 6d6d 6974 2061 6e64 2072 656d 6f76 6520  mmit and remove 
+000038f0: 5061 7269 7320 7265 6c61 7465 6420 4353  Paris related CS
+00003900: 530a 2a20 4c69 6e6b 2074 6865 2041 7061  S.* Link the Apa
+00003910: 6368 6520 322e 3020 6c69 6365 6e73 6520  che 2.0 license 
+00003920: 6e6f 7465 2069 6e20 7468 6520 666f 6f74  note in the foot
+00003930: 6572 0a2a 2052 656d 6f76 6520 2773 7567  er.* Remove 'sug
+00003940: 6765 7374 2065 6469 7473 2720 6c69 6e6b  gest edits' link
+00003950: 2066 726f 6d20 6c61 796f 7574 0a2a 2052   from layout.* R
+00003960: 656d 6f76 6520 6475 706c 6963 6174 6520  emove duplicate 
+00003970: 6173 6b2e 6f70 656e 7374 6163 6b2e 6f72  ask.openstack.or
+00003980: 6720 6c69 6e6b 2066 726f 6d20 7468 6520  g link from the 
+00003990: 666f 6f74 6572 0a0a 312e 322e 310a 2d2d  footer..1.2.1.--
+000039a0: 2d2d 2d0a 0a2a 2046 6978 2022 446f 6373  ---..* Fix "Docs
+000039b0: 2048 6f6d 6522 206c 696e 6b0a 2a20 4f6e   Home" link.* On
+000039c0: 2068 6f76 6572 2064 6f6e 2774 2063 6861   hover don't cha
+000039d0: 6e67 6520 7468 6520 6261 636b 6772 6f75  nge the backgrou
+000039e0: 6e64 2063 6f6c 6f72 206f 6620 7468 6520  nd color of the 
+000039f0: 7369 6465 6261 7220 544f 430a 2a20 4669  sidebar TOC.* Fi
+00003a00: 7820 6c69 6e6b 2074 6f20 436c 6f75 6420  x link to Cloud 
+00003a10: 4164 6d69 6e20 4775 6964 650a 2a20 5265  Admin Guide.* Re
+00003a20: 6d6f 7665 206a 7175 6572 7920 7375 6264  move jquery subd
+00003a30: 6972 0a2a 204a 6176 6173 6372 6970 7420  ir.* Javascript 
+00003a40: 636c 6561 6e75 700a 2a20 5265 6d6f 7665  cleanup.* Remove
+00003a50: 2075 6e75 7365 6420 696d 6167 6573 0a2a   unused images.*
+00003a60: 2046 6978 2069 6e63 6c75 7369 6f6e 206f   Fix inclusion o
+00003a70: 6620 6d65 7461 7461 6773 0a0a 312e 322e  f metatags..1.2.
+00003a80: 300a 2d2d 2d2d 2d0a 0a2a 204e 6578 7420  0.-----..* Next 
+00003a90: 7265 6c65 6173 6520 6973 2031 2e32 2e30  release is 1.2.0
+00003aa0: 0a2a 2055 7064 6174 6520 5245 4c45 4153  .* Update RELEAS
+00003ab0: 454e 4f54 4553 2e72 7374 0a2a 2041 6464  ENOTES.rst.* Add
+00003ac0: 206e 6578 742c 2070 7265 7669 6f75 732c   next, previous,
+00003ad0: 2072 6570 6f72 7420 6120 6275 6720 6275   report a bug bu
+00003ae0: 7474 6f6e 7320 6174 2062 6f74 746f 6d0a  ttons at bottom.
+00003af0: 2a20 4669 7820 666f 7220 5253 5420 656e  * Fix for RST en
+00003b00: 756d 6572 6174 6564 206c 6973 742c 206c  umerated list, l
+00003b10: 6f77 6572 616c 7068 610a 2a20 4164 6420  oweralpha.* Add 
+00003b20: 7369 6465 6261 7220 6479 6e61 6d69 6320  sidebar dynamic 
+00003b30: 544f 4320 6f66 2063 6f6e 7465 6e74 0a2a  TOC of content.*
+00003b40: 2046 6978 6564 204b 6f72 6561 6e20 7479   Fixed Korean ty
+00003b50: 706f 206f 6e20 7369 6465 6261 7274 6f63  po on sidebartoc
+00003b60: 0a0a 312e 312e 300a 2d2d 2d2d 2d0a 0a2a  ..1.1.0.-----..*
+00003b70: 204e 6578 7420 7265 6c65 6173 6520 6973   Next release is
+00003b80: 2031 2e31 2e30 0a2a 2041 6464 7320 7265   1.1.0.* Adds re
+00003b90: 6c65 6173 6520 6e6f 7465 7320 656e 7472  lease notes entr
+00003ba0: 6965 7320 666f 7220 312e 302e 3820 616e  ies for 1.0.8 an
+00003bb0: 6420 312e 302e 390a 2a20 4164 6473 206f  d 1.0.9.* Adds o
+00003bc0: 7269 6769 6e61 6c20 6465 7369 676e 2066  riginal design f
+00003bd0: 696c 6573 2069 6e63 6c75 6469 6e67 2043  iles including C
+00003be0: 5353 2061 6e64 204a 530a 2a20 4d6f 7665  SS and JS.* Move
+00003bf0: 2f69 6d70 726f 7665 2074 6865 2070 7265  /improve the pre
+00003c00: 7669 6f75 732f 6e65 7874 206c 696e 6b73  vious/next links
+00003c10: 2069 6e20 7468 6520 6c65 6674 2073 6964   in the left sid
+00003c20: 6562 6172 0a2a 2043 6c65 616e 7570 2063  ebar.* Cleanup c
+00003c30: 7373 2f73 7479 6c65 732e 6373 730a 2a20  ss/styles.css.* 
+00003c40: 4c6f 6741 4275 673a 2050 7562 6c69 7368  LogABug: Publish
+00003c50: 2055 524c 206f 6620 6375 7272 656e 7420   URL of current 
+00003c60: 7061 6765 0a2a 2055 7365 206f 732e 6765  page.* Use os.ge
+00003c70: 7463 7764 2829 2069 6e73 7465 6164 206f  tcwd() instead o
+00003c80: 6620 7368 656c 6c69 6e67 206f 7574 2074  f shelling out t
+00003c90: 6f20 7275 6e20 7077 640a 2a20 2252 6570  o run pwd.* "Rep
+00003ca0: 6f72 7420 6120 6275 6722 206c 696e 6b20  ort a bug" link 
+00003cb0: 696e 2048 544d 4c20 6d61 6e75 616c 7320  in HTML manuals 
+00003cc0: 6175 746f 6d61 7469 6361 6c6c 7920 6669  automatically fi
+00003cd0: 6c6c 7320 696e 2062 7567 2773 2074 6167  lls in bug's tag
+00003ce0: 0a2a 2041 6464 7320 4353 5320 666f 7220  .* Adds CSS for 
+00003cf0: 676c 6f73 7361 7279 2064 6566 696e 6974  glossary definit
+00003d00: 696f 6e73 2074 6f20 6265 2069 6e64 656e  ions to be inden
+00003d10: 7465 640a 2a20 5570 6461 7465 2068 6163  ted.* Update hac
+00003d20: 6b69 6e67 2074 6f20 6669 7820 7065 7038  king to fix pep8
+00003d30: 2066 6169 6c75 7265 0a0a 312e 302e 380a   failure..1.0.8.
+00003d40: 2d2d 2d2d 2d0a 0a2a 204d 616b 6520 7468  -----..* Make th
+00003d50: 6520 6e61 7669 6761 7469 6f6e 206c 696e  e navigation lin
+00003d60: 6b73 2062 6967 6765 720a 2a20 5265 6d6f  ks bigger.* Remo
+00003d70: 7665 202f 7472 756e 6b2c 2069 7420 646f  ve /trunk, it do
+00003d80: 6573 206e 6f74 2065 7869 7374 2061 6e79  es not exist any
+00003d90: 6d6f 7265 0a2a 204b 696c 6f20 6973 2063  more.* Kilo is c
+00003da0: 7572 7265 6e74 2072 656c 6561 7365 0a2a  urrent release.*
+00003db0: 2044 6f63 756d 656e 7420 636f 6e66 2e70   Document conf.p
+00003dc0: 7920 7661 7269 6162 6c65 730a 2a20 4f70  y variables.* Op
+00003dd0: 656e 7374 6163 6b64 6f63 7374 6865 6d65  enstackdocstheme
+00003de0: 3a20 6c6f 672d 612d 6275 6720 7072 6566  : log-a-bug pref
+00003df0: 696c 6c73 2077 726f 6e67 2073 6f75 7263  ills wrong sourc
+00003e00: 6520 6669 6c65 0a2a 2049 676e 6f72 6520  e file.* Ignore 
+00003e10: 746f 7820 6469 7265 6374 6f72 790a 0a31  tox directory..1
+00003e20: 2e30 2e37 0a2d 2d2d 2d2d 0a0a 2a20 4164  .0.7.-----..* Ad
+00003e30: 6473 2072 656c 6561 7365 206e 6f74 6573  ds release notes
+00003e40: 2066 6f72 2031 2e30 2e37 0a2a 2022 6c6f   for 1.0.7.* "lo
+00003e50: 6720 6120 6275 6722 206c 696e 6b20 6164  g a bug" link ad
+00003e60: 6465 6420 746f 2053 7068 696e 782d 6261  ded to Sphinx-ba
+00003e70: 7365 6420 646f 6375 6d65 6e74 6174 696f  sed documentatio
+00003e80: 6e0a 2a20 4669 7820 7479 706f 2069 6e20  n.* Fix typo in 
+00003e90: 696e 6920 626c 6f63 6b20 7365 6374 696f  ini block sectio
+00003ea0: 6e0a 0a31 2e30 2e36 0a2d 2d2d 2d2d 0a0a  n..1.0.6.-----..
+00003eb0: 2a20 4164 6473 2072 656c 6561 7365 206e  * Adds release n
+00003ec0: 6f74 6573 2066 6f72 2031 2e30 2e36 0a2a  otes for 1.0.6.*
+00003ed0: 2041 6464 2074 6865 206f 7574 7075 7420   Add the output 
+00003ee0: 6672 6f6d 2070 7967 6d65 6e74 697a 650a  from pygmentize.
+00003ef0: 2a20 4164 6473 206c 696e 6b73 2069 6e20  * Adds links in 
+00003f00: 7369 6465 6261 7220 6e61 7620 7468 6174  sidebar nav that
+00003f10: 2067 6f20 746f 2064 6f63 7320 6c61 6e64   go to docs land
+00003f20: 696e 6720 7061 6765 0a0a 312e 302e 350a  ing page..1.0.5.
+00003f30: 2d2d 2d2d 2d0a 0a2a 2041 6464 7320 7265  -----..* Adds re
+00003f40: 6c65 6173 6520 6e6f 7465 7320 666f 7220  lease notes for 
+00003f50: 312e 302e 350a 2a20 4164 6473 2061 206e  1.0.5.* Adds a n
+00003f60: 6f6e 2d62 7265 616b 696e 6720 7370 6163  on-breaking spac
+00003f70: 6520 6265 666f 7265 204e 4558 5420 666f  e before NEXT fo
+00003f80: 7220 6265 7474 6572 2073 7061 6369 6e67  r better spacing
+00003f90: 2061 726f 756e 6420 7069 7065 0a2a 2041   around pipe.* A
+00003fa0: 6464 7320 476f 6f67 6c65 2043 7573 746f  dds Google Custo
+00003fb0: 6d20 5365 6172 6368 2045 6e67 696e 6520  m Search Engine 
+00003fc0: 7261 7468 6572 2074 6861 6e20 6765 6e65  rather than gene
+00003fd0: 7269 6320 666f 726d 0a2a 2055 7064 6174  ric form.* Updat
+00003fe0: 6573 2066 6f72 2063 632d 6279 206c 6963  es for cc-by lic
+00003ff0: 656e 7369 6e67 0a2a 2041 6464 7320 6e65  ensing.* Adds ne
+00004000: 7874 2061 6e64 2070 7265 7669 6f75 7320  xt and previous 
+00004010: 6c69 6e6b 730a 0a31 2e30 2e34 0a2d 2d2d  links..1.0.4.---
+00004020: 2d2d 0a0a 2a20 4164 6473 2072 656c 6561  --..* Adds relea
+00004030: 7365 206e 6f74 6573 2066 6f72 2031 2e30  se notes for 1.0
+00004040: 2e33 2061 6e64 2031 2e30 2e34 0a2a 2052  .3 and 1.0.4.* R
+00004050: 656e 6465 7269 6e67 2061 646d 6f6e 6974  endering admonit
+00004060: 696f 6e73 2077 6974 6820 466f 6e74 2041  ions with Font A
+00004070: 7765 736f 6d65 2069 636f 6e73 0a2a 2046  wesome icons.* F
+00004080: 6978 2066 6f72 2075 6e77 616e 7465 6420  ix for unwanted 
+00004090: 706c 7573 2073 6967 6e20 696e 2073 7562  plus sign in sub
+000040a0: 6c69 7374 730a 2a20 436f 6d6d 656e 7473  lists.* Comments
+000040b0: 206f 7574 206e 6f6e 2d77 6f72 6b69 6e67   out non-working
+000040c0: 2064 6f63 7320 6163 7469 6f6e 7320 666f   docs actions fo
+000040d0: 7220 6e6f 770a 0a31 2e30 2e33 0a2d 2d2d  r now..1.0.3.---
+000040e0: 2d2d 0a0a 2a20 4164 6420 696e 7374 7275  --..* Add instru
+000040f0: 6374 696f 6e73 2074 6f20 7468 6520 5245  ctions to the RE
+00004100: 4144 4d45 0a2a 2052 656d 6f76 6564 206c  ADME.* Removed l
+00004110: 6974 6572 616c 2063 6172 7269 6167 6520  iteral carriage 
+00004120: 7265 7475 726e 7320 6672 6f6d 206c 6963  returns from lic
+00004130: 656e 7365 2e74 7874 0a2a 204d 6f76 6520  ense.txt.* Move 
+00004140: 7468 6520 6c69 6365 6e73 6520 696e 666f  the license info
+00004150: 726d 6174 696f 6e20 696e 746f 2061 2073  rmation into a s
+00004160: 6570 6172 6174 6520 6669 6c65 0a2a 2041  eparate file.* A
+00004170: 6464 7320 5265 6c65 6173 6520 4e6f 7465  dds Release Note
+00004180: 730a 2a20 5570 6461 7465 7320 7361 6d70  s.* Updates samp
+00004190: 6c65 2074 6f20 696e 636c 7564 6520 6c69  le to include li
+000041a0: 6e65 6e6f 7320 666f 7220 5370 6869 6e78  nenos for Sphinx
+000041b0: 206c 696e 6520 6e75 6d62 6572 696e 670a   line numbering.
+000041c0: 2a20 6164 6420 6120 2e67 6974 7265 7669  * add a .gitrevi
+000041d0: 6577 2066 696c 650a 0a31 2e30 2e31 0a2d  ew file..1.0.1.-
+000041e0: 2d2d 2d2d 0a0a 2a20 5468 656d 6520 6e65  ----..* Theme ne
+000041f0: 6564 7320 6120 7365 7475 7020 6675 6e63  eds a setup func
+00004200: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+00004210: 6672 6f6d 2070 6163 6b61 6765 0a0a 312e  from package..1.
+00004220: 302e 320a 2d2d 2d2d 2d0a 0a2a 204d 6f64  0.2.-----..* Mod
+00004230: 6966 6965 7320 636f 6d62 696e 6564 2e63  ifies combined.c
+00004240: 7373 2074 6f20 6d61 7463 6820 636c 6173  ss to match clas
+00004250: 7365 7320 666f 7220 6164 6d6f 6e69 7469  ses for admoniti
+00004260: 6f6e 0a2a 2041 6464 7320 636f 7272 6563  on.* Adds correc
+00004270: 7420 3a72 6566 3a20 666f 7220 6372 6f73  t :ref: for cros
+00004280: 7320 6c69 6e6b 696e 670a 2a20 4164 6473  s linking.* Adds
+00004290: 2063 6f72 7265 6374 2072 7374 206d 6172   correct rst mar
+000042a0: 6b75 7020 666f 7220 696d 6167 6520 696e  kup for image in
+000042b0: 7365 7274 696f 6e0a 2a20 4164 6473 206d  sertion.* Adds m
+000042c0: 6f72 6520 7273 7420 666f 7220 7465 7374  ore rst for test
+000042d0: 696e 670a 2a20 5570 6461 7465 7320 636f  ing.* Updates co
+000042e0: 6d62 696e 6564 2e63 7373 2074 6f20 6869  mbined.css to hi
+000042f0: 6465 2070 6172 6120 7379 6d62 6f6c 2075  de para symbol u
+00004300: 6e74 696c 2075 7365 7220 686f 7665 7273  ntil user hovers
+00004310: 206f 7665 7220 6974 0a2a 204d 6f76 6573   over it.* Moves
+00004320: 2043 5353 2063 6861 6e67 6520 6672 6f6d   CSS change from
+00004330: 2062 6f6f 7473 7472 6170 2074 6f20 636f   bootstrap to co
+00004340: 6d62 696e 6564 2e63 7373 0a2a 2055 7064  mbined.css.* Upd
+00004350: 6174 6573 203c 7072 653e 2073 6f20 7468  ates <pre> so th
+00004360: 6174 2079 6f75 2063 616e 2073 6565 2077  at you can see w
+00004370: 6869 7465 2074 6578 7420 6f6e 2064 6172  hite text on dar
+00004380: 6b20 6772 6579 2062 6163 6b67 726f 756e  k grey backgroun
+00004390: 640a 2a20 4164 6473 2061 6e6f 7468 6572  d.* Adds another
+000043a0: 2073 616d 706c 6520 5253 5420 6669 6c65   sample RST file
+000043b0: 2066 6f72 2074 6573 7469 6e67 0a2a 2041   for testing.* A
+000043c0: 6464 7320 7365 6374 696f 6e20 666f 7220  dds section for 
+000043d0: 7465 7374 696e 6720 7075 7270 6f73 6573  testing purposes
+000043e0: 0a2a 2066 6978 2070 6174 6820 746f 206a  .* fix path to j
+000043f0: 7175 6572 790a 2a20 6669 7820 7273 7420  query.* fix rst 
+00004400: 7379 6e74 6178 0a2a 2055 7365 2070 6174  syntax.* Use pat
+00004410: 6874 6f28 2920 746f 2063 6f6d 7075 7465  hto() to compute
+00004420: 2072 656c 6174 6976 6520 7061 7468 7320   relative paths 
+00004430: 746f 2073 7461 7469 6320 6669 6c65 730a  to static files.
+00004440: 2a20 5265 6e61 6d65 205c 5f73 7461 7469  * Rename \_stati
+00004450: 6320 746f 2073 7461 7469 630a 2a20 436c  c to static.* Cl
+00004460: 6561 6e20 7570 2067 6574 5c5f 6874 6d6c  ean up get\_html
+00004470: 5c5f 7468 656d 655c 5f70 6174 680a 2a20  \_theme\_path.* 
+00004480: 446f 6e27 7420 666f 7263 652d 696e 6a65  Don't force-inje
+00004490: 6374 2074 6865 2074 6865 6d65 0a2a 204d  ct the theme.* M
+000044a0: 6f76 6520 7468 656d 6520 6669 6c65 7320  ove theme files 
+000044b0: 696e 746f 2063 6f72 7265 6374 2066 6f72  into correct for
+000044c0: 6d61 7469 6f6e 0a2a 2055 7064 6174 6520  mation.* Update 
+000044d0: 666c 616b 6538 2063 6f6d 6d61 6e64 730a  flake8 commands.
+000044e0: 2a20 5570 6461 7465 202e 6769 7469 676e  * Update .gitign
+000044f0: 6f72 650a 2a20 5265 6d6f 7665 7320 7265  ore.* Removes re
+00004500: 6475 6e64 616e 7420 7374 6174 6963 2066  dundant static f
+00004510: 696c 6573 2061 6e64 2074 656d 706c 6174  iles and templat
+00004520: 6520 6669 6c65 730a 2a20 5265 6d6f 7665  e files.* Remove
+00004530: 7320 756e 6565 6465 6420 6669 6c65 730a  s uneeded files.
+00004540: 2a20 4164 6473 2072 6561 7272 616e 6765  * Adds rearrange
+00004550: 6420 6669 6c65 7320 666f 7220 7265 6e61  d files for rena
+00004560: 6d65 2074 6f20 6f70 656e 7374 6163 6b64  me to openstackd
+00004570: 6f63 7374 6865 6d65 0a2a 2041 6464 7320  ocstheme.* Adds 
+00004580: 776f 726b 696e 6720 6c69 6e6b 7320 746f  working links to
+00004590: 206e 6176 6967 6174 696f 6e20 6472 6f70   navigation drop
+000045a0: 646f 776e 2061 6e64 2063 6f6c 756d 6e0a  down and column.
+000045b0: 2a20 5465 6d70 6c61 7465 7320 6e6f 7720  * Templates now 
+000045c0: 7375 7070 6f72 7420 6469 7673 2063 6f72  support divs cor
+000045d0: 7265 6374 6c79 0a2a 2041 6464 7320 7469  rectly.* Adds ti
+000045e0: 746c 6520 726f 772c 2062 7574 746f 6e20  tle row, button 
+000045f0: 726f 772c 2075 7064 6174 6564 2072 6f77  row, updated row
+00004600: 732c 2061 6e64 2073 6964 6562 6172 0a2a  s, and sidebar.*
+00004610: 2053 7461 7274 696e 6720 706f 696e 7420   Starting point 
+00004620: 666f 7220 5370 6869 6e78 2074 6865 6d65  for Sphinx theme
+00004630: 2066 6f72 2064 6f63 732e 6f70 656e 7374   for docs.openst
+00004640: 6163 6b2e 6f72 6720 636f 6e74 656e 740a  ack.org content.
```

### Comparing `openstackdocstheme-3.1.0/LICENSE` & `openstackdocstheme-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/Makefile` & `openstackdocstheme-3.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/PKG-INFO` & `openstackdocstheme-3.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstackdocstheme
-Version: 3.1.0
+Version: 3.1.1
 Summary: OpenStack Docs Theme
 Home-page: https://docs.openstack.org/openstackdocstheme/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `openstackdocstheme-3.1.0/README.rst` & `openstackdocstheme-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/api-ref/source/conf.py` & `openstackdocstheme-3.1.1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/api-ref/source/image.inc` & `openstackdocstheme-3.1.1/api-ref/source/image.inc`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/api-ref/source/parameters.yaml` & `openstackdocstheme-3.1.1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/api-ref/source/service.inc` & `openstackdocstheme-3.1.1/api-ref/source/service.inc`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/bin/docstheme-build-pdf` & `openstackdocstheme-3.1.1/bin/docstheme-build-pdf`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/bin/docstheme-build-translated.sh` & `openstackdocstheme-3.1.1/bin/docstheme-build-translated.sh`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/bin/docstheme-lang-display-name.py` & `openstackdocstheme-3.1.1/bin/docstheme-lang-display-name.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/bindep.txt` & `openstackdocstheme-3.1.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/conf.py` & `openstackdocstheme-3.1.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/configure_access_and_security_for_instances.rst` & `openstackdocstheme-3.1.1/doc/source/demo/configure_access_and_security_for_instances.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/create_and_manage_databases.rst` & `openstackdocstheme-3.1.1/doc/source/demo/create_and_manage_databases.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/create_and_manage_networks.rst` & `openstackdocstheme-3.1.1/doc/source/demo/create_and_manage_networks.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/dashboard_demo.rst` & `openstackdocstheme-3.1.1/doc/source/demo/dashboard_demo.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/figures/dashboard-project-tab.png` & `openstackdocstheme-3.1.1/doc/source/demo/figures/dashboard-project-tab.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/figures/dashboard_admin_project_tab.png` & `openstackdocstheme-3.1.1/doc/source/demo/figures/dashboard_admin_project_tab.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/figures/doc-logo-fox.jpg` & `openstackdocstheme-3.1.1/doc/source/demo/figures/doc-logo-fox.jpg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/index.rst` & `openstackdocstheme-3.1.1/doc/source/demo/index.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/launch-instance.rst` & `openstackdocstheme-3.1.1/doc/source/demo/launch-instance.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/demo/section_dashboard_access_and_security.rst` & `openstackdocstheme-3.1.1/doc/source/demo/section_dashboard_access_and_security.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/doc/source/index.rst` & `openstackdocstheme-3.1.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/index.rst` & `openstackdocstheme-3.1.1/index.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/__init__.py` & `openstackdocstheme-3.1.1/openstackdocstheme/__init__.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/ext.py` & `openstackdocstheme-3.1.1/openstackdocstheme/ext.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/page_context.py` & `openstackdocstheme-3.1.1/openstackdocstheme/page_context.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/paths.py` & `openstackdocstheme-3.1.1/openstackdocstheme/paths.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/css.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/css.html`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/footer.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <div class="container">
     <div class="row footer-links">
       <div class="col-lg-2 col-sm-2">
         <h3>OpenStack</h3>
         <ul>
           <li><a href="https://www.openstack.org/software/project-navigator/">Projects</a></li>
           <li><a href="https://security.openstack.org/">OpenStack Security</a></li>
-          <li><a href="https://openstack.org/blog/">Blog</a></li>g
+          <li><a href="https://openstack.org/blog/">Blog</a></li>
           <li><a href="https://openstack.org/news/">News</a></li>
         </ul>
       </div>
       <div class="col-lg-2 col-sm-2">
         <h3>Community</h3>
         <ul>
           <li><a href="https://www.meetup.com/pro/openinfradev/">User Groups</a></li>
@@ -26,18 +26,18 @@
           <li><a href="https://docs.openstack.org">OpenStack Manuals</a></li>
           <li><a href="https://openstack.org/software/start/">Getting Started</a></li>
           <li><a href="https://developer.openstack.org">API Documentation</a></li>
           <li><a href="https://wiki.openstack.org">Wiki</a></li>
         </ul>
       </div>
       <div class="col-lg-2 col-sm-2">
-        <h3>Branding & Legal</h3>
+        <h3>Branding &amp; Legal</h3>
         <ul>
           <li><a href="https://openinfra.dev/legal">Legal Docs</a></li>
-          <li><a href="https://openstack.org/brand/">Logos & Guidelines</a></li>
+          <li><a href="https://openstack.org/brand/">Logos &amp; Guidelines</a></li>
           <li><a href="https://openinfra.dev/legal/trademark-policy">Trademark Policy</a></li>
           <li><a href="https://openinfra.dev/privacy-policy">Privacy Policy</a></li>
           <li><a href="https://docs.openstack.org/contributors/common/setup-gerrit.html#individual-contributor-license-agreement">OpenInfra CLA</a></li>
         </ul>
       </div>
       <div class="col-lg-4 col-sm-4">
         <h3>Stay In Touch</h3>
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 **** OpenStack ****
     * Projects
     * OpenStack_Security
     * Blog
-    * g
     * News
 **** Community ****
     * User_Groups
     * Events
     * Jobs
     * Companies
     * Contribute
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/header.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/header.html`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         <span class="icon-bar"></span>
       </button>
       <div class="brand-wrapper">
         <a class="navbar-brand" href="https://www.openstack.org/"></a>
       </div>
       <div class="search-icon show"><i class="fa fa-search"></i> Search</div></div>
       <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
-      {% include 'os_search.html' %}
+{% include 'os_search.html' %}
       <ul class="nav navbar-nav navbar-main show">
-        {% include 'os_search_mobile.html' %}
+{% include 'os_search_mobile.html' %}
         <li> <!--Software -->
           <a href="{{osf_base_url}}/software/" class="drop" id="dropdownMenuSoftware">Software <i class="fa fa-caret-down"></i></a>
           <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenuSoftware">
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/software/">Overview</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/software/project-navigator/openstack-components">OpenStack Components</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/software/project-navigator/sdks">SDKs</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/software/project-navigator/deployment-tools">Deployment Tools</a></li>
@@ -37,29 +37,29 @@
         <li> <!-- Use Cases -->
           <a href="{{osf_base_url}}/use-cases/" class="drop" id="dropdownMenuUsers">Use Cases <i class="fa fa-caret-down"></i></a>
           <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenuUsers">
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/">Users in Production</a></li>
             <li role="presentation" class="divider"></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/bare-metal/">Ironic Bare Metal</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/edge-computing/">Edge Computing</a></li>
-            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/telecoms-and-nfv/">Telecom & NFV</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/telecoms-and-nfv/">Telecom &amp; NFV</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/science/">Science and HPC</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/containers/">Containers</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/use-cases/enterprise/">Enterprise</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/surveys/landing">User Survey</a></li>
           </ul>
         </li>
         <li> <!-- Events -->
           <a href="{{osf_base_url}}/events/" class="drop" id="dropdownMenuEvents">Events <i class="fa fa-caret-down"></i></a>
           <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenuEvents">
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/summit/">Open Infrastructure Summits</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/ptg/">Project Teams Gathering</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/events/opendev-2020/">OpenDev</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/events/community-events/">Community Events</a></li>
-            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/events/openstackdays">OpenStack & OpenInfra Days</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/events/openstackdays">OpenStack &amp; OpenInfra Days</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/videos/">Summit Videos</a></li>
           </ul>
         </li>
         <li><!-- Community -->
           <a href="{{osf_base_url}}/community/" class="drop" id="dropdownMenuCommunity">Community <i class="fa fa-caret-down"></i></a>
           <ul class="dropdown-menu" role="menu" aria-labelledby="dropdownMenuCommunity">
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/community/">Welcome! Start Here</a></li>
@@ -76,39 +76,37 @@
             <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev">Open Infrastructure Foundation (OpenInfra Foundation)</a></li>
           </ul>
         </li>
         <li><!-- Marketplace -->
           <a href="{{osf_base_url}}/marketplace/" class="drop" id="dropdownMenuLearn">Marketplace <i class="fa fa-caret-down"></i></a>
           <ul class="dropdown-menu dropdown-hover" role="menu" aria-labelledby="dropdownMenuEvents">
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/training/">Training</a></li>
-            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/distros/">Distros & Appliances</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/distros/">Distros &amp; Appliances</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/public-clouds/">Public Clouds</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/hosted-private-clouds/">Hosted Private Clouds</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/remotely-managed-private-clouds/">Remotely Managed Private Clouds</a></li>
-            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/consulting/">Consulting & Integrators</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/consulting/">Consulting &amp; Integrators</a></li>
             <li role="presentation"><a role="menuitem" tabindex="-1" href="{{osf_base_url}}/marketplace/drivers/">Drivers</a></li>
           </ul>
         </li>
         <li><!-- Blog -->
           <a href="{{osf_base_url}}/blog/">Blog</a>
         </li>
         <li><!-- Docs -->
           <a href="http://docs.openstack.org/">Docs</a>
         </li>
-        <li> <!-- Join -->
-            <li class="join-nav-section">
-              <a href="https://openinfra.dev/join/" id="dropdownMenuJoin">Join <i class="fa fa-caret-down"></i></a>
-              <ul class="dropdown-menu dropdown-hover" role="menu" aria-labelledby="dropdownMenuJoin" style="display: none;">
-                <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev/join/">Sign up for Foundation Membership</a></li>
-                <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev/join/">Sponsor the Foundation</a></li>
-                <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev">More about the Foundation</a></li>
-              </ul>
-            </li>
-            <li>
-              <a href="{{osf_base_url}}/Security/login/?BackURL=/home/" class="sign-in-btn">Log In</a>
-            </li>
+        <li class="join-nav-section"> <!-- Join -->
+          <a href="https://openinfra.dev/join/" id="dropdownMenuJoin">Join <i class="fa fa-caret-down"></i></a>
+          <ul class="dropdown-menu dropdown-hover" role="menu" aria-labelledby="dropdownMenuJoin" style="display: none;">
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev/join/">Sign up for Foundation Membership</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev/join/">Sponsor the Foundation</a></li>
+            <li role="presentation"><a role="menuitem" tabindex="-1" href="https://openinfra.dev">More about the Foundation</a></li>
+          </ul>
+        </li>
+        <li> <!-- Login -->
+          <a href="{{osf_base_url}}/Security/login/?BackURL=/home/" class="sign-in-btn">Log In</a>
         </li>
       </ul>
     </div>
   </div>
   <!-- /.container -->
 </nav>
```

#### html2text {}

```diff
@@ -50,13 +50,14 @@
           o Public_Clouds
           o Hosted_Private_Clouds
           o Remotely_Managed_Private_Clouds
           o Consulting_&_Integrators
           o Drivers
     * Blog
     * Docs
-    * Join
+    *
+      Join
           o Sign_up_for_Foundation_Membership
           o Sponsor_the_Foundation
           o More_about_the_Foundation
-    * Log_In
+    *  Log_In
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/layout.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/layout.html`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 {%- block relbar2 %}{% endblock %}
 
 {%- block footer %}
 {% include 'footer.html' %}
 {% include 'script_footer.html' %}
 {% block script_footer %}{% endblock %}
 {% if display_badge %}
-<script type="text/javascript">
+<script>
     $(document).ready(function(){
 
           $.ajax({
             context: this,
             dataType : "html",
             url : "https://docs.openstack.org/{{ series }}/badge.html",
             success : function(results) {
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/script_footer.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/script_footer.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 <!-- jQuery -->
-<script type="text/javascript" src="{{pathto('_static/js/jquery-3.2.1.min.js', 1)}}"></script>
+<script src="{{pathto('_static/js/jquery-3.2.1.min.js', 1)}}"></script>
 
 <!-- Bootstrap JavaScript -->
-<script type="text/javascript" src="{{pathto('_static/js/bootstrap.min.js', 1)}}"></script>
+<script src="{{pathto('_static/js/bootstrap.min.js', 1)}}"></script>
 
 <!-- The rest of the JS -->
-<script type="text/javascript" src="{{pathto('_static/js/navigation.js', 1)}}"></script>
+<script src="{{pathto('_static/js/navigation.js', 1)}}"></script>
 
 <!-- Docs JS -->
-<script type="text/javascript" src="{{pathto('_static/js/docs.js', 1)}}"></script>
+<script src="{{pathto('_static/js/docs.js', 1)}}"></script>
 
 <!-- standard sphinx include libraries, which allow search highlighting -->
-<script type="text/javascript" src="{{pathto('_static/underscore.js', 1)}}"></script>
-<script type="text/javascript" src="{{pathto('_static/doctools.js', 1)}}"></script>
-<script type="text/javascript" src="{{pathto('_static/searchtools.js', 1)}}"></script>
-<script type="text/javascript" src="{{ pathto('_static/language_data.js', 1) }}"></script>
+<script src="{{pathto('_static/underscore.js', 1)}}"></script>
+<script src="{{pathto('_static/doctools.js', 1)}}"></script>
+<script src="{{pathto('_static/searchtools.js', 1)}}"></script>
+<script src="{{ pathto('_static/language_data.js', 1) }}"></script>
 
-<script type="text/javascript">
+<script>
     var DOCUMENTATION_OPTIONS = {
       URL_ROOT:    './',
       VERSION:     '{{ version }}',
       COLLAPSE_INDEX: false,
       FILE_SUFFIX: '.html',
       LINK_SUFFIX: '.html',
       SOURCELINK_SUFFIX: '.txt',
       HAS_SOURCE:  true
     };
 </script>
 
 <!-- Javascript for page -->
-<script language="JavaScript">
+<script>
   /* Build a description of this page including SHA, source location on git
    * repo, build time and the project's launchpad bug tag. Set the HREF of the
    * bug buttons
    */
 
 {%- if bug_project %}
     var lineFeed = "%0A";
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/script_search.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/script_search.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-<script src="https://www.google.com/jsapi" type="text/javascript"></script>
-<script type="text/javascript">
+<script src="https://www.google.com/jsapi"></script>
+<script>
  //<![CDATA[
 google.load('search', '1', {
     language: 'en'
 });
 var _gaq = _gaq ||[];
 _gaq.push([ "_setAccount", "UA-17511903-1"]);
 function _trackQuery(control, searcher, query) {
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/search.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/search.html`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 {% extends "layout.html" %}
 {% set title = _('Search') %}
 {% block extrahead %}
 {{ super() }}
 {% endblock %}
 {% block body %}
   <div id="fallback" class="admonition warning">
-  <script type="text/javascript">document.getElementById('fallback').style.display = 'none';</script>
+  <script>document.getElementById('fallback').style.display = 'none';</script>
   <p>
-    {% trans %}Please activate JavaScript to enable the search
-    functionality.{% endtrans %}
+    {% trans %}Please activate JavaScript to enable the search functionality.{% endtrans %}
   </p>
   </div>
   <p>
     {% trans %}To search the documentation for {{ project }}, type your query into the
     box below and press Enter.{% endtrans %}
   </p>
     <form action="" method="get">
@@ -31,13 +30,13 @@
 
     <div id="search-results">
 
     </div>
 {% endblock %}
 
 {% block script_footer %}
-  <script type="text/javascript">
+  <script>
     jQuery(function() { Search.loadIndex("searchindex.js"); });
   </script>
 
-  <script type="text/javascript" id="searchindexloader"></script>
+  <script id="searchindexloader"></script>
 {% endblock %}
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc.html`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc_menu.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc_menu.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-<button href="#" type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">OpenStack Documentation<i class="fa fa-caret-down"></i></button>
-    <ul class="dropdown-menu docs-sidebar-dropdown" role="menu" aria-labelledby="dLabel">
-      <li role="presentation" class="dropdown-header">Guides</li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#install-guides">Install Guides</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#user-guides">User Guides</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#configuration-guides">Configuration Guides</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#ops-and-admin-guides">Operations and Administration Guides</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#api-guides">API Guides</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#contributor-guides">Contributor Guides</a></li>
-      <li role="presentation" class="dropdown-header">Languages</li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/de/">Deutsch (German)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/fr/">Français (French)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/id/">Bahasa Indonesia (Indonesian)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/it/">Italiano (Italian)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/ja/">日本語 (Japanese)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/ko_KR/">한국어 (Korean)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/pt_BR/">Português (Portuguese)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/tr_TR/">Türkçe (Türkiye)</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/zh_CN/">简体中文 (Simplified Chinese)</a></li>
-    </ul>
+<button type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">OpenStack Documentation<i class="fa fa-caret-down"></i></button>
+<ul class="dropdown-menu docs-sidebar-dropdown" role="menu">
+  <li role="presentation" class="dropdown-header">Guides</li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#install-guides">Install Guides</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#user-guides">User Guides</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#configuration-guides">Configuration Guides</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#ops-and-admin-guides">Operations and Administration Guides</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#api-guides">API Guides</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/index.html#contributor-guides">Contributor Guides</a></li>
+  <li role="presentation" class="dropdown-header">Languages</li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/de/">Deutsch (German)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/fr/">Français (French)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/id/">Bahasa Indonesia (Indonesian)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/it/">Italiano (Italian)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/ja/">日本語 (Japanese)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/ko_KR/">한국어 (Korean)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/pt_BR/">Português (Portuguese)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/tr_TR/">Türkçe (Türkiye)</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/zh_CN/">简体中文 (Simplified Chinese)</a></li>
+</ul>
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/sidebartoc_menu_apiref.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/sidebartoc_menu_apiref.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-<button href="#" type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">OpenStack APIs<i class="fa fa-caret-down"></i></button>
-    <ul class="dropdown-menu docs-sidebar-dropdown" role="menu" aria-labelledby="dLabel">
-      <li role="presentation" class="dropdown-header">References</li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/accelerator/index.html">Accelerator</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/application-catalog/index.html">Application Catalog</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/application-container/index.html">Application Container</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/backup/index.html">Backup</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/baremetal/index.html">Bare Metal</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/baremetal-introspection/index.html">Bare Metal Introspection</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/block-storage/index.html">Block Storage</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/clustering/index.html">Clustering</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/compute/index.html">Compute</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/container-infrastructure-management/index.html">Container Infrastructure Management</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/data-processing/index.html">Data Processing</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/data-protection-orchestration/index.html">Data Protection Orchestration</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/dns/index.html">DNS</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/ec2-api/index.html">EC2</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/function-engine/index.html">Function Engine</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/identity/index.html">Identity</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/image/index.html">Image</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/instance-ha/index.html">Instance HA</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/key-manager/index.html">Key Manager</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/load-balancer/index.html">Load Balancer</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/message/index.html">Message</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring/index.html">Monitoring</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring-events/index.html">Monitoring Events</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring-logging/index.html">Monitoring Logging</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/network/index.html">Network</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/nfv-orchestration/index.html">NFV Orchestration</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/object-store/index.html">Object Store</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/orchestration/index.html">Orchestration</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/placement/index.html">Placement</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/reservation/index.html">Reservation</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/resource-optimization/index.html">Resource Optimization</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/search/index.html">Search</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/shared-file-system/index.html">Shared File System</a></li>
-      <li role="presentation" class="dropdown-header">Guides</li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-quick-start/">API Quick Start</a></li>
-     <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-guide/compute/">Compute API Guide</a></li>
-    </ul>
+<button type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">OpenStack APIs<i class="fa fa-caret-down"></i></button>
+<ul class="dropdown-menu docs-sidebar-dropdown" role="menu">
+  <li role="presentation" class="dropdown-header">References</li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/accelerator/index.html">Accelerator</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/application-catalog/index.html">Application Catalog</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/application-container/index.html">Application Container</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/backup/index.html">Backup</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/baremetal/index.html">Bare Metal</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/baremetal-introspection/index.html">Bare Metal Introspection</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/block-storage/index.html">Block Storage</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/clustering/index.html">Clustering</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/compute/index.html">Compute</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/container-infrastructure-management/index.html">Container Infrastructure Management</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/data-processing/index.html">Data Processing</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/data-protection-orchestration/index.html">Data Protection Orchestration</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/dns/index.html">DNS</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/ec2-api/index.html">EC2</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/function-engine/index.html">Function Engine</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/identity/index.html">Identity</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/image/index.html">Image</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/instance-ha/index.html">Instance HA</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/key-manager/index.html">Key Manager</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/load-balancer/index.html">Load Balancer</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/message/index.html">Message</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring/index.html">Monitoring</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring-events/index.html">Monitoring Events</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/monitoring-logging/index.html">Monitoring Logging</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/network/index.html">Network</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/nfv-orchestration/index.html">NFV Orchestration</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/object-store/index.html">Object Store</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/orchestration/index.html">Orchestration</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/placement/index.html">Placement</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/reservation/index.html">Reservation</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/resource-optimization/index.html">Resource Optimization</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/search/index.html">Search</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-ref/shared-file-system/index.html">Shared File System</a></li>
+  <li role="presentation" class="dropdown-header">Guides</li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-quick-start/">API Quick Start</a></li>
+ <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.openstack.org/api-guide/compute/">Compute API Guide</a></li>
+</ul>
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.min.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/combined.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/combined.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.min.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/css/search.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/css/search.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/FontAwesome.otf` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.eot` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.ttf` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff2` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.eot` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.ttf` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff2` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/license.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/license.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser1.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser1.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser2.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser2.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser3.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser3.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser4.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/docs/superuser4.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook-hover.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook-hover.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-facebook.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin-hover.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin-hover.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-linkedin.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter-hover.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter-hover.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-twitter.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube-hover.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube-hover.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/footer-youtube.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/loading.gif` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/loading.gif`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-full.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-full.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-full.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-full.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/logo-vert.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-full.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/images/openstack-logo-vert.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.min.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/docs.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/docs.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.min.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/static/js/navigation.js` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/static/js/navigation.js`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs/titlerow.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs/titlerow.html`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs_pdf/logo-full.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs_pdf/logo-full.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/openstackdocs_pdf/pdftheme.sty` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/openstackdocs_pdf/pdftheme.sty`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/footer.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
         <ul>
           <li><a href="https://docs.starlingx.io">StarlingX Manuals</a></li>
           <li><a href="https://docs.starlingx.io/api-ref/">API Documentation</a></li>
           <li><a href="https://wiki.openstack.org/StarlingX">Wiki</a></li>
         </ul>
       </div>
       <div class="col-lg-2 col-sm-2">
-        <h3>Branding & Legal</h3>
+        <h3>Branding &amp; Legal</h3>
         <ul>
           <li><a href="https://openinfra.dev/legal">Legal Docs</a></li>
-          <li><a href="https://openstack.org/brand/">Logos & Guidelines</a></li>
+          <li><a href="https://openstack.org/brand/">Logos &amp; Guidelines</a></li>
           <li><a href="https://openinfra.dev/legal/trademark-policy">Trademark Policy</a></li>
           <li><a href="https://openinfra.dev/privacy-policy">Privacy Policy</a></li>
           <li><a href="https://docs.openstack.org/contributors/common/setup-gerrit.html#individual-contributor-license-agreement">OpenInfra CLA</a></li>
         </ul>
       </div>
       <div class="col-lg-4 col-sm-4">
         <h3>Stay In Touch</h3>
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/header.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/header.html`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu_apiref.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/sidebartoc_menu_apiref.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-<button href="#" type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">StarlingX APIs<i class="fa fa-caret-down"></i></button>
-    <ul class="dropdown-menu docs-sidebar-dropdown" role="menu" aria-labelledby="dLabel">
-      <li role="presentation" class="dropdown-header">References</li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-metal/">Bare Metal</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-config/">Configuration</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-distcloud/">Distributed Cloud</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-fault/">Fault Management</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-ha/">High Availability</a></li>
-      <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-nfv/">Network Function Virtualization</a></li>
-    </ul>
+<button type="button" data-toggle="dropdown" class="btn docs-sidebar-release-select">StarlingX APIs<i class="fa fa-caret-down"></i></button>
+<ul class="dropdown-menu docs-sidebar-dropdown" role="menu">
+  <li role="presentation" class="dropdown-header">References</li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-metal/">Bare Metal</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-config/">Configuration</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-distcloud/">Distributed Cloud</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-fault/">Fault Management</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-ha/">High Availability</a></li>
+  <li role="presentation"><a role="menuitem" tabindex="-1" href="https://docs.starlingx.io/api-ref/stx-nfv/">Network Function Virtualization</a></li>
+</ul>
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/css/combined.css` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/css/combined.css`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Horizontal_2color.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/StarlingX_Logo_RGB_Stacked_2color.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-full.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/static/images/logo-vert.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs/titlerow.html` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs/titlerow.html`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.png` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.png`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.svg` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/logo-full.svg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/theme/starlingxdocs_pdf/pdftheme.sty` & `openstackdocstheme-3.1.1/openstackdocstheme/theme/starlingxdocs_pdf/pdftheme.sty`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme/version.py` & `openstackdocstheme-3.1.1/openstackdocstheme/version.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme.egg-info/PKG-INFO` & `openstackdocstheme-3.1.1/openstackdocstheme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: openstackdocstheme
-Version: 3.1.0
+Version: 3.1.1
 Summary: OpenStack Docs Theme
 Home-page: https://docs.openstack.org/openstackdocstheme/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `openstackdocstheme-3.1.0/openstackdocstheme.egg-info/SOURCES.txt` & `openstackdocstheme-3.1.1/openstackdocstheme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/add-openstackdocs_auto_version-option-fd03f20373eede39.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/add-openstackdocs_auto_version-option-fd03f20373eede39.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/add-translations-9238b0f56b677a6b.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/add-translations-9238b0f56b677a6b.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/autoconfigure-settings-7083fdeeb121da89.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/autoconfigure-settings-7083fdeeb121da89.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/custom-bug-link-ec64bdf9ce357d16.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/custom-bug-link-ec64bdf9ce357d16.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/renamed-opts-bbf5d1390ed6ba71.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/renamed-opts-bbf5d1390ed6ba71.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/sidebar_dropdown_apiref-993b4dba4c0369f6.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/sidebar_dropdown_apiref-993b4dba4c0369f6.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/notes/version-dropdown-1aa39974f524dd75.yaml` & `openstackdocstheme-3.1.1/releasenotes/notes/version-dropdown-1aa39974f524dd75.yaml`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/source/conf.py` & `openstackdocstheme-3.1.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/releasenotes/source/historic.rst` & `openstackdocstheme-3.1.1/releasenotes/source/historic.rst`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/setup.cfg` & `openstackdocstheme-3.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/setup.py` & `openstackdocstheme-3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `openstackdocstheme-3.1.0/tox.ini` & `openstackdocstheme-3.1.1/tox.ini`

 * *Files identical despite different names*

