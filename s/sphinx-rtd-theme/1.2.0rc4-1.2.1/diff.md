# Comparing `tmp/sphinx_rtd_theme-1.2.0rc4.tar.gz` & `tmp/sphinx_rtd_theme-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_rtd_theme-1.2.0rc4.tar", last modified: Mon Feb  6 17:04:36 2023, max compression
+gzip compressed data, was "sphinx_rtd_theme-1.2.1.tar", last modified: Tue May 23 09:16:49 2023, max compression
```

## Comparing `sphinx_rtd_theme-1.2.0rc4.tar` & `sphinx_rtd_theme-1.2.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.801783 sphinx_rtd_theme-1.2.0rc4/
--rw-r--r--   0 balder    (1000) balder    (1000)    11379 2019-02-17 15:27:39.000000 sphinx_rtd_theme-1.2.0rc4/Apache-License-2.0.txt
--rw-r--r--   0 balder    (1000) balder    (1000)     1119 2019-02-17 15:27:39.000000 sphinx_rtd_theme-1.2.0rc4/LICENSE
--rw-rw-r--   0 balder    (1000) balder    (1000)      576 2022-08-27 07:48:38.000000 sphinx_rtd_theme-1.2.0rc4/MANIFEST.in
--rw-r--r--   0 balder    (1000) balder    (1000)     4438 2019-02-17 15:27:39.000000 sphinx_rtd_theme-1.2.0rc4/OFL-License.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     4205 2023-02-06 17:04:36.801783 sphinx_rtd_theme-1.2.0rc4/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     2742 2022-08-27 20:29:16.000000 sphinx_rtd_theme-1.2.0rc4/README.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)      338 2022-08-27 07:48:38.000000 sphinx_rtd_theme-1.2.0rc4/babel.cfg
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.749781 sphinx_rtd_theme-1.2.0rc4/bin/
--rwxrwxr-x   0 balder    (1000) balder    (1000)      853 2022-08-27 07:48:38.000000 sphinx_rtd_theme-1.2.0rc4/bin/preinstall.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     2993 2023-02-06 17:04:36.801783 sphinx_rtd_theme-1.2.0rc4/setup.cfg
--rw-rw-r--   0 balder    (1000) balder    (1000)     2111 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/setup.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.753781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/
--rw-rw-r--   0 balder    (1000) balder    (1000)     3196 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     4277 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2915 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/footer.html
--rw-r--r--   0 balder    (1000) balder    (1000)     9716 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/layout.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.753781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2514 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5820 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2087 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4023 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/en/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/en/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)      457 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4912 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2567 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5094 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2380 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4828 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2693 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5018 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2522 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5050 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)      575 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)      842 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hu/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)      501 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)      765 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2703 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5824 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2750 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5711 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.757781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2549 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5505 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2339 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4257 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2354 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5038 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2780 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5830 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     3449 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     6468 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
--rw-rw-r--   0 balder    (1000) balder    (1000)     4633 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sphinx.pot
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2132 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4353 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2117 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     4142 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)     2511 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)     5523 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.741781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_TW/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 balder    (1000) balder    (1000)      506 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-rw-r--   0 balder    (1000) balder    (1000)      769 2023-02-06 17:03:37.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0 balder    (1000) balder    (1000)     1759 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/search.html
--rw-r--r--   0 balder    (1000) balder    (1000)      405 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/searchbox.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.745781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.761781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/
--rw-r--r--   0 balder    (1000) balder    (1000)     3229 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/badge_only.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.793783 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/
--rw-r--r--   0 balder    (1000) balder    (1000)    87624 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    67312 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)    86288 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    66444 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   165742 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   444379 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 balder    (1000) balder    (1000)   165548 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    98024 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    77160 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   323344 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   193308 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309728 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   184912 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   328412 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   195704 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309192 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   182708 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   135235 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/theme.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.797783 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/
--rw-r--r--   0 balder    (1000) balder    (1000)      934 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/badge_only.js
--rw-r--r--   0 balder    (1000) balder    (1000)     4370 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     2734 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/html5shiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     5023 2023-01-17 22:58:39.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 balder    (1000) balder    (1000)      407 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 balder    (1000) balder    (1000)     1247 2023-01-17 22:58:32.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/versions.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.753781 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4205 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     4199 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       58 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/entry_points.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2022-10-10 21:07:10.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/not-zip-safe
--rw-rw-r--   0 balder    (1000) balder    (1000)      158 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/requires.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       17 2023-02-06 17:04:36.000000 sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/top_level.txt
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.797783 sphinx_rtd_theme-1.2.0rc4/tests/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.745781 sphinx_rtd_theme-1.2.0rc4/tests/roots/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.797783 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-basic/
--rw-rw-r--   0 balder    (1000) balder    (1000)        8 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-basic/bar.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-basic/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       31 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-basic/foo.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       85 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-basic/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.801783 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-empty/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-empty/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-empty/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-02-06 17:04:36.801783 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-missing-toctree/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-missing-toctree/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       42 2017-06-15 20:20:48.000000 sphinx_rtd_theme-1.2.0rc4/tests/roots/test-missing-toctree/index.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)     3159 2022-08-27 20:29:16.000000 sphinx_rtd_theme-1.2.0rc4/tests/test_builders.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1770 2022-08-27 20:29:16.000000 sphinx_rtd_theme-1.2.0rc4/tests/util.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    11379 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/Apache-License-2.0.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1119 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/LICENSE
+-rw-rw-r--   0 balder    (1000) balder    (1000)      576 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/MANIFEST.in
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4438 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/OFL-License.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4182 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2742 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/README.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)      338 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/babel.cfg
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/bin/
+-rwxrwxr-x   0 balder    (1000) balder    (1000)      853 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/bin/preinstall.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2978 2023-05-23 09:16:49.108001 sphinx_rtd_theme-1.2.1/setup.cfg
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2108 2023-05-23 09:16:33.000000 sphinx_rtd_theme-1.2.1/setup.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3477 2023-05-23 09:16:33.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     4277 2023-03-28 12:09:17.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2915 2023-03-28 12:09:17.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     9716 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/layout.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2514 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5820 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2087 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4023 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/en/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/en/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      457 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4912 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2567 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5094 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2380 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4828 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2693 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5018 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2522 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5050 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      575 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      842 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hu/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      501 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      765 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2703 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5824 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2750 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5711 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2549 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5505 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2339 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4257 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2354 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5038 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2780 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5830 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.088001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     3449 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     6468 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 balder    (1000) balder    (1000)     4633 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sphinx.pot
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.100001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2132 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4353 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.100001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2117 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4142 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.100001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2511 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5523 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_TW/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.100001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      506 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      769 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 balder    (1000) balder    (1000)     1759 2023-03-28 12:09:17.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/search.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      405 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/searchbox.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.100001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 balder    (1000) balder    (1000)     3229 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/badge_only.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/
+-rw-r--r--   0 balder    (1000) balder    (1000)    87624 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    67312 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)    86288 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    66444 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   165742 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 balder    (1000) balder    (1000)   444379 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 balder    (1000) balder    (1000)   165548 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 balder    (1000) balder    (1000)    98024 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    77160 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   323344 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   193308 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   309728 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   184912 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   328412 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   195704 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   309192 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   182708 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
+-rw-rw-r--   0 balder    (1000) balder    (1000)   135235 2023-05-23 09:12:23.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/theme.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 balder    (1000) balder    (1000)      934 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/badge_only.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     4370 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     2734 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/html5shiv.min.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     5023 2023-03-28 12:09:22.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 balder    (1000) balder    (1000)      407 2023-03-28 12:09:18.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 balder    (1000) balder    (1000)     1247 2023-03-28 12:09:17.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/versions.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.096001 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4182 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4199 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/SOURCES.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)       57 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/entry_points.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-01-13 09:47:39.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/not-zip-safe
+-rw-rw-r--   0 balder    (1000) balder    (1000)      158 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/requires.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)       17 2023-05-23 09:16:49.000000 sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/top_level.txt
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/tests/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.092001 sphinx_rtd_theme-1.2.1/tests/roots/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/tests/roots/test-basic/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        8 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-basic/bar.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-basic/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       31 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-basic/foo.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)       85 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-basic/index.rst
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/tests/roots/test-empty/
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-empty/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-empty/index.rst
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-05-23 09:16:49.104001 sphinx_rtd_theme-1.2.1/tests/roots/test-missing-toctree/
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-missing-toctree/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       42 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/roots/test-missing-toctree/index.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3159 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/test_builders.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1770 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.1/tests/util.py
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/Apache-License-2.0.txt` & `sphinx_rtd_theme-1.2.1/Apache-License-2.0.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/LICENSE` & `sphinx_rtd_theme-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/MANIFEST.in` & `sphinx_rtd_theme-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/OFL-License.txt` & `sphinx_rtd_theme-1.2.1/OFL-License.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/PKG-INFO` & `sphinx_rtd_theme-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: sphinx_rtd_theme
-Version: 1.2.0rc4
+Version: 1.2.1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
 Project-URL: Issue Tracker, https://github.com/readthedocs/sphinx_rtd_theme/issues
-Platform: UNKNOWN
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -102,9 +101,7 @@
 Contributing
 ============
 
 If you would like to help modify or translate the theme, you'll find more
 information on contributing in our `contributing guide`_.
 
 .. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
-
-
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/README.rst` & `sphinx_rtd_theme-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/bin/preinstall.js` & `sphinx_rtd_theme-1.2.1/bin/preinstall.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/setup.cfg` & `sphinx_rtd_theme-1.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0rc4
+current_version = 1.2.1
 commit = false
 tag = false
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)((?P<release>[a-z]+)(?P<dev>\d+))?
 serialize = 
 	{major}.{minor}.{patch}{release}{dev}
 	{major}.{minor}.{patch}
 
@@ -109,14 +109,14 @@
 [bumpversion:file:sphinx_rtd_theme/__init__.py]
 
 [bumpversion:file:package.json]
 search = "version": "{current_version}",
 replace = "version": "{new_version}",
 
 [bumpversion:file:docs/changelog.rst]
-search = .. |development_version| replace:: {current_version}
-replace = .. |development_version| replace:: {new_version}
+search = .. |theme_version| replace:: {current_version}
+replace = .. |theme_version| replace:: {new_version}
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/setup.py` & `sphinx_rtd_theme-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def run(self):
         subprocess.run(['tx', 'push', '--source'], check=True)
         subprocess.run(['tx', 'pull', '--mode', 'onlyreviewed', '-f', '-a'], check=True)
 
 
 setup(
-    version='1.2.0rc4',
+    version='1.2.1',
     cmdclass={
         'update_translations': UpdateTranslationsCommand,
         'transifex': TransifexCommand,
         'build_assets': WebpackBuildCommand,
         'watch': WebpackDevelopCommand,
     },
 )
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/__init__.py` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sys import version_info as python_version
 
 from sphinx import version_info as sphinx_version
 from sphinx.locale import _
 from sphinx.util.logging import getLogger
 
 
-__version__ = '1.2.0rc4'
+__version__ = '1.2.1'
 __version_full__ = __version__
 
 logger = getLogger(__name__)
 
 
 def get_html_theme_path():
     """Return list of HTML theme paths."""
@@ -54,14 +54,18 @@
     # the sphinxcontrib-jquery extension is enabled.
     # See: https://dev.readthedocs.io/en/latest/design/sphinx-jquery.html
     if sphinx_version >= (6, 0, 0):
         # Documentation of Sphinx guarantees that an extension is added and
         # enabled at most once.
         # See: https://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx.application.Sphinx.setup_extension
         app.setup_extension("sphinxcontrib.jquery")
+        # However, we need to call the extension's callback since setup_extension doesn't do it
+        # See: https://github.com/sphinx-contrib/jquery/issues/23
+        from sphinxcontrib.jquery import add_js_files as jquery_add_js_files
+        jquery_add_js_files(app, app.config)
 
     # Register the theme that can be referenced without adding a theme path
     app.add_html_theme('sphinx_rtd_theme', path.abspath(path.dirname(__file__)))
 
     if sphinx_version >= (1, 8, 0):
         # Add Sphinx message catalog for newer versions of Sphinx
         # See http://www.sphinx-doc.org/en/master/extdev/appapi.html#sphinx.application.Sphinx.add_message_catalog
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/breadcrumbs.html` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/footer.html` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/layout.html` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sphinx.pot` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/search.html` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/badge_only.css` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal.woff` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/css/theme.css` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/badge_only.js` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/html5shiv.min.js` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/static/js/theme.js` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme/versions.html` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/PKG-INFO` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: sphinx-rtd-theme
-Version: 1.2.0rc4
+Version: 1.2.1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
 Project-URL: Issue Tracker, https://github.com/readthedocs/sphinx_rtd_theme/issues
-Platform: UNKNOWN
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -102,9 +101,7 @@
 Contributing
 ============
 
 If you would like to help modify or translate the theme, you'll find more
 information on contributing in our `contributing guide`_.
 
 .. _contributing guide: https://sphinx-rtd-theme.readthedocs.io/en/stable/contributing.html
-
-
```

### Comparing `sphinx_rtd_theme-1.2.0rc4/sphinx_rtd_theme.egg-info/SOURCES.txt` & `sphinx_rtd_theme-1.2.1/sphinx_rtd_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/tests/test_builders.py` & `sphinx_rtd_theme-1.2.1/tests/test_builders.py`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.0rc4/tests/util.py` & `sphinx_rtd_theme-1.2.1/tests/util.py`

 * *Files identical despite different names*

