# Comparing `tmp/clld-9.2.1.tar.gz` & `tmp/clld-9.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clld-9.2.1.tar", last modified: Wed Jul  6 09:55:11 2022, max compression
+gzip compressed data, was "clld-9.2.2.tar", last modified: Thu Nov  3 16:11:23 2022, max compression
```

## Comparing `clld-9.2.1.tar` & `clld-9.2.2.tar`

### file list

```diff
@@ -1,356 +1,358 @@
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       52 2021-02-27 10:49:50.000000 clld-9.2.1/MANIFEST.in
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6130 2022-07-06 09:55:11.881164 clld-9.2.1/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4489 2021-08-07 13:22:12.000000 clld-9.2.1/README.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      832 2022-07-06 09:55:11.881164 clld-9.2.1/setup.cfg
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2583 2022-07-06 09:53:10.000000 clld-9.2.1/setup.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.849164 clld-9.2.1/src/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.853164 clld-9.2.1/src/clld/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1438 2022-07-06 09:53:23.000000 clld-9.2.1/src/clld/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1046 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/__main__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       53 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/appconf.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7167 2021-12-09 09:01:15.000000 clld-9.2.1/src/clld/cliutil.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.853164 clld-9.2.1/src/clld/commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2387 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/commands/create.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      961 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/commands/create_downloads.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2377 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/commands/initdb.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      924 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/config.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/db/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      471 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      453 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/fts.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    10331 2021-12-15 08:10:41.000000 clld-9.2.1/src/clld/db/meta.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/db/models/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1437 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4394 2021-08-07 14:17:55.000000 clld-9.2.1/src/clld/db/models/_mixins.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1382 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/common.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2241 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/config.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2860 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/contribution.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      999 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/contributor.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3440 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/dataset.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      538 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/gloss.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3955 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/language.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5930 2021-09-27 09:11:38.000000 clld-9.2.1/src/clld/db/models/parameter.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2331 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/sentence.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3958 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/source.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      858 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/unit.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1644 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/unitparameter.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2514 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/unitvalue.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2918 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/value.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2613 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/db/models/valueset.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4267 2022-03-16 12:09:52.000000 clld-9.2.1/src/clld/db/util.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4083 2021-08-20 08:04:35.000000 clld-9.2.1/src/clld/interfaces.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/lib/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      122 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/lib/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2450 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/lib/bibo.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13473 2021-08-16 11:25:29.000000 clld-9.2.1/src/clld/lib/bibtex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13319 2021-03-30 11:35:09.000000 clld-9.2.1/src/clld/lib/coins.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15795 2021-12-15 08:41:45.000000 clld-9.2.1/src/clld/lib/latex.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3740 2021-12-09 09:54:58.000000 clld-9.2.1/src/clld/lib/rdf.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/locale/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6797 2021-12-15 10:26:18.000000 clld-9.2.1/src/clld/locale/clld.pot
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.849164 clld-9.2.1/src/clld/locale/en/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/locale/en/LC_MESSAGES/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      436 2021-12-15 10:26:34.000000 clld-9.2.1/src/clld/locale/en/LC_MESSAGES/clld.mo
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7324 2021-12-15 10:26:27.000000 clld-9.2.1/src/clld/locale/en/LC_MESSAGES/clld.po
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       85 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/cookiecutter.json
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      339 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/.gitignore
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      841 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/CONTRIBUTING.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      154 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/MANIFEST.in
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      896 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/development.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       70 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/requirements.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      927 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/setup.cfg
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1215 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/setup.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      118 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/tox.ini
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/
--rwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)     1909 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       32 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/adapters.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      524 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/appconf.ini
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      336 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/assets.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1142 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/datatables.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/interfaces.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/locale/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/locale/{{cookiecutter.directory_name}}.pot
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/maps.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1474 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/models.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5976 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/initializedb.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/download/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       71 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/download/.gitignore
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/project.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/project.js
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.857164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/dataset/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      291 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/dataset/detail_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1055 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      270 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/{{cookiecutter.directory_name}}.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       65 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/conftest.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/test_functional.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      285 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/test_selenium.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/views.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2149 2021-12-09 08:13:03.000000 clld-9.2.1/src/clld/util.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/__init__.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/adapters/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6072 2021-12-15 07:58:03.000000 clld-9.2.1/src/clld/web/adapters/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2692 2021-12-15 07:58:03.000000 clld-9.2.1/src/clld/web/adapters/base.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1187 2021-08-16 11:24:29.000000 clld-9.2.1/src/clld/web/adapters/biblio.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8654 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/adapters/cldf.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1027 2021-12-15 07:54:56.000000 clld-9.2.1/src/clld/web/adapters/csv.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7511 2021-03-30 11:39:43.000000 clld-9.2.1/src/clld/web/adapters/download.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7964 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/adapters/geojson.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2360 2021-08-16 11:24:29.000000 clld-9.2.1/src/clld/web/adapters/md.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1594 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/adapters/rdf.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    25563 2022-03-16 12:17:39.000000 clld-9.2.1/src/clld/web/app.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1445 2022-07-05 15:01:24.000000 clld-9.2.1/src/clld/web/assets.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/datatables/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      586 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    21461 2022-07-06 07:58:45.000000 clld-9.2.1/src/clld/web/datatables/base.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      881 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/contribution.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1221 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/contributor.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      610 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/language.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      334 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/parameter.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3105 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/sentence.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1489 2022-07-06 07:57:34.000000 clld-9.2.1/src/clld/web/datatables/source.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      943 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/unit.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      262 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/unitparameter.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1806 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/unitvalue.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3929 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/value.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2324 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/datatables/valueset.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2106 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/icon.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/maps/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15060 2021-12-15 07:05:47.000000 clld-9.2.1/src/clld/web/maps/__init__.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/static/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.861164 clld-9.2.1/src/clld/web/static/.webassets-cache/
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       47 2022-07-06 09:52:35.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/015d42f9b9be17c428735fc2da7d100d
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-12-15 10:34:30.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/0f53c117ac9549ffa9f101e3c3387ac6
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-03-31 07:11:23.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/3f456709c2d379e7bc1d107305c8ffd4
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-08-20 08:34:15.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/41d5df099f12f83d958e29620444cba6
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   119477 2022-07-05 15:39:13.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/5b4852e05666144e7e3ce5e914f43408
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-11-18 14:03:24.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/6def061fc1f206f1c5e9672af7eb1bc9
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-12-15 10:34:30.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/8f4b3e65e12b7f18c0f7f08bcfea73b5
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       47 2022-07-06 09:52:35.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/be17c11ffe27fb172d20a504bf7e763b
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-08-20 08:34:15.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/d2e00d907e770875761338a1cfd6d1ce
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-11-18 14:03:24.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/efb1db9169c4f4105d132b859dd4467a
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   113434 2022-07-05 15:06:23.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/f51920bd59c7599547bc5a8c2a5e2d87
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   113217 2021-03-31 07:11:23.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/fd4682d5ae13ae9cabb4ca7b41fdaae1
--rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-03-31 07:11:23.000000 clld-9.2.1/src/clld/web/static/.webassets-cache/fd5d083cd17123bf4d67d9e6f78f79f4
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       92 2022-07-06 09:52:35.000000 clld-9.2.1/src/clld/web/static/.webassets-manifest
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.865164 clld-9.2.1/src/clld/web/static/css/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2227 2021-12-15 10:02:17.000000 clld-9.2.1/src/clld/web/static/css/L.Control.Resizer.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    21751 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/bootstrap-responsive.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    16840 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/bootstrap-responsive.min.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   124223 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/bootstrap.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   106006 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/bootstrap.min.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      577 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/charissil.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5090 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/clld.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      299 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/fullscreen.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      420 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/fullscreen@2x.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6312 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/hint.css
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.865164 clld-9.2.1/src/clld/web/static/css/images/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1259 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/images/layers-2x.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      696 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/images/layers.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2464 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/images/marker-icon-2x.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1466 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/images/marker-icon.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      618 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/images/marker-shadow.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4095 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/introjs.min.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2912 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/jqtree.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    17186 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/jquery.dataTables.css
--rw-r--r--   0 robert_forkel  (1001) robert_forkel  (1001)    14661 2022-04-18 10:42:32.000000 clld-9.2.1/src/clld/web/static/css/leaflet.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      994 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/leaflet.fullscreen.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1849 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/select2-spinner.gif
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    20979 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/select2.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      613 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/select2.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      845 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/select2x2.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4011 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/css/slider.css
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.869164 clld-9.2.1/src/clld/web/static/fonts/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1443920 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-B.ttf
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   550966 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-B.woff
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1504932 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-BI.ttf
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   578214 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-BI.woff
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1510100 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-I.ttf
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   579182 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-I.woff
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1508296 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-R.ttf
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   563806 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-R.woff
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    14176 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/fonts/CharisSIL-WOFF-metadata.xml
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.873164 clld-9.2.1/src/clld/web/static/images/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3256 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/GitHub_Logo.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1361 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/back_disabled.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1379 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/back_enabled.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1375 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/back_enabled_hover.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5488 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc-nd-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5647 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc-nd.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5724 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc-sa-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5811 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc-sa.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4779 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4679 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nc.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4729 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nd-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4488 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-nd.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5064 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-sa-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4641 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-sa.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3978 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4739 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-by.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2574 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-zero-small.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1911 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/cc-zero.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    23710 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/concepticon.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2179 2021-03-26 09:59:16.000000 clld-9.2.1/src/clld/web/static/images/doi_logo.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      198 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/favicon.ico
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1363 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/forward_disabled.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1380 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/forward_enabled.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1379 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/forward_enabled_hover.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2515 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/glottolog.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2520 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/glottolog_white.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      389 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/icon-fullscreen.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11822 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/minerva.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1091 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/pdf-icon.gif
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1118 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/sort_asc.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2916 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/sort_asc_disabled.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1136 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/sort_both.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1127 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/sort_desc.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1045 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/images/sort_desc_disabled.png
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.873164 clld-9.2.1/src/clld/web/static/img/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8777 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/img/glyphicons-halflings-white.png
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12799 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/img/glyphicons-halflings.png
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/static/js/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6305 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/L.Control.Resizer.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5041 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/Leaflet.fullscreen.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    22494 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/bootstrap-slider.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    58516 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/bootstrap.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    28631 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/bootstrap.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7291 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/bootstrapx-clickover.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    34601 2021-03-12 08:07:38.000000 clld-9.2.1/src/clld/web/static/js/clld.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6061 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/intro.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   450399 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/jquery.dataTables.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    86550 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/jquery.dataTables.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   293430 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/jquery.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    33811 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/jsphylosvg.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3462 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/leaflet-hash.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    28980 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/leaflet-providers.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   431150 2022-07-06 09:46:48.000000 clld-9.2.1/src/clld/web/static/js/leaflet-src.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   143873 2022-07-06 09:46:21.000000 clld-9.2.1/src/clld/web/static/js/leaflet.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5630 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/oms.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    54846 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/raphael.min.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   120838 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/select2.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    88248 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/js/tree.jquery.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/project.css
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       55 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/static/project.js
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1772 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/subscribers.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9047 2022-07-05 15:27:50.000000 clld-9.2.1/src/clld/web/templates/app.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      433 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/atom_feed.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/combination/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1663 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/combination/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       34 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/combination/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1607 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/combined.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      938 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contact.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       72 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contactmail_body.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       53 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contactmail_subject.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/contribution/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      377 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contribution/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      308 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contribution/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      590 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contribution/md_txt.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      385 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contribution/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contribution/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/contributor/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      828 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contributor/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      255 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contributor/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      423 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contributor/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/contributor/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/dataset/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       38 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/dataset/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      369 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/dataset/md_txt.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3445 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/dataset/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       35 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/dataset/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2249 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/datatable.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      649 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/download.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      334 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/home_comp.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      676 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/index_atom.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1102 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/index_rdf.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.877164 clld-9.2.1/src/clld/web/templates/language/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      421 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      349 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      858 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/kml.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/map_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1328 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1123 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/language/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      336 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/legal.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1355 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/map.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       61 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/md_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      683 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/multiselect.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3473 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/olac.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      899 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/olac_archive.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1304 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/olac_record.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/parameter/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      490 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/parameter/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      291 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/parameter/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      112 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/parameter/kml.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/parameter/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      809 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/parameter/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1011 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/resource_rdf.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/sentence/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1166 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/sentence/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      248 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/sentence/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      745 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/sentence/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      110 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/sentence/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       47 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/snippet.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/source/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2678 2021-08-16 11:24:29.000000 clld-9.2.1/src/clld/web/templates/source/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      290 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/source/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1358 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/source/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      689 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/source/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      224 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unapiformats.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/unit/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      613 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unit/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      241 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unit/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      154 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unit/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unit/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/unitparameter/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      409 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitparameter/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      260 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitparameter/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1026 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitparameter/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitparameter/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/unitvalue/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      233 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitvalue/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      256 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitvalue/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      572 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitvalue/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/unitvalue/snippet_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    14483 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/util.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/value/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1046 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/value/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      250 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/value/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      700 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/value/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      550 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/value/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/templates/valueset/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2068 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/valueset/detail_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      254 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/valueset/index_html.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      750 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/valueset/rdf.mako
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      510 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/templates/valueset/snippet_html.mako
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/util/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1498 2021-12-15 08:41:02.000000 clld-9.2.1/src/clld/web/util/component.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      898 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/concepticon.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1003 2021-03-26 11:13:58.000000 clld-9.2.1/src/clld/web/util/doi.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3233 2022-05-12 14:22:58.000000 clld-9.2.1/src/clld/web/util/downloadwidget.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      751 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/glottolog.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    23936 2022-07-06 07:16:38.000000 clld-9.2.1/src/clld/web/util/helpers.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      286 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/htmllib.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2973 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/multiselect.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      946 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/util/pager.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.881164 clld-9.2.1/src/clld/web/views/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8411 2021-12-15 08:00:34.000000 clld-9.2.1/src/clld/web/views/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9598 2021-02-27 10:49:50.000000 clld-9.2.1/src/clld/web/views/olac.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4660 2021-08-07 14:38:34.000000 clld-9.2.1/src/clld/web/views/sitemap.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-07-06 09:55:11.853164 clld-9.2.1/src/clld.egg-info/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6130 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13809 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/SOURCES.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/dependency_links.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       64 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/entry_points.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-03-01 08:55:38.000000 clld-9.2.1/src/clld.egg-info/not-zip-safe
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      462 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/requires.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        5 2022-07-06 09:55:11.000000 clld-9.2.1/src/clld.egg-info/top_level.txt
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.129714 clld-9.2.2/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12419 2021-02-27 10:49:50.000000 clld-9.2.2/LICENSE.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       52 2021-02-27 10:49:50.000000 clld-9.2.2/MANIFEST.in
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6064 2022-11-03 16:11:23.129714 clld-9.2.2/PKG-INFO
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4380 2022-11-03 15:55:29.000000 clld-9.2.2/README.md
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       81 2022-07-28 11:14:15.000000 clld-9.2.2/pyproject.toml
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      832 2022-11-03 16:11:23.129714 clld-9.2.2/setup.cfg
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2654 2022-11-03 16:10:15.000000 clld-9.2.2/setup.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.093714 clld-9.2.2/src/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.097714 clld-9.2.2/src/clld/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1438 2022-11-03 16:10:26.000000 clld-9.2.2/src/clld/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1046 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/__main__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       53 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/appconf.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7167 2021-12-09 09:01:15.000000 clld-9.2.2/src/clld/cliutil.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.097714 clld-9.2.2/src/clld/commands/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/commands/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2387 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/commands/create.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      961 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/commands/create_downloads.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2377 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/commands/initdb.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      924 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/config.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.097714 clld-9.2.2/src/clld/db/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      471 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      453 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/fts.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    10331 2021-12-15 08:10:41.000000 clld-9.2.2/src/clld/db/meta.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/db/models/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1437 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4394 2021-08-07 14:17:55.000000 clld-9.2.2/src/clld/db/models/_mixins.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1382 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/common.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2241 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/config.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2860 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/contribution.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      999 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/contributor.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3440 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/dataset.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      538 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/gloss.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3955 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/language.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5930 2021-09-27 09:11:38.000000 clld-9.2.2/src/clld/db/models/parameter.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2331 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/sentence.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3958 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/source.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      858 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/unit.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1644 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/unitparameter.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2514 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/unitvalue.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2918 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/value.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2613 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/db/models/valueset.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4267 2022-03-16 12:09:52.000000 clld-9.2.2/src/clld/db/util.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4083 2021-08-20 08:04:35.000000 clld-9.2.2/src/clld/interfaces.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/lib/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      122 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/lib/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2450 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/lib/bibo.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13473 2021-08-16 11:25:29.000000 clld-9.2.2/src/clld/lib/bibtex.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13319 2021-03-30 11:35:09.000000 clld-9.2.2/src/clld/lib/coins.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15795 2021-12-15 08:41:45.000000 clld-9.2.2/src/clld/lib/latex.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3740 2021-12-09 09:54:58.000000 clld-9.2.2/src/clld/lib/rdf.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/locale/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6797 2021-12-15 10:26:18.000000 clld-9.2.2/src/clld/locale/clld.pot
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.093714 clld-9.2.2/src/clld/locale/en/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      436 2021-12-15 10:26:34.000000 clld-9.2.2/src/clld/locale/en/LC_MESSAGES/clld.mo
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7324 2021-12-15 10:26:27.000000 clld-9.2.2/src/clld/locale/en/LC_MESSAGES/clld.po
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       85 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/cookiecutter.json
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      339 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/.gitignore
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      841 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/CONTRIBUTING.md
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      154 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/MANIFEST.in
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      896 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/development.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       70 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/requirements.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      927 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/setup.cfg
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1215 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/setup.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      118 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/tox.ini
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/
+-rwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)     1909 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       32 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/adapters.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      524 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/appconf.ini
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      336 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/assets.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1142 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/datatables.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/interfaces.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/locale/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/locale/{{cookiecutter.directory_name}}.pot
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/maps.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1474 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/models.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5976 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/initializedb.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/download/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       71 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/download/.gitignore
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/project.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/static/project.js
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/dataset/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      291 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/dataset/detail_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1055 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      270 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/{{cookiecutter.directory_name}}.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       65 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/conftest.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/test_functional.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      285 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/tests/test_selenium.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        2 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/views.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2149 2021-12-09 08:13:03.000000 clld-9.2.2/src/clld/util.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.101714 clld-9.2.2/src/clld/web/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/__init__.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.105714 clld-9.2.2/src/clld/web/adapters/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6072 2021-12-15 07:58:03.000000 clld-9.2.2/src/clld/web/adapters/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2692 2021-12-15 07:58:03.000000 clld-9.2.2/src/clld/web/adapters/base.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1187 2021-08-16 11:24:29.000000 clld-9.2.2/src/clld/web/adapters/biblio.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8654 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/adapters/cldf.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1027 2021-12-15 07:54:56.000000 clld-9.2.2/src/clld/web/adapters/csv.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7511 2021-03-30 11:39:43.000000 clld-9.2.2/src/clld/web/adapters/download.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7964 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/adapters/geojson.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2360 2021-08-16 11:24:29.000000 clld-9.2.2/src/clld/web/adapters/md.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1594 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/adapters/rdf.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    25563 2022-03-16 12:17:39.000000 clld-9.2.2/src/clld/web/app.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1445 2022-07-05 15:01:24.000000 clld-9.2.2/src/clld/web/assets.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.105714 clld-9.2.2/src/clld/web/datatables/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      586 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    21461 2022-07-06 07:58:45.000000 clld-9.2.2/src/clld/web/datatables/base.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      881 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/contribution.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1221 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/contributor.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      610 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/language.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      334 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/parameter.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3105 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/sentence.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1489 2022-07-06 07:57:34.000000 clld-9.2.2/src/clld/web/datatables/source.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      943 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/unit.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      262 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/unitparameter.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1806 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/unitvalue.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3929 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/value.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2324 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/datatables/valueset.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2106 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/icon.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.105714 clld-9.2.2/src/clld/web/maps/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    15060 2021-12-15 07:05:47.000000 clld-9.2.2/src/clld/web/maps/__init__.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.105714 clld-9.2.2/src/clld/web/static/
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.105714 clld-9.2.2/src/clld/web/static/.webassets-cache/
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       47 2022-07-06 09:52:35.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/015d42f9b9be17c428735fc2da7d100d
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-12-15 10:34:30.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/0f53c117ac9549ffa9f101e3c3387ac6
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-03-31 07:11:23.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/3f456709c2d379e7bc1d107305c8ffd4
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-08-20 08:34:15.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/41d5df099f12f83d958e29620444cba6
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   119477 2022-07-05 15:39:13.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/5b4852e05666144e7e3ce5e914f43408
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-11-18 14:03:24.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/6def061fc1f206f1c5e9672af7eb1bc9
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-12-15 10:34:30.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/8f4b3e65e12b7f18c0f7f08bcfea73b5
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       47 2022-07-06 09:52:35.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/be17c11ffe27fb172d20a504bf7e763b
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-08-20 08:34:15.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/d2e00d907e770875761338a1cfd6d1ce
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-11-18 14:03:24.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/efb1db9169c4f4105d132b859dd4467a
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   113434 2022-07-05 15:06:23.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/f51920bd59c7599547bc5a8c2a5e2d87
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)   113217 2021-03-31 07:11:23.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/fd4682d5ae13ae9cabb4ca7b41fdaae1
+-rw-------   0 robert_forkel  (1001) robert_forkel  (1001)       15 2021-03-31 07:11:23.000000 clld-9.2.2/src/clld/web/static/.webassets-cache/fd5d083cd17123bf4d67d9e6f78f79f4
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       92 2022-07-06 09:52:35.000000 clld-9.2.2/src/clld/web/static/.webassets-manifest
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.109714 clld-9.2.2/src/clld/web/static/css/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2227 2021-12-15 10:02:17.000000 clld-9.2.2/src/clld/web/static/css/L.Control.Resizer.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    21751 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/bootstrap-responsive.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    16840 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/bootstrap-responsive.min.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   124223 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/bootstrap.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   106006 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/bootstrap.min.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      577 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/charissil.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5090 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/clld.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      299 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/fullscreen.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      420 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/fullscreen@2x.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6312 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/hint.css
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.109714 clld-9.2.2/src/clld/web/static/css/images/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1259 2022-09-23 08:57:12.000000 clld-9.2.2/src/clld/web/static/css/images/layers-2x.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      696 2022-09-23 08:57:12.000000 clld-9.2.2/src/clld/web/static/css/images/layers.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2464 2022-09-23 08:57:12.000000 clld-9.2.2/src/clld/web/static/css/images/marker-icon-2x.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1466 2022-09-23 08:57:12.000000 clld-9.2.2/src/clld/web/static/css/images/marker-icon.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      618 2022-09-23 08:57:12.000000 clld-9.2.2/src/clld/web/static/css/images/marker-shadow.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4095 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/introjs.min.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2912 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/jqtree.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    17186 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/jquery.dataTables.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    14670 2022-09-28 10:37:58.000000 clld-9.2.2/src/clld/web/static/css/leaflet.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      994 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/leaflet.fullscreen.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1849 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/select2-spinner.gif
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    20979 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/select2.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      613 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/select2.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      845 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/select2x2.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4011 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/css/slider.css
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.113714 clld-9.2.2/src/clld/web/static/fonts/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1443920 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-B.ttf
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   550966 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-B.woff
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1504932 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-BI.ttf
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   578214 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-BI.woff
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1510100 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-I.ttf
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   579182 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-I.woff
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)  1508296 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-R.ttf
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   563806 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-R.woff
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    14176 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/fonts/CharisSIL-WOFF-metadata.xml
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.117714 clld-9.2.2/src/clld/web/static/images/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3256 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/GitHub_Logo.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1361 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/back_disabled.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1379 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/back_enabled.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1375 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/back_enabled_hover.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5488 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc-nd-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5647 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc-nd.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5724 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc-sa-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5811 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc-sa.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4779 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4679 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nc.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4729 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nd-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4488 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-nd.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5064 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-sa-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4641 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-sa.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3978 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4739 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-by.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2574 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-zero-small.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1911 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/cc-zero.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    23710 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/concepticon.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2179 2021-03-26 09:59:16.000000 clld-9.2.2/src/clld/web/static/images/doi_logo.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      198 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/favicon.ico
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1363 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/forward_disabled.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1380 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/forward_enabled.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1379 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/forward_enabled_hover.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2515 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/glottolog.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2520 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/glottolog_white.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      389 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/icon-fullscreen.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11822 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/minerva.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1091 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/pdf-icon.gif
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1118 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/sort_asc.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2916 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/sort_asc_disabled.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1136 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/sort_both.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1127 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/sort_desc.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1045 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/images/sort_desc_disabled.png
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.117714 clld-9.2.2/src/clld/web/static/img/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8777 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/img/glyphicons-halflings-white.png
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    12799 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/img/glyphicons-halflings.png
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.121714 clld-9.2.2/src/clld/web/static/js/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6305 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/L.Control.Resizer.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5041 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/Leaflet.fullscreen.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    22494 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/bootstrap-slider.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    58516 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/bootstrap.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    28631 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/bootstrap.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     7291 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/bootstrapx-clickover.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    34424 2022-11-03 15:06:55.000000 clld-9.2.2/src/clld/web/static/js/clld.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6061 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/intro.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   450399 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/jquery.dataTables.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    86550 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/jquery.dataTables.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   293430 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/jquery.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    33811 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/jsphylosvg.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3462 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/leaflet-hash.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    32423 2022-11-03 15:05:11.000000 clld-9.2.2/src/clld/web/static/js/leaflet-providers.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   431150 2022-07-06 09:46:48.000000 clld-9.2.2/src/clld/web/static/js/leaflet-src.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   147555 2022-09-28 10:36:27.000000 clld-9.2.2/src/clld/web/static/js/leaflet.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     5630 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/oms.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    54846 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/raphael.min.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)   120838 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/select2.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    88248 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/js/tree.jquery.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/project.css
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       55 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/static/project.js
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1772 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/subscribers.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.121714 clld-9.2.2/src/clld/web/templates/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9047 2022-07-05 15:27:50.000000 clld-9.2.2/src/clld/web/templates/app.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      433 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/atom_feed.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.121714 clld-9.2.2/src/clld/web/templates/combination/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1663 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/combination/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       34 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/combination/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1607 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/combined.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      938 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contact.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       72 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contactmail_body.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       53 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contactmail_subject.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.121714 clld-9.2.2/src/clld/web/templates/contribution/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      377 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contribution/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      308 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contribution/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      590 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contribution/md_txt.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      385 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contribution/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contribution/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/contributor/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      828 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contributor/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      255 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contributor/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      423 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contributor/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/contributor/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/dataset/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       38 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/dataset/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      369 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/dataset/md_txt.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3445 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/dataset/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       35 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/dataset/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2249 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/datatable.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      649 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/download.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      334 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/home_comp.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      676 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/index_atom.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1102 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/index_rdf.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/language/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      421 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      349 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      858 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/kml.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/map_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1328 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1123 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/language/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      336 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/legal.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1355 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/map.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       61 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/md_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      683 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/multiselect.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3473 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/olac.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      899 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/olac_archive.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1304 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/olac_record.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/parameter/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      490 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/parameter/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      291 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/parameter/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      112 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/parameter/kml.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/parameter/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      809 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/parameter/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1011 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/resource_rdf.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/sentence/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1166 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/sentence/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      248 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/sentence/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      745 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/sentence/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      110 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/sentence/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       47 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/snippet.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/source/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2678 2021-08-16 11:24:29.000000 clld-9.2.2/src/clld/web/templates/source/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      290 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/source/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1358 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/source/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      689 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/source/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      224 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unapiformats.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/unit/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      613 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unit/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      241 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unit/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      154 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unit/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unit/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/unitparameter/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      409 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitparameter/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      260 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitparameter/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1026 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitparameter/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitparameter/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/unitvalue/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      233 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitvalue/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      256 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitvalue/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      572 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitvalue/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      141 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/unitvalue/snippet_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    14483 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/util.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/value/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1046 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/value/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      250 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/value/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      700 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/value/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      550 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/value/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.125714 clld-9.2.2/src/clld/web/templates/valueset/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2068 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/valueset/detail_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      254 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/valueset/index_html.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      750 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/valueset/rdf.mako
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      510 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/templates/valueset/snippet_html.mako
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.129714 clld-9.2.2/src/clld/web/util/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       54 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1498 2021-12-15 08:41:02.000000 clld-9.2.2/src/clld/web/util/component.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      898 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/concepticon.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1003 2021-03-26 11:13:58.000000 clld-9.2.2/src/clld/web/util/doi.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3233 2022-05-12 14:22:58.000000 clld-9.2.2/src/clld/web/util/downloadwidget.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      751 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/glottolog.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    23936 2022-07-06 07:16:38.000000 clld-9.2.2/src/clld/web/util/helpers.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      286 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/htmllib.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     2973 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/multiselect.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      946 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/util/pager.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.129714 clld-9.2.2/src/clld/web/views/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     8411 2021-12-15 08:00:34.000000 clld-9.2.2/src/clld/web/views/__init__.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9598 2021-02-27 10:49:50.000000 clld-9.2.2/src/clld/web/views/olac.py
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     4660 2021-08-07 14:38:34.000000 clld-9.2.2/src/clld/web/views/sitemap.py
+drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-11-03 16:11:23.097714 clld-9.2.2/src/clld.egg-info/
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     6064 2022-11-03 16:11:22.000000 clld-9.2.2/src/clld.egg-info/PKG-INFO
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    13836 2022-11-03 16:11:23.000000 clld-9.2.2/src/clld.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-11-03 16:11:22.000000 clld-9.2.2/src/clld.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       64 2022-11-03 16:11:22.000000 clld-9.2.2/src/clld.egg-info/entry_points.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-03-01 08:55:38.000000 clld-9.2.2/src/clld.egg-info/not-zip-safe
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      468 2022-11-03 16:11:22.000000 clld-9.2.2/src/clld.egg-info/requires.txt
+-rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        5 2022-11-03 16:11:22.000000 clld-9.2.2/src/clld.egg-info/top_level.txt
```

### Comparing `clld-9.2.1/PKG-INFO` & `clld-9.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: clld
-Version: 9.2.1
+Version: 9.2.2
 Summary: Python library supporting the development of cross-linguistic databases
 Home-page: https://clld.org
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache Software License
 Description: # clld
         
         The `clld` toolkit - a web framework for the publication of
         [Cross-Linguistic Linked Data](https://clld.org).
         
         Documentation for the code base and its use is available at http://clld.readthedocs.org/en/latest/. The source for this documentation is in the `docs` directory.
         
         [![Build Status](https://github.com/clld/clld/workflows/tests/badge.svg)](https://github.com/clld/clld/actions?query=workflow%3Atests)
-        [![codecov](https://codecov.io/gh/clld/clld/branch/master/graph/badge.svg)](https://codecov.io/gh/clld/clld)
         [![Requirements Status](https://requires.io/github/clld/clld/requirements.svg?branch=master)](https://requires.io/github/clld/clld/requirements/?branch=master)
         [![PyPI](https://img.shields.io/pypi/v/clld.svg)](https://pypi.python.org/pypi/clld)
         [![Documentation Status](http://readthedocs.org/projects/clld/badge/?version=latest)](http://clld.readthedocs.io/en/latest/?badge=latest)
         
         
         ## Cite
         
@@ -92,14 +91,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `clld-9.2.1/README.md` & `clld-9.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 The `clld` toolkit - a web framework for the publication of
 [Cross-Linguistic Linked Data](https://clld.org).
 
 Documentation for the code base and its use is available at http://clld.readthedocs.org/en/latest/. The source for this documentation is in the `docs` directory.
 
 [![Build Status](https://github.com/clld/clld/workflows/tests/badge.svg)](https://github.com/clld/clld/actions?query=workflow%3Atests)
-[![codecov](https://codecov.io/gh/clld/clld/branch/master/graph/badge.svg)](https://codecov.io/gh/clld/clld)
 [![Requirements Status](https://requires.io/github/clld/clld/requirements.svg?branch=master)](https://requires.io/github/clld/clld/requirements/?branch=master)
 [![PyPI](https://img.shields.io/pypi/v/clld.svg)](https://pypi.python.org/pypi/clld)
 [![Documentation Status](http://readthedocs.org/projects/clld/badge/?version=latest)](http://clld.readthedocs.io/en/latest/?badge=latest)
 
 
 ## Cite
```

### Comparing `clld-9.2.1/setup.cfg` & `clld-9.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/setup.py` & `clld-9.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='clld',
-    version='9.2.1',
+    version='9.2.2',
     description=(
         'Python library supporting the development of cross-linguistic databases'),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Internet :: WWW/HTTP",
         "Topic :: Internet :: WWW/HTTP :: WSGI",
     ],
     keywords='web pyramid LRL Linguistics',
     author="Robert Forkel",
     author_email="robert_forkel@eva.mpg.de",
@@ -55,14 +56,15 @@
             'cldfcatalog',
             'waitress',
             'pyramid_debugtoolbar',
             'tox',
             'flake8',
             'wheel',
             'twine',
+            'build',
         ],
         'test': [
             'cookiecutter',
             'pytest>=6',
             'pytest-clld>=1.0.3',
             'pytest-mock',
             'pytest-cov',
```

### Comparing `clld-9.2.1/src/clld/__init__.py` & `clld-9.2.2/src/clld/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 
 from clld.db.models import common
 from clld import interfaces
 
-__version__ = "9.2.1"
+__version__ = "9.2.2"
 
 
 class Resource(collections.namedtuple('Resource', 'name model interface with_index with_rdfdump')):
 
     def __new__(cls, name, model, interface, with_index=True, with_rdfdump=True):
         return super(Resource, cls).__new__(cls, name, model, interface, with_index, with_rdfdump)
```

### Comparing `clld-9.2.1/src/clld/__main__.py` & `clld-9.2.2/src/clld/__main__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/cliutil.py` & `clld-9.2.2/src/clld/cliutil.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/commands/create.py` & `clld-9.2.2/src/clld/commands/create.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/commands/create_downloads.py` & `clld-9.2.2/src/clld/commands/create_downloads.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/commands/initdb.py` & `clld-9.2.2/src/clld/commands/initdb.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/config.py` & `clld-9.2.2/src/clld/config.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/meta.py` & `clld-9.2.2/src/clld/db/meta.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/__init__.py` & `clld-9.2.2/src/clld/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/_mixins.py` & `clld-9.2.2/src/clld/db/models/_mixins.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/common.py` & `clld-9.2.2/src/clld/db/models/common.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/config.py` & `clld-9.2.2/src/clld/db/models/config.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/contribution.py` & `clld-9.2.2/src/clld/db/models/contribution.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/contributor.py` & `clld-9.2.2/src/clld/db/models/contributor.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/dataset.py` & `clld-9.2.2/src/clld/db/models/dataset.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/gloss.py` & `clld-9.2.2/src/clld/db/models/gloss.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/language.py` & `clld-9.2.2/src/clld/db/models/language.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/parameter.py` & `clld-9.2.2/src/clld/db/models/parameter.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/sentence.py` & `clld-9.2.2/src/clld/db/models/sentence.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/source.py` & `clld-9.2.2/src/clld/db/models/source.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/unit.py` & `clld-9.2.2/src/clld/db/models/unit.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/unitparameter.py` & `clld-9.2.2/src/clld/db/models/unitparameter.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/unitvalue.py` & `clld-9.2.2/src/clld/db/models/unitvalue.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/value.py` & `clld-9.2.2/src/clld/db/models/value.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/models/valueset.py` & `clld-9.2.2/src/clld/db/models/valueset.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/db/util.py` & `clld-9.2.2/src/clld/db/util.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/interfaces.py` & `clld-9.2.2/src/clld/interfaces.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/lib/bibo.py` & `clld-9.2.2/src/clld/lib/bibo.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/lib/bibtex.py` & `clld-9.2.2/src/clld/lib/bibtex.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/lib/coins.py` & `clld-9.2.2/src/clld/lib/coins.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/lib/latex.py` & `clld-9.2.2/src/clld/lib/latex.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/lib/rdf.py` & `clld-9.2.2/src/clld/lib/rdf.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/locale/clld.pot` & `clld-9.2.2/src/clld/locale/clld.pot`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/locale/en/LC_MESSAGES/clld.po` & `clld-9.2.2/src/clld/locale/en/LC_MESSAGES/clld.po`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/CONTRIBUTING.md` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/development.ini` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/development.ini`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/setup.cfg` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/setup.py` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/setup.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/__init__.py` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/appconf.ini` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/appconf.ini`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/datatables.py` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/datatables.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/models.py` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/models.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/initializedb.py` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/scripts/initializedb.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/detail_html.mako` & `clld-9.2.2/src/clld/project_template/{{cookiecutter.directory_name}}/{{cookiecutter.directory_name}}/templates/parameter/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/util.py` & `clld-9.2.2/src/clld/util.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/__init__.py` & `clld-9.2.2/src/clld/web/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/base.py` & `clld-9.2.2/src/clld/web/adapters/base.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/biblio.py` & `clld-9.2.2/src/clld/web/adapters/biblio.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/cldf.py` & `clld-9.2.2/src/clld/web/adapters/cldf.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/csv.py` & `clld-9.2.2/src/clld/web/adapters/csv.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/download.py` & `clld-9.2.2/src/clld/web/adapters/download.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/geojson.py` & `clld-9.2.2/src/clld/web/adapters/geojson.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/md.py` & `clld-9.2.2/src/clld/web/adapters/md.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/adapters/rdf.py` & `clld-9.2.2/src/clld/web/adapters/rdf.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/app.py` & `clld-9.2.2/src/clld/web/app.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/assets.py` & `clld-9.2.2/src/clld/web/assets.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/__init__.py` & `clld-9.2.2/src/clld/web/datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/base.py` & `clld-9.2.2/src/clld/web/datatables/base.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/contribution.py` & `clld-9.2.2/src/clld/web/datatables/contribution.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/contributor.py` & `clld-9.2.2/src/clld/web/datatables/contributor.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/language.py` & `clld-9.2.2/src/clld/web/datatables/language.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/sentence.py` & `clld-9.2.2/src/clld/web/datatables/sentence.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/source.py` & `clld-9.2.2/src/clld/web/datatables/source.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/unit.py` & `clld-9.2.2/src/clld/web/datatables/unit.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/unitvalue.py` & `clld-9.2.2/src/clld/web/datatables/unitvalue.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/value.py` & `clld-9.2.2/src/clld/web/datatables/value.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/datatables/valueset.py` & `clld-9.2.2/src/clld/web/datatables/valueset.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/icon.py` & `clld-9.2.2/src/clld/web/icon.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/maps/__init__.py` & `clld-9.2.2/src/clld/web/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/.webassets-cache/5b4852e05666144e7e3ce5e914f43408` & `clld-9.2.2/src/clld/web/static/.webassets-cache/5b4852e05666144e7e3ce5e914f43408`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/.webassets-cache/f51920bd59c7599547bc5a8c2a5e2d87` & `clld-9.2.2/src/clld/web/static/.webassets-cache/f51920bd59c7599547bc5a8c2a5e2d87`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/.webassets-cache/fd4682d5ae13ae9cabb4ca7b41fdaae1` & `clld-9.2.2/src/clld/web/static/.webassets-cache/fd4682d5ae13ae9cabb4ca7b41fdaae1`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/L.Control.Resizer.css` & `clld-9.2.2/src/clld/web/static/css/L.Control.Resizer.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/bootstrap-responsive.css` & `clld-9.2.2/src/clld/web/static/css/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/bootstrap-responsive.min.css` & `clld-9.2.2/src/clld/web/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/bootstrap.css` & `clld-9.2.2/src/clld/web/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/bootstrap.min.css` & `clld-9.2.2/src/clld/web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/charissil.css` & `clld-9.2.2/src/clld/web/static/css/charissil.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/clld.css` & `clld-9.2.2/src/clld/web/static/css/clld.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/hint.css` & `clld-9.2.2/src/clld/web/static/css/hint.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/images/layers-2x.png` & `clld-9.2.2/src/clld/web/static/css/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/images/layers.png` & `clld-9.2.2/src/clld/web/static/css/images/layers.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/images/marker-icon-2x.png` & `clld-9.2.2/src/clld/web/static/css/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/images/marker-icon.png` & `clld-9.2.2/src/clld/web/static/css/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/images/marker-shadow.png` & `clld-9.2.2/src/clld/web/static/css/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/introjs.min.css` & `clld-9.2.2/src/clld/web/static/css/introjs.min.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/jqtree.css` & `clld-9.2.2/src/clld/web/static/css/jqtree.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/jquery.dataTables.css` & `clld-9.2.2/src/clld/web/static/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/leaflet.css` & `clld-9.2.2/src/clld/web/static/css/leaflet.css`

 * *Files 2% similar despite different names*

```diff
@@ -419,16 +419,19 @@
 .leaflet-control-attribution a {
 	text-decoration: none;
 	}
 .leaflet-control-attribution a:hover,
 .leaflet-control-attribution a:focus {
 	text-decoration: underline;
 	}
-.leaflet-control-attribution svg {
+.leaflet-attribution-flag {
 	display: inline !important;
+	vertical-align: baseline !important;
+	width: 1em;
+	height: 0.6669em;
 	}
 .leaflet-left .leaflet-control-scale {
 	margin-left: 5px;
 	}
 .leaflet-bottom .leaflet-control-scale {
 	margin-bottom: 5px;
 	}
@@ -533,16 +536,14 @@
 	}
 .leaflet-container a.leaflet-popup-close-button:hover,
 .leaflet-container a.leaflet-popup-close-button:focus {
 	color: #585858;
 	}
 .leaflet-popup-scrolled {
 	overflow: auto;
-	border-bottom: 1px solid #ddd;
-	border-top: 1px solid #ddd;
 	}
 
 .leaflet-oldie .leaflet-popup-content-wrapper {
 	-ms-zoom: 1;
 	}
 .leaflet-oldie .leaflet-popup-tip {
 	width: 24px;
@@ -648,10 +649,10 @@
 
 /* Printing */
 	
 @media print {
 	/* Prevent printers from removing background-images of controls. */
 	.leaflet-control {
 		-webkit-print-color-adjust: exact;
-		color-adjust: exact;
+		print-color-adjust: exact;
 		}
 	}
```

### Comparing `clld-9.2.1/src/clld/web/static/css/leaflet.fullscreen.css` & `clld-9.2.2/src/clld/web/static/css/leaflet.fullscreen.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/select2-spinner.gif` & `clld-9.2.2/src/clld/web/static/css/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/select2.css` & `clld-9.2.2/src/clld/web/static/css/select2.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/select2.png` & `clld-9.2.2/src/clld/web/static/css/select2.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/select2x2.png` & `clld-9.2.2/src/clld/web/static/css/select2x2.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/css/slider.css` & `clld-9.2.2/src/clld/web/static/css/slider.css`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-B.ttf` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-B.ttf`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-B.woff` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-B.woff`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-BI.ttf` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-BI.ttf`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-BI.woff` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-BI.woff`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-I.ttf` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-I.ttf`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-I.woff` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-I.woff`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-R.ttf` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-R.ttf`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-R.woff` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-R.woff`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/fonts/CharisSIL-WOFF-metadata.xml` & `clld-9.2.2/src/clld/web/static/fonts/CharisSIL-WOFF-metadata.xml`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/GitHub_Logo.png` & `clld-9.2.2/src/clld/web/static/images/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/back_disabled.png` & `clld-9.2.2/src/clld/web/static/images/back_disabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/back_enabled.png` & `clld-9.2.2/src/clld/web/static/images/back_enabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/back_enabled_hover.png` & `clld-9.2.2/src/clld/web/static/images/back_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc-nd-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc-nd-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc-nd.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc-nd.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc-sa-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc-sa-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc-sa.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nc.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nc.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nd-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nd-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-nd.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-nd.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-sa-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-sa-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-sa.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-sa.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-by-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-by.png` & `clld-9.2.2/src/clld/web/static/images/cc-by.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-zero-small.png` & `clld-9.2.2/src/clld/web/static/images/cc-zero-small.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/cc-zero.png` & `clld-9.2.2/src/clld/web/static/images/cc-zero.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/concepticon.png` & `clld-9.2.2/src/clld/web/static/images/concepticon.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/doi_logo.png` & `clld-9.2.2/src/clld/web/static/images/doi_logo.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/forward_disabled.png` & `clld-9.2.2/src/clld/web/static/images/forward_disabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/forward_enabled.png` & `clld-9.2.2/src/clld/web/static/images/forward_enabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/forward_enabled_hover.png` & `clld-9.2.2/src/clld/web/static/images/forward_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/glottolog.png` & `clld-9.2.2/src/clld/web/static/images/glottolog.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/glottolog_white.png` & `clld-9.2.2/src/clld/web/static/images/glottolog_white.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/minerva.png` & `clld-9.2.2/src/clld/web/static/images/minerva.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/pdf-icon.gif` & `clld-9.2.2/src/clld/web/static/images/pdf-icon.gif`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/sort_asc.png` & `clld-9.2.2/src/clld/web/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/sort_asc_disabled.png` & `clld-9.2.2/src/clld/web/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/sort_both.png` & `clld-9.2.2/src/clld/web/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/sort_desc.png` & `clld-9.2.2/src/clld/web/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/images/sort_desc_disabled.png` & `clld-9.2.2/src/clld/web/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/img/glyphicons-halflings-white.png` & `clld-9.2.2/src/clld/web/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/img/glyphicons-halflings.png` & `clld-9.2.2/src/clld/web/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/L.Control.Resizer.js` & `clld-9.2.2/src/clld/web/static/js/L.Control.Resizer.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/Leaflet.fullscreen.js` & `clld-9.2.2/src/clld/web/static/js/Leaflet.fullscreen.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/bootstrap-slider.js` & `clld-9.2.2/src/clld/web/static/js/bootstrap-slider.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/bootstrap.js` & `clld-9.2.2/src/clld/web/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/bootstrap.min.js` & `clld-9.2.2/src/clld/web/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/bootstrapx-clickover.js` & `clld-9.2.2/src/clld/web/static/js/bootstrapx-clickover.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/clld.js` & `clld-9.2.2/src/clld/web/static/js/clld.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -414,22 +414,17 @@
         overlays = {},
         baseLayers = [
             "OpenStreetMap.Mapnik",
             "OpenTopoMap",
             "Stamen.Watercolor",
             "Stamen.Terrain",
             "Stamen.TerrainBackground",
-            "Esri.WorldStreetMap",
-            "Esri.DeLorme",
-            "Esri.NatGeoWorldMap",
-            "Esri.WorldTopoMap",
-            "Esri.WorldImagery",
-            "Esri.WorldTerrain",
-            "Esri.WorldShadedRelief",
-            "Esri.WorldPhysical"
+            "USGS.USTopo",
+            "USGS.USImagery",
+            "USGS.USImageryTopo",
         ];
     CLLD.Maps[eid] = this;
     options = options === undefined ? {} : options;
 
     this.options = {};
     this.options.info_route = options.info_route === undefined ? 'language_alt' : options.info_route;
     this.options.info_query = options.info_query === undefined ? {} : options.info_query;
```

### Comparing `clld-9.2.1/src/clld/web/static/js/intro.min.js` & `clld-9.2.2/src/clld/web/static/js/intro.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/jquery.dataTables.js` & `clld-9.2.2/src/clld/web/static/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/jquery.dataTables.min.js` & `clld-9.2.2/src/clld/web/static/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/jquery.js` & `clld-9.2.2/src/clld/web/static/js/jquery.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/jsphylosvg.min.js` & `clld-9.2.2/src/clld/web/static/js/jsphylosvg.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/leaflet-hash.js` & `clld-9.2.2/src/clld/web/static/js/leaflet-hash.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/leaflet-providers.js` & `clld-9.2.2/src/clld/web/static/js/leaflet-providers.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -100,15 +100,15 @@
                         ]
                     }
                 },
                 France: {
                     url: 'https://{s}.tile.openstreetmap.fr/osmfr/{z}/{x}/{y}.png',
                     options: {
                         maxZoom: 20,
-                        attribution: '&copy; Openstreetmap France | {attribution.OpenStreetMap}'
+                        attribution: '&copy; OpenStreetMap France | {attribution.OpenStreetMap}'
                     }
                 },
                 HOT: {
                     url: 'https://{s}.tile.openstreetmap.fr/hot/{z}/{x}/{y}.png',
                     options: {
                         attribution: '{attribution.OpenStreetMap}, ' +
                             'Tiles style by <a href="https://www.hotosm.org/" target="_blank">Humanitarian OpenStreetMap Team</a> ' +
@@ -129,19 +129,19 @@
         },
         OpenSeaMap: {
             url: 'https://tiles.openseamap.org/seamark/{z}/{x}/{y}.png',
             options: {
                 attribution: 'Map data: &copy; <a href="http://www.openseamap.org">OpenSeaMap</a> contributors'
             }
         },
-        OpenPtMap: {
-            url: 'http://openptmap.org/tiles/{z}/{x}/{y}.png',
+        OPNVKarte: {
+            url: 'https://tileserver.memomaps.de/tilegen/{z}/{x}/{y}.png',
             options: {
-                maxZoom: 17,
-                attribution: 'Map data: &copy; <a href="http://www.openptmap.org">OpenPtMap</a> contributors'
+                maxZoom: 18,
+                attribution: 'Map <a href="https://memomaps.de/">memomaps.de</a> <a href="http://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, map data {attribution.OpenStreetMap}'
             }
         },
         OpenTopoMap: {
             url: 'https://{s}.tile.opentopomap.org/{z}/{x}/{y}.png',
             options: {
                 maxZoom: 17,
                 attribution: 'Map data: {attribution.OpenStreetMap}, <a href="http://viewfinderpanoramas.org">SRTM</a> | Map style: &copy; <a href="https://opentopomap.org">OpenTopoMap</a> (<a href="https://creativecommons.org/licenses/by-sa/3.0/">CC-BY-SA</a>)'
@@ -739,15 +739,15 @@
             }
         },
         CartoDB: {
             url: 'https://{s}.basemaps.cartocdn.com/{variant}/{z}/{x}/{y}{r}.png',
             options: {
                 attribution: '{attribution.OpenStreetMap} &copy; <a href="https://carto.com/attributions">CARTO</a>',
                 subdomains: 'abcd',
-                maxZoom: 19,
+                maxZoom: 20,
                 variant: 'light_all'
             },
             variants: {
                 Positron: 'light_all',
                 PositronNoLabels: 'light_nolabels',
                 PositronOnlyLabels: 'light_only_labels',
                 DarkMatter: 'dark_all',
@@ -833,22 +833,22 @@
             options: {
                 minZoom: 6,
                 maxZoom: 19,
                 bounds: [
                     [50.5, 3.25],
                     [54, 7.6]
                 ],
-                attribution: 'Kaartgegevens &copy; <a href="kadaster.nl">Kadaster</a>'
+                attribution: 'Kaartgegevens &copy; <a href="https://www.kadaster.nl">Kadaster</a>'
             },
             variants: {
                 'standaard': 'brtachtergrondkaart',
                 'pastel': 'brtachtergrondkaartpastel',
                 'grijs': 'brtachtergrondkaartgrijs',
                 'luchtfoto': {
-                    'url': 'https://geodata.nationaalgeoregister.nl/luchtfoto/rgb/wmts/2018_ortho25/EPSG:3857/{z}/{x}/{y}.png',
+                    'url': 'https://service.pdok.nl/hwh/luchtfotorgb/wmts/v1_0/Actueel_ortho25/EPSG:3857/{z}/{x}/{y}.jpeg',
                 }
             }
         },
         NASAGIBS: {
             url: 'https://map1.vis.earthdata.nasa.gov/wmts-webmerc/{variant}/default/{time}/{tilematrixset}{maxZoom}/{z}/{y}/{x}.{format}',
             options: {
                 attribution: 'Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System ' +
@@ -878,15 +878,15 @@
                         format: 'png',
                         maxZoom: 7,
                         opacity: 0.75
                     }
                 },
                 ModisTerraSnowCover: {
                     options: {
-                        variant: 'MODIS_Terra_Snow_Cover',
+                        variant: 'MODIS_Terra_NDSI_Snow_Cover',
                         format: 'png',
                         maxZoom: 8,
                         opacity: 0.75
                     }
                 },
                 ModisTerraAOD: {
                     options: {
@@ -927,15 +927,15 @@
                 subdomains: '0123',
             }
         },
         JusticeMap: {
             // Justice Map (http://www.justicemap.org/)
             // Visualize race and income data for your community, county and country.
             // Includes tools for data journalists, bloggers and community activists.
-            url: 'http://www.justicemap.org/tile/{size}/{variant}/{z}/{x}/{y}.png',
+            url: 'https://www.justicemap.org/tile/{size}/{variant}/{z}/{x}/{y}.png',
             options: {
                 attribution: '<a href="http://www.justicemap.org/terms.php">Justice Map</a>',
                 // one of 'county', 'tract', 'block'
                 size: 'county',
                 // Bounds for USA, including Alaska and Hawaii
                 bounds: [
                     [14, -180],
@@ -950,53 +950,44 @@
                 hispanic: 'hispanic',
                 multi: 'multi',
                 nonWhite: 'nonwhite',
                 white: 'white',
                 plurality: 'plural'
             }
         },
-        Wikimedia: {
-            url: 'https://maps.wikimedia.org/osm-intl/{z}/{x}/{y}{r}.png',
-            options: {
-                attribution: '<a href="https://wikimediafoundation.org/wiki/Maps_Terms_of_Use">Wikimedia</a>',
-                minZoom: 1,
-                maxZoom: 19
-            }
-        },
         GeoportailFrance: {
             url: 'https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET=PM&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}',
             options: {
                 attribution: '<a target="_blank" href="https://www.geoportail.gouv.fr/">Geoportail France</a>',
                 bounds: [
                     [-75, -180],
                     [81, 180]
                 ],
                 minZoom: 2,
                 maxZoom: 18,
                 // Get your own geoportail apikey here : http://professionnels.ign.fr/ign/contrats/
                 // NB : 'choisirgeoportail' is a demonstration key that comes with no guarantee
                 apikey: 'choisirgeoportail',
-                format: 'image/jpeg',
+                format: 'image/png',
                 style: 'normal',
-                variant: 'GEOGRAPHICALGRIDSYSTEMS.MAPS.SCAN-EXPRESS.STANDARD'
+                variant: 'GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2'
             },
             variants: {
+                plan: 'GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2',
                 parcels: {
                     options: {
-                        variant: 'CADASTRALPARCELS.PARCELS',
-                        maxZoom: 20,
-                        style: 'bdparcellaire',
-                        format: 'image/png'
+                        variant: 'CADASTRALPARCELS.PARCELLAIRE_EXPRESS',
+                        style: 'PCI vecteur',
+                        maxZoom: 20
                     }
                 },
-                ignMaps: 'GEOGRAPHICALGRIDSYSTEMS.MAPS',
-                maps: 'GEOGRAPHICALGRIDSYSTEMS.MAPS.SCAN-EXPRESS.STANDARD',
                 orthos: {
                     options: {
                         maxZoom: 19,
+                        format: 'image/jpeg',
                         variant: 'ORTHOIMAGERY.ORTHOPHOTOS'
                     }
                 }
             }
         },
         OneMapSG: {
             url: 'https://maps-{s}.onemap.sg/v3/{variant}/{z}/{x}/{y}.png',
@@ -1013,14 +1004,109 @@
             variants: {
                 Default: 'Default',
                 Night: 'Night',
                 Original: 'Original',
                 Grey: 'Grey',
                 LandLot: 'LandLot'
             }
+        },
+        USGS: {
+            url: 'https://basemap.nationalmap.gov/arcgis/rest/services/USGSTopo/MapServer/tile/{z}/{y}/{x}',
+            options: {
+                maxZoom: 20,
+                attribution: 'Tiles courtesy of the <a href="https://usgs.gov/">U.S. Geological Survey</a>'
+            },
+            variants: {
+                USTopo: {},
+                USImagery: {
+                    url: 'https://basemap.nationalmap.gov/arcgis/rest/services/USGSImageryOnly/MapServer/tile/{z}/{y}/{x}'
+                },
+                USImageryTopo: {
+                    url: 'https://basemap.nationalmap.gov/arcgis/rest/services/USGSImageryTopo/MapServer/tile/{z}/{y}/{x}'
+                }
+            }
+        },
+        WaymarkedTrails: {
+            url: 'https://tile.waymarkedtrails.org/{variant}/{z}/{x}/{y}.png',
+            options: {
+                maxZoom: 18,
+                attribution: 'Map data: {attribution.OpenStreetMap} | Map style: &copy; <a href="https://waymarkedtrails.org">waymarkedtrails.org</a> (<a href="https://creativecommons.org/licenses/by-sa/3.0/">CC-BY-SA</a>)'
+            },
+            variants: {
+                hiking: 'hiking',
+                cycling: 'cycling',
+                mtb: 'mtb',
+                slopes: 'slopes',
+                riding: 'riding',
+                skating: 'skating'
+            }
+        },
+        OpenAIP: {
+            url: 'https://{s}.tile.maps.openaip.net/geowebcache/service/tms/1.0.0/openaip_basemap@EPSG%3A900913@png/{z}/{x}/{y}.{ext}',
+            options: {
+                attribution: '<a href="https://www.openaip.net/">openAIP Data</a> (<a href="https://creativecommons.org/licenses/by-sa/3.0/">CC-BY-NC-SA</a>)',
+                ext: 'png',
+                minZoom: 4,
+                maxZoom: 14,
+                tms: true,
+                detectRetina: true,
+                subdomains: '12'
+            }
+        },
+        OpenSnowMap: {
+            url: 'https://tiles.opensnowmap.org/{variant}/{z}/{x}/{y}.png',
+            options: {
+                minZoom: 9,
+                maxZoom: 18,
+                attribution: 'Map data: {attribution.OpenStreetMap} & ODbL, &copy; <a href="https://www.opensnowmap.org/iframes/data.html">www.opensnowmap.org</a> <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>'
+            },
+            variants: {
+                pistes: 'pistes',
+            }
+        },
+        AzureMaps: {
+            url: 'https://atlas.microsoft.com/map/tile?api-version={apiVersion}' +
+                '&tilesetId={variant}&x={x}&y={y}&zoom={z}&language={language}' +
+                '&subscription-key={subscriptionKey}',
+            options: {
+                attribution: 'See https://docs.microsoft.com/en-US/rest/api/maps/renderv2/getmaptilepreview for details.',
+                apiVersion: '2.0',
+                variant: 'microsoft.imagery',
+                subscriptionKey: '<insert your subscription key here>',
+                language: 'en-US',
+            },
+            variants: {
+                MicrosoftImagery: 'microsoft.imagery',
+                MicrosoftBaseDarkGrey: 'microsoft.base.darkgrey',
+                MicrosoftBaseRoad: 'microsoft.base.road',
+                MicrosoftBaseHybridRoad: 'microsoft.base.hybrid.road',
+                MicrosoftTerraMain: 'microsoft.terra.main',
+                MicrosoftWeatherInfraredMain: {
+                    url: 'https://atlas.microsoft.com/map/tile?api-version={apiVersion}' +
+                        '&tilesetId={variant}&x={x}&y={y}&zoom={z}' +
+                        '&timeStamp={timeStamp}&language={language}' +
+                        '&subscription-key={subscriptionKey}',
+                    options: {
+                        timeStamp: '2021-05-08T09:03:00Z',
+                        attribution: 'See https://docs.microsoft.com/en-US/rest/api/maps/renderv2/getmaptilepreview#uri-parameters for details.',
+                        variant: 'microsoft.weather.infrared.main',
+                    },
+                },
+                MicrosoftWeatherRadarMain: {
+                    url: 'https://atlas.microsoft.com/map/tile?api-version={apiVersion}' +
+                        '&tilesetId={variant}&x={x}&y={y}&zoom={z}' +
+                        '&timeStamp={timeStamp}&language={language}' +
+                        '&subscription-key={subscriptionKey}',
+                    options: {
+                        timeStamp: '2021-05-08T09:03:00Z',
+                        attribution: 'See https://docs.microsoft.com/en-US/rest/api/maps/renderv2/getmaptilepreview#uri-parameters for details.',
+                        variant: 'microsoft.weather.radar.main',
+                    },
+                }
+            },
         }
     };
 
     L.tileLayer.provider = function(provider, options) {
         return new L.TileLayer.Provider(provider, options);
     };
```

### Comparing `clld-9.2.1/src/clld/web/static/js/leaflet-src.js` & `clld-9.2.2/src/clld/web/static/js/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/leaflet.js` & `clld-9.2.2/src/clld/web/static/js/leaflet.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,340 +1,335 @@
 /* @preserve
- * Leaflet 1.8.0, a JS library for interactive maps. https://leafletjs.com
+ * Leaflet 1.9.1, a JS library for interactive maps. https://leafletjs.com
  * (c) 2010-2022 Vladimir Agafonkin, (c) 2010-2011 CloudMade
  */
-! function(t, i) {
-    "object" == typeof exports && "undefined" != typeof module ? i(exports) : "function" == typeof define && define.amd ? define(["exports"], i) : i((t = "undefined" != typeof globalThis ? globalThis : t || self).leaflet = {})
+! function(t, e) {
+    "object" == typeof exports && "undefined" != typeof module ? e(exports) : "function" == typeof define && define.amd ? define(["exports"], e) : e((t = "undefined" != typeof globalThis ? globalThis : t || self).leaflet = {})
 }(this, function(t) {
     "use strict";
+    var R = "1.9.1";
 
     function l(t) {
-        for (var i, e, n = 1, o = arguments.length; n < o; n++)
-            for (i in e = arguments[n]) t[i] = e[i];
+        for (var e, i, n = 1, o = arguments.length; n < o; n++)
+            for (e in i = arguments[n]) t[e] = i[e];
         return t
     }
-    var R = Object.create || function(t) {
-        return N.prototype = t, new N
+    var N = Object.create || function(t) {
+        return D.prototype = t, new D
     };
 
-    function N() {}
+    function D() {}
 
-    function a(t, i) {
-        var e = Array.prototype.slice;
-        if (t.bind) return t.bind.apply(t, e.call(arguments, 1));
-        var n = e.call(arguments, 2);
-        return function() {
-            return t.apply(i, n.length ? n.concat(e.call(arguments)) : arguments)
-        }
+    function a(t, e) {
+        var i, n = Array.prototype.slice;
+        return t.bind ? t.bind.apply(t, n.call(arguments, 1)) : (i = n.call(arguments, 2), function() {
+            return t.apply(e, i.length ? i.concat(n.call(arguments)) : arguments)
+        })
     }
-    var D = 0;
+    var j = 0;
 
     function h(t) {
-        return "_leaflet_id" in t || (t._leaflet_id = ++D), t._leaflet_id
+        return "_leaflet_id" in t || (t._leaflet_id = ++j), t._leaflet_id
     }
 
-    function j(t, i, e) {
+    function H(t, e, i) {
         var n, o, s = function() {
-                n = !1, o && (r.apply(e, o), o = !1)
+                n = !1, o && (r.apply(i, o), o = !1)
             },
             r = function() {
-                n ? o = arguments : (t.apply(e, arguments), setTimeout(s, i), n = !0)
+                n ? o = arguments : (t.apply(i, arguments), setTimeout(s, e), n = !0)
             };
         return r
     }
 
-    function H(t, i, e) {
-        var n = i[1],
-            i = i[0],
-            o = n - i;
-        return t === n && e ? t : ((t - i) % o + o) % o + i
+    function F(t, e, i) {
+        var n = e[1],
+            e = e[0],
+            o = n - e;
+        return t === n && i ? t : ((t - e) % o + o) % o + e
     }
 
     function u() {
         return !1
     }
 
-    function e(t, i) {
-        if (!1 === i) return t;
-        i = Math.pow(10, void 0 === i ? 6 : i);
-        return Math.round(t * i) / i
+    function i(t, e) {
+        return !1 === e ? t : (e = Math.pow(10, void 0 === e ? 6 : e), Math.round(t * e) / e)
     }
 
     function W(t) {
         return t.trim ? t.trim() : t.replace(/^\s+|\s+$/g, "")
     }
 
-    function F(t) {
+    function U(t) {
         return W(t).split(/\s+/)
     }
 
-    function c(t, i) {
-        for (var e in Object.prototype.hasOwnProperty.call(t, "options") || (t.options = t.options ? R(t.options) : {}), i) t.options[e] = i[e];
+    function c(t, e) {
+        for (var i in Object.prototype.hasOwnProperty.call(t, "options") || (t.options = t.options ? N(t.options) : {}), e) t.options[i] = e[i];
         return t.options
     }
 
-    function U(t, i, e) {
+    function V(t, e, i) {
         var n, o = [];
-        for (n in t) o.push(encodeURIComponent(e ? n.toUpperCase() : n) + "=" + encodeURIComponent(t[n]));
-        return (i && -1 !== i.indexOf("?") ? "&" : "?") + o.join("&")
+        for (n in t) o.push(encodeURIComponent(i ? n.toUpperCase() : n) + "=" + encodeURIComponent(t[n]));
+        return (e && -1 !== e.indexOf("?") ? "&" : "?") + o.join("&")
     }
-    var V = /\{ *([\w_ -]+) *\}/g;
+    var G = /\{ *([\w_ -]+) *\}/g;
 
-    function q(t, e) {
-        return t.replace(V, function(t, i) {
-            i = e[i];
-            if (void 0 === i) throw new Error("No value provided for variable " + t);
-            return i = "function" == typeof i ? i(e) : i
+    function q(t, i) {
+        return t.replace(G, function(t, e) {
+            e = i[e];
+            if (void 0 === e) throw new Error("No value provided for variable " + t);
+            return e = "function" == typeof e ? e(i) : e
         })
     }
     var d = Array.isArray || function(t) {
         return "[object Array]" === Object.prototype.toString.call(t)
     };
 
-    function G(t, i) {
-        for (var e = 0; e < t.length; e++)
-            if (t[e] === i) return e;
+    function K(t, e) {
+        for (var i = 0; i < t.length; i++)
+            if (t[i] === e) return i;
         return -1
     }
-    var K = "data:image/gif;base64,R0lGODlhAQABAAD/ACwAAAAAAQABAAACADs=";
+    var Y = "data:image/gif;base64,R0lGODlhAQABAAD/ACwAAAAAAQABAAACADs=";
 
-    function Y(t) {
+    function J(t) {
         return window["webkit" + t] || window["moz" + t] || window["ms" + t]
     }
     var X = 0;
 
-    function J(t) {
-        var i = +new Date,
-            e = Math.max(0, 16 - (i - X));
-        return X = i + e, window.setTimeout(t, e)
+    function $(t) {
+        var e = +new Date,
+            i = Math.max(0, 16 - (e - X));
+        return X = e + i, window.setTimeout(t, i)
     }
-    var $ = window.requestAnimationFrame || Y("RequestAnimationFrame") || J,
-        Q = window.cancelAnimationFrame || Y("CancelAnimationFrame") || Y("CancelRequestAnimationFrame") || function(t) {
+    var Q = window.requestAnimationFrame || J("RequestAnimationFrame") || $,
+        tt = window.cancelAnimationFrame || J("CancelAnimationFrame") || J("CancelRequestAnimationFrame") || function(t) {
             window.clearTimeout(t)
         };
 
-    function x(t, i, e) {
-        if (!e || $ !== J) return $.call(window, a(t, i));
-        t.call(i)
+    function x(t, e, i) {
+        if (!i || Q !== $) return Q.call(window, a(t, e));
+        t.call(e)
     }
 
     function r(t) {
-        t && Q.call(window, t)
+        t && tt.call(window, t)
     }
-    var tt = {
+    var et = {
         __proto__: null,
         extend: l,
-        create: R,
+        create: N,
         bind: a,
         get lastId() {
-            return D
+            return j
         },
         stamp: h,
-        throttle: j,
-        wrapNum: H,
+        throttle: H,
+        wrapNum: F,
         falseFn: u,
-        formatNum: e,
+        formatNum: i,
         trim: W,
-        splitWords: F,
+        splitWords: U,
         setOptions: c,
-        getParamString: U,
+        getParamString: V,
         template: q,
         isArray: d,
-        indexOf: G,
-        emptyImageUrl: K,
-        requestFn: $,
-        cancelFn: Q,
+        indexOf: K,
+        emptyImageUrl: Y,
+        requestFn: Q,
+        cancelFn: tt,
         requestAnimFrame: x,
         cancelAnimFrame: r
     };
 
-    function it() {}
-    it.extend = function(t) {
-        function i() {
+    function e() {}
+    e.extend = function(t) {
+        function e() {
             c(this), this.initialize && this.initialize.apply(this, arguments), this.callInitHooks()
         }
-        var e, n = i.__super__ = this.prototype,
-            o = R(n);
-        for (e in (o.constructor = i).prototype = o, this) Object.prototype.hasOwnProperty.call(this, e) && "prototype" !== e && "__super__" !== e && (i[e] = this[e]);
-        if (t.statics && l(i, t.statics), t.includes) {
+        var i, n = e.__super__ = this.prototype,
+            o = N(n);
+        for (i in (o.constructor = e).prototype = o, this) Object.prototype.hasOwnProperty.call(this, i) && "prototype" !== i && "__super__" !== i && (e[i] = this[i]);
+        if (t.statics && l(e, t.statics), t.includes) {
             var s = t.includes;
             if ("undefined" != typeof L && L && L.Mixin) {
                 s = d(s) ? s : [s];
                 for (var r = 0; r < s.length; r++) s[r] === L.Mixin.Events && console.warn("Deprecated include of L.Mixin.Events: this property will be removed in future releases, please inherit from L.Evented instead.", (new Error).stack)
             }
             l.apply(null, [o].concat(t.includes))
         }
-        return l(o, t), delete o.statics, delete o.includes, o.options && (o.options = n.options ? R(n.options) : {}, l(o.options, t.options)), o._initHooks = [], o.callInitHooks = function() {
+        return l(o, t), delete o.statics, delete o.includes, o.options && (o.options = n.options ? N(n.options) : {}, l(o.options, t.options)), o._initHooks = [], o.callInitHooks = function() {
             if (!this._initHooksCalled) {
                 n.callInitHooks && n.callInitHooks.call(this), this._initHooksCalled = !0;
-                for (var t = 0, i = o._initHooks.length; t < i; t++) o._initHooks[t].call(this)
+                for (var t = 0, e = o._initHooks.length; t < e; t++) o._initHooks[t].call(this)
             }
-        }, i
-    }, it.include = function(t) {
-        var i = this.prototype.options;
-        return l(this.prototype, t), t.options && (this.prototype.options = i, this.mergeOptions(t.options)), this
-    }, it.mergeOptions = function(t) {
+        }, e
+    }, e.include = function(t) {
+        var e = this.prototype.options;
+        return l(this.prototype, t), t.options && (this.prototype.options = e, this.mergeOptions(t.options)), this
+    }, e.mergeOptions = function(t) {
         return l(this.prototype.options, t), this
-    }, it.addInitHook = function(t) {
-        var i = Array.prototype.slice.call(arguments, 1),
-            e = "function" == typeof t ? t : function() {
-                this[t].apply(this, i)
+    }, e.addInitHook = function(t) {
+        var e = Array.prototype.slice.call(arguments, 1),
+            i = "function" == typeof t ? t : function() {
+                this[t].apply(this, e)
             };
-        return this.prototype._initHooks = this.prototype._initHooks || [], this.prototype._initHooks.push(e), this
+        return this.prototype._initHooks = this.prototype._initHooks || [], this.prototype._initHooks.push(i), this
     };
-    var i = {
-            on: function(t, i, e) {
+    var n = {
+            on: function(t, e, i) {
                 if ("object" == typeof t)
-                    for (var n in t) this._on(n, t[n], i);
+                    for (var n in t) this._on(n, t[n], e);
                 else
-                    for (var o = 0, s = (t = F(t)).length; o < s; o++) this._on(t[o], i, e);
+                    for (var o = 0, s = (t = U(t)).length; o < s; o++) this._on(t[o], e, i);
                 return this
             },
-            off: function(t, i, e) {
+            off: function(t, e, i) {
                 if (arguments.length)
                     if ("object" == typeof t)
-                        for (var n in t) this._off(n, t[n], i);
+                        for (var n in t) this._off(n, t[n], e);
                     else {
-                        t = F(t);
-                        for (var o = 1 === arguments.length, s = 0, r = t.length; s < r; s++) o ? this._off(t[s]) : this._off(t[s], i, e)
+                        t = U(t);
+                        for (var o = 1 === arguments.length, s = 0, r = t.length; s < r; s++) o ? this._off(t[s]) : this._off(t[s], e, i)
                     }
                 else delete this._events;
                 return this
             },
-            _on: function(t, i, e) {
-                if ("function" != typeof i) console.warn("wrong listener type: " + typeof i);
-                else {
-                    this._events = this._events || {};
-                    for (var n = this._events[t], t = (n || (this._events[t] = n = []), {
-                            fn: i,
-                            ctx: e = e === this ? void 0 : e
-                        }), o = n, s = 0, r = o.length; s < r; s++)
-                        if (o[s].fn === i && o[s].ctx === e) return;
-                    o.push(t)
-                }
+            _on: function(t, e, i, n) {
+                "function" != typeof e ? console.warn("wrong listener type: " + typeof e) : !1 === this._listens(t, e, i) && (e = {
+                    fn: e,
+                    ctx: i = i === this ? void 0 : i
+                }, n && (e.once = !0), this._events = this._events || {}, this._events[t] = this._events[t] || [], this._events[t].push(e))
             },
-            _off: function(t, i, e) {
+            _off: function(t, e, i) {
                 var n, o, s;
                 if (this._events && (n = this._events[t]))
                     if (1 === arguments.length) {
                         if (this._firingCount)
                             for (o = 0, s = n.length; o < s; o++) n[o].fn = u;
                         delete this._events[t]
-                    } else if (e === this && (e = void 0), "function" != typeof i) console.warn("wrong listener type: " + typeof i);
-                else {
-                    for (o = 0, s = n.length; o < s; o++) {
-                        var r = n[o];
-                        if (r.ctx === e && r.fn === i) return this._firingCount && (r.fn = u, this._events[t] = n = n.slice()), void n.splice(o, 1)
-                    }
-                    console.warn("listener not found")
-                }
+                    } else "function" != typeof e ? console.warn("wrong listener type: " + typeof e) : !1 !== (e = this._listens(t, e, i)) && (i = n[e], this._firingCount && (i.fn = u, this._events[t] = n = n.slice()), n.splice(e, 1))
             },
-            fire: function(t, i, e) {
-                if (!this.listens(t, e)) return this;
-                var n = l({}, i, {
-                    type: t,
-                    target: this,
-                    sourceTarget: i && i.sourceTarget || this
-                });
-                if (this._events) {
-                    var o = this._events[t];
-                    if (o) {
-                        this._firingCount = this._firingCount + 1 || 1;
-                        for (var s = 0, r = o.length; s < r; s++) {
-                            var a = o[s];
-                            a.fn.call(a.ctx || this, n)
+            fire: function(t, e, i) {
+                if (this.listens(t, i)) {
+                    var n = l({}, e, {
+                        type: t,
+                        target: this,
+                        sourceTarget: e && e.sourceTarget || this
+                    });
+                    if (this._events) {
+                        var o = this._events[t];
+                        if (o) {
+                            this._firingCount = this._firingCount + 1 || 1;
+                            for (var s = 0, r = o.length; s < r; s++) {
+                                var a = o[s],
+                                    h = a.fn;
+                                a.once && this.off(t, h, a.ctx), h.call(a.ctx || this, n)
+                            }
+                            this._firingCount--
                         }
-                        this._firingCount--
                     }
+                    i && this._propagateEvent(n)
                 }
-                return e && this._propagateEvent(n), this
+                return this
             },
-            listens: function(t, i) {
+            listens: function(t, e, i, n) {
                 "string" != typeof t && console.warn('"string" type argument expected');
-                var e = this._events && this._events[t];
-                if (e && e.length) return !0;
-                if (i)
-                    for (var n in this._eventParents)
-                        if (this._eventParents[n].listens(t, i)) return !0;
+                var o = e,
+                    s = ("function" != typeof e && (n = !!e, i = o = void 0), this._events && this._events[t]);
+                if (s && s.length && !1 !== this._listens(t, o, i)) return !0;
+                if (n)
+                    for (var r in this._eventParents)
+                        if (this._eventParents[r].listens(t, e, i, n)) return !0;
                 return !1
             },
-            once: function(t, i, e) {
-                if ("object" == typeof t) {
-                    for (var n in t) this.once(n, t[n], i);
-                    return this
+            _listens: function(t, e, i) {
+                if (this._events) {
+                    var n = this._events[t] || [];
+                    if (!e) return !!n.length;
+                    i === this && (i = void 0);
+                    for (var o = 0, s = n.length; o < s; o++)
+                        if (n[o].fn === e && n[o].ctx === i) return o
                 }
-                var o = a(function() {
-                    this.off(t, i, e).off(t, o, e)
-                }, this);
-                return this.on(t, i, e).on(t, o, e)
+                return !1
+            },
+            once: function(t, e, i) {
+                if ("object" == typeof t)
+                    for (var n in t) this._on(n, t[n], e, !0);
+                else
+                    for (var o = 0, s = (t = U(t)).length; o < s; o++) this._on(t[o], e, i, !0);
+                return this
             },
             addEventParent: function(t) {
                 return this._eventParents = this._eventParents || {}, this._eventParents[h(t)] = t, this
             },
             removeEventParent: function(t) {
                 return this._eventParents && delete this._eventParents[h(t)], this
             },
             _propagateEvent: function(t) {
-                for (var i in this._eventParents) this._eventParents[i].fire(t.type, l({
+                for (var e in this._eventParents) this._eventParents[e].fire(t.type, l({
                     layer: t.target,
                     propagatedFrom: t.target
                 }, t), !0)
             }
         },
-        et = (i.addEventListener = i.on, i.removeEventListener = i.clearAllEventListeners = i.off, i.addOneTimeEventListener = i.once, i.fireEvent = i.fire, i.hasEventListeners = i.listens, it.extend(i));
+        it = (n.addEventListener = n.on, n.removeEventListener = n.clearAllEventListeners = n.off, n.addOneTimeEventListener = n.once, n.fireEvent = n.fire, n.hasEventListeners = n.listens, e.extend(n));
 
-    function p(t, i, e) {
-        this.x = e ? Math.round(t) : t, this.y = e ? Math.round(i) : i
+    function p(t, e, i) {
+        this.x = i ? Math.round(t) : t, this.y = i ? Math.round(e) : e
     }
     var nt = Math.trunc || function(t) {
         return 0 < t ? Math.floor(t) : Math.ceil(t)
     };
 
-    function _(t, i, e) {
-        return t instanceof p ? t : d(t) ? new p(t[0], t[1]) : null == t ? t : "object" == typeof t && "x" in t && "y" in t ? new p(t.x, t.y) : new p(t, i, e)
+    function m(t, e, i) {
+        return t instanceof p ? t : d(t) ? new p(t[0], t[1]) : null == t ? t : "object" == typeof t && "x" in t && "y" in t ? new p(t.x, t.y) : new p(t, e, i)
     }
 
-    function m(t, i) {
+    function f(t, e) {
         if (t)
-            for (var e = i ? [t, i] : t, n = 0, o = e.length; n < o; n++) this.extend(e[n])
+            for (var i = e ? [t, e] : t, n = 0, o = i.length; n < o; n++) this.extend(i[n])
     }
 
-    function f(t, i) {
-        return !t || t instanceof m ? t : new m(t, i)
+    function _(t, e) {
+        return !t || t instanceof f ? t : new f(t, e)
     }
 
-    function s(t, i) {
+    function s(t, e) {
         if (t)
-            for (var e = i ? [t, i] : t, n = 0, o = e.length; n < o; n++) this.extend(e[n])
+            for (var i = e ? [t, e] : t, n = 0, o = i.length; n < o; n++) this.extend(i[n])
     }
 
-    function g(t, i) {
-        return t instanceof s ? t : new s(t, i)
+    function g(t, e) {
+        return t instanceof s ? t : new s(t, e)
     }
 
-    function v(t, i, e) {
-        if (isNaN(t) || isNaN(i)) throw new Error("Invalid LatLng object: (" + t + ", " + i + ")");
-        this.lat = +t, this.lng = +i, void 0 !== e && (this.alt = +e)
+    function v(t, e, i) {
+        if (isNaN(t) || isNaN(e)) throw new Error("Invalid LatLng object: (" + t + ", " + e + ")");
+        this.lat = +t, this.lng = +e, void 0 !== i && (this.alt = +i)
     }
 
-    function w(t, i, e) {
-        return t instanceof v ? t : d(t) && "object" != typeof t[0] ? 3 === t.length ? new v(t[0], t[1], t[2]) : 2 === t.length ? new v(t[0], t[1]) : null : null == t ? t : "object" == typeof t && "lat" in t ? new v(t.lat, "lng" in t ? t.lng : t.lon, t.alt) : void 0 === i ? null : new v(t, i, e)
+    function w(t, e, i) {
+        return t instanceof v ? t : d(t) && "object" != typeof t[0] ? 3 === t.length ? new v(t[0], t[1], t[2]) : 2 === t.length ? new v(t[0], t[1]) : null : null == t ? t : "object" == typeof t && "lat" in t ? new v(t.lat, "lng" in t ? t.lng : t.lon, t.alt) : void 0 === e ? null : new v(t, e, i)
     }
     p.prototype = {
         clone: function() {
             return new p(this.x, this.y)
         },
         add: function(t) {
-            return this.clone()._add(_(t))
+            return this.clone()._add(m(t))
         },
         _add: function(t) {
             return this.x += t.x, this.y += t.y, this
         },
         subtract: function(t) {
-            return this.clone()._subtract(_(t))
+            return this.clone()._subtract(m(t))
         },
         _subtract: function(t) {
             return this.x -= t.x, this.y -= t.y, this
         },
         divideBy: function(t) {
             return this.clone()._divideBy(t)
         },
@@ -374,93 +369,109 @@
         trunc: function() {
             return this.clone()._trunc()
         },
         _trunc: function() {
             return this.x = nt(this.x), this.y = nt(this.y), this
         },
         distanceTo: function(t) {
-            var i = (t = _(t)).x - this.x,
+            var e = (t = m(t)).x - this.x,
                 t = t.y - this.y;
-            return Math.sqrt(i * i + t * t)
+            return Math.sqrt(e * e + t * t)
         },
         equals: function(t) {
-            return (t = _(t)).x === this.x && t.y === this.y
+            return (t = m(t)).x === this.x && t.y === this.y
         },
         contains: function(t) {
-            return t = _(t), Math.abs(t.x) <= Math.abs(this.x) && Math.abs(t.y) <= Math.abs(this.y)
+            return t = m(t), Math.abs(t.x) <= Math.abs(this.x) && Math.abs(t.y) <= Math.abs(this.y)
         },
         toString: function() {
-            return "Point(" + e(this.x) + ", " + e(this.y) + ")"
+            return "Point(" + i(this.x) + ", " + i(this.y) + ")"
         }
-    }, m.prototype = {
+    }, f.prototype = {
         extend: function(t) {
-            return t = _(t), this.min || this.max ? (this.min.x = Math.min(t.x, this.min.x), this.max.x = Math.max(t.x, this.max.x), this.min.y = Math.min(t.y, this.min.y), this.max.y = Math.max(t.y, this.max.y)) : (this.min = t.clone(), this.max = t.clone()), this
+            var e, i;
+            if (t) {
+                if (t instanceof p || "number" == typeof t[0] || "x" in t) e = i = m(t);
+                else if (e = (t = _(t)).min, i = t.max, !e || !i) return this;
+                this.min || this.max ? (this.min.x = Math.min(e.x, this.min.x), this.max.x = Math.max(i.x, this.max.x), this.min.y = Math.min(e.y, this.min.y), this.max.y = Math.max(i.y, this.max.y)) : (this.min = e.clone(), this.max = i.clone())
+            }
+            return this
         },
         getCenter: function(t) {
-            return new p((this.min.x + this.max.x) / 2, (this.min.y + this.max.y) / 2, t)
+            return m((this.min.x + this.max.x) / 2, (this.min.y + this.max.y) / 2, t)
         },
         getBottomLeft: function() {
-            return new p(this.min.x, this.max.y)
+            return m(this.min.x, this.max.y)
         },
         getTopRight: function() {
-            return new p(this.max.x, this.min.y)
+            return m(this.max.x, this.min.y)
         },
         getTopLeft: function() {
             return this.min
         },
         getBottomRight: function() {
             return this.max
         },
         getSize: function() {
             return this.max.subtract(this.min)
         },
         contains: function(t) {
-            var i, e;
-            return (t = ("number" == typeof t[0] || t instanceof p ? _ : f)(t)) instanceof m ? (i = t.min, e = t.max) : i = e = t, i.x >= this.min.x && e.x <= this.max.x && i.y >= this.min.y && e.y <= this.max.y
+            var e, i;
+            return (t = ("number" == typeof t[0] || t instanceof p ? m : _)(t)) instanceof f ? (e = t.min, i = t.max) : e = i = t, e.x >= this.min.x && i.x <= this.max.x && e.y >= this.min.y && i.y <= this.max.y
         },
         intersects: function(t) {
-            t = f(t);
-            var i = this.min,
-                e = this.max,
+            t = _(t);
+            var e = this.min,
+                i = this.max,
                 n = t.min,
                 t = t.max,
-                o = t.x >= i.x && n.x <= e.x,
-                t = t.y >= i.y && n.y <= e.y;
+                o = t.x >= e.x && n.x <= i.x,
+                t = t.y >= e.y && n.y <= i.y;
             return o && t
         },
         overlaps: function(t) {
-            t = f(t);
-            var i = this.min,
-                e = this.max,
+            t = _(t);
+            var e = this.min,
+                i = this.max,
                 n = t.min,
                 t = t.max,
-                o = t.x > i.x && n.x < e.x,
-                t = t.y > i.y && n.y < e.y;
+                o = t.x > e.x && n.x < i.x,
+                t = t.y > e.y && n.y < i.y;
             return o && t
         },
         isValid: function() {
             return !(!this.min || !this.max)
+        },
+        pad: function(t) {
+            var e = this.min,
+                i = this.max,
+                n = Math.abs(e.x - i.x) * t,
+                t = Math.abs(e.y - i.y) * t;
+            return _(m(e.x - n, e.y - t), m(i.x + n, i.y + t))
+        },
+        equals: function(t) {
+            return !!t && (t = _(t), this.min.equals(t.getTopLeft()) && this.max.equals(t.getBottomRight()))
         }
     }, s.prototype = {
         extend: function(t) {
-            var i, e, n = this._southWest,
+            var e, i, n = this._southWest,
                 o = this._northEast;
-            if (t instanceof v) e = i = t;
+            if (t instanceof v) i = e = t;
             else {
                 if (!(t instanceof s)) return t ? this.extend(w(t) || g(t)) : this;
-                if (i = t._southWest, e = t._northEast, !i || !e) return this
+                if (e = t._southWest, i = t._northEast, !e || !i) return this
             }
-            return n || o ? (n.lat = Math.min(i.lat, n.lat), n.lng = Math.min(i.lng, n.lng), o.lat = Math.max(e.lat, o.lat), o.lng = Math.max(e.lng, o.lng)) : (this._southWest = new v(i.lat, i.lng), this._northEast = new v(e.lat, e.lng)), this
+            return n || o ? (n.lat = Math.min(e.lat, n.lat), n.lng = Math.min(e.lng, n.lng), o.lat = Math.max(i.lat, o.lat), o.lng = Math.max(i.lng, o.lng)) : (this._southWest = new v(e.lat, e.lng), this._northEast = new v(i.lat, i.lng)), this
         },
         pad: function(t) {
-            var i = this._southWest,
-                e = this._northEast,
-                n = Math.abs(i.lat - e.lat) * t,
-                t = Math.abs(i.lng - e.lng) * t;
-            return new s(new v(i.lat - n, i.lng - t), new v(e.lat + n, e.lng + t))
+            var e = this._southWest,
+                i = this._northEast,
+                n = Math.abs(e.lat - i.lat) * t,
+                t = Math.abs(e.lng - i.lng) * t;
+            return new s(new v(e.lat - n, e.lng - t), new v(i.lat + n, i.lng + t))
         },
         getCenter: function() {
             return new v((this._southWest.lat + this._northEast.lat) / 2, (this._southWest.lng + this._northEast.lng) / 2)
         },
         getSouthWest: function() {
             return this._southWest
         },
@@ -483,55 +494,55 @@
             return this._northEast.lng
         },
         getNorth: function() {
             return this._northEast.lat
         },
         contains: function(t) {
             t = ("number" == typeof t[0] || t instanceof v || "lat" in t ? w : g)(t);
-            var i, e, n = this._southWest,
+            var e, i, n = this._southWest,
                 o = this._northEast;
-            return t instanceof s ? (i = t.getSouthWest(), e = t.getNorthEast()) : i = e = t, i.lat >= n.lat && e.lat <= o.lat && i.lng >= n.lng && e.lng <= o.lng
+            return t instanceof s ? (e = t.getSouthWest(), i = t.getNorthEast()) : e = i = t, e.lat >= n.lat && i.lat <= o.lat && e.lng >= n.lng && i.lng <= o.lng
         },
         intersects: function(t) {
             t = g(t);
-            var i = this._southWest,
-                e = this._northEast,
+            var e = this._southWest,
+                i = this._northEast,
                 n = t.getSouthWest(),
                 t = t.getNorthEast(),
-                o = t.lat >= i.lat && n.lat <= e.lat,
-                t = t.lng >= i.lng && n.lng <= e.lng;
+                o = t.lat >= e.lat && n.lat <= i.lat,
+                t = t.lng >= e.lng && n.lng <= i.lng;
             return o && t
         },
         overlaps: function(t) {
             t = g(t);
-            var i = this._southWest,
-                e = this._northEast,
+            var e = this._southWest,
+                i = this._northEast,
                 n = t.getSouthWest(),
                 t = t.getNorthEast(),
-                o = t.lat > i.lat && n.lat < e.lat,
-                t = t.lng > i.lng && n.lng < e.lng;
+                o = t.lat > e.lat && n.lat < i.lat,
+                t = t.lng > e.lng && n.lng < i.lng;
             return o && t
         },
         toBBoxString: function() {
             return [this.getWest(), this.getSouth(), this.getEast(), this.getNorth()].join(",")
         },
-        equals: function(t, i) {
-            return !!t && (t = g(t), this._southWest.equals(t.getSouthWest(), i) && this._northEast.equals(t.getNorthEast(), i))
+        equals: function(t, e) {
+            return !!t && (t = g(t), this._southWest.equals(t.getSouthWest(), e) && this._northEast.equals(t.getNorthEast(), e))
         },
         isValid: function() {
             return !(!this._southWest || !this._northEast)
         }
     };
     var ot = {
-            latLngToPoint: function(t, i) {
-                t = this.projection.project(t), i = this.scale(i);
-                return this.transformation._transform(t, i)
+            latLngToPoint: function(t, e) {
+                t = this.projection.project(t), e = this.scale(e);
+                return this.transformation._transform(t, e)
             },
-            pointToLatLng: function(t, i) {
-                i = this.scale(i), t = this.transformation.untransform(t, i);
+            pointToLatLng: function(t, e) {
+                e = this.scale(e), t = this.transformation.untransform(t, e);
                 return this.projection.unproject(t)
             },
             project: function(t) {
                 return this.projection.project(t)
             },
             unproject: function(t) {
                 return this.projection.unproject(t)
@@ -539,104 +550,99 @@
             scale: function(t) {
                 return 256 * Math.pow(2, t)
             },
             zoom: function(t) {
                 return Math.log(t / 256) / Math.LN2
             },
             getProjectedBounds: function(t) {
-                if (this.infinite) return null;
-                var i = this.projection.bounds,
-                    t = this.scale(t);
-                return new m(this.transformation.transform(i.min, t), this.transformation.transform(i.max, t))
+                var e;
+                return this.infinite ? null : (e = this.projection.bounds, t = this.scale(t), new f(this.transformation.transform(e.min, t), this.transformation.transform(e.max, t)))
             },
             infinite: !(v.prototype = {
-                equals: function(t, i) {
-                    return !!t && (t = w(t), Math.max(Math.abs(this.lat - t.lat), Math.abs(this.lng - t.lng)) <= (void 0 === i ? 1e-9 : i))
+                equals: function(t, e) {
+                    return !!t && (t = w(t), Math.max(Math.abs(this.lat - t.lat), Math.abs(this.lng - t.lng)) <= (void 0 === e ? 1e-9 : e))
                 },
                 toString: function(t) {
-                    return "LatLng(" + e(this.lat, t) + ", " + e(this.lng, t) + ")"
+                    return "LatLng(" + i(this.lat, t) + ", " + i(this.lng, t) + ")"
                 },
                 distanceTo: function(t) {
                     return st.distance(this, w(t))
                 },
                 wrap: function() {
                     return st.wrapLatLng(this)
                 },
                 toBounds: function(t) {
                     var t = 180 * t / 40075017,
-                        i = t / Math.cos(Math.PI / 180 * this.lat);
-                    return g([this.lat - t, this.lng - i], [this.lat + t, this.lng + i])
+                        e = t / Math.cos(Math.PI / 180 * this.lat);
+                    return g([this.lat - t, this.lng - e], [this.lat + t, this.lng + e])
                 },
                 clone: function() {
                     return new v(this.lat, this.lng, this.alt)
                 }
             }),
             wrapLatLng: function(t) {
-                var i = this.wrapLng ? H(t.lng, this.wrapLng, !0) : t.lng;
-                return new v(this.wrapLat ? H(t.lat, this.wrapLat, !0) : t.lat, i, t.alt)
+                var e = this.wrapLng ? F(t.lng, this.wrapLng, !0) : t.lng;
+                return new v(this.wrapLat ? F(t.lat, this.wrapLat, !0) : t.lat, e, t.alt)
             },
             wrapLatLngBounds: function(t) {
-                var i = t.getCenter(),
-                    e = this.wrapLatLng(i),
-                    n = i.lat - e.lat,
-                    i = i.lng - e.lng;
-                if (0 == n && 0 == i) return t;
-                e = t.getSouthWest(), t = t.getNorthEast();
-                return new s(new v(e.lat - n, e.lng - i), new v(t.lat - n, t.lng - i))
+                var e = t.getCenter(),
+                    i = this.wrapLatLng(e),
+                    n = e.lat - i.lat,
+                    e = e.lng - i.lng;
+                return 0 == n && 0 == e ? t : (i = t.getSouthWest(), t = t.getNorthEast(), new s(new v(i.lat - n, i.lng - e), new v(t.lat - n, t.lng - e)))
             }
         },
         st = l({}, ot, {
             wrapLng: [-180, 180],
             R: 6371e3,
-            distance: function(t, i) {
-                var e = Math.PI / 180,
-                    n = t.lat * e,
-                    o = i.lat * e,
-                    s = Math.sin((i.lat - t.lat) * e / 2),
-                    i = Math.sin((i.lng - t.lng) * e / 2),
-                    t = s * s + Math.cos(n) * Math.cos(o) * i * i,
-                    e = 2 * Math.atan2(Math.sqrt(t), Math.sqrt(1 - t));
-                return this.R * e
+            distance: function(t, e) {
+                var i = Math.PI / 180,
+                    n = t.lat * i,
+                    o = e.lat * i,
+                    s = Math.sin((e.lat - t.lat) * i / 2),
+                    e = Math.sin((e.lng - t.lng) * i / 2),
+                    t = s * s + Math.cos(n) * Math.cos(o) * e * e,
+                    i = 2 * Math.atan2(Math.sqrt(t), Math.sqrt(1 - t));
+                return this.R * i
             }
         }),
         rt = 6378137,
         rt = {
             R: rt,
             MAX_LATITUDE: 85.0511287798,
             project: function(t) {
-                var i = Math.PI / 180,
-                    e = this.MAX_LATITUDE,
-                    e = Math.max(Math.min(e, t.lat), -e),
-                    e = Math.sin(e * i);
-                return new p(this.R * t.lng * i, this.R * Math.log((1 + e) / (1 - e)) / 2)
+                var e = Math.PI / 180,
+                    i = this.MAX_LATITUDE,
+                    i = Math.max(Math.min(i, t.lat), -i),
+                    i = Math.sin(i * e);
+                return new p(this.R * t.lng * e, this.R * Math.log((1 + i) / (1 - i)) / 2)
             },
             unproject: function(t) {
-                var i = 180 / Math.PI;
-                return new v((2 * Math.atan(Math.exp(t.y / this.R)) - Math.PI / 2) * i, t.x * i / this.R)
+                var e = 180 / Math.PI;
+                return new v((2 * Math.atan(Math.exp(t.y / this.R)) - Math.PI / 2) * e, t.x * e / this.R)
             },
-            bounds: new m([-(rt = rt * Math.PI), -rt], [rt, rt])
+            bounds: new f([-(rt = rt * Math.PI), -rt], [rt, rt])
         };
 
-    function at(t, i, e, n) {
-        if (d(t)) return this._a = t[0], this._b = t[1], this._c = t[2], void(this._d = t[3]);
-        this._a = t, this._b = i, this._c = e, this._d = n
+    function at(t, e, i, n) {
+        d(t) ? (this._a = t[0], this._b = t[1], this._c = t[2], this._d = t[3]) : (this._a = t, this._b = e, this._c = i, this._d = n)
     }
 
-    function ht(t, i, e, n) {
-        return new at(t, i, e, n)
+    function ht(t, e, i, n) {
+        return new at(t, e, i, n)
     }
     at.prototype = {
-        transform: function(t, i) {
-            return this._transform(t.clone(), i)
+        transform: function(t, e) {
+            return this._transform(t.clone(), e)
         },
-        _transform: function(t, i) {
-            return t.x = (i = i || 1) * (this._a * t.x + this._b), t.y = i * (this._c * t.y + this._d), t
+        _transform: function(t, e) {
+            return t.x = (e = e || 1) * (this._a * t.x + this._b), t.y = e * (this._c * t.y + this._d), t
         },
-        untransform: function(t, i) {
-            return new p((t.x / (i = i || 1) - this._b) / this._a, (t.y / i - this._d) / this._c)
+        untransform: function(t, e) {
+            return new p((t.x / (e = e || 1) - this._b) / this._a, (t.y / e - this._d) / this._c)
         }
     };
     var lt = l({}, st, {
             code: "EPSG:3857",
             projection: rt,
             transformation: ht(lt = .5 / (Math.PI * rt.R), .5, -lt, .5)
         }),
@@ -644,481 +650,490 @@
             code: "EPSG:900913"
         });
 
     function ct(t) {
         return document.createElementNS("http://www.w3.org/2000/svg", t)
     }
 
-    function dt(t, i) {
-        for (var e, n, o, s, r = "", a = 0, h = t.length; a < h; a++) {
-            for (e = 0, n = (o = t[a]).length; e < n; e++) r += (e ? "L" : "M") + (s = o[e]).x + " " + s.y;
-            r += i ? P.svg ? "z" : "x" : ""
+    function dt(t, e) {
+        for (var i, n, o, s, r = "", a = 0, h = t.length; a < h; a++) {
+            for (i = 0, n = (o = t[a]).length; i < n; i++) r += (i ? "L" : "M") + (s = o[i]).x + " " + s.y;
+            r += e ? b.svg ? "z" : "x" : ""
         }
         return r || "M0 0"
     }
     var _t = document.documentElement.style,
         pt = "ActiveXObject" in window,
         mt = pt && !document.addEventListener,
-        n = "msLaunchUri" in navigator && !("documentMode" in document),
-        ft = y("webkit"),
-        gt = y("android"),
-        vt = y("android 2") || y("android 3"),
+        o = "msLaunchUri" in navigator && !("documentMode" in document),
+        ft = Wt("webkit"),
+        gt = Wt("android"),
+        vt = Wt("android 2") || Wt("android 3"),
         yt = parseInt(/WebKit\/([0-9]+)|$/.exec(navigator.userAgent)[1], 10),
-        yt = gt && y("Google") && yt < 537 && !("AudioNode" in window),
+        yt = gt && Wt("Google") && yt < 537 && !("AudioNode" in window),
         xt = !!window.opera,
-        wt = !n && y("chrome"),
-        Pt = y("gecko") && !ft && !xt && !pt,
-        bt = !wt && y("safari"),
-        Lt = y("phantom"),
-        o = "OTransition" in _t,
+        wt = !o && Wt("chrome"),
+        bt = Wt("gecko") && !ft && !xt && !pt,
+        Pt = !wt && Wt("safari"),
+        Lt = Wt("phantom"),
+        y = "OTransition" in _t,
         Tt = 0 === navigator.platform.indexOf("Win"),
-        zt = pt && "transition" in _t,
-        Mt = "WebKitCSSMatrix" in window && "m11" in new window.WebKitCSSMatrix && !vt,
+        Mt = pt && "transition" in _t,
+        zt = "WebKitCSSMatrix" in window && "m11" in new window.WebKitCSSMatrix && !vt,
         _t = "MozPerspective" in _t,
-        Ct = !window.L_DISABLE_3D && (zt || Mt || _t) && !o && !Lt,
-        Zt = "undefined" != typeof orientation || y("mobile"),
+        Ct = !window.L_DISABLE_3D && (Mt || zt || _t) && !y && !Lt,
+        Zt = "undefined" != typeof orientation || Wt("mobile"),
         St = Zt && ft,
-        kt = Zt && Mt,
-        Et = !window.PointerEvent && window.MSPointerEvent,
-        Bt = !(!window.PointerEvent && !Et),
-        At = "ontouchstart" in window || !!window.TouchEvent,
-        It = !window.L_NO_TOUCH && (At || Bt),
-        Ot = Zt && xt,
-        Rt = Zt && Pt,
+        Et = Zt && zt,
+        kt = !window.PointerEvent && window.MSPointerEvent,
+        Ot = !(!window.PointerEvent && !kt),
+        Bt = "ontouchstart" in window || !!window.TouchEvent,
+        At = !window.L_NO_TOUCH && (Bt || Ot),
+        It = Zt && xt,
+        Rt = Zt && bt,
         Nt = 1 < (window.devicePixelRatio || window.screen.deviceXDPI / window.screen.logicalXDPI),
         Dt = function() {
             var t = !1;
             try {
-                var i = Object.defineProperty({}, "passive", {
+                var e = Object.defineProperty({}, "passive", {
                     get: function() {
                         t = !0
                     }
                 });
-                window.addEventListener("testPassiveEventSupport", u, i), window.removeEventListener("testPassiveEventSupport", u, i)
+                window.addEventListener("testPassiveEventSupport", u, e), window.removeEventListener("testPassiveEventSupport", u, e)
             } catch (t) {}
             return t
         }(),
         jt = !!document.createElement("canvas").getContext,
         Ht = !(!document.createElementNS || !ct("svg").createSVGRect),
-        Wt = !!Ht && ((Wt = document.createElement("div")).innerHTML = "<svg/>", "http://www.w3.org/2000/svg" === (Wt.firstChild && Wt.firstChild.namespaceURI));
+        Ft = !!Ht && ((Ft = document.createElement("div")).innerHTML = "<svg/>", "http://www.w3.org/2000/svg" === (Ft.firstChild && Ft.firstChild.namespaceURI));
 
-    function y(t) {
+    function Wt(t) {
         return 0 <= navigator.userAgent.toLowerCase().indexOf(t)
     }
-    var P = {
+    var b = {
             ie: pt,
             ielt9: mt,
-            edge: n,
+            edge: o,
             webkit: ft,
             android: gt,
             android23: vt,
             androidStock: yt,
             opera: xt,
             chrome: wt,
-            gecko: Pt,
-            safari: bt,
+            gecko: bt,
+            safari: Pt,
             phantom: Lt,
-            opera12: o,
+            opera12: y,
             win: Tt,
-            ie3d: zt,
-            webkit3d: Mt,
+            ie3d: Mt,
+            webkit3d: zt,
             gecko3d: _t,
             any3d: Ct,
             mobile: Zt,
             mobileWebkit: St,
-            mobileWebkit3d: kt,
-            msPointer: Et,
-            pointer: Bt,
-            touch: It,
-            touchNative: At,
-            mobileOpera: Ot,
+            mobileWebkit3d: Et,
+            msPointer: kt,
+            pointer: Ot,
+            touch: At,
+            touchNative: Bt,
+            mobileOpera: It,
             mobileGecko: Rt,
             retina: Nt,
             passiveEvents: Dt,
             canvas: jt,
             svg: Ht,
             vml: !Ht && function() {
                 try {
                     var t = document.createElement("div"),
-                        i = (t.innerHTML = '<v:shape adj="1"/>', t.firstChild);
-                    return i.style.behavior = "url(#default#VML)", i && "object" == typeof i.adj
+                        e = (t.innerHTML = '<v:shape adj="1"/>', t.firstChild);
+                    return e.style.behavior = "url(#default#VML)", e && "object" == typeof e.adj
                 } catch (t) {
                     return !1
                 }
             }(),
-            inlineSvg: Wt
-        },
-        Ft = P.msPointer ? "MSPointerDown" : "pointerdown",
-        Ut = P.msPointer ? "MSPointerMove" : "pointermove",
-        Vt = P.msPointer ? "MSPointerUp" : "pointerup",
-        qt = P.msPointer ? "MSPointerCancel" : "pointercancel",
-        Gt = {
-            touchstart: Ft,
-            touchmove: Ut,
-            touchend: Vt,
+            inlineSvg: Ft,
+            mac: 0 === navigator.platform.indexOf("Mac"),
+            linux: 0 === navigator.platform.indexOf("Linux")
+        },
+        Ut = b.msPointer ? "MSPointerDown" : "pointerdown",
+        Vt = b.msPointer ? "MSPointerMove" : "pointermove",
+        Gt = b.msPointer ? "MSPointerUp" : "pointerup",
+        qt = b.msPointer ? "MSPointerCancel" : "pointercancel",
+        Kt = {
+            touchstart: Ut,
+            touchmove: Vt,
+            touchend: Gt,
             touchcancel: qt
         },
-        Kt = {
-            touchstart: function(t, i) {
-                i.MSPOINTER_TYPE_TOUCH && i.pointerType === i.MSPOINTER_TYPE_TOUCH && B(i);
-                ii(t, i)
-            },
-            touchmove: ii,
-            touchend: ii,
-            touchcancel: ii
+        Yt = {
+            touchstart: function(t, e) {
+                e.MSPOINTER_TYPE_TOUCH && e.pointerType === e.MSPOINTER_TYPE_TOUCH && k(e);
+                ie(t, e)
+            },
+            touchmove: ie,
+            touchend: ie,
+            touchcancel: ie
         },
-        Yt = {},
+        Jt = {},
         Xt = !1;
 
-    function Jt(t, i, e) {
-        return "touchstart" !== i || Xt || (document.addEventListener(Ft, $t, !0), document.addEventListener(Ut, Qt, !0), document.addEventListener(Vt, ti, !0), document.addEventListener(qt, ti, !0), Xt = !0), Kt[i] ? (e = Kt[i].bind(this, e), t.addEventListener(Gt[i], e, !1), e) : (console.warn("wrong event specified:", i), L.Util.falseFn)
+    function $t(t, e, i) {
+        return "touchstart" !== e || Xt || (document.addEventListener(Ut, Qt, !0), document.addEventListener(Vt, te, !0), document.addEventListener(Gt, ee, !0), document.addEventListener(qt, ee, !0), Xt = !0), Yt[e] ? (i = Yt[e].bind(this, i), t.addEventListener(Kt[e], i, !1), i) : (console.warn("wrong event specified:", e), L.Util.falseFn)
     }
 
-    function $t(t) {
-        Yt[t.pointerId] = t
+    function Qt(t) {
+        Jt[t.pointerId] = t
     }
 
-    function Qt(t) {
-        Yt[t.pointerId] && (Yt[t.pointerId] = t)
+    function te(t) {
+        Jt[t.pointerId] && (Jt[t.pointerId] = t)
     }
 
-    function ti(t) {
-        delete Yt[t.pointerId]
+    function ee(t) {
+        delete Jt[t.pointerId]
     }
 
-    function ii(t, i) {
-        if (i.pointerType !== (i.MSPOINTER_TYPE_MOUSE || "mouse")) {
-            for (var e in i.touches = [], Yt) i.touches.push(Yt[e]);
-            i.changedTouches = [i], t(i)
+    function ie(t, e) {
+        if (e.pointerType !== (e.MSPOINTER_TYPE_MOUSE || "mouse")) {
+            for (var i in e.touches = [], Jt) e.touches.push(Jt[i]);
+            e.changedTouches = [e], t(e)
         }
     }
-    var ei = 200;
+    var ne = 200;
 
-    function ni(t, e) {
-        t.addEventListener("dblclick", e);
+    function oe(t, i) {
+        t.addEventListener("dblclick", i);
         var n, o = 0;
 
-        function i(t) {
-            var i;
-            1 !== t.detail ? n = t.detail : "mouse" === t.pointerType || t.sourceCapabilities && !t.sourceCapabilities.firesTouchEvents || ((i = Date.now()) - o <= ei ? 2 === ++n && e(function(t) {
-                var i, e, n = {};
-                for (e in t) i = t[e], n[e] = i && i.bind ? i.bind(t) : i;
+        function e(t) {
+            var e;
+            1 !== t.detail ? n = t.detail : "mouse" === t.pointerType || t.sourceCapabilities && !t.sourceCapabilities.firesTouchEvents || ((e = je(t)).some(function(t) {
+                return t instanceof HTMLLabelElement && t.attributes.for
+            }) && !e.some(function(t) {
+                return t instanceof HTMLInputElement || t instanceof HTMLSelectElement
+            }) || ((e = Date.now()) - o <= ne ? 2 === ++n && i(function(t) {
+                var e, i, n = {};
+                for (i in t) e = t[i], n[i] = e && e.bind ? e.bind(t) : e;
                 return (t = n).type = "dblclick", n.detail = 2, n.isTrusted = !1, n._simulated = !0, n
-            }(t)) : n = 1, o = i)
+            }(t)) : n = 1, o = e))
         }
-        return t.addEventListener("click", i), {
-            dblclick: e,
-            simDblclick: i
+        return t.addEventListener("click", e), {
+            dblclick: i,
+            simDblclick: e
         }
     }
-    var oi, si, ri, ai, hi, li, ui = wi(["transform", "webkitTransform", "OTransform", "MozTransform", "msTransform"]),
-        ci = wi(["webkitTransition", "transition", "OTransition", "MozTransition", "msTransition"]),
-        di = "webkitTransition" === ci || "OTransition" === ci ? ci + "End" : "transitionend";
+    var se, re, ae, he, le, ue, ce = be(["transform", "webkitTransform", "OTransform", "MozTransform", "msTransform"]),
+        de = be(["webkitTransition", "transition", "OTransition", "MozTransition", "msTransition"]),
+        _e = "webkitTransition" === de || "OTransition" === de ? de + "End" : "transitionend";
 
-    function _i(t) {
+    function pe(t) {
         return "string" == typeof t ? document.getElementById(t) : t
     }
 
-    function pi(t, i) {
-        var e = t.style[i] || t.currentStyle && t.currentStyle[i];
-        return "auto" === (e = e && "auto" !== e || !document.defaultView ? e : (t = document.defaultView.getComputedStyle(t, null)) ? t[i] : null) ? null : e
+    function me(t, e) {
+        var i = t.style[e] || t.currentStyle && t.currentStyle[e];
+        return "auto" === (i = i && "auto" !== i || !document.defaultView ? i : (t = document.defaultView.getComputedStyle(t, null)) ? t[e] : null) ? null : i
     }
 
-    function b(t, i, e) {
+    function P(t, e, i) {
         t = document.createElement(t);
-        return t.className = i || "", e && e.appendChild(t), t
+        return t.className = e || "", i && i.appendChild(t), t
     }
 
     function T(t) {
-        var i = t.parentNode;
-        i && i.removeChild(t)
+        var e = t.parentNode;
+        e && e.removeChild(t)
     }
 
-    function mi(t) {
+    function fe(t) {
         for (; t.firstChild;) t.removeChild(t.firstChild)
     }
 
-    function fi(t) {
-        var i = t.parentNode;
-        i && i.lastChild !== t && i.appendChild(t)
+    function ge(t) {
+        var e = t.parentNode;
+        e && e.lastChild !== t && e.appendChild(t)
     }
 
-    function gi(t) {
-        var i = t.parentNode;
-        i && i.firstChild !== t && i.insertBefore(t, i.firstChild)
+    function ve(t) {
+        var e = t.parentNode;
+        e && e.firstChild !== t && e.insertBefore(t, e.firstChild)
     }
 
-    function vi(t, i) {
-        if (void 0 !== t.classList) return t.classList.contains(i);
-        t = xi(t);
-        return 0 < t.length && new RegExp("(^|\\s)" + i + "(\\s|$)").test(t)
+    function ye(t, e) {
+        return void 0 !== t.classList ? t.classList.contains(e) : 0 < (t = we(t)).length && new RegExp("(^|\\s)" + e + "(\\s|$)").test(t)
     }
 
-    function z(t, i) {
-        var e;
+    function M(t, e) {
+        var i;
         if (void 0 !== t.classList)
-            for (var n = F(i), o = 0, s = n.length; o < s; o++) t.classList.add(n[o]);
-        else vi(t, i) || yi(t, ((e = xi(t)) ? e + " " : "") + i)
+            for (var n = U(e), o = 0, s = n.length; o < s; o++) t.classList.add(n[o]);
+        else ye(t, e) || xe(t, ((i = we(t)) ? i + " " : "") + e)
     }
 
-    function M(t, i) {
-        void 0 !== t.classList ? t.classList.remove(i) : yi(t, W((" " + xi(t) + " ").replace(" " + i + " ", " ")))
+    function z(t, e) {
+        void 0 !== t.classList ? t.classList.remove(e) : xe(t, W((" " + we(t) + " ").replace(" " + e + " ", " ")))
     }
 
-    function yi(t, i) {
-        void 0 === t.className.baseVal ? t.className = i : t.className.baseVal = i
+    function xe(t, e) {
+        void 0 === t.className.baseVal ? t.className = e : t.className.baseVal = e
     }
 
-    function xi(t) {
+    function we(t) {
         return void 0 === (t = t.correspondingElement ? t.correspondingElement : t).className.baseVal ? t.className : t.className.baseVal
     }
 
-    function C(t, i) {
-        if ("opacity" in t.style) t.style.opacity = i;
+    function C(t, e) {
+        if ("opacity" in t.style) t.style.opacity = e;
         else if ("filter" in t.style) {
-            var e = !1,
+            var i = !1,
                 n = "DXImageTransform.Microsoft.Alpha";
             try {
-                e = t.filters.item(n)
+                i = t.filters.item(n)
             } catch (t) {
-                if (1 === i) return
+                if (1 === e) return
             }
-            i = Math.round(100 * i), e ? (e.Enabled = 100 !== i, e.Opacity = i) : t.style.filter += " progid:" + n + "(opacity=" + i + ")"
+            e = Math.round(100 * e), i ? (i.Enabled = 100 !== e, i.Opacity = e) : t.style.filter += " progid:" + n + "(opacity=" + e + ")"
         }
     }
 
-    function wi(t) {
-        for (var i = document.documentElement.style, e = 0; e < t.length; e++)
-            if (t[e] in i) return t[e];
+    function be(t) {
+        for (var e = document.documentElement.style, i = 0; i < t.length; i++)
+            if (t[i] in e) return t[i];
         return !1
     }
 
-    function Pi(t, i, e) {
-        i = i || new p(0, 0);
-        t.style[ui] = (P.ie3d ? "translate(" + i.x + "px," + i.y + "px)" : "translate3d(" + i.x + "px," + i.y + "px,0)") + (e ? " scale(" + e + ")" : "")
+    function Pe(t, e, i) {
+        e = e || new p(0, 0);
+        t.style[ce] = (b.ie3d ? "translate(" + e.x + "px," + e.y + "px)" : "translate3d(" + e.x + "px," + e.y + "px,0)") + (i ? " scale(" + i + ")" : "")
     }
 
-    function Z(t, i) {
-        t._leaflet_pos = i, P.any3d ? Pi(t, i) : (t.style.left = i.x + "px", t.style.top = i.y + "px")
+    function Z(t, e) {
+        t._leaflet_pos = e, b.any3d ? Pe(t, e) : (t.style.left = e.x + "px", t.style.top = e.y + "px")
     }
 
-    function bi(t) {
+    function Le(t) {
         return t._leaflet_pos || new p(0, 0)
     }
 
-    function Li() {
-        S(window, "dragstart", B)
+    function Te() {
+        S(window, "dragstart", k)
     }
 
-    function Ti() {
-        E(window, "dragstart", B)
+    function Me() {
+        E(window, "dragstart", k)
     }
 
-    function zi(t) {
+    function ze(t) {
         for (; - 1 === t.tabIndex;) t = t.parentNode;
-        t.style && (Mi(), li = (hi = t).style.outline, t.style.outline = "none", S(window, "keydown", Mi))
+        t.style && (Ce(), ue = (le = t).style.outline, t.style.outline = "none", S(window, "keydown", Ce))
     }
 
-    function Mi() {
-        hi && (hi.style.outline = li, li = hi = void 0, E(window, "keydown", Mi))
+    function Ce() {
+        le && (le.style.outline = ue, ue = le = void 0, E(window, "keydown", Ce))
     }
 
-    function Ci(t) {
+    function Ze(t) {
         for (; !((t = t.parentNode).offsetWidth && t.offsetHeight || t === document.body););
         return t
     }
 
-    function Zi(t) {
-        var i = t.getBoundingClientRect();
+    function Se(t) {
+        var e = t.getBoundingClientRect();
         return {
-            x: i.width / t.offsetWidth || 1,
-            y: i.height / t.offsetHeight || 1,
-            boundingClientRect: i
+            x: e.width / t.offsetWidth || 1,
+            y: e.height / t.offsetHeight || 1,
+            boundingClientRect: e
         }
     }
-    ai = "onselectstart" in document ? (ri = function() {
-        S(window, "selectstart", B)
+    he = "onselectstart" in document ? (ae = function() {
+        S(window, "selectstart", k)
     }, function() {
-        E(window, "selectstart", B)
-    }) : (si = wi(["userSelect", "WebkitUserSelect", "OUserSelect", "MozUserSelect", "msUserSelect"]), ri = function() {
+        E(window, "selectstart", k)
+    }) : (re = be(["userSelect", "WebkitUserSelect", "OUserSelect", "MozUserSelect", "msUserSelect"]), ae = function() {
         var t;
-        si && (t = document.documentElement.style, oi = t[si], t[si] = "none")
+        re && (t = document.documentElement.style, se = t[re], t[re] = "none")
     }, function() {
-        si && (document.documentElement.style[si] = oi, oi = void 0)
+        re && (document.documentElement.style[re] = se, se = void 0)
     });
     pt = {
         __proto__: null,
-        TRANSFORM: ui,
-        TRANSITION: ci,
-        TRANSITION_END: di,
-        get: _i,
-        getStyle: pi,
-        create: b,
+        TRANSFORM: ce,
+        TRANSITION: de,
+        TRANSITION_END: _e,
+        get: pe,
+        getStyle: me,
+        create: P,
         remove: T,
-        empty: mi,
-        toFront: fi,
-        toBack: gi,
-        hasClass: vi,
-        addClass: z,
-        removeClass: M,
-        setClass: yi,
-        getClass: xi,
+        empty: fe,
+        toFront: ge,
+        toBack: ve,
+        hasClass: ye,
+        addClass: M,
+        removeClass: z,
+        setClass: xe,
+        getClass: we,
         setOpacity: C,
-        testProp: wi,
-        setTransform: Pi,
+        testProp: be,
+        setTransform: Pe,
         setPosition: Z,
-        getPosition: bi,
+        getPosition: Le,
         get disableTextSelection() {
-            return ri
+            return ae
         },
         get enableTextSelection() {
-            return ai
+            return he
         },
-        disableImageDrag: Li,
-        enableImageDrag: Ti,
-        preventOutline: zi,
-        restoreOutline: Mi,
-        getSizedParentNode: Ci,
-        getScale: Zi
+        disableImageDrag: Te,
+        enableImageDrag: Me,
+        preventOutline: ze,
+        restoreOutline: Ce,
+        getSizedParentNode: Ze,
+        getScale: Se
     };
 
-    function S(t, i, e, n) {
-        if (i && "object" == typeof i)
-            for (var o in i) Ei(t, o, i[o], e);
+    function S(t, e, i, n) {
+        if (e && "object" == typeof e)
+            for (var o in e) Be(t, o, e[o], i);
         else
-            for (var s = 0, r = (i = F(i)).length; s < r; s++) Ei(t, i[s], e, n);
+            for (var s = 0, r = (e = U(e)).length; s < r; s++) Be(t, e[s], i, n);
         return this
     }
-    var k = "_leaflet_events";
+    var Ee = "_leaflet_events";
 
-    function E(t, i, e, n) {
-        if (1 === arguments.length) Si(t), delete t[k];
-        else if (i && "object" == typeof i)
-            for (var o in i) Bi(t, o, i[o], e);
-        else if (i = F(i), 2 === arguments.length) Si(t, function(t) {
-            return -1 !== G(i, t)
+    function E(t, e, i, n) {
+        if (1 === arguments.length) ke(t), delete t[Ee];
+        else if (e && "object" == typeof e)
+            for (var o in e) Ae(t, o, e[o], i);
+        else if (e = U(e), 2 === arguments.length) ke(t, function(t) {
+            return -1 !== K(e, t)
         });
         else
-            for (var s = 0, r = i.length; s < r; s++) Bi(t, i[s], e, n);
+            for (var s = 0, r = e.length; s < r; s++) Ae(t, e[s], i, n);
         return this
     }
 
-    function Si(t, i) {
-        for (var e in t[k]) {
-            var n = e.split(/\d/)[0];
-            i && !i(n) || Bi(t, n, null, null, e)
+    function ke(t, e) {
+        for (var i in t[Ee]) {
+            var n = i.split(/\d/)[0];
+            e && !e(n) || Ae(t, n, null, null, i)
         }
     }
-    var ki = {
+    var Oe = {
         mouseenter: "mouseover",
         mouseleave: "mouseout",
         wheel: !("onwheel" in window) && "mousewheel"
     };
 
-    function Ei(i, t, e, n) {
-        var o, s, r = t + h(e) + (n ? "_" + h(n) : "");
-        i[k] && i[k][r] || (s = o = function(t) {
-            return e.call(n || i, t || window.event)
-        }, !P.touchNative && P.pointer && 0 === t.indexOf("touch") ? o = Jt(i, t, o) : P.touch && "dblclick" === t ? o = ni(i, o) : "addEventListener" in i ? "touchstart" === t || "touchmove" === t || "wheel" === t || "mousewheel" === t ? i.addEventListener(ki[t] || t, o, !!P.passiveEvents && {
+    function Be(e, t, i, n) {
+        var o, s, r = t + h(i) + (n ? "_" + h(n) : "");
+        e[Ee] && e[Ee][r] || (s = o = function(t) {
+            return i.call(n || e, t || window.event)
+        }, !b.touchNative && b.pointer && 0 === t.indexOf("touch") ? o = $t(e, t, o) : b.touch && "dblclick" === t ? o = oe(e, o) : "addEventListener" in e ? "touchstart" === t || "touchmove" === t || "wheel" === t || "mousewheel" === t ? e.addEventListener(Oe[t] || t, o, !!b.passiveEvents && {
             passive: !1
-        }) : "mouseenter" === t || "mouseleave" === t ? i.addEventListener(ki[t], o = function(t) {
-            t = t || window.event, Hi(i, t) && s(t)
-        }, !1) : i.addEventListener(t, s, !1) : i.attachEvent("on" + t, o), i[k] = i[k] || {}, i[k][r] = o)
+        }) : "mouseenter" === t || "mouseleave" === t ? e.addEventListener(Oe[t], o = function(t) {
+            t = t || window.event, Ue(e, t) && s(t)
+        }, !1) : e.addEventListener(t, s, !1) : e.attachEvent("on" + t, o), e[Ee] = e[Ee] || {}, e[Ee][r] = o)
     }
 
-    function Bi(t, i, e, n, o) {
-        o = o || i + h(e) + (n ? "_" + h(n) : "");
-        var s, r, e = t[k] && t[k][o];
-        e && (!P.touchNative && P.pointer && 0 === i.indexOf("touch") ? (n = t, r = e, Gt[s = i] ? n.removeEventListener(Gt[s], r, !1) : console.warn("wrong event specified:", s)) : P.touch && "dblclick" === i ? (n = e, (r = t).removeEventListener("dblclick", n.dblclick), r.removeEventListener("click", n.simDblclick)) : "removeEventListener" in t ? t.removeEventListener(ki[i] || i, e, !1) : t.detachEvent("on" + i, e), t[k][o] = null)
+    function Ae(t, e, i, n, o) {
+        o = o || e + h(i) + (n ? "_" + h(n) : "");
+        var s, r, i = t[Ee] && t[Ee][o];
+        i && (!b.touchNative && b.pointer && 0 === e.indexOf("touch") ? (n = t, r = i, Kt[s = e] ? n.removeEventListener(Kt[s], r, !1) : console.warn("wrong event specified:", s)) : b.touch && "dblclick" === e ? (n = i, (r = t).removeEventListener("dblclick", n.dblclick), r.removeEventListener("click", n.simDblclick)) : "removeEventListener" in t ? t.removeEventListener(Oe[e] || e, i, !1) : t.detachEvent("on" + e, i), t[Ee][o] = null)
     }
 
-    function Ai(t) {
+    function Ie(t) {
         return t.stopPropagation ? t.stopPropagation() : t.originalEvent ? t.originalEvent._stopped = !0 : t.cancelBubble = !0, this
     }
 
-    function Ii(t) {
-        return Ei(t, "wheel", Ai), this
+    function Re(t) {
+        return Be(t, "wheel", Ie), this
     }
 
-    function Oi(t) {
-        return S(t, "mousedown touchstart dblclick contextmenu", Ai), t._leaflet_disable_click = !0, this
+    function Ne(t) {
+        return S(t, "mousedown touchstart dblclick contextmenu", Ie), t._leaflet_disable_click = !0, this
     }
 
-    function B(t) {
+    function k(t) {
         return t.preventDefault ? t.preventDefault() : t.returnValue = !1, this
     }
 
-    function Ri(t) {
-        return B(t), Ai(t), this
+    function De(t) {
+        return k(t), Ie(t), this
     }
 
-    function Ni(t, i) {
-        if (!i) return new p(t.clientX, t.clientY);
-        var e = Zi(i),
-            n = e.boundingClientRect;
-        return new p((t.clientX - n.left) / e.x - i.clientLeft, (t.clientY - n.top) / e.y - i.clientTop)
+    function je(t) {
+        if (t.composedPath) return t.composedPath();
+        for (var e = [], i = t.target; i;) e.push(i), i = i.parentNode;
+        return e
+    }
+
+    function He(t, e) {
+        var i, n;
+        return e ? (n = (i = Se(e)).boundingClientRect, new p((t.clientX - n.left) / i.x - e.clientLeft, (t.clientY - n.top) / i.y - e.clientTop)) : new p(t.clientX, t.clientY)
     }
-    var Di = P.win && P.chrome ? 2 * window.devicePixelRatio : P.gecko ? window.devicePixelRatio : 1;
+    var Fe = b.linux && b.chrome ? window.devicePixelRatio : b.mac ? 3 * window.devicePixelRatio : 0 < window.devicePixelRatio ? 2 * window.devicePixelRatio : 1;
 
-    function ji(t) {
-        return P.edge ? t.wheelDeltaY / 2 : t.deltaY && 0 === t.deltaMode ? -t.deltaY / Di : t.deltaY && 1 === t.deltaMode ? 20 * -t.deltaY : t.deltaY && 2 === t.deltaMode ? 60 * -t.deltaY : t.deltaX || t.deltaZ ? 0 : t.wheelDelta ? (t.wheelDeltaY || t.wheelDelta) / 2 : t.detail && Math.abs(t.detail) < 32765 ? 20 * -t.detail : t.detail ? t.detail / -32765 * 60 : 0
+    function We(t) {
+        return b.edge ? t.wheelDeltaY / 2 : t.deltaY && 0 === t.deltaMode ? -t.deltaY / Fe : t.deltaY && 1 === t.deltaMode ? 20 * -t.deltaY : t.deltaY && 2 === t.deltaMode ? 60 * -t.deltaY : t.deltaX || t.deltaZ ? 0 : t.wheelDelta ? (t.wheelDeltaY || t.wheelDelta) / 2 : t.detail && Math.abs(t.detail) < 32765 ? 20 * -t.detail : t.detail ? t.detail / -32765 * 60 : 0
     }
 
-    function Hi(t, i) {
-        var e = i.relatedTarget;
-        if (!e) return !0;
+    function Ue(t, e) {
+        var i = e.relatedTarget;
+        if (!i) return !0;
         try {
-            for (; e && e !== t;) e = e.parentNode
+            for (; i && i !== t;) i = i.parentNode
         } catch (t) {
             return !1
         }
-        return e !== t
+        return i !== t
     }
     var mt = {
             __proto__: null,
             on: S,
             off: E,
-            stopPropagation: Ai,
-            disableScrollPropagation: Ii,
-            disableClickPropagation: Oi,
-            preventDefault: B,
-            stop: Ri,
-            getMousePosition: Ni,
-            getWheelDelta: ji,
-            isExternalTarget: Hi,
+            stopPropagation: Ie,
+            disableScrollPropagation: Re,
+            disableClickPropagation: Ne,
+            preventDefault: k,
+            stop: De,
+            getPropagationPath: je,
+            getMousePosition: He,
+            getWheelDelta: We,
+            isExternalTarget: Ue,
             addListener: S,
             removeListener: E
         },
-        Wi = et.extend({
-            run: function(t, i, e, n) {
-                this.stop(), this._el = t, this._inProgress = !0, this._duration = e || .25, this._easeOutPower = 1 / Math.max(n || .5, .2), this._startPos = bi(t), this._offset = i.subtract(this._startPos), this._startTime = +new Date, this.fire("start"), this._animate()
+        Ve = it.extend({
+            run: function(t, e, i, n) {
+                this.stop(), this._el = t, this._inProgress = !0, this._duration = i || .25, this._easeOutPower = 1 / Math.max(n || .5, .2), this._startPos = Le(t), this._offset = e.subtract(this._startPos), this._startTime = +new Date, this.fire("start"), this._animate()
             },
             stop: function() {
                 this._inProgress && (this._step(!0), this._complete())
             },
             _animate: function() {
                 this._animId = x(this._animate, this), this._step()
             },
             _step: function(t) {
-                var i = +new Date - this._startTime,
-                    e = 1e3 * this._duration;
-                i < e ? this._runFrame(this._easeOut(i / e), t) : (this._runFrame(1), this._complete())
+                var e = +new Date - this._startTime,
+                    i = 1e3 * this._duration;
+                e < i ? this._runFrame(this._easeOut(e / i), t) : (this._runFrame(1), this._complete())
             },
-            _runFrame: function(t, i) {
+            _runFrame: function(t, e) {
                 t = this._startPos.add(this._offset.multiplyBy(t));
-                i && t._round(), Z(this._el, t), this.fire("step")
+                e && t._round(), Z(this._el, t), this.fire("step")
             },
             _complete: function() {
                 r(this._animId), this._inProgress = !1, this.fire("end")
             },
             _easeOut: function(t) {
                 return 1 - Math.pow(1 - t, this._easeOutPower)
             }
         }),
-        A = et.extend({
+        O = it.extend({
             options: {
                 crs: lt,
                 center: void 0,
                 zoom: void 0,
                 minZoom: void 0,
                 maxZoom: void 0,
                 layers: [],
@@ -1129,101 +1144,98 @@
                 fadeAnimation: !0,
                 markerZoomAnimation: !0,
                 transform3DLimit: 8388608,
                 zoomSnap: 1,
                 zoomDelta: 1,
                 trackResize: !0
             },
-            initialize: function(t, i) {
-                i = c(this, i), this._handlers = [], this._layers = {}, this._zoomBoundLayers = {}, this._sizeChanged = !0, this._initContainer(t), this._initLayout(), this._onResize = a(this._onResize, this), this._initEvents(), i.maxBounds && this.setMaxBounds(i.maxBounds), void 0 !== i.zoom && (this._zoom = this._limitZoom(i.zoom)), i.center && void 0 !== i.zoom && this.setView(w(i.center), i.zoom, {
+            initialize: function(t, e) {
+                e = c(this, e), this._handlers = [], this._layers = {}, this._zoomBoundLayers = {}, this._sizeChanged = !0, this._initContainer(t), this._initLayout(), this._onResize = a(this._onResize, this), this._initEvents(), e.maxBounds && this.setMaxBounds(e.maxBounds), void 0 !== e.zoom && (this._zoom = this._limitZoom(e.zoom)), e.center && void 0 !== e.zoom && this.setView(w(e.center), e.zoom, {
                     reset: !0
-                }), this.callInitHooks(), this._zoomAnimated = ci && P.any3d && !P.mobileOpera && this.options.zoomAnimation, this._zoomAnimated && (this._createAnimProxy(), S(this._proxy, di, this._catchTransitionEnd, this)), this._addLayers(this.options.layers)
+                }), this.callInitHooks(), this._zoomAnimated = de && b.any3d && !b.mobileOpera && this.options.zoomAnimation, this._zoomAnimated && (this._createAnimProxy(), S(this._proxy, _e, this._catchTransitionEnd, this)), this._addLayers(this.options.layers)
             },
-            setView: function(t, i, e) {
-                if ((i = void 0 === i ? this._zoom : this._limitZoom(i), t = this._limitCenter(w(t), i, this.options.maxBounds), e = e || {}, this._stop(), this._loaded && !e.reset && !0 !== e) && (void 0 !== e.animate && (e.zoom = l({
-                        animate: e.animate
-                    }, e.zoom), e.pan = l({
-                        animate: e.animate,
-                        duration: e.duration
-                    }, e.pan)), this._zoom !== i ? this._tryAnimatedZoom && this._tryAnimatedZoom(t, i, e.zoom) : this._tryAnimatedPan(t, e.pan))) return clearTimeout(this._sizeTimer), this;
-                return this._resetView(t, i), this
+            setView: function(t, e, i) {
+                if ((e = void 0 === e ? this._zoom : this._limitZoom(e), t = this._limitCenter(w(t), e, this.options.maxBounds), i = i || {}, this._stop(), this._loaded && !i.reset && !0 !== i) && (void 0 !== i.animate && (i.zoom = l({
+                        animate: i.animate
+                    }, i.zoom), i.pan = l({
+                        animate: i.animate,
+                        duration: i.duration
+                    }, i.pan)), this._zoom !== e ? this._tryAnimatedZoom && this._tryAnimatedZoom(t, e, i.zoom) : this._tryAnimatedPan(t, i.pan))) return clearTimeout(this._sizeTimer), this;
+                return this._resetView(t, e, i.pan && i.pan.noMoveStart), this
             },
-            setZoom: function(t, i) {
+            setZoom: function(t, e) {
                 return this._loaded ? this.setView(this.getCenter(), t, {
-                    zoom: i
+                    zoom: e
                 }) : (this._zoom = t, this)
             },
-            zoomIn: function(t, i) {
-                return t = t || (P.any3d ? this.options.zoomDelta : 1), this.setZoom(this._zoom + t, i)
+            zoomIn: function(t, e) {
+                return t = t || (b.any3d ? this.options.zoomDelta : 1), this.setZoom(this._zoom + t, e)
             },
-            zoomOut: function(t, i) {
-                return t = t || (P.any3d ? this.options.zoomDelta : 1), this.setZoom(this._zoom - t, i)
+            zoomOut: function(t, e) {
+                return t = t || (b.any3d ? this.options.zoomDelta : 1), this.setZoom(this._zoom - t, e)
             },
-            setZoomAround: function(t, i, e) {
-                var n = this.getZoomScale(i),
+            setZoomAround: function(t, e, i) {
+                var n = this.getZoomScale(e),
                     o = this.getSize().divideBy(2),
                     t = (t instanceof p ? t : this.latLngToContainerPoint(t)).subtract(o).multiplyBy(1 - 1 / n),
                     n = this.containerPointToLatLng(o.add(t));
-                return this.setView(n, i, {
-                    zoom: e
+                return this.setView(n, e, {
+                    zoom: i
                 })
             },
-            _getBoundsCenterZoom: function(t, i) {
-                i = i || {}, t = t.getBounds ? t.getBounds() : g(t);
-                var e = _(i.paddingTopLeft || i.padding || [0, 0]),
-                    n = _(i.paddingBottomRight || i.padding || [0, 0]),
-                    o = this.getBoundsZoom(t, !1, e.add(n));
-                if ((o = "number" == typeof i.maxZoom ? Math.min(i.maxZoom, o) : o) === 1 / 0) return {
+            _getBoundsCenterZoom: function(t, e) {
+                e = e || {}, t = t.getBounds ? t.getBounds() : g(t);
+                var i = m(e.paddingTopLeft || e.padding || [0, 0]),
+                    n = m(e.paddingBottomRight || e.padding || [0, 0]),
+                    o = this.getBoundsZoom(t, !1, i.add(n));
+                return (o = "number" == typeof e.maxZoom ? Math.min(e.maxZoom, o) : o) === 1 / 0 ? {
                     center: t.getCenter(),
                     zoom: o
-                };
-                i = n.subtract(e).divideBy(2), n = this.project(t.getSouthWest(), o), e = this.project(t.getNorthEast(), o);
-                return {
-                    center: this.unproject(n.add(e).divideBy(2).add(i), o),
+                } : (e = n.subtract(i).divideBy(2), n = this.project(t.getSouthWest(), o), i = this.project(t.getNorthEast(), o), {
+                    center: this.unproject(n.add(i).divideBy(2).add(e), o),
                     zoom: o
-                }
+                })
             },
-            fitBounds: function(t, i) {
-                if (!(t = g(t)).isValid()) throw new Error("Bounds are not valid.");
-                t = this._getBoundsCenterZoom(t, i);
-                return this.setView(t.center, t.zoom, i)
+            fitBounds: function(t, e) {
+                if ((t = g(t)).isValid()) return t = this._getBoundsCenterZoom(t, e), this.setView(t.center, t.zoom, e);
+                throw new Error("Bounds are not valid.")
             },
             fitWorld: function(t) {
                 return this.fitBounds([
                     [-90, -180],
                     [90, 180]
                 ], t)
             },
-            panTo: function(t, i) {
+            panTo: function(t, e) {
                 return this.setView(t, this._zoom, {
-                    pan: i
+                    pan: e
                 })
             },
-            panBy: function(t, i) {
-                return i = i || {}, (t = _(t).round()).x || t.y ? (!0 === i.animate || this.getSize().contains(t) ? (this._panAnim || (this._panAnim = new Wi, this._panAnim.on({
+            panBy: function(t, e) {
+                var i;
+                return e = e || {}, (t = m(t).round()).x || t.y ? (!0 === e.animate || this.getSize().contains(t) ? (this._panAnim || (this._panAnim = new Ve, this._panAnim.on({
                     step: this._onPanTransitionStep,
                     end: this._onPanTransitionEnd
-                }, this)), i.noMoveStart || this.fire("movestart"), !1 !== i.animate ? (z(this._mapPane, "leaflet-pan-anim"), e = this._getMapPanePos().subtract(t).round(), this._panAnim.run(this._mapPane, e, i.duration || .25, i.easeLinearity)) : (this._rawPanBy(t), this.fire("move").fire("moveend"))) : this._resetView(this.unproject(this.project(this.getCenter()).add(t)), this.getZoom()), this) : this.fire("moveend");
-                var e
+                }, this)), e.noMoveStart || this.fire("movestart"), !1 !== e.animate ? (M(this._mapPane, "leaflet-pan-anim"), i = this._getMapPanePos().subtract(t).round(), this._panAnim.run(this._mapPane, i, e.duration || .25, e.easeLinearity)) : (this._rawPanBy(t), this.fire("move").fire("moveend"))) : this._resetView(this.unproject(this.project(this.getCenter()).add(t)), this.getZoom()), this) : this.fire("moveend")
             },
             flyTo: function(n, o, t) {
-                if (!1 === (t = t || {}).animate || !P.any3d) return this.setView(n, o, t);
+                if (!1 === (t = t || {}).animate || !b.any3d) return this.setView(n, o, t);
                 this._stop();
                 var s = this.project(this.getCenter()),
                     r = this.project(n),
-                    i = this.getSize(),
+                    e = this.getSize(),
                     a = this._zoom,
-                    h = (n = w(n), o = void 0 === o ? a : o, Math.max(i.x, i.y)),
-                    e = h * this.getZoomScale(a, o),
+                    h = (n = w(n), o = void 0 === o ? a : o, Math.max(e.x, e.y)),
+                    i = h * this.getZoomScale(a, o),
                     l = r.distanceTo(s) || 1,
                     u = 1.42,
                     c = u * u;
 
                 function d(t) {
-                    t = (e * e - h * h + (t ? -1 : 1) * c * c * l * l) / (2 * (t ? e : h) * c * l), t = Math.sqrt(t * t + 1) - t;
+                    t = (i * i - h * h + (t ? -1 : 1) * c * c * l * l) / (2 * (t ? i : h) * c * l), t = Math.sqrt(t * t + 1) - t;
                     return t < 1e-9 ? -18 : Math.log(t)
                 }
 
                 function _(t) {
                     return (Math.exp(t) - Math.exp(-t)) / 2
                 }
 
@@ -1236,167 +1248,163 @@
                     return h * (p(m) * (_(t = m + u * t) / p(t)) - _(m)) / c
                 }
                 var g = Date.now(),
                     v = (d(1) - m) / u,
                     y = t.duration ? 1e3 * t.duration : 1e3 * v * .8;
                 return this._moveStart(!0, t.noMoveStart),
                     function t() {
-                        var i = (Date.now() - g) / y,
-                            e = (1 - Math.pow(1 - i, 1.5)) * v;
-                        i <= 1 ? (this._flyToFrame = x(t, this), this._move(this.unproject(s.add(r.subtract(s).multiplyBy(f(e) / l)), a), this.getScaleZoom(h / (i = e, h * (p(m) / p(m + u * i))), a), {
+                        var e = (Date.now() - g) / y,
+                            i = (1 - Math.pow(1 - e, 1.5)) * v;
+                        e <= 1 ? (this._flyToFrame = x(t, this), this._move(this.unproject(s.add(r.subtract(s).multiplyBy(f(i) / l)), a), this.getScaleZoom(h / (e = i, h * (p(m) / p(m + u * e))), a), {
                             flyTo: !0
                         })) : this._move(n, o)._moveEnd(!0)
                     }.call(this), this
             },
-            flyToBounds: function(t, i) {
-                t = this._getBoundsCenterZoom(t, i);
-                return this.flyTo(t.center, t.zoom, i)
+            flyToBounds: function(t, e) {
+                t = this._getBoundsCenterZoom(t, e);
+                return this.flyTo(t.center, t.zoom, e)
             },
             setMaxBounds: function(t) {
-                return (t = g(t)).isValid() ? (this.options.maxBounds && this.off("moveend", this._panInsideMaxBounds), this.options.maxBounds = t, this._loaded && this._panInsideMaxBounds(), this.on("moveend", this._panInsideMaxBounds)) : (this.options.maxBounds = null, this.off("moveend", this._panInsideMaxBounds))
+                return t = g(t), this.listens("moveend", this._panInsideMaxBounds) && this.off("moveend", this._panInsideMaxBounds), t.isValid() ? (this.options.maxBounds = t, this._loaded && this._panInsideMaxBounds(), this.on("moveend", this._panInsideMaxBounds)) : (this.options.maxBounds = null, this)
             },
             setMinZoom: function(t) {
-                var i = this.options.minZoom;
-                return this.options.minZoom = t, this._loaded && i !== t && (this.fire("zoomlevelschange"), this.getZoom() < this.options.minZoom) ? this.setZoom(t) : this
+                var e = this.options.minZoom;
+                return this.options.minZoom = t, this._loaded && e !== t && (this.fire("zoomlevelschange"), this.getZoom() < this.options.minZoom) ? this.setZoom(t) : this
             },
             setMaxZoom: function(t) {
-                var i = this.options.maxZoom;
-                return this.options.maxZoom = t, this._loaded && i !== t && (this.fire("zoomlevelschange"), this.getZoom() > this.options.maxZoom) ? this.setZoom(t) : this
+                var e = this.options.maxZoom;
+                return this.options.maxZoom = t, this._loaded && e !== t && (this.fire("zoomlevelschange"), this.getZoom() > this.options.maxZoom) ? this.setZoom(t) : this
             },
-            panInsideBounds: function(t, i) {
+            panInsideBounds: function(t, e) {
                 this._enforcingBounds = !0;
-                var e = this.getCenter(),
-                    t = this._limitCenter(e, this._zoom, g(t));
-                return e.equals(t) || this.panTo(t, i), this._enforcingBounds = !1, this
-            },
-            panInside: function(t, i) {
-                var e = _((i = i || {}).paddingTopLeft || i.padding || [0, 0]),
-                    n = _(i.paddingBottomRight || i.padding || [0, 0]),
+                var i = this.getCenter(),
+                    t = this._limitCenter(i, this._zoom, g(t));
+                return i.equals(t) || this.panTo(t, e), this._enforcingBounds = !1, this
+            },
+            panInside: function(t, e) {
+                var i = m((e = e || {}).paddingTopLeft || e.padding || [0, 0]),
+                    n = m(e.paddingBottomRight || e.padding || [0, 0]),
                     o = this.project(this.getCenter()),
                     t = this.project(t),
                     s = this.getPixelBounds(),
-                    e = f([s.min.add(e), s.max.subtract(n)]),
-                    s = e.getSize();
-                return e.contains(t) || (this._enforcingBounds = !0, n = t.subtract(e.getCenter()), e = e.extend(t).getSize().subtract(s), o.x += n.x < 0 ? -e.x : e.x, o.y += n.y < 0 ? -e.y : e.y, this.panTo(this.unproject(o), i), this._enforcingBounds = !1), this
+                    i = _([s.min.add(i), s.max.subtract(n)]),
+                    s = i.getSize();
+                return i.contains(t) || (this._enforcingBounds = !0, n = t.subtract(i.getCenter()), i = i.extend(t).getSize().subtract(s), o.x += n.x < 0 ? -i.x : i.x, o.y += n.y < 0 ? -i.y : i.y, this.panTo(this.unproject(o), e), this._enforcingBounds = !1), this
             },
             invalidateSize: function(t) {
                 if (!this._loaded) return this;
                 t = l({
                     animate: !1,
                     pan: !0
                 }, !0 === t ? {
                     animate: !0
                 } : t);
-                var i = this.getSize(),
-                    e = (this._sizeChanged = !0, this._lastCenter = null, this.getSize()),
-                    n = i.divideBy(2).round(),
-                    o = e.divideBy(2).round(),
+                var e = this.getSize(),
+                    i = (this._sizeChanged = !0, this._lastCenter = null, this.getSize()),
+                    n = e.divideBy(2).round(),
+                    o = i.divideBy(2).round(),
                     n = n.subtract(o);
                 return n.x || n.y ? (t.animate && t.pan ? this.panBy(n) : (t.pan && this._rawPanBy(n), this.fire("move"), t.debounceMoveend ? (clearTimeout(this._sizeTimer), this._sizeTimer = setTimeout(a(this.fire, this, "moveend"), 200)) : this.fire("moveend")), this.fire("resize", {
-                    oldSize: i,
-                    newSize: e
+                    oldSize: e,
+                    newSize: i
                 })) : this
             },
             stop: function() {
                 return this.setZoom(this._limitZoom(this._zoom)), this.options.zoomSnap || this.fire("viewreset"), this._stop()
             },
             locate: function(t) {
-                if (t = this._locateOptions = l({
-                        timeout: 1e4,
-                        watch: !1
-                    }, t), !("geolocation" in navigator)) return this._handleGeolocationError({
+                var e, i;
+                return t = this._locateOptions = l({
+                    timeout: 1e4,
+                    watch: !1
+                }, t), "geolocation" in navigator ? (e = a(this._handleGeolocationResponse, this), i = a(this._handleGeolocationError, this), t.watch ? this._locationWatchId = navigator.geolocation.watchPosition(e, i, t) : navigator.geolocation.getCurrentPosition(e, i, t)) : this._handleGeolocationError({
                     code: 0,
                     message: "Geolocation not supported."
-                }), this;
-                var i = a(this._handleGeolocationResponse, this),
-                    e = a(this._handleGeolocationError, this);
-                return t.watch ? this._locationWatchId = navigator.geolocation.watchPosition(i, e, t) : navigator.geolocation.getCurrentPosition(i, e, t), this
+                }), this
             },
             stopLocate: function() {
                 return navigator.geolocation && navigator.geolocation.clearWatch && navigator.geolocation.clearWatch(this._locationWatchId), this._locateOptions && (this._locateOptions.setView = !1), this
             },
             _handleGeolocationError: function(t) {
-                var i;
-                this._container._leaflet_id && (i = t.code, t = t.message || (1 === i ? "permission denied" : 2 === i ? "position unavailable" : "timeout"), this._locateOptions.setView && !this._loaded && this.fitWorld(), this.fire("locationerror", {
-                    code: i,
+                var e;
+                this._container._leaflet_id && (e = t.code, t = t.message || (1 === e ? "permission denied" : 2 === e ? "position unavailable" : "timeout"), this._locateOptions.setView && !this._loaded && this.fitWorld(), this.fire("locationerror", {
+                    code: e,
                     message: "Geolocation error: " + t + "."
                 }))
             },
             _handleGeolocationResponse: function(t) {
                 if (this._container._leaflet_id) {
-                    var i, e, n = new v(t.coords.latitude, t.coords.longitude),
+                    var e, i, n = new v(t.coords.latitude, t.coords.longitude),
                         o = n.toBounds(2 * t.coords.accuracy),
                         s = this._locateOptions,
-                        r = (s.setView && (i = this.getBoundsZoom(o), this.setView(n, s.maxZoom ? Math.min(i, s.maxZoom) : i)), {
+                        r = (s.setView && (e = this.getBoundsZoom(o), this.setView(n, s.maxZoom ? Math.min(e, s.maxZoom) : e)), {
                             latlng: n,
                             bounds: o,
                             timestamp: t.timestamp
                         });
-                    for (e in t.coords) "number" == typeof t.coords[e] && (r[e] = t.coords[e]);
+                    for (i in t.coords) "number" == typeof t.coords[i] && (r[i] = t.coords[i]);
                     this.fire("locationfound", r)
                 }
             },
-            addHandler: function(t, i) {
-                if (!i) return this;
-                i = this[t] = new i(this);
-                return this._handlers.push(i), this.options[t] && i.enable(), this
+            addHandler: function(t, e) {
+                return e && (e = this[t] = new e(this), this._handlers.push(e), this.options[t] && e.enable()), this
             },
             remove: function() {
                 if (this._initEvents(!0), this.options.maxBounds && this.off("moveend", this._panInsideMaxBounds), this._containerId !== this._container._leaflet_id) throw new Error("Map container is being reused by another instance");
                 try {
                     delete this._container._leaflet_id, delete this._containerId
                 } catch (t) {
                     this._container._leaflet_id = void 0, this._containerId = void 0
                 }
                 for (var t in void 0 !== this._locationWatchId && this.stopLocate(), this._stop(), T(this._mapPane), this._clearControlPos && this._clearControlPos(), this._resizeRequest && (r(this._resizeRequest), this._resizeRequest = null), this._clearHandlers(), this._loaded && this.fire("unload"), this._layers) this._layers[t].remove();
                 for (t in this._panes) T(this._panes[t]);
                 return this._layers = [], this._panes = [], delete this._mapPane, delete this._renderer, this
             },
-            createPane: function(t, i) {
-                i = b("div", "leaflet-pane" + (t ? " leaflet-" + t.replace("Pane", "") + "-pane" : ""), i || this._mapPane);
-                return t && (this._panes[t] = i), i
+            createPane: function(t, e) {
+                e = P("div", "leaflet-pane" + (t ? " leaflet-" + t.replace("Pane", "") + "-pane" : ""), e || this._mapPane);
+                return t && (this._panes[t] = e), e
             },
             getCenter: function() {
-                return this._checkIfLoaded(), this._lastCenter && !this._moved() ? this._lastCenter : this.layerPointToLatLng(this._getCenterLayerPoint())
+                return this._checkIfLoaded(), this._lastCenter && !this._moved() ? this._lastCenter.clone() : this.layerPointToLatLng(this._getCenterLayerPoint())
             },
             getZoom: function() {
                 return this._zoom
             },
             getBounds: function() {
                 var t = this.getPixelBounds();
                 return new s(this.unproject(t.getBottomLeft()), this.unproject(t.getTopRight()))
             },
             getMinZoom: function() {
                 return void 0 === this.options.minZoom ? this._layersMinZoom || 0 : this.options.minZoom
             },
             getMaxZoom: function() {
                 return void 0 === this.options.maxZoom ? void 0 === this._layersMaxZoom ? 1 / 0 : this._layersMaxZoom : this.options.maxZoom
             },
-            getBoundsZoom: function(t, i, e) {
-                t = g(t), e = _(e || [0, 0]);
+            getBoundsZoom: function(t, e, i) {
+                t = g(t), i = m(i || [0, 0]);
                 var n = this.getZoom() || 0,
                     o = this.getMinZoom(),
                     s = this.getMaxZoom(),
                     r = t.getNorthWest(),
                     t = t.getSouthEast(),
-                    e = this.getSize().subtract(e),
-                    t = f(this.project(t, n), this.project(r, n)).getSize(),
-                    r = P.any3d ? this.options.zoomSnap : 1,
-                    a = e.x / t.x,
-                    e = e.y / t.y,
-                    t = i ? Math.max(a, e) : Math.min(a, e),
+                    i = this.getSize().subtract(i),
+                    t = _(this.project(t, n), this.project(r, n)).getSize(),
+                    r = b.any3d ? this.options.zoomSnap : 1,
+                    a = i.x / t.x,
+                    i = i.y / t.y,
+                    t = e ? Math.max(a, i) : Math.min(a, i),
                     n = this.getScaleZoom(t, n);
-                return r && (n = Math.round(n / (r / 100)) * (r / 100), n = i ? Math.ceil(n / r) * r : Math.floor(n / r) * r), Math.max(o, Math.min(s, n))
+                return r && (n = Math.round(n / (r / 100)) * (r / 100), n = e ? Math.ceil(n / r) * r : Math.floor(n / r) * r), Math.max(o, Math.min(s, n))
             },
             getSize: function() {
                 return this._size && !this._sizeChanged || (this._size = new p(this._container.clientWidth || 0, this._container.clientHeight || 0), this._sizeChanged = !1), this._size.clone()
             },
-            getPixelBounds: function(t, i) {
-                t = this._getTopLeftPoint(t, i);
-                return new m(t, t.add(this.getSize()))
+            getPixelBounds: function(t, e) {
+                t = this._getTopLeftPoint(t, e);
+                return new f(t, t.add(this.getSize()))
             },
             getPixelOrigin: function() {
                 return this._checkIfLoaded(), this._pixelOrigin
             },
             getPixelWorldBounds: function(t) {
                 return this.options.crs.getProjectedBounds(void 0 === t ? this.getZoom() : t)
             },
@@ -1405,95 +1413,95 @@
             },
             getPanes: function() {
                 return this._panes
             },
             getContainer: function() {
                 return this._container
             },
-            getZoomScale: function(t, i) {
-                var e = this.options.crs;
-                return i = void 0 === i ? this._zoom : i, e.scale(t) / e.scale(i)
-            },
-            getScaleZoom: function(t, i) {
-                var e = this.options.crs,
-                    t = (i = void 0 === i ? this._zoom : i, e.zoom(t * e.scale(i)));
+            getZoomScale: function(t, e) {
+                var i = this.options.crs;
+                return e = void 0 === e ? this._zoom : e, i.scale(t) / i.scale(e)
+            },
+            getScaleZoom: function(t, e) {
+                var i = this.options.crs,
+                    t = (e = void 0 === e ? this._zoom : e, i.zoom(t * i.scale(e)));
                 return isNaN(t) ? 1 / 0 : t
             },
-            project: function(t, i) {
-                return i = void 0 === i ? this._zoom : i, this.options.crs.latLngToPoint(w(t), i)
+            project: function(t, e) {
+                return e = void 0 === e ? this._zoom : e, this.options.crs.latLngToPoint(w(t), e)
             },
-            unproject: function(t, i) {
-                return i = void 0 === i ? this._zoom : i, this.options.crs.pointToLatLng(_(t), i)
+            unproject: function(t, e) {
+                return e = void 0 === e ? this._zoom : e, this.options.crs.pointToLatLng(m(t), e)
             },
             layerPointToLatLng: function(t) {
-                t = _(t).add(this.getPixelOrigin());
+                t = m(t).add(this.getPixelOrigin());
                 return this.unproject(t)
             },
             latLngToLayerPoint: function(t) {
                 return this.project(w(t))._round()._subtract(this.getPixelOrigin())
             },
             wrapLatLng: function(t) {
                 return this.options.crs.wrapLatLng(w(t))
             },
             wrapLatLngBounds: function(t) {
                 return this.options.crs.wrapLatLngBounds(g(t))
             },
-            distance: function(t, i) {
-                return this.options.crs.distance(w(t), w(i))
+            distance: function(t, e) {
+                return this.options.crs.distance(w(t), w(e))
             },
             containerPointToLayerPoint: function(t) {
-                return _(t).subtract(this._getMapPanePos())
+                return m(t).subtract(this._getMapPanePos())
             },
             layerPointToContainerPoint: function(t) {
-                return _(t).add(this._getMapPanePos())
+                return m(t).add(this._getMapPanePos())
             },
             containerPointToLatLng: function(t) {
-                t = this.containerPointToLayerPoint(_(t));
+                t = this.containerPointToLayerPoint(m(t));
                 return this.layerPointToLatLng(t)
             },
             latLngToContainerPoint: function(t) {
                 return this.layerPointToContainerPoint(this.latLngToLayerPoint(w(t)))
             },
             mouseEventToContainerPoint: function(t) {
-                return Ni(t, this._container)
+                return He(t, this._container)
             },
             mouseEventToLayerPoint: function(t) {
                 return this.containerPointToLayerPoint(this.mouseEventToContainerPoint(t))
             },
             mouseEventToLatLng: function(t) {
                 return this.layerPointToLatLng(this.mouseEventToLayerPoint(t))
             },
             _initContainer: function(t) {
-                t = this._container = _i(t);
+                t = this._container = pe(t);
                 if (!t) throw new Error("Map container not found.");
                 if (t._leaflet_id) throw new Error("Map container is already initialized.");
                 S(t, "scroll", this._onScroll, this), this._containerId = h(t)
             },
             _initLayout: function() {
                 var t = this._container,
-                    i = (this._fadeAnimated = this.options.fadeAnimation && P.any3d, z(t, "leaflet-container" + (P.touch ? " leaflet-touch" : "") + (P.retina ? " leaflet-retina" : "") + (P.ielt9 ? " leaflet-oldie" : "") + (P.safari ? " leaflet-safari" : "") + (this._fadeAnimated ? " leaflet-fade-anim" : "")), pi(t, "position"));
-                "absolute" !== i && "relative" !== i && "fixed" !== i && (t.style.position = "relative"), this._initPanes(), this._initControlPos && this._initControlPos()
+                    e = (this._fadeAnimated = this.options.fadeAnimation && b.any3d, M(t, "leaflet-container" + (b.touch ? " leaflet-touch" : "") + (b.retina ? " leaflet-retina" : "") + (b.ielt9 ? " leaflet-oldie" : "") + (b.safari ? " leaflet-safari" : "") + (this._fadeAnimated ? " leaflet-fade-anim" : "")), me(t, "position"));
+                "absolute" !== e && "relative" !== e && "fixed" !== e && (t.style.position = "relative"), this._initPanes(), this._initControlPos && this._initControlPos()
             },
             _initPanes: function() {
                 var t = this._panes = {};
-                this._paneRenderers = {}, this._mapPane = this.createPane("mapPane", this._container), Z(this._mapPane, new p(0, 0)), this.createPane("tilePane"), this.createPane("overlayPane"), this.createPane("shadowPane"), this.createPane("markerPane"), this.createPane("tooltipPane"), this.createPane("popupPane"), this.options.markerZoomAnimation || (z(t.markerPane, "leaflet-zoom-hide"), z(t.shadowPane, "leaflet-zoom-hide"))
+                this._paneRenderers = {}, this._mapPane = this.createPane("mapPane", this._container), Z(this._mapPane, new p(0, 0)), this.createPane("tilePane"), this.createPane("overlayPane"), this.createPane("shadowPane"), this.createPane("markerPane"), this.createPane("tooltipPane"), this.createPane("popupPane"), this.options.markerZoomAnimation || (M(t.markerPane, "leaflet-zoom-hide"), M(t.shadowPane, "leaflet-zoom-hide"))
             },
-            _resetView: function(t, i) {
+            _resetView: function(t, e, i) {
                 Z(this._mapPane, new p(0, 0));
-                var e = !this._loaded,
-                    n = (this._loaded = !0, i = this._limitZoom(i), this.fire("viewprereset"), this._zoom !== i);
-                this._moveStart(n, !1)._move(t, i)._moveEnd(n), this.fire("viewreset"), e && this.fire("load")
-            },
-            _moveStart: function(t, i) {
-                return t && this.fire("zoomstart"), i || this.fire("movestart"), this
-            },
-            _move: function(t, i, e, n) {
-                void 0 === i && (i = this._zoom);
-                var o = this._zoom !== i;
-                return this._zoom = i, this._lastCenter = t, this._pixelOrigin = this._getNewPixelOrigin(t), n ? e && e.pinch && this.fire("zoom", e) : ((o || e && e.pinch) && this.fire("zoom", e), this.fire("move", e)), this
+                var n = !this._loaded,
+                    o = (this._loaded = !0, e = this._limitZoom(e), this.fire("viewprereset"), this._zoom !== e);
+                this._moveStart(o, i)._move(t, e)._moveEnd(o), this.fire("viewreset"), n && this.fire("load")
+            },
+            _moveStart: function(t, e) {
+                return t && this.fire("zoomstart"), e || this.fire("movestart"), this
+            },
+            _move: function(t, e, i, n) {
+                void 0 === e && (e = this._zoom);
+                var o = this._zoom !== e;
+                return this._zoom = e, this._lastCenter = t, this._pixelOrigin = this._getNewPixelOrigin(t), n ? i && i.pinch && this.fire("zoom", i) : ((o || i && i.pinch) && this.fire("zoom", i), this.fire("move", i)), this
             },
             _moveEnd: function(t) {
                 return t && this.fire("zoomend"), this.fire("moveend")
             },
             _stop: function() {
                 return r(this._flyToFrame), this._panAnim && this._panAnim.stop(), this
             },
@@ -1507,16 +1515,16 @@
                 this._enforcingBounds || this.panInsideBounds(this.options.maxBounds)
             },
             _checkIfLoaded: function() {
                 if (!this._loaded) throw new Error("Set map center and zoom first.")
             },
             _initEvents: function(t) {
                 this._targets = {};
-                var i = t ? E : S;
-                i((this._targets[h(this._container)] = this)._container, "click dblclick mousedown mouseup mouseover mouseout mousemove contextmenu keypress keydown keyup", this._handleDOMEvent, this), this.options.trackResize && i(window, "resize", this._onResize, this), P.any3d && this.options.transform3DLimit && (t ? this.off : this.on).call(this, "moveend", this._onMoveEnd)
+                var e = t ? E : S;
+                e((this._targets[h(this._container)] = this)._container, "click dblclick mousedown mouseup mouseover mouseout mousemove contextmenu keypress keydown keyup", this._handleDOMEvent, this), this.options.trackResize && e(window, "resize", this._onResize, this), b.any3d && this.options.transform3DLimit && (t ? this.off : this.on).call(this, "moveend", this._onMoveEnd)
             },
             _onResize: function() {
                 r(this._resizeRequest), this._resizeRequest = x(function() {
                     this.invalidateSize({
                         debounceMoveend: !0
                     })
                 }, this)
@@ -1524,358 +1532,361 @@
             _onScroll: function() {
                 this._container.scrollTop = 0, this._container.scrollLeft = 0
             },
             _onMoveEnd: function() {
                 var t = this._getMapPanePos();
                 Math.max(Math.abs(t.x), Math.abs(t.y)) >= this.options.transform3DLimit && this._resetView(this.getCenter(), this.getZoom())
             },
-            _findEventTargets: function(t, i) {
-                for (var e, n = [], o = "mouseout" === i || "mouseover" === i, s = t.target || t.srcElement, r = !1; s;) {
-                    if ((e = this._targets[h(s)]) && ("click" === i || "preclick" === i) && this._draggableMoved(e)) {
+            _findEventTargets: function(t, e) {
+                for (var i, n = [], o = "mouseout" === e || "mouseover" === e, s = t.target || t.srcElement, r = !1; s;) {
+                    if ((i = this._targets[h(s)]) && ("click" === e || "preclick" === e) && this._draggableMoved(i)) {
                         r = !0;
                         break
                     }
-                    if (e && e.listens(i, !0)) {
-                        if (o && !Hi(s, t)) break;
-                        if (n.push(e), o) break
+                    if (i && i.listens(e, !0)) {
+                        if (o && !Ue(s, t)) break;
+                        if (n.push(i), o) break
                     }
                     if (s === this._container) break;
                     s = s.parentNode
                 }
-                return n = n.length || r || o || !this.listens(i, !0) ? n : [this]
+                return n = n.length || r || o || !this.listens(e, !0) ? n : [this]
             },
             _isClickDisabled: function(t) {
-                for (; t !== this._container;) {
+                for (; t && t !== this._container;) {
                     if (t._leaflet_disable_click) return !0;
                     t = t.parentNode
                 }
             },
             _handleDOMEvent: function(t) {
-                var i, e = t.target || t.srcElement;
-                !this._loaded || e._leaflet_disable_events || "click" === t.type && this._isClickDisabled(e) || ("mousedown" === (i = t.type) && zi(e), this._fireDOMEvent(t, i))
+                var e, i = t.target || t.srcElement;
+                !this._loaded || i._leaflet_disable_events || "click" === t.type && this._isClickDisabled(i) || ("mousedown" === (e = t.type) && ze(i), this._fireDOMEvent(t, e))
             },
             _mouseEvents: ["click", "dblclick", "mouseover", "mouseout", "contextmenu"],
-            _fireDOMEvent: function(t, i, e) {
-                "click" === t.type && ((a = l({}, t)).type = "preclick", this._fireDOMEvent(a, a.type, e));
-                var n = this._findEventTargets(t, i);
-                if (e) {
-                    for (var o = [], s = 0; s < e.length; s++) e[s].listens(i, !0) && o.push(e[s]);
+            _fireDOMEvent: function(t, e, i) {
+                "click" === t.type && ((a = l({}, t)).type = "preclick", this._fireDOMEvent(a, a.type, i));
+                var n = this._findEventTargets(t, e);
+                if (i) {
+                    for (var o = [], s = 0; s < i.length; s++) i[s].listens(e, !0) && o.push(i[s]);
                     n = o.concat(n)
                 }
                 if (n.length) {
-                    "contextmenu" === i && B(t);
+                    "contextmenu" === e && k(t);
                     var r, a = n[0],
                         h = {
                             originalEvent: t
                         };
                     for ("keypress" !== t.type && "keydown" !== t.type && "keyup" !== t.type && (r = a.getLatLng && (!a._radius || a._radius <= 10), h.containerPoint = r ? this.latLngToContainerPoint(a.getLatLng()) : this.mouseEventToContainerPoint(t), h.layerPoint = this.containerPointToLayerPoint(h.containerPoint), h.latlng = r ? a.getLatLng() : this.layerPointToLatLng(h.layerPoint)), s = 0; s < n.length; s++)
-                        if (n[s].fire(i, h, !0), h.originalEvent._stopped || !1 === n[s].options.bubblingMouseEvents && -1 !== G(this._mouseEvents, i)) return
+                        if (n[s].fire(e, h, !0), h.originalEvent._stopped || !1 === n[s].options.bubblingMouseEvents && -1 !== K(this._mouseEvents, e)) return
                 }
             },
             _draggableMoved: function(t) {
                 return (t = t.dragging && t.dragging.enabled() ? t : this).dragging && t.dragging.moved() || this.boxZoom && this.boxZoom.moved()
             },
             _clearHandlers: function() {
-                for (var t = 0, i = this._handlers.length; t < i; t++) this._handlers[t].disable()
+                for (var t = 0, e = this._handlers.length; t < e; t++) this._handlers[t].disable()
             },
-            whenReady: function(t, i) {
-                return this._loaded ? t.call(i || this, {
+            whenReady: function(t, e) {
+                return this._loaded ? t.call(e || this, {
                     target: this
-                }) : this.on("load", t, i), this
+                }) : this.on("load", t, e), this
             },
             _getMapPanePos: function() {
-                return bi(this._mapPane) || new p(0, 0)
+                return Le(this._mapPane) || new p(0, 0)
             },
             _moved: function() {
                 var t = this._getMapPanePos();
                 return t && !t.equals([0, 0])
             },
-            _getTopLeftPoint: function(t, i) {
-                return (t && void 0 !== i ? this._getNewPixelOrigin(t, i) : this.getPixelOrigin()).subtract(this._getMapPanePos())
+            _getTopLeftPoint: function(t, e) {
+                return (t && void 0 !== e ? this._getNewPixelOrigin(t, e) : this.getPixelOrigin()).subtract(this._getMapPanePos())
             },
-            _getNewPixelOrigin: function(t, i) {
-                var e = this.getSize()._divideBy(2);
-                return this.project(t, i)._subtract(e)._add(this._getMapPanePos())._round()
-            },
-            _latLngToNewLayerPoint: function(t, i, e) {
-                e = this._getNewPixelOrigin(e, i);
-                return this.project(t, i)._subtract(e)
-            },
-            _latLngBoundsToNewLayerBounds: function(t, i, e) {
-                e = this._getNewPixelOrigin(e, i);
-                return f([this.project(t.getSouthWest(), i)._subtract(e), this.project(t.getNorthWest(), i)._subtract(e), this.project(t.getSouthEast(), i)._subtract(e), this.project(t.getNorthEast(), i)._subtract(e)])
+            _getNewPixelOrigin: function(t, e) {
+                var i = this.getSize()._divideBy(2);
+                return this.project(t, e)._subtract(i)._add(this._getMapPanePos())._round()
+            },
+            _latLngToNewLayerPoint: function(t, e, i) {
+                i = this._getNewPixelOrigin(i, e);
+                return this.project(t, e)._subtract(i)
+            },
+            _latLngBoundsToNewLayerBounds: function(t, e, i) {
+                i = this._getNewPixelOrigin(i, e);
+                return _([this.project(t.getSouthWest(), e)._subtract(i), this.project(t.getNorthWest(), e)._subtract(i), this.project(t.getSouthEast(), e)._subtract(i), this.project(t.getNorthEast(), e)._subtract(i)])
             },
             _getCenterLayerPoint: function() {
                 return this.containerPointToLayerPoint(this.getSize()._divideBy(2))
             },
             _getCenterOffset: function(t) {
                 return this.latLngToLayerPoint(t).subtract(this._getCenterLayerPoint())
             },
-            _limitCenter: function(t, i, e) {
-                if (!e) return t;
-                var n = this.project(t, i),
-                    o = this.getSize().divideBy(2),
-                    o = new m(n.subtract(o), n.add(o)),
-                    o = this._getBoundsOffset(o, e, i);
-                return o.round().equals([0, 0]) ? t : this.unproject(n.add(o), i)
-            },
-            _limitOffset: function(t, i) {
-                if (!i) return t;
-                var e = this.getPixelBounds(),
-                    e = new m(e.min.add(t), e.max.add(t));
-                return t.add(this._getBoundsOffset(e, i))
-            },
-            _getBoundsOffset: function(t, i, e) {
-                i = f(this.project(i.getNorthEast(), e), this.project(i.getSouthWest(), e)), e = i.min.subtract(t.min), i = i.max.subtract(t.max);
-                return new p(this._rebound(e.x, -i.x), this._rebound(e.y, -i.y))
+            _limitCenter: function(t, e, i) {
+                var n, o;
+                return !i || (n = this.project(t, e), o = this.getSize().divideBy(2), o = new f(n.subtract(o), n.add(o)), (o = this._getBoundsOffset(o, i, e)).round().equals([0, 0])) ? t : this.unproject(n.add(o), e)
+            },
+            _limitOffset: function(t, e) {
+                var i;
+                return e ? (i = new f((i = this.getPixelBounds()).min.add(t), i.max.add(t)), t.add(this._getBoundsOffset(i, e))) : t
+            },
+            _getBoundsOffset: function(t, e, i) {
+                e = _(this.project(e.getNorthEast(), i), this.project(e.getSouthWest(), i)), i = e.min.subtract(t.min), e = e.max.subtract(t.max);
+                return new p(this._rebound(i.x, -e.x), this._rebound(i.y, -e.y))
             },
-            _rebound: function(t, i) {
-                return 0 < t + i ? Math.round(t - i) / 2 : Math.max(0, Math.ceil(t)) - Math.max(0, Math.floor(i))
+            _rebound: function(t, e) {
+                return 0 < t + e ? Math.round(t - e) / 2 : Math.max(0, Math.ceil(t)) - Math.max(0, Math.floor(e))
             },
             _limitZoom: function(t) {
-                var i = this.getMinZoom(),
-                    e = this.getMaxZoom(),
-                    n = P.any3d ? this.options.zoomSnap : 1;
-                return n && (t = Math.round(t / n) * n), Math.max(i, Math.min(e, t))
+                var e = this.getMinZoom(),
+                    i = this.getMaxZoom(),
+                    n = b.any3d ? this.options.zoomSnap : 1;
+                return n && (t = Math.round(t / n) * n), Math.max(e, Math.min(i, t))
             },
             _onPanTransitionStep: function() {
                 this.fire("move")
             },
             _onPanTransitionEnd: function() {
-                M(this._mapPane, "leaflet-pan-anim"), this.fire("moveend")
+                z(this._mapPane, "leaflet-pan-anim"), this.fire("moveend")
             },
-            _tryAnimatedPan: function(t, i) {
+            _tryAnimatedPan: function(t, e) {
                 t = this._getCenterOffset(t)._trunc();
-                return !(!0 !== (i && i.animate) && !this.getSize().contains(t)) && (this.panBy(t, i), !0)
+                return !(!0 !== (e && e.animate) && !this.getSize().contains(t)) && (this.panBy(t, e), !0)
             },
             _createAnimProxy: function() {
-                var t = this._proxy = b("div", "leaflet-proxy leaflet-zoom-animated");
+                var t = this._proxy = P("div", "leaflet-proxy leaflet-zoom-animated");
                 this._panes.mapPane.appendChild(t), this.on("zoomanim", function(t) {
-                    var i = ui,
-                        e = this._proxy.style[i];
-                    Pi(this._proxy, this.project(t.center, t.zoom), this.getZoomScale(t.zoom, 1)), e === this._proxy.style[i] && this._animatingZoom && this._onZoomTransitionEnd()
+                    var e = ce,
+                        i = this._proxy.style[e];
+                    Pe(this._proxy, this.project(t.center, t.zoom), this.getZoomScale(t.zoom, 1)), i === this._proxy.style[e] && this._animatingZoom && this._onZoomTransitionEnd()
                 }, this), this.on("load moveend", this._animMoveEnd, this), this._on("unload", this._destroyAnimProxy, this)
             },
             _destroyAnimProxy: function() {
                 T(this._proxy), this.off("load moveend", this._animMoveEnd, this), delete this._proxy
             },
             _animMoveEnd: function() {
                 var t = this.getCenter(),
-                    i = this.getZoom();
-                Pi(this._proxy, this.project(t, i), this.getZoomScale(i, 1))
+                    e = this.getZoom();
+                Pe(this._proxy, this.project(t, e), this.getZoomScale(e, 1))
             },
             _catchTransitionEnd: function(t) {
                 this._animatingZoom && 0 <= t.propertyName.indexOf("transform") && this._onZoomTransitionEnd()
             },
             _nothingToAnimate: function() {
                 return !this._container.getElementsByClassName("leaflet-zoom-animated").length
             },
-            _tryAnimatedZoom: function(t, i, e) {
-                if (this._animatingZoom) return !0;
-                if (e = e || {}, !this._zoomAnimated || !1 === e.animate || this._nothingToAnimate() || Math.abs(i - this._zoom) > this.options.zoomAnimationThreshold) return !1;
-                var n = this.getZoomScale(i),
-                    n = this._getCenterOffset(t)._divideBy(1 - 1 / n);
-                return !(!0 !== e.animate && !this.getSize().contains(n)) && (x(function() {
-                    this._moveStart(!0, !1)._animateZoom(t, i, !0)
-                }, this), !0)
+            _tryAnimatedZoom: function(t, e, i) {
+                if (!this._animatingZoom) {
+                    if (i = i || {}, !this._zoomAnimated || !1 === i.animate || this._nothingToAnimate() || Math.abs(e - this._zoom) > this.options.zoomAnimationThreshold) return !1;
+                    var n = this.getZoomScale(e),
+                        n = this._getCenterOffset(t)._divideBy(1 - 1 / n);
+                    if (!0 !== i.animate && !this.getSize().contains(n)) return !1;
+                    x(function() {
+                        this._moveStart(!0, !1)._animateZoom(t, e, !0)
+                    }, this)
+                }
+                return !0
             },
-            _animateZoom: function(t, i, e, n) {
-                this._mapPane && (e && (this._animatingZoom = !0, this._animateToCenter = t, this._animateToZoom = i, z(this._mapPane, "leaflet-zoom-anim")), this.fire("zoomanim", {
+            _animateZoom: function(t, e, i, n) {
+                this._mapPane && (i && (this._animatingZoom = !0, this._animateToCenter = t, this._animateToZoom = e, M(this._mapPane, "leaflet-zoom-anim")), this.fire("zoomanim", {
                     center: t,
-                    zoom: i,
+                    zoom: e,
                     noUpdate: n
                 }), this._tempFireZoomEvent || (this._tempFireZoomEvent = this._zoom !== this._animateToZoom), this._move(this._animateToCenter, this._animateToZoom, void 0, !0), setTimeout(a(this._onZoomTransitionEnd, this), 250))
             },
             _onZoomTransitionEnd: function() {
-                this._animatingZoom && (this._mapPane && M(this._mapPane, "leaflet-zoom-anim"), this._animatingZoom = !1, this._move(this._animateToCenter, this._animateToZoom, void 0, !0), this._tempFireZoomEvent && this.fire("zoom"), delete this._tempFireZoomEvent, this.fire("move"), this._moveEnd(!0))
+                this._animatingZoom && (this._mapPane && z(this._mapPane, "leaflet-zoom-anim"), this._animatingZoom = !1, this._move(this._animateToCenter, this._animateToZoom, void 0, !0), this._tempFireZoomEvent && this.fire("zoom"), delete this._tempFireZoomEvent, this.fire("move"), this._moveEnd(!0))
             }
         });
 
-    function Fi(t) {
-        return new I(t)
+    function Ge(t, e) {
+        return new O(t, e)
+    }
+
+    function qe(t) {
+        return new B(t)
     }
-    var Ui, I = it.extend({
+    var Ke, B = e.extend({
             options: {
                 position: "topright"
             },
             initialize: function(t) {
                 c(this, t)
             },
             getPosition: function() {
                 return this.options.position
             },
             setPosition: function(t) {
-                var i = this._map;
-                return i && i.removeControl(this), this.options.position = t, i && i.addControl(this), this
+                var e = this._map;
+                return e && e.removeControl(this), this.options.position = t, e && e.addControl(this), this
             },
             getContainer: function() {
                 return this._container
             },
             addTo: function(t) {
                 this.remove(), this._map = t;
-                var i = this._container = this.onAdd(t),
-                    e = this.getPosition(),
-                    t = t._controlCorners[e];
-                return z(i, "leaflet-control"), -1 !== e.indexOf("bottom") ? t.insertBefore(i, t.firstChild) : t.appendChild(i), this._map.on("unload", this.remove, this), this
+                var e = this._container = this.onAdd(t),
+                    i = this.getPosition(),
+                    t = t._controlCorners[i];
+                return M(e, "leaflet-control"), -1 !== i.indexOf("bottom") ? t.insertBefore(e, t.firstChild) : t.appendChild(e), this._map.on("unload", this.remove, this), this
             },
             remove: function() {
                 return this._map && (T(this._container), this.onRemove && this.onRemove(this._map), this._map.off("unload", this.remove, this), this._map = null), this
             },
             _refocusOnMap: function(t) {
                 this._map && t && 0 < t.screenX && 0 < t.screenY && this._map.getContainer().focus()
             }
         }),
-        Vi = (A.include({
+        Ye = (O.include({
             addControl: function(t) {
                 return t.addTo(this), this
             },
             removeControl: function(t) {
                 return t.remove(), this
             },
             _initControlPos: function() {
-                var e = this._controlCorners = {},
+                var i = this._controlCorners = {},
                     n = "leaflet-",
-                    o = this._controlContainer = b("div", n + "control-container", this._container);
+                    o = this._controlContainer = P("div", n + "control-container", this._container);
 
-                function t(t, i) {
-                    e[t + i] = b("div", n + t + " " + n + i, o)
+                function t(t, e) {
+                    i[t + e] = P("div", n + t + " " + n + e, o)
                 }
                 t("top", "left"), t("top", "right"), t("bottom", "left"), t("bottom", "right")
             },
             _clearControlPos: function() {
                 for (var t in this._controlCorners) T(this._controlCorners[t]);
                 T(this._controlContainer), delete this._controlCorners, delete this._controlContainer
             }
-        }), I.extend({
+        }), B.extend({
             options: {
                 collapsed: !0,
                 position: "topright",
                 autoZIndex: !0,
                 hideSingleBase: !1,
                 sortLayers: !1,
-                sortFunction: function(t, i, e, n) {
-                    return e < n ? -1 : n < e ? 1 : 0
+                sortFunction: function(t, e, i, n) {
+                    return i < n ? -1 : n < i ? 1 : 0
                 }
             },
-            initialize: function(t, i, e) {
-                for (var n in c(this, e), this._layerControlInputs = [], this._layers = [], this._lastZIndex = 0, this._handlingClick = !1, t) this._addLayer(t[n], n);
-                for (n in i) this._addLayer(i[n], n, !0)
+            initialize: function(t, e, i) {
+                for (var n in c(this, i), this._layerControlInputs = [], this._layers = [], this._lastZIndex = 0, this._handlingClick = !1, t) this._addLayer(t[n], n);
+                for (n in e) this._addLayer(e[n], n, !0)
             },
             onAdd: function(t) {
                 this._initLayout(), this._update(), (this._map = t).on("zoomend", this._checkDisabledLayers, this);
-                for (var i = 0; i < this._layers.length; i++) this._layers[i].layer.on("add remove", this._onLayerChange, this);
+                for (var e = 0; e < this._layers.length; e++) this._layers[e].layer.on("add remove", this._onLayerChange, this);
                 return this._container
             },
             addTo: function(t) {
-                return I.prototype.addTo.call(this, t), this._expandIfNotCollapsed()
+                return B.prototype.addTo.call(this, t), this._expandIfNotCollapsed()
             },
             onRemove: function() {
                 this._map.off("zoomend", this._checkDisabledLayers, this);
                 for (var t = 0; t < this._layers.length; t++) this._layers[t].layer.off("add remove", this._onLayerChange, this)
             },
-            addBaseLayer: function(t, i) {
-                return this._addLayer(t, i), this._map ? this._update() : this
+            addBaseLayer: function(t, e) {
+                return this._addLayer(t, e), this._map ? this._update() : this
             },
-            addOverlay: function(t, i) {
-                return this._addLayer(t, i, !0), this._map ? this._update() : this
+            addOverlay: function(t, e) {
+                return this._addLayer(t, e, !0), this._map ? this._update() : this
             },
             removeLayer: function(t) {
                 t.off("add remove", this._onLayerChange, this);
                 t = this._getLayer(h(t));
                 return t && this._layers.splice(this._layers.indexOf(t), 1), this._map ? this._update() : this
             },
             expand: function() {
-                z(this._container, "leaflet-control-layers-expanded"), this._section.style.height = null;
+                M(this._container, "leaflet-control-layers-expanded"), this._section.style.height = null;
                 var t = this._map.getSize().y - (this._container.offsetTop + 50);
-                return t < this._section.clientHeight ? (z(this._section, "leaflet-control-layers-scrollbar"), this._section.style.height = t + "px") : M(this._section, "leaflet-control-layers-scrollbar"), this._checkDisabledLayers(), this
+                return t < this._section.clientHeight ? (M(this._section, "leaflet-control-layers-scrollbar"), this._section.style.height = t + "px") : z(this._section, "leaflet-control-layers-scrollbar"), this._checkDisabledLayers(), this
             },
             collapse: function() {
-                return M(this._container, "leaflet-control-layers-expanded"), this
+                return z(this._container, "leaflet-control-layers-expanded"), this
             },
             _initLayout: function() {
                 var t = "leaflet-control-layers",
-                    i = this._container = b("div", t),
-                    e = this.options.collapsed,
-                    n = (i.setAttribute("aria-haspopup", !0), Oi(i), Ii(i), this._section = b("section", t + "-list")),
-                    o = (e && (this._map.on("click", this.collapse, this), S(i, {
+                    e = this._container = P("div", t),
+                    i = this.options.collapsed,
+                    n = (e.setAttribute("aria-haspopup", !0), Ne(e), Re(e), this._section = P("section", t + "-list")),
+                    o = (i && (this._map.on("click", this.collapse, this), S(e, {
                         mouseenter: function() {
-                            S(n, "click", B), this.expand(), setTimeout(function() {
-                                E(n, "click", B)
+                            S(n, "click", k), this.expand(), setTimeout(function() {
+                                E(n, "click", k)
                             })
                         },
                         mouseleave: this.collapse
-                    }, this)), this._layersLink = b("a", t + "-toggle", i));
-                o.href = "#", o.title = "Layers", o.setAttribute("role", "button"), S(o, "click", B), S(o, "focus", this.expand, this), e || this.expand(), this._baseLayersList = b("div", t + "-base", n), this._separator = b("div", t + "-separator", n), this._overlaysList = b("div", t + "-overlays", n), i.appendChild(n)
+                    }, this)), this._layersLink = P("a", t + "-toggle", e));
+                o.href = "#", o.title = "Layers", o.setAttribute("role", "button"), S(o, "click", k), S(o, "focus", this.expand, this), i || this.expand(), this._baseLayersList = P("div", t + "-base", n), this._separator = P("div", t + "-separator", n), this._overlaysList = P("div", t + "-overlays", n), e.appendChild(n)
             },
             _getLayer: function(t) {
-                for (var i = 0; i < this._layers.length; i++)
-                    if (this._layers[i] && h(this._layers[i].layer) === t) return this._layers[i]
+                for (var e = 0; e < this._layers.length; e++)
+                    if (this._layers[e] && h(this._layers[e].layer) === t) return this._layers[e]
             },
-            _addLayer: function(t, i, e) {
+            _addLayer: function(t, e, i) {
                 this._map && t.on("add remove", this._onLayerChange, this), this._layers.push({
                     layer: t,
-                    name: i,
-                    overlay: e
-                }), this.options.sortLayers && this._layers.sort(a(function(t, i) {
-                    return this.options.sortFunction(t.layer, i.layer, t.name, i.name)
+                    name: e,
+                    overlay: i
+                }), this.options.sortLayers && this._layers.sort(a(function(t, e) {
+                    return this.options.sortFunction(t.layer, e.layer, t.name, e.name)
                 }, this)), this.options.autoZIndex && t.setZIndex && (this._lastZIndex++, t.setZIndex(this._lastZIndex)), this._expandIfNotCollapsed()
             },
             _update: function() {
-                if (!this._container) return this;
-                mi(this._baseLayersList), mi(this._overlaysList), this._layerControlInputs = [];
-                for (var t, i, e, n = 0, o = 0; o < this._layers.length; o++) e = this._layers[o], this._addItem(e), i = i || e.overlay, t = t || !e.overlay, n += e.overlay ? 0 : 1;
-                return this.options.hideSingleBase && (this._baseLayersList.style.display = (t = t && 1 < n) ? "" : "none"), this._separator.style.display = i && t ? "" : "none", this
+                if (this._container) {
+                    fe(this._baseLayersList), fe(this._overlaysList), this._layerControlInputs = [];
+                    for (var t, e, i, n = 0, o = 0; o < this._layers.length; o++) i = this._layers[o], this._addItem(i), e = e || i.overlay, t = t || !i.overlay, n += i.overlay ? 0 : 1;
+                    this.options.hideSingleBase && (this._baseLayersList.style.display = (t = t && 1 < n) ? "" : "none"), this._separator.style.display = e && t ? "" : "none"
+                }
+                return this
             },
             _onLayerChange: function(t) {
                 this._handlingClick || this._update();
-                var i = this._getLayer(h(t.target)),
-                    t = i.overlay ? "add" === t.type ? "overlayadd" : "overlayremove" : "add" === t.type ? "baselayerchange" : null;
-                t && this._map.fire(t, i)
-            },
-            _createRadioElement: function(t, i) {
-                t = '<input type="radio" class="leaflet-control-layers-selector" name="' + t + '"' + (i ? ' checked="checked"' : "") + "/>", i = document.createElement("div");
-                return i.innerHTML = t, i.firstChild
+                var e = this._getLayer(h(t.target)),
+                    t = e.overlay ? "add" === t.type ? "overlayadd" : "overlayremove" : "add" === t.type ? "baselayerchange" : null;
+                t && this._map.fire(t, e)
+            },
+            _createRadioElement: function(t, e) {
+                t = '<input type="radio" class="leaflet-control-layers-selector" name="' + t + '"' + (e ? ' checked="checked"' : "") + "/>", e = document.createElement("div");
+                return e.innerHTML = t, e.firstChild
             },
             _addItem: function(t) {
-                var i, e = document.createElement("label"),
+                var e, i = document.createElement("label"),
                     n = this._map.hasLayer(t.layer),
-                    n = (t.overlay ? ((i = document.createElement("input")).type = "checkbox", i.className = "leaflet-control-layers-selector", i.defaultChecked = n) : i = this._createRadioElement("leaflet-base-layers_" + h(this), n), this._layerControlInputs.push(i), i.layerId = h(t.layer), S(i, "click", this._onInputClick, this), document.createElement("span")),
+                    n = (t.overlay ? ((e = document.createElement("input")).type = "checkbox", e.className = "leaflet-control-layers-selector", e.defaultChecked = n) : e = this._createRadioElement("leaflet-base-layers_" + h(this), n), this._layerControlInputs.push(e), e.layerId = h(t.layer), S(e, "click", this._onInputClick, this), document.createElement("span")),
                     o = (n.innerHTML = " " + t.name, document.createElement("span"));
-                return e.appendChild(o), o.appendChild(i), o.appendChild(n), (t.overlay ? this._overlaysList : this._baseLayersList).appendChild(e), this._checkDisabledLayers(), e
+                return i.appendChild(o), o.appendChild(e), o.appendChild(n), (t.overlay ? this._overlaysList : this._baseLayersList).appendChild(i), this._checkDisabledLayers(), i
             },
             _onInputClick: function() {
-                var t, i, e = this._layerControlInputs,
+                var t, e, i = this._layerControlInputs,
                     n = [],
                     o = [];
                 this._handlingClick = !0;
-                for (var s = e.length - 1; 0 <= s; s--) t = e[s], i = this._getLayer(t.layerId).layer, t.checked ? n.push(i) : t.checked || o.push(i);
+                for (var s = i.length - 1; 0 <= s; s--) t = i[s], e = this._getLayer(t.layerId).layer, t.checked ? n.push(e) : t.checked || o.push(e);
                 for (s = 0; s < o.length; s++) this._map.hasLayer(o[s]) && this._map.removeLayer(o[s]);
                 for (s = 0; s < n.length; s++) this._map.hasLayer(n[s]) || this._map.addLayer(n[s]);
                 this._handlingClick = !1, this._refocusOnMap()
             },
             _checkDisabledLayers: function() {
-                for (var t, i, e = this._layerControlInputs, n = this._map.getZoom(), o = e.length - 1; 0 <= o; o--) t = e[o], i = this._getLayer(t.layerId).layer, t.disabled = void 0 !== i.options.minZoom && n < i.options.minZoom || void 0 !== i.options.maxZoom && n > i.options.maxZoom
+                for (var t, e, i = this._layerControlInputs, n = this._map.getZoom(), o = i.length - 1; 0 <= o; o--) t = i[o], e = this._getLayer(t.layerId).layer, t.disabled = void 0 !== e.options.minZoom && n < e.options.minZoom || void 0 !== e.options.maxZoom && n > e.options.maxZoom
             },
             _expandIfNotCollapsed: function() {
                 return this._map && !this.options.collapsed && this.expand(), this
             }
         })),
-        qi = I.extend({
+        Je = B.extend({
             options: {
                 position: "topleft",
                 zoomInText: '<span aria-hidden="true">+</span>',
                 zoomInTitle: "Zoom in",
                 zoomOutText: '<span aria-hidden="true">&#x2212;</span>',
                 zoomOutTitle: "Zoom out"
             },
             onAdd: function(t) {
-                var i = "leaflet-control-zoom",
-                    e = b("div", i + " leaflet-bar"),
+                var e = "leaflet-control-zoom",
+                    i = P("div", e + " leaflet-bar"),
                     n = this.options;
-                return this._zoomInButton = this._createButton(n.zoomInText, n.zoomInTitle, i + "-in", e, this._zoomIn), this._zoomOutButton = this._createButton(n.zoomOutText, n.zoomOutTitle, i + "-out", e, this._zoomOut), this._updateDisabled(), t.on("zoomend zoomlevelschange", this._updateDisabled, this), e
+                return this._zoomInButton = this._createButton(n.zoomInText, n.zoomInTitle, e + "-in", i, this._zoomIn), this._zoomOutButton = this._createButton(n.zoomOutText, n.zoomOutTitle, e + "-out", i, this._zoomOut), this._updateDisabled(), t.on("zoomend zoomlevelschange", this._updateDisabled, this), i
             },
             onRemove: function(t) {
                 t.off("zoomend zoomlevelschange", this._updateDisabled, this)
             },
             disable: function() {
                 return this._disabled = !0, this._updateDisabled(), this
             },
@@ -1884,83 +1895,83 @@
             },
             _zoomIn: function(t) {
                 !this._disabled && this._map._zoom < this._map.getMaxZoom() && this._map.zoomIn(this._map.options.zoomDelta * (t.shiftKey ? 3 : 1))
             },
             _zoomOut: function(t) {
                 !this._disabled && this._map._zoom > this._map.getMinZoom() && this._map.zoomOut(this._map.options.zoomDelta * (t.shiftKey ? 3 : 1))
             },
-            _createButton: function(t, i, e, n, o) {
-                e = b("a", e, n);
-                return e.innerHTML = t, e.href = "#", e.title = i, e.setAttribute("role", "button"), e.setAttribute("aria-label", i), Oi(e), S(e, "click", Ri), S(e, "click", o, this), S(e, "click", this._refocusOnMap, this), e
+            _createButton: function(t, e, i, n, o) {
+                i = P("a", i, n);
+                return i.innerHTML = t, i.href = "#", i.title = e, i.setAttribute("role", "button"), i.setAttribute("aria-label", e), Ne(i), S(i, "click", De), S(i, "click", o, this), S(i, "click", this._refocusOnMap, this), i
             },
             _updateDisabled: function() {
                 var t = this._map,
-                    i = "leaflet-disabled";
-                M(this._zoomInButton, i), M(this._zoomOutButton, i), this._zoomInButton.setAttribute("aria-disabled", "false"), this._zoomOutButton.setAttribute("aria-disabled", "false"), !this._disabled && t._zoom !== t.getMinZoom() || (z(this._zoomOutButton, i), this._zoomOutButton.setAttribute("aria-disabled", "true")), !this._disabled && t._zoom !== t.getMaxZoom() || (z(this._zoomInButton, i), this._zoomInButton.setAttribute("aria-disabled", "true"))
+                    e = "leaflet-disabled";
+                z(this._zoomInButton, e), z(this._zoomOutButton, e), this._zoomInButton.setAttribute("aria-disabled", "false"), this._zoomOutButton.setAttribute("aria-disabled", "false"), !this._disabled && t._zoom !== t.getMinZoom() || (M(this._zoomOutButton, e), this._zoomOutButton.setAttribute("aria-disabled", "true")), !this._disabled && t._zoom !== t.getMaxZoom() || (M(this._zoomInButton, e), this._zoomInButton.setAttribute("aria-disabled", "true"))
             }
         }),
-        Gi = (A.mergeOptions({
+        Xe = (O.mergeOptions({
             zoomControl: !0
-        }), A.addInitHook(function() {
-            this.options.zoomControl && (this.zoomControl = new qi, this.addControl(this.zoomControl))
-        }), I.extend({
+        }), O.addInitHook(function() {
+            this.options.zoomControl && (this.zoomControl = new Je, this.addControl(this.zoomControl))
+        }), B.extend({
             options: {
                 position: "bottomleft",
                 maxWidth: 100,
                 metric: !0,
                 imperial: !0
             },
             onAdd: function(t) {
-                var i = "leaflet-control-scale",
-                    e = b("div", i),
+                var e = "leaflet-control-scale",
+                    i = P("div", e),
                     n = this.options;
-                return this._addScales(n, i + "-line", e), t.on(n.updateWhenIdle ? "moveend" : "move", this._update, this), t.whenReady(this._update, this), e
+                return this._addScales(n, e + "-line", i), t.on(n.updateWhenIdle ? "moveend" : "move", this._update, this), t.whenReady(this._update, this), i
             },
             onRemove: function(t) {
                 t.off(this.options.updateWhenIdle ? "moveend" : "move", this._update, this)
             },
-            _addScales: function(t, i, e) {
-                t.metric && (this._mScale = b("div", i, e)), t.imperial && (this._iScale = b("div", i, e))
+            _addScales: function(t, e, i) {
+                t.metric && (this._mScale = P("div", e, i)), t.imperial && (this._iScale = P("div", e, i))
             },
             _update: function() {
                 var t = this._map,
-                    i = t.getSize().y / 2,
-                    t = t.distance(t.containerPointToLatLng([0, i]), t.containerPointToLatLng([this.options.maxWidth, i]));
+                    e = t.getSize().y / 2,
+                    t = t.distance(t.containerPointToLatLng([0, e]), t.containerPointToLatLng([this.options.maxWidth, e]));
                 this._updateScales(t)
             },
             _updateScales: function(t) {
                 this.options.metric && t && this._updateMetric(t), this.options.imperial && t && this._updateImperial(t)
             },
             _updateMetric: function(t) {
-                var i = this._getRoundNum(t);
-                this._updateScale(this._mScale, i < 1e3 ? i + " m" : i / 1e3 + " km", i / t)
+                var e = this._getRoundNum(t);
+                this._updateScale(this._mScale, e < 1e3 ? e + " m" : e / 1e3 + " km", e / t)
             },
             _updateImperial: function(t) {
-                var i, e, t = 3.2808399 * t;
-                5280 < t ? (e = this._getRoundNum(i = t / 5280), this._updateScale(this._iScale, e + " mi", e / i)) : (e = this._getRoundNum(t), this._updateScale(this._iScale, e + " ft", e / t))
+                var e, i, t = 3.2808399 * t;
+                5280 < t ? (i = this._getRoundNum(e = t / 5280), this._updateScale(this._iScale, i + " mi", i / e)) : (i = this._getRoundNum(t), this._updateScale(this._iScale, i + " ft", i / t))
             },
-            _updateScale: function(t, i, e) {
-                t.style.width = Math.round(this.options.maxWidth * e) + "px", t.innerHTML = i
+            _updateScale: function(t, e, i) {
+                t.style.width = Math.round(this.options.maxWidth * i) + "px", t.innerHTML = e
             },
             _getRoundNum: function(t) {
-                var i = Math.pow(10, (Math.floor(t) + "").length - 1),
-                    t = t / i;
-                return i * (t = 10 <= t ? 10 : 5 <= t ? 5 : 3 <= t ? 3 : 2 <= t ? 2 : 1)
+                var e = Math.pow(10, (Math.floor(t) + "").length - 1),
+                    t = t / e;
+                return e * (t = 10 <= t ? 10 : 5 <= t ? 5 : 3 <= t ? 3 : 2 <= t ? 2 : 1)
             }
         })),
-        Ki = I.extend({
+        $e = B.extend({
             options: {
                 position: "bottomright",
-                prefix: '<a href="https://leafletjs.com" title="A JavaScript library for interactive maps">' + (P.inlineSvg ? '<svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="12" height="8"><path fill="#4C7BE1" d="M0 0h12v4H0z"/><path fill="#FFD500" d="M0 4h12v3H0z"/><path fill="#E0BC00" d="M0 7h12v1H0z"/></svg> ' : "") + "Leaflet</a>"
+                prefix: '<a href="https://leafletjs.com" title="A JavaScript library for interactive maps">' + (b.inlineSvg ? '<svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" width="12" height="8" viewBox="0 0 12 8" class="leaflet-attribution-flag"><path fill="#4C7BE1" d="M0 0h12v4H0z"/><path fill="#FFD500" d="M0 4h12v3H0z"/><path fill="#E0BC00" d="M0 7h12v1H0z"/></svg> ' : "") + "Leaflet</a>"
             },
             initialize: function(t) {
                 c(this, t), this._attributions = {}
             },
             onAdd: function(t) {
-                for (var i in (t.attributionControl = this)._container = b("div", "leaflet-control-attribution"), Oi(this._container), t._layers) t._layers[i].getAttribution && this.addAttribution(t._layers[i].getAttribution());
+                for (var e in (t.attributionControl = this)._container = P("div", "leaflet-control-attribution"), Ne(this._container), t._layers) t._layers[e].getAttribution && this.addAttribution(t._layers[e].getAttribution());
                 return this._update(), t.on("layeradd", this._addAttribution, this), this._container
             },
             onRemove: function(t) {
                 t.off("layeradd", this._addAttribution, this)
             },
             _addAttribution: function(t) {
                 t.layer.getAttribution && (this.addAttribution(t.layer.getAttribution()), t.layer.once("remove", function() {
@@ -1974,249 +1985,285 @@
                 return t && (this._attributions[t] || (this._attributions[t] = 0), this._attributions[t]++, this._update()), this
             },
             removeAttribution: function(t) {
                 return t && this._attributions[t] && (this._attributions[t]--, this._update()), this
             },
             _update: function() {
                 if (this._map) {
-                    var t, i = [];
-                    for (t in this._attributions) this._attributions[t] && i.push(t);
-                    var e = [];
-                    this.options.prefix && e.push(this.options.prefix), i.length && e.push(i.join(", ")), this._container.innerHTML = e.join(' <span aria-hidden="true">|</span> ')
+                    var t, e = [];
+                    for (t in this._attributions) this._attributions[t] && e.push(t);
+                    var i = [];
+                    this.options.prefix && i.push(this.options.prefix), e.length && i.push(e.join(", ")), this._container.innerHTML = i.join(' <span aria-hidden="true">|</span> ')
                 }
             }
         }),
-        n = (A.mergeOptions({
+        o = (O.mergeOptions({
             attributionControl: !0
-        }), A.addInitHook(function() {
-            this.options.attributionControl && (new Ki).addTo(this)
-        }), I.Layers = Vi, I.Zoom = qi, I.Scale = Gi, I.Attribution = Ki, Fi.layers = function(t, i, e) {
-            return new Vi(t, i, e)
-        }, Fi.zoom = function(t) {
-            return new qi(t)
-        }, Fi.scale = function(t) {
-            return new Gi(t)
-        }, Fi.attribution = function(t) {
-            return new Ki(t)
-        }, it.extend({
+        }), O.addInitHook(function() {
+            this.options.attributionControl && (new $e).addTo(this)
+        }), B.Layers = Ye, B.Zoom = Je, B.Scale = Xe, B.Attribution = $e, qe.layers = function(t, e, i) {
+            return new Ye(t, e, i)
+        }, qe.zoom = function(t) {
+            return new Je(t)
+        }, qe.scale = function(t) {
+            return new Xe(t)
+        }, qe.attribution = function(t) {
+            return new $e(t)
+        }, e.extend({
             initialize: function(t) {
                 this._map = t
             },
             enable: function() {
                 return this._enabled || (this._enabled = !0, this.addHooks()), this
             },
             disable: function() {
                 return this._enabled && (this._enabled = !1, this.removeHooks()), this
             },
             enabled: function() {
                 return !!this._enabled
             }
         })),
-        ft = (n.addTo = function(t, i) {
-            return t.addHandler(i, this), this
+        ft = (o.addTo = function(t, e) {
+            return t.addHandler(e, this), this
         }, {
-            Events: i
+            Events: n
         }),
-        Yi = P.touch ? "touchstart mousedown" : "mousedown",
-        Xi = et.extend({
+        Qe = b.touch ? "touchstart mousedown" : "mousedown",
+        ti = it.extend({
             options: {
                 clickTolerance: 3
             },
-            initialize: function(t, i, e, n) {
-                c(this, n), this._element = t, this._dragStartTarget = i || t, this._preventOutline = e
+            initialize: function(t, e, i, n) {
+                c(this, n), this._element = t, this._dragStartTarget = e || t, this._preventOutline = i
             },
             enable: function() {
-                this._enabled || (S(this._dragStartTarget, Yi, this._onDown, this), this._enabled = !0)
+                this._enabled || (S(this._dragStartTarget, Qe, this._onDown, this), this._enabled = !0)
             },
             disable: function() {
-                this._enabled && (Xi._dragging === this && this.finishDrag(!0), E(this._dragStartTarget, Yi, this._onDown, this), this._enabled = !1, this._moved = !1)
+                this._enabled && (ti._dragging === this && this.finishDrag(!0), E(this._dragStartTarget, Qe, this._onDown, this), this._enabled = !1, this._moved = !1)
             },
             _onDown: function(t) {
-                var i, e;
-                this._enabled && (this._moved = !1, vi(this._element, "leaflet-zoom-anim") || (t.touches && 1 !== t.touches.length ? Xi._dragging === this && this.finishDrag() : Xi._dragging || t.shiftKey || 1 !== t.which && 1 !== t.button && !t.touches || ((Xi._dragging = this)._preventOutline && zi(this._element), Li(), ri(), this._moving || (this.fire("down"), e = t.touches ? t.touches[0] : t, i = Ci(this._element), this._startPoint = new p(e.clientX, e.clientY), this._startPos = bi(this._element), this._parentScale = Zi(i), e = "mousedown" === t.type, S(document, e ? "mousemove" : "touchmove", this._onMove, this), S(document, e ? "mouseup" : "touchend touchcancel", this._onUp, this)))))
+                var e, i;
+                this._enabled && (this._moved = !1, ye(this._element, "leaflet-zoom-anim") || (t.touches && 1 !== t.touches.length ? ti._dragging === this && this.finishDrag() : ti._dragging || t.shiftKey || 1 !== t.which && 1 !== t.button && !t.touches || ((ti._dragging = this)._preventOutline && ze(this._element), Te(), ae(), this._moving || (this.fire("down"), i = t.touches ? t.touches[0] : t, e = Ze(this._element), this._startPoint = new p(i.clientX, i.clientY), this._startPos = Le(this._element), this._parentScale = Se(e), i = "mousedown" === t.type, S(document, i ? "mousemove" : "touchmove", this._onMove, this), S(document, i ? "mouseup" : "touchend touchcancel", this._onUp, this)))))
             },
             _onMove: function(t) {
-                var i;
-                this._enabled && (t.touches && 1 < t.touches.length ? this._moved = !0 : !(i = new p((i = t.touches && 1 === t.touches.length ? t.touches[0] : t).clientX, i.clientY)._subtract(this._startPoint)).x && !i.y || Math.abs(i.x) + Math.abs(i.y) < this.options.clickTolerance || (i.x /= this._parentScale.x, i.y /= this._parentScale.y, B(t), this._moved || (this.fire("dragstart"), this._moved = !0, z(document.body, "leaflet-dragging"), this._lastTarget = t.target || t.srcElement, window.SVGElementInstance && this._lastTarget instanceof window.SVGElementInstance && (this._lastTarget = this._lastTarget.correspondingUseElement), z(this._lastTarget, "leaflet-drag-target")), this._newPos = this._startPos.add(i), this._moving = !0, this._lastEvent = t, this._updatePosition()))
+                var e;
+                this._enabled && (t.touches && 1 < t.touches.length ? this._moved = !0 : !(e = new p((e = t.touches && 1 === t.touches.length ? t.touches[0] : t).clientX, e.clientY)._subtract(this._startPoint)).x && !e.y || Math.abs(e.x) + Math.abs(e.y) < this.options.clickTolerance || (e.x /= this._parentScale.x, e.y /= this._parentScale.y, k(t), this._moved || (this.fire("dragstart"), this._moved = !0, M(document.body, "leaflet-dragging"), this._lastTarget = t.target || t.srcElement, window.SVGElementInstance && this._lastTarget instanceof window.SVGElementInstance && (this._lastTarget = this._lastTarget.correspondingUseElement), M(this._lastTarget, "leaflet-drag-target")), this._newPos = this._startPos.add(e), this._moving = !0, this._lastEvent = t, this._updatePosition()))
             },
             _updatePosition: function() {
                 var t = {
                     originalEvent: this._lastEvent
                 };
                 this.fire("predrag", t), Z(this._element, this._newPos), this.fire("drag", t)
             },
             _onUp: function() {
                 this._enabled && this.finishDrag()
             },
             finishDrag: function(t) {
-                M(document.body, "leaflet-dragging"), this._lastTarget && (M(this._lastTarget, "leaflet-drag-target"), this._lastTarget = null), E(document, "mousemove touchmove", this._onMove, this), E(document, "mouseup touchend touchcancel", this._onUp, this), Ti(), ai(), this._moved && this._moving && this.fire("dragend", {
+                z(document.body, "leaflet-dragging"), this._lastTarget && (z(this._lastTarget, "leaflet-drag-target"), this._lastTarget = null), E(document, "mousemove touchmove", this._onMove, this), E(document, "mouseup touchend touchcancel", this._onUp, this), Me(), he(), this._moved && this._moving && this.fire("dragend", {
                     noInertia: t,
                     distance: this._newPos.distanceTo(this._startPos)
-                }), this._moving = !1, Xi._dragging = !1
+                }), this._moving = !1, ti._dragging = !1
             }
         });
 
-    function Ji(t, i) {
-        if (!i || !t.length) return t.slice();
-        i *= i;
-        return t = function(t, i) {
-            var e = t.length,
-                n = new(typeof Uint8Array != void 0 + "" ? Uint8Array : Array)(e);
-            n[0] = n[e - 1] = 1,
-                function t(i, e, n, o, s) {
+    function ei(t, e) {
+        if (e && t.length) {
+            var i = t = function(t, e) {
+                    for (var i = [t[0]], n = 1, o = 0, s = t.length; n < s; n++)(function(t, e) {
+                        var i = e.x - t.x,
+                            e = e.y - t.y;
+                        return i * i + e * e
+                    })(t[n], t[o]) > e && (i.push(t[n]), o = n);
+                    o < s - 1 && i.push(t[s - 1]);
+                    return i
+                }(t, e = e * e),
+                n = i.length,
+                o = new(typeof Uint8Array != void 0 + "" ? Uint8Array : Array)(n);
+            o[0] = o[n - 1] = 1,
+                function t(e, i, n, o, s) {
                     var r, a, h, l = 0;
-                    for (a = o + 1; a <= s - 1; a++) h = ee(i[a], i[o], i[s], !0), l < h && (r = a, l = h);
-                    n < l && (e[r] = 1, t(i, e, n, o, r), t(i, e, n, r, s))
-                }(t, n, i, 0, e - 1);
-            var o, s = [];
-            for (o = 0; o < e; o++) n[o] && s.push(t[o]);
-            return s
-        }(t = function(t, i) {
-            for (var e = [t[0]], n = 1, o = 0, s = t.length; n < s; n++)(function(t, i) {
-                var e = i.x - t.x,
-                    i = i.y - t.y;
-                return e * e + i * i
-            })(t[n], t[o]) > i && (e.push(t[n]), o = n);
-            o < s - 1 && e.push(t[s - 1]);
-            return e
-        }(t, i), i)
+                    for (a = o + 1; a <= s - 1; a++) h = ri(e[a], e[o], e[s], !0), l < h && (r = a, l = h);
+                    n < l && (i[r] = 1, t(e, i, n, o, r), t(e, i, n, r, s))
+                }(i, o, e, 0, n - 1);
+            var s, r = [];
+            for (s = 0; s < n; s++) o[s] && r.push(i[s]);
+            return r
+        }
+        return t.slice()
     }
 
-    function $i(t, i, e) {
-        return Math.sqrt(ee(t, i, e, !0))
+    function ii(t, e, i) {
+        return Math.sqrt(ri(t, e, i, !0))
     }
 
-    function Qi(t, i, e, n, o) {
-        var s, r, a, h = n ? Ui : ie(t, e),
-            l = ie(i, e);
-        for (Ui = l;;) {
-            if (!(h | l)) return [t, i];
+    function ni(t, e, i, n, o) {
+        var s, r, a, h = n ? Ke : si(t, i),
+            l = si(e, i);
+        for (Ke = l;;) {
+            if (!(h | l)) return [t, e];
             if (h & l) return !1;
-            a = ie(r = te(t, i, s = h || l, e, o), e), s === h ? (t = r, h = a) : (i = r, l = a)
+            a = si(r = oi(t, e, s = h || l, i, o), i), s === h ? (t = r, h = a) : (e = r, l = a)
         }
     }
 
-    function te(t, i, e, n, o) {
-        var s, r, a = i.x - t.x,
-            i = i.y - t.y,
+    function oi(t, e, i, n, o) {
+        var s, r, a = e.x - t.x,
+            e = e.y - t.y,
             h = n.min,
             n = n.max;
-        return 8 & e ? (s = t.x + a * (n.y - t.y) / i, r = n.y) : 4 & e ? (s = t.x + a * (h.y - t.y) / i, r = h.y) : 2 & e ? (s = n.x, r = t.y + i * (n.x - t.x) / a) : 1 & e && (s = h.x, r = t.y + i * (h.x - t.x) / a), new p(s, r, o)
+        return 8 & i ? (s = t.x + a * (n.y - t.y) / e, r = n.y) : 4 & i ? (s = t.x + a * (h.y - t.y) / e, r = h.y) : 2 & i ? (s = n.x, r = t.y + e * (n.x - t.x) / a) : 1 & i && (s = h.x, r = t.y + e * (h.x - t.x) / a), new p(s, r, o)
     }
 
-    function ie(t, i) {
-        var e = 0;
-        return t.x < i.min.x ? e |= 1 : t.x > i.max.x && (e |= 2), t.y < i.min.y ? e |= 4 : t.y > i.max.y && (e |= 8), e
+    function si(t, e) {
+        var i = 0;
+        return t.x < e.min.x ? i |= 1 : t.x > e.max.x && (i |= 2), t.y < e.min.y ? i |= 4 : t.y > e.max.y && (i |= 8), i
     }
 
-    function ee(t, i, e, n) {
-        var o = i.x,
-            i = i.y,
-            s = e.x - o,
-            r = e.y - i,
+    function ri(t, e, i, n) {
+        var o = e.x,
+            e = e.y,
+            s = i.x - o,
+            r = i.y - e,
             a = s * s + r * r;
-        return 0 < a && (1 < (a = ((t.x - o) * s + (t.y - i) * r) / a) ? (o = e.x, i = e.y) : 0 < a && (o += s * a, i += r * a)), s = t.x - o, r = t.y - i, n ? s * s + r * r : new p(o, i)
+        return 0 < a && (1 < (a = ((t.x - o) * s + (t.y - e) * r) / a) ? (o = i.x, e = i.y) : 0 < a && (o += s * a, e += r * a)), s = t.x - o, r = t.y - e, n ? s * s + r * r : new p(o, e)
     }
 
-    function ne(t) {
+    function A(t) {
         return !d(t[0]) || "object" != typeof t[0][0] && void 0 !== t[0][0]
     }
 
-    function oe(t) {
-        return console.warn("Deprecated use of _flat, please use L.LineUtil.isFlat instead."), ne(t)
+    function ai(t) {
+        return console.warn("Deprecated use of _flat, please use L.LineUtil.isFlat instead."), A(t)
+    }
+
+    function hi(t, e) {
+        var i, n, o, s, r;
+        if (!t || 0 === t.length) throw new Error("latlngs not passed");
+        A(t) || (console.warn("latlngs are not flat! Only the first ring will be used"), t = t[0]);
+        var a, h = [];
+        for (a in t) h.push(e.project(w(t[a])));
+        for (var l = h.length, u = 0, c = 0; u < l - 1; u++) c += h[u].distanceTo(h[u + 1]) / 2;
+        if (0 === c) r = h[0];
+        else
+            for (i = u = 0; u < l - 1; u++)
+                if (n = h[u], o = h[u + 1], c < (i += s = n.distanceTo(o))) {
+                    r = [o.x - (s = (i - c) / s) * (o.x - n.x), o.y - s * (o.y - n.y)];
+                    break
+                } return e.unproject(m(r))
     }
     gt = {
         __proto__: null,
-        simplify: Ji,
-        pointToSegmentDistance: $i,
-        closestPointOnSegment: function(t, i, e) {
-            return ee(t, i, e)
-        },
-        clipSegment: Qi,
-        _getEdgeIntersection: te,
-        _getBitCode: ie,
-        _sqClosestPointOnSegment: ee,
-        isFlat: ne,
-        _flat: oe
+        simplify: ei,
+        pointToSegmentDistance: ii,
+        closestPointOnSegment: function(t, e, i) {
+            return ri(t, e, i)
+        },
+        clipSegment: ni,
+        _getEdgeIntersection: oi,
+        _getBitCode: si,
+        _sqClosestPointOnSegment: ri,
+        isFlat: A,
+        _flat: ai,
+        polylineCenter: hi
     };
 
-    function se(t, i, e) {
-        for (var n, o, s, r, a, h, l, u = [1, 4, 2, 8], c = 0, d = t.length; c < d; c++) t[c]._code = ie(t[c], i);
+    function li(t, e, i) {
+        for (var n, o, s, r, a, h, l, u = [1, 4, 2, 8], c = 0, d = t.length; c < d; c++) t[c]._code = si(t[c], e);
         for (s = 0; s < 4; s++) {
-            for (h = u[s], n = [], c = 0, o = (d = t.length) - 1; c < d; o = c++) r = t[c], a = t[o], r._code & h ? a._code & h || ((l = te(a, r, h, i, e))._code = ie(l, i), n.push(l)) : (a._code & h && ((l = te(a, r, h, i, e))._code = ie(l, i), n.push(l)), n.push(r));
+            for (h = u[s], n = [], c = 0, o = (d = t.length) - 1; c < d; o = c++) r = t[c], a = t[o], r._code & h ? a._code & h || ((l = oi(a, r, h, e, i))._code = si(l, e), n.push(l)) : (a._code & h && ((l = oi(a, r, h, e, i))._code = si(l, e), n.push(l)), n.push(r));
             t = n
         }
         return t
     }
+
+    function ui(t, e) {
+        var i, n, o, s, r, a;
+        if (!t || 0 === t.length) throw new Error("latlngs not passed");
+        A(t) || (console.warn("latlngs are not flat! Only the first ring will be used"), t = t[0]);
+        var h, l = [];
+        for (h in t) l.push(e.project(w(t[h])));
+        for (var u = l.length, c = s = r = 0, d = 0, _ = u - 1; d < u; _ = d++) i = l[d], n = l[_], o = i.y * n.x - n.y * i.x, s += (i.x + n.x) * o, r += (i.y + n.y) * o, c += 3 * o;
+        return a = 0 === c ? l[0] : [s / c, r / c], e.unproject(m(a))
+    }
+
+    function ci(t, e) {
+        return new pi(t, e)
+    }
+
+    function di(t, e) {
+        return new mi(t, e)
+    }
     var vt = {
             __proto__: null,
-            clipPolygon: se
+            clipPolygon: li,
+            polygonCenter: ui
         },
         yt = {
             project: function(t) {
                 return new p(t.lng, t.lat)
             },
             unproject: function(t) {
                 return new v(t.y, t.x)
             },
-            bounds: new m([-180, -90], [180, 90])
+            bounds: new f([-180, -90], [180, 90])
         },
         xt = {
             R: 6378137,
             R_MINOR: 6356752.314245179,
-            bounds: new m([-20037508.34279, -15496570.73972], [20037508.34279, 18764656.23138]),
+            bounds: new f([-20037508.34279, -15496570.73972], [20037508.34279, 18764656.23138]),
             project: function(t) {
-                var i = Math.PI / 180,
-                    e = this.R,
-                    n = t.lat * i,
-                    o = this.R_MINOR / e,
+                var e = Math.PI / 180,
+                    i = this.R,
+                    n = t.lat * e,
+                    o = this.R_MINOR / i,
                     o = Math.sqrt(1 - o * o),
                     s = o * Math.sin(n),
                     s = Math.tan(Math.PI / 4 - n / 2) / Math.pow((1 - s) / (1 + s), o / 2),
-                    n = -e * Math.log(Math.max(s, 1e-10));
-                return new p(t.lng * i * e, n)
+                    n = -i * Math.log(Math.max(s, 1e-10));
+                return new p(t.lng * e * i, n)
             },
             unproject: function(t) {
-                for (var i, e = 180 / Math.PI, n = this.R, o = this.R_MINOR / n, s = Math.sqrt(1 - o * o), r = Math.exp(-t.y / n), a = Math.PI / 2 - 2 * Math.atan(r), h = 0, l = .1; h < 15 && 1e-7 < Math.abs(l); h++) i = s * Math.sin(a), i = Math.pow((1 - i) / (1 + i), s / 2), a += l = Math.PI / 2 - 2 * Math.atan(r * i) - a;
-                return new v(a * e, t.x * e / n)
+                for (var e, i = 180 / Math.PI, n = this.R, o = this.R_MINOR / n, s = Math.sqrt(1 - o * o), r = Math.exp(-t.y / n), a = Math.PI / 2 - 2 * Math.atan(r), h = 0, l = .1; h < 15 && 1e-7 < Math.abs(l); h++) e = s * Math.sin(a), e = Math.pow((1 - e) / (1 + e), s / 2), a += l = Math.PI / 2 - 2 * Math.atan(r * e) - a;
+                return new v(a * i, t.x * i / n)
             }
         },
         wt = {
             __proto__: null,
             LonLat: yt,
             Mercator: xt,
             SphericalMercator: rt
         },
-        bt = l({}, st, {
+        Pt = l({}, st, {
             code: "EPSG:3395",
             projection: xt,
-            transformation: ht(Pt = .5 / (Math.PI * xt.R), .5, -Pt, .5)
+            transformation: ht(bt = .5 / (Math.PI * xt.R), .5, -bt, .5)
         }),
-        re = l({}, st, {
+        _i = l({}, st, {
             code: "EPSG:4326",
             projection: yt,
             transformation: ht(1 / 180, 1, -1 / 180, .5)
         }),
         Lt = l({}, ot, {
             projection: yt,
             transformation: ht(1, 0, -1, 0),
             scale: function(t) {
                 return Math.pow(2, t)
             },
             zoom: function(t) {
                 return Math.log(t) / Math.LN2
             },
-            distance: function(t, i) {
-                var e = i.lng - t.lng,
-                    i = i.lat - t.lat;
-                return Math.sqrt(e * e + i * i)
+            distance: function(t, e) {
+                var i = e.lng - t.lng,
+                    e = e.lat - t.lat;
+                return Math.sqrt(i * i + e * e)
             },
             infinite: !0
         }),
-        o = (ot.Earth = st, ot.EPSG3395 = bt, ot.EPSG3857 = lt, ot.EPSG900913 = ut, ot.EPSG4326 = re, ot.Simple = Lt, et.extend({
+        y = (ot.Earth = st, ot.EPSG3395 = Pt, ot.EPSG3857 = lt, ot.EPSG900913 = ut, ot.EPSG4326 = _i, ot.Simple = Lt, it.extend({
             options: {
                 pane: "overlayPane",
                 attribution: null,
                 bubblingMouseEvents: !0
             },
             addTo: function(t) {
                 return t.addLayer(this), this
@@ -2236,259 +2283,258 @@
             removeInteractiveTarget: function(t) {
                 return delete this._map._targets[h(t)], this
             },
             getAttribution: function() {
                 return this.options.attribution
             },
             _layerAdd: function(t) {
-                var i, e = t.target;
-                e.hasLayer(this) && (this._map = e, this._zoomAnimated = e._zoomAnimated, this.getEvents && (i = this.getEvents(), e.on(i, this), this.once("remove", function() {
-                    e.off(i, this)
-                }, this)), this.onAdd(e), this.fire("add"), e.fire("layeradd", {
+                var e, i = t.target;
+                i.hasLayer(this) && (this._map = i, this._zoomAnimated = i._zoomAnimated, this.getEvents && (e = this.getEvents(), i.on(e, this), this.once("remove", function() {
+                    i.off(e, this)
+                }, this)), this.onAdd(i), this.fire("add"), i.fire("layeradd", {
                     layer: this
                 }))
             }
         })),
-        ae = (A.include({
+        pi = (O.include({
             addLayer: function(t) {
-                if (!t._layerAdd) throw new Error("The provided object is not a Layer.");
-                var i = h(t);
-                return this._layers[i] || ((this._layers[i] = t)._mapToAdd = this, t.beforeAdd && t.beforeAdd(this), this.whenReady(t._layerAdd, t)), this
+                var e;
+                if (t._layerAdd) return e = h(t), this._layers[e] || ((this._layers[e] = t)._mapToAdd = this, t.beforeAdd && t.beforeAdd(this), this.whenReady(t._layerAdd, t)), this;
+                throw new Error("The provided object is not a Layer.")
             },
             removeLayer: function(t) {
-                var i = h(t);
-                return this._layers[i] && (this._loaded && t.onRemove(this), delete this._layers[i], this._loaded && (this.fire("layerremove", {
+                var e = h(t);
+                return this._layers[e] && (this._loaded && t.onRemove(this), delete this._layers[e], this._loaded && (this.fire("layerremove", {
                     layer: t
                 }), t.fire("remove")), t._map = t._mapToAdd = null), this
             },
             hasLayer: function(t) {
                 return h(t) in this._layers
             },
-            eachLayer: function(t, i) {
-                for (var e in this._layers) t.call(i, this._layers[e]);
+            eachLayer: function(t, e) {
+                for (var i in this._layers) t.call(e, this._layers[i]);
                 return this
             },
             _addLayers: function(t) {
-                for (var i = 0, e = (t = t ? d(t) ? t : [t] : []).length; i < e; i++) this.addLayer(t[i])
+                for (var e = 0, i = (t = t ? d(t) ? t : [t] : []).length; e < i; e++) this.addLayer(t[e])
             },
             _addZoomLimit: function(t) {
                 isNaN(t.options.maxZoom) && isNaN(t.options.minZoom) || (this._zoomBoundLayers[h(t)] = t, this._updateZoomLevels())
             },
             _removeZoomLimit: function(t) {
                 t = h(t);
                 this._zoomBoundLayers[t] && (delete this._zoomBoundLayers[t], this._updateZoomLevels())
             },
             _updateZoomLevels: function() {
-                var t, i = 1 / 0,
-                    e = -1 / 0,
+                var t, e = 1 / 0,
+                    i = -1 / 0,
                     n = this._getZoomSpan();
                 for (t in this._zoomBoundLayers) var o = this._zoomBoundLayers[t].options,
-                    i = void 0 === o.minZoom ? i : Math.min(i, o.minZoom),
-                    e = void 0 === o.maxZoom ? e : Math.max(e, o.maxZoom);
-                this._layersMaxZoom = e === -1 / 0 ? void 0 : e, this._layersMinZoom = i === 1 / 0 ? void 0 : i, n !== this._getZoomSpan() && this.fire("zoomlevelschange"), void 0 === this.options.maxZoom && this._layersMaxZoom && this.getZoom() > this._layersMaxZoom && this.setZoom(this._layersMaxZoom), void 0 === this.options.minZoom && this._layersMinZoom && this.getZoom() < this._layersMinZoom && this.setZoom(this._layersMinZoom)
-            }
-        }), o.extend({
-            initialize: function(t, i) {
-                var e, n;
-                if (c(this, i), this._layers = {}, t)
-                    for (e = 0, n = t.length; e < n; e++) this.addLayer(t[e])
+                    e = void 0 === o.minZoom ? e : Math.min(e, o.minZoom),
+                    i = void 0 === o.maxZoom ? i : Math.max(i, o.maxZoom);
+                this._layersMaxZoom = i === -1 / 0 ? void 0 : i, this._layersMinZoom = e === 1 / 0 ? void 0 : e, n !== this._getZoomSpan() && this.fire("zoomlevelschange"), void 0 === this.options.maxZoom && this._layersMaxZoom && this.getZoom() > this._layersMaxZoom && this.setZoom(this._layersMaxZoom), void 0 === this.options.minZoom && this._layersMinZoom && this.getZoom() < this._layersMinZoom && this.setZoom(this._layersMinZoom)
+            }
+        }), y.extend({
+            initialize: function(t, e) {
+                var i, n;
+                if (c(this, e), this._layers = {}, t)
+                    for (i = 0, n = t.length; i < n; i++) this.addLayer(t[i])
             },
             addLayer: function(t) {
-                var i = this.getLayerId(t);
-                return this._layers[i] = t, this._map && this._map.addLayer(t), this
+                var e = this.getLayerId(t);
+                return this._layers[e] = t, this._map && this._map.addLayer(t), this
             },
             removeLayer: function(t) {
                 t = t in this._layers ? t : this.getLayerId(t);
                 return this._map && this._layers[t] && this._map.removeLayer(this._layers[t]), delete this._layers[t], this
             },
             hasLayer: function(t) {
                 return ("number" == typeof t ? t : this.getLayerId(t)) in this._layers
             },
             clearLayers: function() {
                 return this.eachLayer(this.removeLayer, this)
             },
             invoke: function(t) {
-                var i, e, n = Array.prototype.slice.call(arguments, 1);
-                for (i in this._layers)(e = this._layers[i])[t] && e[t].apply(e, n);
+                var e, i, n = Array.prototype.slice.call(arguments, 1);
+                for (e in this._layers)(i = this._layers[e])[t] && i[t].apply(i, n);
                 return this
             },
             onAdd: function(t) {
                 this.eachLayer(t.addLayer, t)
             },
             onRemove: function(t) {
                 this.eachLayer(t.removeLayer, t)
             },
-            eachLayer: function(t, i) {
-                for (var e in this._layers) t.call(i, this._layers[e]);
+            eachLayer: function(t, e) {
+                for (var i in this._layers) t.call(e, this._layers[i]);
                 return this
             },
             getLayer: function(t) {
                 return this._layers[t]
             },
             getLayers: function() {
                 var t = [];
                 return this.eachLayer(t.push, t), t
             },
             setZIndex: function(t) {
                 return this.invoke("setZIndex", t)
             },
             getLayerId: h
         })),
-        he = ae.extend({
+        mi = pi.extend({
             addLayer: function(t) {
-                return this.hasLayer(t) ? this : (t.addEventParent(this), ae.prototype.addLayer.call(this, t), this.fire("layeradd", {
+                return this.hasLayer(t) ? this : (t.addEventParent(this), pi.prototype.addLayer.call(this, t), this.fire("layeradd", {
                     layer: t
                 }))
             },
             removeLayer: function(t) {
-                return this.hasLayer(t) ? ((t = t in this._layers ? this._layers[t] : t).removeEventParent(this), ae.prototype.removeLayer.call(this, t), this.fire("layerremove", {
+                return this.hasLayer(t) ? ((t = t in this._layers ? this._layers[t] : t).removeEventParent(this), pi.prototype.removeLayer.call(this, t), this.fire("layerremove", {
                     layer: t
                 })) : this
             },
             setStyle: function(t) {
                 return this.invoke("setStyle", t)
             },
             bringToFront: function() {
                 return this.invoke("bringToFront")
             },
             bringToBack: function() {
                 return this.invoke("bringToBack")
             },
             getBounds: function() {
-                var t, i = new s;
+                var t, e = new s;
                 for (t in this._layers) {
-                    var e = this._layers[t];
-                    i.extend(e.getBounds ? e.getBounds() : e.getLatLng())
+                    var i = this._layers[t];
+                    e.extend(i.getBounds ? i.getBounds() : i.getLatLng())
                 }
-                return i
+                return e
             }
         }),
-        le = it.extend({
+        fi = e.extend({
             options: {
                 popupAnchor: [0, 0],
                 tooltipAnchor: [0, 0],
                 crossOrigin: !1
             },
             initialize: function(t) {
                 c(this, t)
             },
             createIcon: function(t) {
                 return this._createIcon("icon", t)
             },
             createShadow: function(t) {
                 return this._createIcon("shadow", t)
             },
-            _createIcon: function(t, i) {
-                var e = this._getIconUrl(t);
-                if (!e) {
-                    if ("icon" === t) throw new Error("iconUrl not set in Icon options (see the docs).");
-                    return null
-                }
-                e = this._createImg(e, i && "IMG" === i.tagName ? i : null);
-                return this._setIconStyles(e, t), !this.options.crossOrigin && "" !== this.options.crossOrigin || (e.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), e
+            _createIcon: function(t, e) {
+                var i = this._getIconUrl(t);
+                if (i) return i = this._createImg(i, e && "IMG" === e.tagName ? e : null), this._setIconStyles(i, t), !this.options.crossOrigin && "" !== this.options.crossOrigin || (i.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), i;
+                if ("icon" === t) throw new Error("iconUrl not set in Icon options (see the docs).");
+                return null
             },
-            _setIconStyles: function(t, i) {
-                var e = this.options,
-                    n = e[i + "Size"],
-                    n = _(n = "number" == typeof n ? [n, n] : n),
-                    o = _("shadow" === i && e.shadowAnchor || e.iconAnchor || n && n.divideBy(2, !0));
-                t.className = "leaflet-marker-" + i + " " + (e.className || ""), o && (t.style.marginLeft = -o.x + "px", t.style.marginTop = -o.y + "px"), n && (t.style.width = n.x + "px", t.style.height = n.y + "px")
+            _setIconStyles: function(t, e) {
+                var i = this.options,
+                    n = i[e + "Size"],
+                    n = m(n = "number" == typeof n ? [n, n] : n),
+                    o = m("shadow" === e && i.shadowAnchor || i.iconAnchor || n && n.divideBy(2, !0));
+                t.className = "leaflet-marker-" + e + " " + (i.className || ""), o && (t.style.marginLeft = -o.x + "px", t.style.marginTop = -o.y + "px"), n && (t.style.width = n.x + "px", t.style.height = n.y + "px")
             },
-            _createImg: function(t, i) {
-                return (i = i || document.createElement("img")).src = t, i
+            _createImg: function(t, e) {
+                return (e = e || document.createElement("img")).src = t, e
             },
             _getIconUrl: function(t) {
-                return P.retina && this.options[t + "RetinaUrl"] || this.options[t + "Url"]
+                return b.retina && this.options[t + "RetinaUrl"] || this.options[t + "Url"]
             }
         });
-    var ue = le.extend({
+
+    function gi(t) {
+        return new fi(t)
+    }
+    var vi = fi.extend({
             options: {
                 iconUrl: "marker-icon.png",
                 iconRetinaUrl: "marker-icon-2x.png",
                 shadowUrl: "marker-shadow.png",
                 iconSize: [25, 41],
                 iconAnchor: [12, 41],
                 popupAnchor: [1, -34],
                 tooltipAnchor: [16, -28],
                 shadowSize: [41, 41]
             },
             _getIconUrl: function(t) {
-                return "string" != typeof ue.imagePath && (ue.imagePath = this._detectIconPath()), (this.options.imagePath || ue.imagePath) + le.prototype._getIconUrl.call(this, t)
+                return "string" != typeof vi.imagePath && (vi.imagePath = this._detectIconPath()), (this.options.imagePath || vi.imagePath) + fi.prototype._getIconUrl.call(this, t)
             },
             _stripUrl: function(t) {
-                function i(t, i, e) {
-                    return (i = i.exec(t)) && i[e]
+                function e(t, e, i) {
+                    return (e = e.exec(t)) && e[i]
                 }
-                return (t = i(t, /^url\((['"])?(.+)\1\)$/, 2)) && i(t, /^(.*)marker-icon\.png$/, 1)
+                return (t = e(t, /^url\((['"])?(.+)\1\)$/, 2)) && e(t, /^(.*)marker-icon\.png$/, 1)
             },
             _detectIconPath: function() {
-                var t = b("div", "leaflet-default-icon-path", document.body),
-                    i = pi(t, "background-image") || pi(t, "backgroundImage");
-                if (document.body.removeChild(t), i = this._stripUrl(i)) return i;
-                t = document.querySelector('link[href$="leaflet.css"]');
-                return t ? t.href.substring(0, t.href.length - "leaflet.css".length - 1) : ""
+                var t = P("div", "leaflet-default-icon-path", document.body),
+                    e = me(t, "background-image") || me(t, "backgroundImage");
+                return document.body.removeChild(t), (e = this._stripUrl(e)) ? e : (t = document.querySelector('link[href$="leaflet.css"]')) ? t.href.substring(0, t.href.length - "leaflet.css".length - 1) : ""
             }
         }),
-        ce = n.extend({
+        yi = o.extend({
             initialize: function(t) {
                 this._marker = t
             },
             addHooks: function() {
                 var t = this._marker._icon;
-                this._draggable || (this._draggable = new Xi(t, t, !0)), this._draggable.on({
+                this._draggable || (this._draggable = new ti(t, t, !0)), this._draggable.on({
                     dragstart: this._onDragStart,
                     predrag: this._onPreDrag,
                     drag: this._onDrag,
                     dragend: this._onDragEnd
-                }, this).enable(), z(t, "leaflet-marker-draggable")
+                }, this).enable(), M(t, "leaflet-marker-draggable")
             },
             removeHooks: function() {
                 this._draggable.off({
                     dragstart: this._onDragStart,
                     predrag: this._onPreDrag,
                     drag: this._onDrag,
                     dragend: this._onDragEnd
-                }, this).disable(), this._marker._icon && M(this._marker._icon, "leaflet-marker-draggable")
+                }, this).disable(), this._marker._icon && z(this._marker._icon, "leaflet-marker-draggable")
             },
             moved: function() {
                 return this._draggable && this._draggable._moved
             },
             _adjustPan: function(t) {
-                var i = this._marker,
-                    e = i._map,
+                var e = this._marker,
+                    i = e._map,
                     n = this._marker.options.autoPanSpeed,
                     o = this._marker.options.autoPanPadding,
-                    s = bi(i._icon),
-                    r = e.getPixelBounds(),
-                    a = e.getPixelOrigin(),
-                    a = f(r.min._subtract(a).add(o), r.max._subtract(a).subtract(o));
-                a.contains(s) || (o = _((Math.max(a.max.x, s.x) - a.max.x) / (r.max.x - a.max.x) - (Math.min(a.min.x, s.x) - a.min.x) / (r.min.x - a.min.x), (Math.max(a.max.y, s.y) - a.max.y) / (r.max.y - a.max.y) - (Math.min(a.min.y, s.y) - a.min.y) / (r.min.y - a.min.y)).multiplyBy(n), e.panBy(o, {
+                    s = Le(e._icon),
+                    r = i.getPixelBounds(),
+                    a = i.getPixelOrigin(),
+                    a = _(r.min._subtract(a).add(o), r.max._subtract(a).subtract(o));
+                a.contains(s) || (o = m((Math.max(a.max.x, s.x) - a.max.x) / (r.max.x - a.max.x) - (Math.min(a.min.x, s.x) - a.min.x) / (r.min.x - a.min.x), (Math.max(a.max.y, s.y) - a.max.y) / (r.max.y - a.max.y) - (Math.min(a.min.y, s.y) - a.min.y) / (r.min.y - a.min.y)).multiplyBy(n), i.panBy(o, {
                     animate: !1
-                }), this._draggable._newPos._add(o), this._draggable._startPos._add(o), Z(i._icon, this._draggable._newPos), this._onDrag(t), this._panRequest = x(this._adjustPan.bind(this, t)))
+                }), this._draggable._newPos._add(o), this._draggable._startPos._add(o), Z(e._icon, this._draggable._newPos), this._onDrag(t), this._panRequest = x(this._adjustPan.bind(this, t)))
             },
             _onDragStart: function() {
                 this._oldLatLng = this._marker.getLatLng(), this._marker.closePopup && this._marker.closePopup(), this._marker.fire("movestart").fire("dragstart")
             },
             _onPreDrag: function(t) {
                 this._marker.options.autoPan && (r(this._panRequest), this._panRequest = x(this._adjustPan.bind(this, t)))
             },
             _onDrag: function(t) {
-                var i = this._marker,
-                    e = i._shadow,
-                    n = bi(i._icon),
-                    o = i._map.layerPointToLatLng(n);
-                e && Z(e, n), i._latlng = o, t.latlng = o, t.oldLatLng = this._oldLatLng, i.fire("move", t).fire("drag", t)
+                var e = this._marker,
+                    i = e._shadow,
+                    n = Le(e._icon),
+                    o = e._map.layerPointToLatLng(n);
+                i && Z(i, n), e._latlng = o, t.latlng = o, t.oldLatLng = this._oldLatLng, e.fire("move", t).fire("drag", t)
             },
             _onDragEnd: function(t) {
                 r(this._panRequest), delete this._oldLatLng, this._marker.fire("moveend").fire("dragend", t)
             }
         }),
-        de = o.extend({
+        xi = y.extend({
             options: {
-                icon: new ue,
+                icon: new vi,
                 interactive: !0,
                 keyboard: !0,
                 title: "",
                 alt: "Marker",
                 zIndexOffset: 0,
                 opacity: 1,
                 riseOnHover: !1,
@@ -2498,16 +2544,16 @@
                 bubblingMouseEvents: !1,
                 autoPanOnFocus: !0,
                 draggable: !1,
                 autoPan: !1,
                 autoPanPadding: [50, 50],
                 autoPanSpeed: 10
             },
-            initialize: function(t, i) {
-                c(this, i), this._latlng = w(t)
+            initialize: function(t, e) {
+                c(this, e), this._latlng = w(t)
             },
             onAdd: function(t) {
                 this._zoomAnimated = this._zoomAnimated && t.options.markerZoomAnimation, this._zoomAnimated && t.on("zoomanim", this._animateZoom, this), this._initIcon(), this.update()
             },
             onRemove: function(t) {
                 this.dragging && this.dragging.enabled() && (this.options.draggable = !0, this.dragging.removeHooks()), delete this.dragging, this._zoomAnimated && t.off("zoomanim", this._animateZoom, this), this._removeIcon(), this._removeShadow()
             },
@@ -2517,17 +2563,17 @@
                     viewreset: this.update
                 }
             },
             getLatLng: function() {
                 return this._latlng
             },
             setLatLng: function(t) {
-                var i = this._latlng;
+                var e = this._latlng;
                 return this._latlng = w(t), this.update(), this.fire("move", {
-                    oldLatLng: i,
+                    oldLatLng: e,
                     latlng: this._latlng
                 })
             },
             setZIndexOffset: function(t) {
                 return this.options.zIndexOffset = t, this.update()
             },
             getIcon: function() {
@@ -2541,23 +2587,23 @@
             },
             update: function() {
                 var t;
                 return this._icon && this._map && (t = this._map.latLngToLayerPoint(this._latlng).round(), this._setPos(t)), this
             },
             _initIcon: function() {
                 var t = this.options,
-                    i = "leaflet-zoom-" + (this._zoomAnimated ? "animated" : "hide"),
-                    e = t.icon.createIcon(this._icon),
+                    e = "leaflet-zoom-" + (this._zoomAnimated ? "animated" : "hide"),
+                    i = t.icon.createIcon(this._icon),
                     n = !1,
-                    e = (e !== this._icon && (this._icon && this._removeIcon(), n = !0, t.title && (e.title = t.title), "IMG" === e.tagName && (e.alt = t.alt || "")), z(e, i), t.keyboard && (e.tabIndex = "0", e.setAttribute("role", "button")), this._icon = e, t.riseOnHover && this.on({
+                    i = (i !== this._icon && (this._icon && this._removeIcon(), n = !0, t.title && (i.title = t.title), "IMG" === i.tagName && (i.alt = t.alt || "")), M(i, e), t.keyboard && (i.tabIndex = "0", i.setAttribute("role", "button")), this._icon = i, t.riseOnHover && this.on({
                         mouseover: this._bringToFront,
                         mouseout: this._resetZIndex
-                    }), this.options.autoPanOnFocus && S(e, "focus", this._panOnFocus, this), t.icon.createShadow(this._shadow)),
+                    }), this.options.autoPanOnFocus && S(i, "focus", this._panOnFocus, this), t.icon.createShadow(this._shadow)),
                     o = !1;
-                e !== this._shadow && (this._removeShadow(), o = !0), e && (z(e, i), e.alt = ""), this._shadow = e, t.opacity < 1 && this._updateOpacity(), n && this.getPane().appendChild(this._icon), this._initInteraction(), e && o && this.getPane(t.shadowPane).appendChild(this._shadow)
+                i !== this._shadow && (this._removeShadow(), o = !0), i && (M(i, e), i.alt = ""), this._shadow = i, t.opacity < 1 && this._updateOpacity(), n && this.getPane().appendChild(this._icon), this._initInteraction(), i && o && this.getPane(t.shadowPane).appendChild(this._shadow)
             },
             _removeIcon: function() {
                 this.options.riseOnHover && this.off({
                     mouseover: this._bringToFront,
                     mouseout: this._resetZIndex
                 }), this.options.autoPanOnFocus && E(this._icon, "focus", this._panOnFocus, this), T(this._icon), this.removeInteractiveTarget(this._icon), this._icon = null
             },
@@ -2572,15 +2618,15 @@
             },
             _animateZoom: function(t) {
                 t = this._map._latLngToNewLayerPoint(this._latlng, t.zoom, t.center).round();
                 this._setPos(t)
             },
             _initInteraction: function() {
                 var t;
-                this.options.interactive && (z(this._icon, "leaflet-interactive"), this.addInteractiveTarget(this._icon), ce && (t = this.options.draggable, this.dragging && (t = this.dragging.enabled(), this.dragging.disable()), this.dragging = new ce(this), t && this.dragging.enable()))
+                this.options.interactive && (M(this._icon, "leaflet-interactive"), this.addInteractiveTarget(this._icon), yi && (t = this.options.draggable, this.dragging && (t = this.dragging.enabled(), this.dragging.disable()), this.dragging = new yi(this), t && this.dragging.enable()))
             },
             setOpacity: function(t) {
                 return this.options.opacity = t, this._map && this._updateOpacity(), this
             },
             _updateOpacity: function() {
                 var t = this.options.opacity;
                 this._icon && C(this._icon, t), this._shadow && C(this._shadow, t)
@@ -2588,28 +2634,32 @@
             _bringToFront: function() {
                 this._updateZIndex(this.options.riseOffset)
             },
             _resetZIndex: function() {
                 this._updateZIndex(0)
             },
             _panOnFocus: function() {
-                var t, i, e = this._map;
-                e && (t = (i = this.options.icon.options).iconSize ? _(i.iconSize) : _(0, 0), i = i.iconAnchor ? _(i.iconAnchor) : _(0, 0), e.panInside(this._latlng, {
-                    paddingTopLeft: i,
-                    paddingBottomRight: t.subtract(i)
+                var t, e, i = this._map;
+                i && (t = (e = this.options.icon.options).iconSize ? m(e.iconSize) : m(0, 0), e = e.iconAnchor ? m(e.iconAnchor) : m(0, 0), i.panInside(this._latlng, {
+                    paddingTopLeft: e,
+                    paddingBottomRight: t.subtract(e)
                 }))
             },
             _getPopupAnchor: function() {
                 return this.options.icon.options.popupAnchor
             },
             _getTooltipAnchor: function() {
                 return this.options.icon.options.tooltipAnchor
             }
         });
-    var _e = o.extend({
+
+    function wi(t, e) {
+        return new xi(t, e)
+    }
+    var bi = y.extend({
             options: {
                 stroke: !0,
                 color: "#3388ff",
                 weight: 3,
                 opacity: 1,
                 lineCap: "round",
                 lineJoin: "round",
@@ -2649,418 +2699,429 @@
             _reset: function() {
                 this._project(), this._update()
             },
             _clickTolerance: function() {
                 return (this.options.stroke ? this.options.weight / 2 : 0) + (this._renderer.options.tolerance || 0)
             }
         }),
-        pe = _e.extend({
+        Pi = bi.extend({
             options: {
                 fill: !0,
                 radius: 10
             },
-            initialize: function(t, i) {
-                c(this, i), this._latlng = w(t), this._radius = this.options.radius
+            initialize: function(t, e) {
+                c(this, e), this._latlng = w(t), this._radius = this.options.radius
             },
             setLatLng: function(t) {
-                var i = this._latlng;
+                var e = this._latlng;
                 return this._latlng = w(t), this.redraw(), this.fire("move", {
-                    oldLatLng: i,
+                    oldLatLng: e,
                     latlng: this._latlng
                 })
             },
             getLatLng: function() {
                 return this._latlng
             },
             setRadius: function(t) {
                 return this.options.radius = this._radius = t, this.redraw()
             },
             getRadius: function() {
                 return this._radius
             },
             setStyle: function(t) {
-                var i = t && t.radius || this._radius;
-                return _e.prototype.setStyle.call(this, t), this.setRadius(i), this
+                var e = t && t.radius || this._radius;
+                return bi.prototype.setStyle.call(this, t), this.setRadius(e), this
             },
             _project: function() {
                 this._point = this._map.latLngToLayerPoint(this._latlng), this._updateBounds()
             },
             _updateBounds: function() {
                 var t = this._radius,
-                    i = this._radiusY || t,
-                    e = this._clickTolerance(),
-                    t = [t + e, i + e];
-                this._pxBounds = new m(this._point.subtract(t), this._point.add(t))
+                    e = this._radiusY || t,
+                    i = this._clickTolerance(),
+                    t = [t + i, e + i];
+                this._pxBounds = new f(this._point.subtract(t), this._point.add(t))
             },
             _update: function() {
                 this._map && this._updatePath()
             },
             _updatePath: function() {
                 this._renderer._updateCircle(this)
             },
             _empty: function() {
                 return this._radius && !this._renderer._bounds.intersects(this._pxBounds)
             },
             _containsPoint: function(t) {
                 return t.distanceTo(this._point) <= this._radius + this._clickTolerance()
             }
         });
-    var me = pe.extend({
-        initialize: function(t, i, e) {
-            if (c(this, i = "number" == typeof i ? l({}, e, {
-                    radius: i
-                }) : i), this._latlng = w(t), isNaN(this.options.radius)) throw new Error("Circle radius cannot be NaN");
+
+    function Li(t, e) {
+        return new Pi(t, e)
+    }
+    var Ti = Pi.extend({
+        initialize: function(t, e, i) {
+            if (c(this, e = "number" == typeof e ? l({}, i, {
+                    radius: e
+                }) : e), this._latlng = w(t), isNaN(this.options.radius)) throw new Error("Circle radius cannot be NaN");
             this._mRadius = this.options.radius
         },
         setRadius: function(t) {
             return this._mRadius = t, this.redraw()
         },
         getRadius: function() {
             return this._mRadius
         },
         getBounds: function() {
             var t = [this._radius, this._radiusY || this._radius];
             return new s(this._map.layerPointToLatLng(this._point.subtract(t)), this._map.layerPointToLatLng(this._point.add(t)))
         },
-        setStyle: _e.prototype.setStyle,
+        setStyle: bi.prototype.setStyle,
         _project: function() {
-            var t, i, e, n, o, s = this._latlng.lng,
+            var t, e, i, n, o, s = this._latlng.lng,
                 r = this._latlng.lat,
                 a = this._map,
                 h = a.options.crs;
-            h.distance === st.distance ? (n = Math.PI / 180, o = this._mRadius / st.R / n, t = a.project([r + o, s]), i = a.project([r - o, s]), i = t.add(i).divideBy(2), e = a.unproject(i).lat, n = Math.acos((Math.cos(o * n) - Math.sin(r * n) * Math.sin(e * n)) / (Math.cos(r * n) * Math.cos(e * n))) / n, !isNaN(n) && 0 !== n || (n = o / Math.cos(Math.PI / 180 * r)), this._point = i.subtract(a.getPixelOrigin()), this._radius = isNaN(n) ? 0 : i.x - a.project([e, s - n]).x, this._radiusY = i.y - t.y) : (o = h.unproject(h.project(this._latlng).subtract([this._mRadius, 0])), this._point = a.latLngToLayerPoint(this._latlng), this._radius = this._point.x - a.latLngToLayerPoint(o).x), this._updateBounds()
+            h.distance === st.distance ? (n = Math.PI / 180, o = this._mRadius / st.R / n, t = a.project([r + o, s]), e = a.project([r - o, s]), e = t.add(e).divideBy(2), i = a.unproject(e).lat, n = Math.acos((Math.cos(o * n) - Math.sin(r * n) * Math.sin(i * n)) / (Math.cos(r * n) * Math.cos(i * n))) / n, !isNaN(n) && 0 !== n || (n = o / Math.cos(Math.PI / 180 * r)), this._point = e.subtract(a.getPixelOrigin()), this._radius = isNaN(n) ? 0 : e.x - a.project([i, s - n]).x, this._radiusY = e.y - t.y) : (o = h.unproject(h.project(this._latlng).subtract([this._mRadius, 0])), this._point = a.latLngToLayerPoint(this._latlng), this._radius = this._point.x - a.latLngToLayerPoint(o).x), this._updateBounds()
         }
     });
-    var fe = _e.extend({
+
+    function Mi(t, e, i) {
+        return new Ti(t, e, i)
+    }
+    var zi = bi.extend({
         options: {
             smoothFactor: 1,
             noClip: !1
         },
-        initialize: function(t, i) {
-            c(this, i), this._setLatLngs(t)
+        initialize: function(t, e) {
+            c(this, e), this._setLatLngs(t)
         },
         getLatLngs: function() {
             return this._latlngs
         },
         setLatLngs: function(t) {
             return this._setLatLngs(t), this.redraw()
         },
         isEmpty: function() {
             return !this._latlngs.length
         },
         closestLayerPoint: function(t) {
-            for (var i = 1 / 0, e = null, n = ee, o = 0, s = this._parts.length; o < s; o++)
+            for (var e = 1 / 0, i = null, n = ri, o = 0, s = this._parts.length; o < s; o++)
                 for (var r = this._parts[o], a = 1, h = r.length; a < h; a++) {
                     var l, u, c = n(t, l = r[a - 1], u = r[a], !0);
-                    c < i && (i = c, e = n(t, l, u))
+                    c < e && (e = c, i = n(t, l, u))
                 }
-            return e && (e.distance = Math.sqrt(i)), e
+            return i && (i.distance = Math.sqrt(e)), i
         },
         getCenter: function() {
-            if (!this._map) throw new Error("Must add layer to map before using getCenter()");
-            var t, i, e, n, o, s, r = this._rings[0],
-                a = r.length;
-            if (!a) return null;
-            for (i = t = 0; t < a - 1; t++) i += r[t].distanceTo(r[t + 1]) / 2;
-            if (0 === i) return this._map.layerPointToLatLng(r[0]);
-            for (e = t = 0; t < a - 1; t++)
-                if (n = r[t], o = r[t + 1], i < (e += s = n.distanceTo(o))) return this._map.layerPointToLatLng([o.x - (s = (e - i) / s) * (o.x - n.x), o.y - s * (o.y - n.y)])
+            if (this._map) return hi(this._defaultShape(), this._map.options.crs);
+            throw new Error("Must add layer to map before using getCenter()")
         },
         getBounds: function() {
             return this._bounds
         },
-        addLatLng: function(t, i) {
-            return i = i || this._defaultShape(), t = w(t), i.push(t), this._bounds.extend(t), this.redraw()
+        addLatLng: function(t, e) {
+            return e = e || this._defaultShape(), t = w(t), e.push(t), this._bounds.extend(t), this.redraw()
         },
         _setLatLngs: function(t) {
             this._bounds = new s, this._latlngs = this._convertLatLngs(t)
         },
         _defaultShape: function() {
-            return ne(this._latlngs) ? this._latlngs : this._latlngs[0]
+            return A(this._latlngs) ? this._latlngs : this._latlngs[0]
         },
         _convertLatLngs: function(t) {
-            for (var i = [], e = ne(t), n = 0, o = t.length; n < o; n++) e ? (i[n] = w(t[n]), this._bounds.extend(i[n])) : i[n] = this._convertLatLngs(t[n]);
-            return i
+            for (var e = [], i = A(t), n = 0, o = t.length; n < o; n++) i ? (e[n] = w(t[n]), this._bounds.extend(e[n])) : e[n] = this._convertLatLngs(t[n]);
+            return e
         },
         _project: function() {
-            var t = new m;
+            var t = new f;
             this._rings = [], this._projectLatlngs(this._latlngs, this._rings, t), this._bounds.isValid() && t.isValid() && (this._rawPxBounds = t, this._updateBounds())
         },
         _updateBounds: function() {
             var t = this._clickTolerance(),
                 t = new p(t, t);
-            this._rawPxBounds && (this._pxBounds = new m([this._rawPxBounds.min.subtract(t), this._rawPxBounds.max.add(t)]))
+            this._rawPxBounds && (this._pxBounds = new f([this._rawPxBounds.min.subtract(t), this._rawPxBounds.max.add(t)]))
         },
-        _projectLatlngs: function(t, i, e) {
+        _projectLatlngs: function(t, e, i) {
             var n, o, s = t[0] instanceof v,
                 r = t.length;
             if (s) {
-                for (o = [], n = 0; n < r; n++) o[n] = this._map.latLngToLayerPoint(t[n]), e.extend(o[n]);
-                i.push(o)
+                for (o = [], n = 0; n < r; n++) o[n] = this._map.latLngToLayerPoint(t[n]), i.extend(o[n]);
+                e.push(o)
             } else
-                for (n = 0; n < r; n++) this._projectLatlngs(t[n], i, e)
+                for (n = 0; n < r; n++) this._projectLatlngs(t[n], e, i)
         },
         _clipPoints: function() {
             var t = this._renderer._bounds;
             if (this._parts = [], this._pxBounds && this._pxBounds.intersects(t))
                 if (this.options.noClip) this._parts = this._rings;
                 else
-                    for (var i, e, n, o, s = this._parts, r = 0, a = 0, h = this._rings.length; r < h; r++)
-                        for (i = 0, e = (o = this._rings[r]).length; i < e - 1; i++)(n = Qi(o[i], o[i + 1], t, i, !0)) && (s[a] = s[a] || [], s[a].push(n[0]), n[1] === o[i + 1] && i !== e - 2 || (s[a].push(n[1]), a++))
+                    for (var e, i, n, o, s = this._parts, r = 0, a = 0, h = this._rings.length; r < h; r++)
+                        for (e = 0, i = (o = this._rings[r]).length; e < i - 1; e++)(n = ni(o[e], o[e + 1], t, e, !0)) && (s[a] = s[a] || [], s[a].push(n[0]), n[1] === o[e + 1] && e !== i - 2 || (s[a].push(n[1]), a++))
         },
         _simplifyPoints: function() {
-            for (var t = this._parts, i = this.options.smoothFactor, e = 0, n = t.length; e < n; e++) t[e] = Ji(t[e], i)
+            for (var t = this._parts, e = this.options.smoothFactor, i = 0, n = t.length; i < n; i++) t[i] = ei(t[i], e)
         },
         _update: function() {
             this._map && (this._clipPoints(), this._simplifyPoints(), this._updatePath())
         },
         _updatePath: function() {
             this._renderer._updatePoly(this)
         },
-        _containsPoint: function(t, i) {
-            var e, n, o, s, r, a, h = this._clickTolerance();
-            if (!this._pxBounds || !this._pxBounds.contains(t)) return !1;
-            for (e = 0, s = this._parts.length; e < s; e++)
-                for (n = 0, o = (r = (a = this._parts[e]).length) - 1; n < r; o = n++)
-                    if ((i || 0 !== n) && $i(t, a[o], a[n]) <= h) return !0;
+        _containsPoint: function(t, e) {
+            var i, n, o, s, r, a, h = this._clickTolerance();
+            if (this._pxBounds && this._pxBounds.contains(t))
+                for (i = 0, s = this._parts.length; i < s; i++)
+                    for (n = 0, o = (r = (a = this._parts[i]).length) - 1; n < r; o = n++)
+                        if ((e || 0 !== n) && ii(t, a[o], a[n]) <= h) return !0;
             return !1
         }
     });
-    fe._flat = oe;
-    var ge = fe.extend({
+
+    function Ci(t, e) {
+        return new zi(t, e)
+    }
+    zi._flat = ai;
+    var Zi = zi.extend({
         options: {
             fill: !0
         },
         isEmpty: function() {
             return !this._latlngs.length || !this._latlngs[0].length
         },
         getCenter: function() {
-            if (!this._map) throw new Error("Must add layer to map before using getCenter()");
-            var t, i, e, n, o, s, r, a, h, l = this._rings[0],
-                u = l.length;
-            if (!u) return null;
-            for (t = s = r = a = 0, i = u - 1; t < u; i = t++) e = l[t], n = l[i], o = e.y * n.x - n.y * e.x, r += (e.x + n.x) * o, a += (e.y + n.y) * o, s += 3 * o;
-            return h = 0 === s ? l[0] : [r / s, a / s], this._map.layerPointToLatLng(h)
+            if (this._map) return ui(this._defaultShape(), this._map.options.crs);
+            throw new Error("Must add layer to map before using getCenter()")
         },
         _convertLatLngs: function(t) {
-            var t = fe.prototype._convertLatLngs.call(this, t),
-                i = t.length;
-            return 2 <= i && t[0] instanceof v && t[0].equals(t[i - 1]) && t.pop(), t
+            var t = zi.prototype._convertLatLngs.call(this, t),
+                e = t.length;
+            return 2 <= e && t[0] instanceof v && t[0].equals(t[e - 1]) && t.pop(), t
         },
         _setLatLngs: function(t) {
-            fe.prototype._setLatLngs.call(this, t), ne(this._latlngs) && (this._latlngs = [this._latlngs])
+            zi.prototype._setLatLngs.call(this, t), A(this._latlngs) && (this._latlngs = [this._latlngs])
         },
         _defaultShape: function() {
-            return (ne(this._latlngs[0]) ? this._latlngs : this._latlngs[0])[0]
+            return (A(this._latlngs[0]) ? this._latlngs : this._latlngs[0])[0]
         },
         _clipPoints: function() {
             var t = this._renderer._bounds,
-                i = this.options.weight,
-                i = new p(i, i),
-                t = new m(t.min.subtract(i), t.max.add(i));
+                e = this.options.weight,
+                e = new p(e, e),
+                t = new f(t.min.subtract(e), t.max.add(e));
             if (this._parts = [], this._pxBounds && this._pxBounds.intersects(t))
                 if (this.options.noClip) this._parts = this._rings;
                 else
-                    for (var e, n = 0, o = this._rings.length; n < o; n++)(e = se(this._rings[n], t, !0)).length && this._parts.push(e)
+                    for (var i, n = 0, o = this._rings.length; n < o; n++)(i = li(this._rings[n], t, !0)).length && this._parts.push(i)
         },
         _updatePath: function() {
             this._renderer._updatePoly(this, !0)
         },
         _containsPoint: function(t) {
-            var i, e, n, o, s, r, a, h, l = !1;
+            var e, i, n, o, s, r, a, h, l = !1;
             if (!this._pxBounds || !this._pxBounds.contains(t)) return !1;
             for (o = 0, a = this._parts.length; o < a; o++)
-                for (s = 0, r = (h = (i = this._parts[o]).length) - 1; s < h; r = s++) e = i[s], n = i[r], e.y > t.y != n.y > t.y && t.x < (n.x - e.x) * (t.y - e.y) / (n.y - e.y) + e.x && (l = !l);
-            return l || fe.prototype._containsPoint.call(this, t, !0)
+                for (s = 0, r = (h = (e = this._parts[o]).length) - 1; s < h; r = s++) i = e[s], n = e[r], i.y > t.y != n.y > t.y && t.x < (n.x - i.x) * (t.y - i.y) / (n.y - i.y) + i.x && (l = !l);
+            return l || zi.prototype._containsPoint.call(this, t, !0)
         }
     });
-    var ve = he.extend({
-        initialize: function(t, i) {
-            c(this, i), this._layers = {}, t && this.addData(t)
+
+    function Si(t, e) {
+        return new Zi(t, e)
+    }
+    var Ei = mi.extend({
+        initialize: function(t, e) {
+            c(this, e), this._layers = {}, t && this.addData(t)
         },
         addData: function(t) {
-            var i, e, n, o = d(t) ? t : t.features;
+            var e, i, n, o = d(t) ? t : t.features;
             if (o) {
-                for (i = 0, e = o.length; i < e; i++)((n = o[i]).geometries || n.geometry || n.features || n.coordinates) && this.addData(n);
+                for (e = 0, i = o.length; e < i; e++)((n = o[e]).geometries || n.geometry || n.features || n.coordinates) && this.addData(n);
                 return this
             }
-            var s = this.options;
-            if (s.filter && !s.filter(t)) return this;
-            var r = ye(t, s);
-            return r ? (r.feature = ze(t), r.defaultOptions = r.options, this.resetStyle(r), s.onEachFeature && s.onEachFeature(t, r), this.addLayer(r)) : this
+            var s, r = this.options;
+            return (!r.filter || r.filter(t)) && (s = ki(t, r)) ? (s.feature = Di(t), s.defaultOptions = s.options, this.resetStyle(s), r.onEachFeature && r.onEachFeature(t, s), this.addLayer(s)) : this
         },
         resetStyle: function(t) {
             return void 0 === t ? this.eachLayer(this.resetStyle, this) : (t.options = l({}, t.defaultOptions), this._setLayerStyle(t, this.options.style), this)
         },
-        setStyle: function(i) {
+        setStyle: function(e) {
             return this.eachLayer(function(t) {
-                this._setLayerStyle(t, i)
+                this._setLayerStyle(t, e)
             }, this)
         },
-        _setLayerStyle: function(t, i) {
-            t.setStyle && ("function" == typeof i && (i = i(t.feature)), t.setStyle(i))
+        _setLayerStyle: function(t, e) {
+            t.setStyle && ("function" == typeof e && (e = e(t.feature)), t.setStyle(e))
         }
     });
 
-    function ye(t, i) {
-        var e, n, o, s, r = "Feature" === t.type ? t.geometry : t,
+    function ki(t, e) {
+        var i, n, o, s, r = "Feature" === t.type ? t.geometry : t,
             a = r ? r.coordinates : null,
             h = [],
-            l = i && i.pointToLayer,
-            u = i && i.coordsToLatLng || we;
+            l = e && e.pointToLayer,
+            u = e && e.coordsToLatLng || Bi;
         if (!a && !r) return null;
         switch (r.type) {
             case "Point":
-                return xe(l, t, e = u(a), i);
+                return Oi(l, t, i = u(a), e);
             case "MultiPoint":
-                for (o = 0, s = a.length; o < s; o++) e = u(a[o]), h.push(xe(l, t, e, i));
-                return new he(h);
+                for (o = 0, s = a.length; o < s; o++) i = u(a[o]), h.push(Oi(l, t, i, e));
+                return new mi(h);
             case "LineString":
             case "MultiLineString":
-                return n = Pe(a, "LineString" === r.type ? 0 : 1, u), new fe(n, i);
+                return n = Ai(a, "LineString" === r.type ? 0 : 1, u), new zi(n, e);
             case "Polygon":
             case "MultiPolygon":
-                return n = Pe(a, "Polygon" === r.type ? 1 : 2, u), new ge(n, i);
+                return n = Ai(a, "Polygon" === r.type ? 1 : 2, u), new Zi(n, e);
             case "GeometryCollection":
                 for (o = 0, s = r.geometries.length; o < s; o++) {
-                    var c = ye({
+                    var c = ki({
                         geometry: r.geometries[o],
                         type: "Feature",
                         properties: t.properties
-                    }, i);
+                    }, e);
                     c && h.push(c)
                 }
-                return new he(h);
+                return new mi(h);
+            case "FeatureCollection":
+                for (o = 0, s = r.features.length; o < s; o++) {
+                    var d = ki(r.features[o], e);
+                    d && h.push(d)
+                }
+                return new mi(h);
             default:
                 throw new Error("Invalid GeoJSON object.")
         }
     }
 
-    function xe(t, i, e, n) {
-        return t ? t(i, e) : new de(e, n && n.markersInheritOptions && n)
+    function Oi(t, e, i, n) {
+        return t ? t(e, i) : new xi(i, n && n.markersInheritOptions && n)
     }
 
-    function we(t) {
+    function Bi(t) {
         return new v(t[1], t[0], t[2])
     }
 
-    function Pe(t, i, e) {
-        for (var n, o = [], s = 0, r = t.length; s < r; s++) n = i ? Pe(t[s], i - 1, e) : (e || we)(t[s]), o.push(n);
+    function Ai(t, e, i) {
+        for (var n, o = [], s = 0, r = t.length; s < r; s++) n = e ? Ai(t[s], e - 1, i) : (i || Bi)(t[s]), o.push(n);
         return o
     }
 
-    function be(t, i) {
-        return void 0 !== (t = w(t)).alt ? [e(t.lng, i), e(t.lat, i), e(t.alt, i)] : [e(t.lng, i), e(t.lat, i)]
+    function Ii(t, e) {
+        return void 0 !== (t = w(t)).alt ? [i(t.lng, e), i(t.lat, e), i(t.alt, e)] : [i(t.lng, e), i(t.lat, e)]
     }
 
-    function Le(t, i, e, n) {
-        for (var o = [], s = 0, r = t.length; s < r; s++) o.push(i ? Le(t[s], i - 1, e, n) : be(t[s], n));
-        return !i && e && o.push(o[0]), o
+    function Ri(t, e, i, n) {
+        for (var o = [], s = 0, r = t.length; s < r; s++) o.push(e ? Ri(t[s], A(t[s]) ? 0 : e - 1, i, n) : Ii(t[s], n));
+        return !e && i && o.push(o[0]), o
     }
 
-    function Te(t, i) {
+    function Ni(t, e) {
         return t.feature ? l({}, t.feature, {
-            geometry: i
-        }) : ze(i)
+            geometry: e
+        }) : Di(e)
     }
 
-    function ze(t) {
+    function Di(t) {
         return "Feature" === t.type || "FeatureCollection" === t.type ? t : {
             type: "Feature",
             properties: {},
             geometry: t
         }
     }
     Tt = {
         toGeoJSON: function(t) {
-            return Te(this, {
+            return Ni(this, {
                 type: "Point",
-                coordinates: be(this.getLatLng(), t)
+                coordinates: Ii(this.getLatLng(), t)
             })
         }
     };
 
-    function Me(t, i) {
-        return new ve(t, i)
+    function ji(t, e) {
+        return new Ei(t, e)
     }
-    de.include(Tt), me.include(Tt), pe.include(Tt), fe.include({
+    xi.include(Tt), Ti.include(Tt), Pi.include(Tt), zi.include({
         toGeoJSON: function(t) {
-            var i = !ne(this._latlngs);
-            return Te(this, {
-                type: (i ? "Multi" : "") + "LineString",
-                coordinates: Le(this._latlngs, i ? 1 : 0, !1, t)
+            var e = !A(this._latlngs);
+            return Ni(this, {
+                type: (e ? "Multi" : "") + "LineString",
+                coordinates: Ri(this._latlngs, e ? 1 : 0, !1, t)
             })
         }
-    }), ge.include({
+    }), Zi.include({
         toGeoJSON: function(t) {
-            var i = !ne(this._latlngs),
-                e = i && !ne(this._latlngs[0]),
-                t = Le(this._latlngs, e ? 2 : i ? 1 : 0, !0, t);
-            return Te(this, {
-                type: (e ? "Multi" : "") + "Polygon",
-                coordinates: t = i ? t : [t]
+            var e = !A(this._latlngs),
+                i = e && !A(this._latlngs[0]),
+                t = Ri(this._latlngs, i ? 2 : e ? 1 : 0, !0, t);
+            return Ni(this, {
+                type: (i ? "Multi" : "") + "Polygon",
+                coordinates: t = e ? t : [t]
             })
         }
-    }), ae.include({
-        toMultiPoint: function(i) {
-            var e = [];
+    }), pi.include({
+        toMultiPoint: function(e) {
+            var i = [];
             return this.eachLayer(function(t) {
-                e.push(t.toGeoJSON(i).geometry.coordinates)
-            }), Te(this, {
+                i.push(t.toGeoJSON(e).geometry.coordinates)
+            }), Ni(this, {
                 type: "MultiPoint",
-                coordinates: e
+                coordinates: i
             })
         },
-        toGeoJSON: function(i) {
-            var t = this.feature && this.feature.geometry && this.feature.geometry.type;
-            if ("MultiPoint" === t) return this.toMultiPoint(i);
-            var e = "GeometryCollection" === t,
-                n = [];
-            return this.eachLayer(function(t) {
-                t.toGeoJSON && (t = t.toGeoJSON(i), e ? n.push(t.geometry) : "FeatureCollection" === (t = ze(t)).type ? n.push.apply(n, t.features) : n.push(t))
-            }), e ? Te(this, {
+        toGeoJSON: function(e) {
+            var i, n, t = this.feature && this.feature.geometry && this.feature.geometry.type;
+            return "MultiPoint" === t ? this.toMultiPoint(e) : (i = "GeometryCollection" === t, n = [], this.eachLayer(function(t) {
+                t.toGeoJSON && (t = t.toGeoJSON(e), i ? n.push(t.geometry) : "FeatureCollection" === (t = Di(t)).type ? n.push.apply(n, t.features) : n.push(t))
+            }), i ? Ni(this, {
                 geometries: n,
                 type: "GeometryCollection"
             }) : {
                 type: "FeatureCollection",
                 features: n
-            }
+            })
         }
     });
-    var zt = Me,
-        Ce = o.extend({
+
+    function Hi(t, e, i) {
+        return new Fi(t, e, i)
+    }
+    var Mt = ji,
+        Fi = y.extend({
             options: {
                 opacity: 1,
                 alt: "",
                 interactive: !1,
                 crossOrigin: !1,
                 errorOverlayUrl: "",
                 zIndex: 1,
                 className: ""
             },
-            initialize: function(t, i, e) {
-                this._url = t, this._bounds = g(i), c(this, e)
+            initialize: function(t, e, i) {
+                this._url = t, this._bounds = g(e), c(this, i)
             },
             onAdd: function() {
-                this._image || (this._initImage(), this.options.opacity < 1 && this._updateOpacity()), this.options.interactive && (z(this._image, "leaflet-interactive"), this.addInteractiveTarget(this._image)), this.getPane().appendChild(this._image), this._reset()
+                this._image || (this._initImage(), this.options.opacity < 1 && this._updateOpacity()), this.options.interactive && (M(this._image, "leaflet-interactive"), this.addInteractiveTarget(this._image)), this.getPane().appendChild(this._image), this._reset()
             },
             onRemove: function() {
                 T(this._image), this.options.interactive && this.removeInteractiveTarget(this._image)
             },
             setOpacity: function(t) {
                 return this.options.opacity = t, this._image && this._updateOpacity(), this
             },
             setStyle: function(t) {
                 return t.opacity && this.setOpacity(t.opacity), this
             },
             bringToFront: function() {
-                return this._map && fi(this._image), this
+                return this._map && ge(this._image), this
             },
             bringToBack: function() {
-                return this._map && gi(this._image), this
+                return this._map && ve(this._image), this
             },
             setUrl: function(t) {
                 return this._url = t, this._image && (this._image.src = t), this
             },
             setBounds: function(t) {
                 return this._bounds = g(t), this._map && this._reset(), this
             },
@@ -3078,27 +3139,27 @@
                 return this._bounds
             },
             getElement: function() {
                 return this._image
             },
             _initImage: function() {
                 var t = "IMG" === this._url.tagName,
-                    i = this._image = t ? this._url : b("img");
-                z(i, "leaflet-image-layer"), this._zoomAnimated && z(i, "leaflet-zoom-animated"), this.options.className && z(i, this.options.className), i.onselectstart = u, i.onmousemove = u, i.onload = a(this.fire, this, "load"), i.onerror = a(this._overlayOnError, this, "error"), !this.options.crossOrigin && "" !== this.options.crossOrigin || (i.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), this.options.zIndex && this._updateZIndex(), t ? this._url = i.src : (i.src = this._url, i.alt = this.options.alt)
+                    e = this._image = t ? this._url : P("img");
+                M(e, "leaflet-image-layer"), this._zoomAnimated && M(e, "leaflet-zoom-animated"), this.options.className && M(e, this.options.className), e.onselectstart = u, e.onmousemove = u, e.onload = a(this.fire, this, "load"), e.onerror = a(this._overlayOnError, this, "error"), !this.options.crossOrigin && "" !== this.options.crossOrigin || (e.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), this.options.zIndex && this._updateZIndex(), t ? this._url = e.src : (e.src = this._url, e.alt = this.options.alt)
             },
             _animateZoom: function(t) {
-                var i = this._map.getZoomScale(t.zoom),
+                var e = this._map.getZoomScale(t.zoom),
                     t = this._map._latLngBoundsToNewLayerBounds(this._bounds, t.zoom, t.center).min;
-                Pi(this._image, t, i)
+                Pe(this._image, t, e)
             },
             _reset: function() {
                 var t = this._image,
-                    i = new m(this._map.latLngToLayerPoint(this._bounds.getNorthWest()), this._map.latLngToLayerPoint(this._bounds.getSouthEast())),
-                    e = i.getSize();
-                Z(t, i.min), t.style.width = e.x + "px", t.style.height = e.y + "px"
+                    e = new f(this._map.latLngToLayerPoint(this._bounds.getNorthWest()), this._map.latLngToLayerPoint(this._bounds.getSouthEast())),
+                    i = e.getSize();
+                Z(t, e.min), t.style.width = i.x + "px", t.style.height = i.y + "px"
             },
             _updateOpacity: function() {
                 C(this._image, this.options.opacity)
             },
             _updateZIndex: function() {
                 this._image && void 0 !== this.options.zIndex && null !== this.options.zIndex && (this._image.style.zIndex = this.options.zIndex)
             },
@@ -3107,67 +3168,84 @@
                 var t = this.options.errorOverlayUrl;
                 t && this._url !== t && (this._url = t, this._image.src = t)
             },
             getCenter: function() {
                 return this._bounds.getCenter()
             }
         }),
-        Ze = Ce.extend({
+        Wi = Fi.extend({
             options: {
                 autoplay: !0,
                 loop: !0,
                 keepAspectRatio: !0,
                 muted: !1,
                 playsInline: !0
             },
             _initImage: function() {
                 var t = "VIDEO" === this._url.tagName,
-                    i = this._image = t ? this._url : b("video");
-                if (z(i, "leaflet-image-layer"), this._zoomAnimated && z(i, "leaflet-zoom-animated"), this.options.className && z(i, this.options.className), i.onselectstart = u, i.onmousemove = u, i.onloadeddata = a(this.fire, this, "load"), t) {
-                    for (var e = i.getElementsByTagName("source"), n = [], o = 0; o < e.length; o++) n.push(e[o].src);
-                    this._url = 0 < e.length ? n : [i.src]
+                    e = this._image = t ? this._url : P("video");
+                if (M(e, "leaflet-image-layer"), this._zoomAnimated && M(e, "leaflet-zoom-animated"), this.options.className && M(e, this.options.className), e.onselectstart = u, e.onmousemove = u, e.onloadeddata = a(this.fire, this, "load"), t) {
+                    for (var i = e.getElementsByTagName("source"), n = [], o = 0; o < i.length; o++) n.push(i[o].src);
+                    this._url = 0 < i.length ? n : [e.src]
                 } else {
-                    d(this._url) || (this._url = [this._url]), !this.options.keepAspectRatio && Object.prototype.hasOwnProperty.call(i.style, "objectFit") && (i.style.objectFit = "fill"), i.autoplay = !!this.options.autoplay, i.loop = !!this.options.loop, i.muted = !!this.options.muted, i.playsInline = !!this.options.playsInline;
+                    d(this._url) || (this._url = [this._url]), !this.options.keepAspectRatio && Object.prototype.hasOwnProperty.call(e.style, "objectFit") && (e.style.objectFit = "fill"), e.autoplay = !!this.options.autoplay, e.loop = !!this.options.loop, e.muted = !!this.options.muted, e.playsInline = !!this.options.playsInline;
                     for (var s = 0; s < this._url.length; s++) {
-                        var r = b("source");
-                        r.src = this._url[s], i.appendChild(r)
+                        var r = P("source");
+                        r.src = this._url[s], e.appendChild(r)
                     }
                 }
             }
         });
-    var Se = Ce.extend({
+
+    function Ui(t, e, i) {
+        return new Wi(t, e, i)
+    }
+    var Vi = Fi.extend({
         _initImage: function() {
             var t = this._image = this._url;
-            z(t, "leaflet-image-layer"), this._zoomAnimated && z(t, "leaflet-zoom-animated"), this.options.className && z(t, this.options.className), t.onselectstart = u, t.onmousemove = u
+            M(t, "leaflet-image-layer"), this._zoomAnimated && M(t, "leaflet-zoom-animated"), this.options.className && M(t, this.options.className), t.onselectstart = u, t.onmousemove = u
         }
     });
-    var O = o.extend({
+
+    function Gi(t, e, i) {
+        return new Vi(t, e, i)
+    }
+
+    function qi(t, e) {
+        return new Yi(t, e)
+    }
+
+    function Ki(t, e) {
+        return new Ji(t, e)
+    }
+    var I = y.extend({
             options: {
                 interactive: !1,
                 offset: [0, 0],
                 className: "",
-                pane: void 0
+                pane: void 0,
+                content: ""
             },
-            initialize: function(t, i) {
-                c(this, t), this._source = i
+            initialize: function(t, e) {
+                t && (t instanceof L.LatLng || d(t)) ? (this._latlng = w(t), c(this, e)) : (c(this, t), this._source = e), this.options.content && (this._content = this.options.content)
             },
             openOn: function(t) {
                 return (t = arguments.length ? t : this._source._map).hasLayer(this) || t.addLayer(this), this
             },
             close: function() {
                 return this._map && this._map.removeLayer(this), this
             },
             toggle: function(t) {
                 return this._map ? this.close() : (arguments.length ? this._source = t : t = this._source, this._prepareOpen(), this.openOn(t._map)), this
             },
             onAdd: function(t) {
-                this._zoomAnimated = t._zoomAnimated, this._container || this._initLayout(), t._fadeAnimated && C(this._container, 0), clearTimeout(this._removeTimeout), this.getPane().appendChild(this._container), this.update(), t._fadeAnimated && C(this._container, 1), this.bringToFront(), this.options.interactive && (z(this._container, "leaflet-interactive"), this.addInteractiveTarget(this._container))
+                this._zoomAnimated = t._zoomAnimated, this._container || this._initLayout(), t._fadeAnimated && C(this._container, 0), clearTimeout(this._removeTimeout), this.getPane().appendChild(this._container), this.update(), t._fadeAnimated && C(this._container, 1), this.bringToFront(), this.options.interactive && (M(this._container, "leaflet-interactive"), this.addInteractiveTarget(this._container))
             },
             onRemove: function(t) {
-                t._fadeAnimated ? (C(this._container, 0), this._removeTimeout = setTimeout(a(T, void 0, this._container), 200)) : T(this._container), this.options.interactive && (M(this._container, "leaflet-interactive"), this.removeInteractiveTarget(this._container))
+                t._fadeAnimated ? (C(this._container, 0), this._removeTimeout = setTimeout(a(T, void 0, this._container), 200)) : T(this._container), this.options.interactive && (z(this._container, "leaflet-interactive"), this.removeInteractiveTarget(this._container))
             },
             getLatLng: function() {
                 return this._latlng
             },
             setLatLng: function(t) {
                 return this._latlng = w(t), this._map && (this._updatePosition(), this._adjustPan()), this
             },
@@ -3190,71 +3268,71 @@
                 };
                 return this._zoomAnimated && (t.zoomanim = this._animateZoom), t
             },
             isOpen: function() {
                 return !!this._map && this._map.hasLayer(this)
             },
             bringToFront: function() {
-                return this._map && fi(this._container), this
+                return this._map && ge(this._container), this
             },
             bringToBack: function() {
-                return this._map && gi(this._container), this
+                return this._map && ve(this._container), this
             },
             _prepareOpen: function(t) {
-                if (!(e = this._source)._map) return !1;
-                if (e instanceof he) {
-                    var i, e = null,
+                if (!(i = this._source)._map) return !1;
+                if (i instanceof mi) {
+                    var e, i = null,
                         n = this._source._layers;
-                    for (i in n)
-                        if (n[i]._map) {
-                            e = n[i];
+                    for (e in n)
+                        if (n[e]._map) {
+                            i = n[e];
                             break
-                        } if (!e) return !1;
-                    this._source = e
+                        } if (!i) return !1;
+                    this._source = i
                 }
                 if (!t)
-                    if (e.getCenter) t = e.getCenter();
-                    else if (e.getLatLng) t = e.getLatLng();
+                    if (i.getCenter) t = i.getCenter();
+                    else if (i.getLatLng) t = i.getLatLng();
                 else {
-                    if (!e.getBounds) throw new Error("Unable to get source layer LatLng.");
-                    t = e.getBounds().getCenter()
+                    if (!i.getBounds) throw new Error("Unable to get source layer LatLng.");
+                    t = i.getBounds().getCenter()
                 }
                 return this.setLatLng(t), this._map && this.update(), !0
             },
             _updateContent: function() {
                 if (this._content) {
                     var t = this._contentNode,
-                        i = "function" == typeof this._content ? this._content(this._source || this) : this._content;
-                    if ("string" == typeof i) t.innerHTML = i;
+                        e = "function" == typeof this._content ? this._content(this._source || this) : this._content;
+                    if ("string" == typeof e) t.innerHTML = e;
                     else {
                         for (; t.hasChildNodes();) t.removeChild(t.firstChild);
-                        t.appendChild(i)
+                        t.appendChild(e)
                     }
                     this.fire("contentupdate")
                 }
             },
             _updatePosition: function() {
-                var t, i, e;
-                this._map && (i = this._map.latLngToLayerPoint(this._latlng), t = _(this.options.offset), e = this._getAnchor(), this._zoomAnimated ? Z(this._container, i.add(e)) : t = t.add(i).add(e), i = this._containerBottom = -t.y, e = this._containerLeft = -Math.round(this._containerWidth / 2) + t.x, this._container.style.bottom = i + "px", this._container.style.left = e + "px")
+                var t, e, i;
+                this._map && (e = this._map.latLngToLayerPoint(this._latlng), t = m(this.options.offset), i = this._getAnchor(), this._zoomAnimated ? Z(this._container, e.add(i)) : t = t.add(e).add(i), e = this._containerBottom = -t.y, i = this._containerLeft = -Math.round(this._containerWidth / 2) + t.x, this._container.style.bottom = e + "px", this._container.style.left = i + "px")
             },
             _getAnchor: function() {
                 return [0, 0]
             }
         }),
-        ke = (A.include({
-            _initOverlay: function(t, i, e, n) {
-                var o = i;
-                return o instanceof t || (o = new t(n).setContent(i)), e && o.setLatLng(e), o
-            }
-        }), o.include({
-            _initOverlay: function(t, i, e, n) {
+        Yi = (O.include({
+            _initOverlay: function(t, e, i, n) {
                 var o = e;
-                return o instanceof t ? (c(o, n), o._source = this) : (o = i && !n ? i : new t(n, this)).setContent(e), o
+                return o instanceof t || (o = new t(n).setContent(e)), i && o.setLatLng(i), o
+            }
+        }), y.include({
+            _initOverlay: function(t, e, i, n) {
+                var o = i;
+                return o instanceof t ? (c(o, n), o._source = this) : (o = e && !n ? e : new t(n, this)).setContent(i), o
             }
-        }), O.extend({
+        }), I.extend({
             options: {
                 pane: "popupPane",
                 offset: [0, 7],
                 maxWidth: 300,
                 minWidth: 50,
                 maxHeight: null,
                 autoPan: !0,
@@ -3264,77 +3342,79 @@
                 keepInView: !1,
                 closeButton: !0,
                 autoClose: !0,
                 closeOnEscapeKey: !0,
                 className: ""
             },
             openOn: function(t) {
-                return !(t = arguments.length ? t : this._source._map).hasLayer(this) && t._popup && t._popup.options.autoClose && t.removeLayer(t._popup), t._popup = this, O.prototype.openOn.call(this, t)
+                return !(t = arguments.length ? t : this._source._map).hasLayer(this) && t._popup && t._popup.options.autoClose && t.removeLayer(t._popup), t._popup = this, I.prototype.openOn.call(this, t)
             },
             onAdd: function(t) {
-                O.prototype.onAdd.call(this, t), t.fire("popupopen", {
+                I.prototype.onAdd.call(this, t), t.fire("popupopen", {
                     popup: this
                 }), this._source && (this._source.fire("popupopen", {
                     popup: this
-                }, !0), this._source instanceof _e || this._source.on("preclick", Ai))
+                }, !0), this._source instanceof bi || this._source.on("preclick", Ie))
             },
             onRemove: function(t) {
-                O.prototype.onRemove.call(this, t), t.fire("popupclose", {
+                I.prototype.onRemove.call(this, t), t.fire("popupclose", {
                     popup: this
                 }), this._source && (this._source.fire("popupclose", {
                     popup: this
-                }, !0), this._source instanceof _e || this._source.off("preclick", Ai))
+                }, !0), this._source instanceof bi || this._source.off("preclick", Ie))
             },
             getEvents: function() {
-                var t = O.prototype.getEvents.call(this);
+                var t = I.prototype.getEvents.call(this);
                 return (void 0 !== this.options.closeOnClick ? this.options.closeOnClick : this._map.options.closePopupOnClick) && (t.preclick = this.close), this.options.keepInView && (t.moveend = this._adjustPan), t
             },
             _initLayout: function() {
                 var t = "leaflet-popup",
-                    i = this._container = b("div", t + " " + (this.options.className || "") + " leaflet-zoom-animated"),
-                    e = this._wrapper = b("div", t + "-content-wrapper", i);
-                this._contentNode = b("div", t + "-content", e), Oi(i), Ii(this._contentNode), S(i, "contextmenu", Ai), this._tipContainer = b("div", t + "-tip-container", i), this._tip = b("div", t + "-tip", this._tipContainer), this.options.closeButton && ((e = this._closeButton = b("a", t + "-close-button", i)).setAttribute("role", "button"), e.setAttribute("aria-label", "Close popup"), e.href = "#close", e.innerHTML = '<span aria-hidden="true">&#215;</span>', S(e, "click", this.close, this))
+                    e = this._container = P("div", t + " " + (this.options.className || "") + " leaflet-zoom-animated"),
+                    i = this._wrapper = P("div", t + "-content-wrapper", e);
+                this._contentNode = P("div", t + "-content", i), Ne(e), Re(this._contentNode), S(e, "contextmenu", Ie), this._tipContainer = P("div", t + "-tip-container", e), this._tip = P("div", t + "-tip", this._tipContainer), this.options.closeButton && ((i = this._closeButton = P("a", t + "-close-button", e)).setAttribute("role", "button"), i.setAttribute("aria-label", "Close popup"), i.href = "#close", i.innerHTML = '<span aria-hidden="true">&#215;</span>', S(i, "click", function(t) {
+                    k(t), this.close()
+                }, this))
             },
             _updateLayout: function() {
                 var t = this._contentNode,
-                    i = t.style,
-                    e = (i.width = "", i.whiteSpace = "nowrap", t.offsetWidth),
-                    e = Math.min(e, this.options.maxWidth),
-                    e = (e = Math.max(e, this.options.minWidth), i.width = e + 1 + "px", i.whiteSpace = "", i.height = "", t.offsetHeight),
+                    e = t.style,
+                    i = (e.width = "", e.whiteSpace = "nowrap", t.offsetWidth),
+                    i = Math.min(i, this.options.maxWidth),
+                    i = (i = Math.max(i, this.options.minWidth), e.width = i + 1 + "px", e.whiteSpace = "", e.height = "", t.offsetHeight),
                     n = this.options.maxHeight,
                     o = "leaflet-popup-scrolled";
-                n && n < e ? (i.height = n + "px", z(t, o)) : M(t, o), this._containerWidth = this._container.offsetWidth
+                (n && n < i ? (e.height = n + "px", M) : z)(t, o), this._containerWidth = this._container.offsetWidth
             },
             _animateZoom: function(t) {
                 var t = this._map._latLngToNewLayerPoint(this._latlng, t.zoom, t.center),
-                    i = this._getAnchor();
-                Z(this._container, t.add(i))
+                    e = this._getAnchor();
+                Z(this._container, t.add(e))
             },
             _adjustPan: function(t) {
-                var i, e, n, o, s, r, a, h;
-                this.options.autoPan && (this._map._panAnim && this._map._panAnim.stop(), i = this._map, e = parseInt(pi(this._container, "marginBottom"), 10) || 0, e = this._container.offsetHeight + e, h = this._containerWidth, (n = new p(this._containerLeft, -e - this._containerBottom))._add(bi(this._container)), n = i.layerPointToContainerPoint(n), s = _(this.options.autoPanPadding), o = _(this.options.autoPanPaddingTopLeft || s), s = _(this.options.autoPanPaddingBottomRight || s), r = i.getSize(), a = 0, n.x + h + s.x > r.x && (a = n.x + h - r.x + s.x), n.x - a - o.x < (h = 0) && (a = n.x - o.x), n.y + e + s.y > r.y && (h = n.y + e - r.y + s.y), n.y - h - o.y < 0 && (h = n.y - o.y), (a || h) && i.fire("autopanstart").panBy([a, h], {
+                var e, i, n, o, s, r, a, h;
+                this.options.autoPan && (this._map._panAnim && this._map._panAnim.stop(), e = this._map, i = parseInt(me(this._container, "marginBottom"), 10) || 0, i = this._container.offsetHeight + i, h = this._containerWidth, (n = new p(this._containerLeft, -i - this._containerBottom))._add(Le(this._container)), n = e.layerPointToContainerPoint(n), s = m(this.options.autoPanPadding), o = m(this.options.autoPanPaddingTopLeft || s), s = m(this.options.autoPanPaddingBottomRight || s), r = e.getSize(), a = 0, n.x + h + s.x > r.x && (a = n.x + h - r.x + s.x), n.x - a - o.x < (h = 0) && (a = n.x - o.x), n.y + i + s.y > r.y && (h = n.y + i - r.y + s.y), n.y - h - o.y < 0 && (h = n.y - o.y), (a || h) && e.fire("autopanstart").panBy([a, h], {
                     animate: t && "moveend" === t.type
                 }))
             },
             _getAnchor: function() {
-                return _(this._source && this._source._getPopupAnchor ? this._source._getPopupAnchor() : [0, 0])
+                return m(this._source && this._source._getPopupAnchor ? this._source._getPopupAnchor() : [0, 0])
             }
         })),
-        Ee = (A.mergeOptions({
+        Ji = (O.mergeOptions({
             closePopupOnClick: !0
-        }), A.include({
-            openPopup: function(t, i, e) {
-                return this._initOverlay(ke, t, i, e).openOn(this), this
+        }), O.include({
+            openPopup: function(t, e, i) {
+                return this._initOverlay(Yi, t, e, i).openOn(this), this
             },
             closePopup: function(t) {
                 return (t = arguments.length ? t : this._popup) && t.close(), this
             }
-        }), o.include({
-            bindPopup: function(t, i) {
-                return this._popup = this._initOverlay(ke, this._popup, t, i), this._popupHandlersAdded || (this.on({
+        }), y.include({
+            bindPopup: function(t, e) {
+                return this._popup = this._initOverlay(Yi, this._popup, t, e), this._popupHandlersAdded || (this.on({
                     click: this._openPopup,
                     keypress: this._onKeyPress,
                     remove: this.closePopup,
                     move: this._movePopup
                 }), this._popupHandlersAdded = !0), this
             },
             unbindPopup: function() {
@@ -3360,107 +3440,107 @@
             setPopupContent: function(t) {
                 return this._popup && this._popup.setContent(t), this
             },
             getPopup: function() {
                 return this._popup
             },
             _openPopup: function(t) {
-                var i;
-                this._popup && this._map && (Ri(t), i = t.layer || t.target, this._popup._source !== i || i instanceof _e ? (this._popup._source = i, this.openPopup(t.latlng)) : this._map.hasLayer(this._popup) ? this.closePopup() : this.openPopup(t.latlng))
+                var e;
+                this._popup && this._map && (De(t), e = t.layer || t.target, this._popup._source !== e || e instanceof bi ? (this._popup._source = e, this.openPopup(t.latlng)) : this._map.hasLayer(this._popup) ? this.closePopup() : this.openPopup(t.latlng))
             },
             _movePopup: function(t) {
                 this._popup.setLatLng(t.latlng)
             },
             _onKeyPress: function(t) {
                 13 === t.originalEvent.keyCode && this._openPopup(t)
             }
-        }), O.extend({
+        }), I.extend({
             options: {
                 pane: "tooltipPane",
                 offset: [0, 0],
                 direction: "auto",
                 permanent: !1,
                 sticky: !1,
                 opacity: .9
             },
             onAdd: function(t) {
-                O.prototype.onAdd.call(this, t), this.setOpacity(this.options.opacity), t.fire("tooltipopen", {
+                I.prototype.onAdd.call(this, t), this.setOpacity(this.options.opacity), t.fire("tooltipopen", {
                     tooltip: this
                 }), this._source && (this.addEventParent(this._source), this._source.fire("tooltipopen", {
                     tooltip: this
                 }, !0))
             },
             onRemove: function(t) {
-                O.prototype.onRemove.call(this, t), t.fire("tooltipclose", {
+                I.prototype.onRemove.call(this, t), t.fire("tooltipclose", {
                     tooltip: this
                 }), this._source && (this.removeEventParent(this._source), this._source.fire("tooltipclose", {
                     tooltip: this
                 }, !0))
             },
             getEvents: function() {
-                var t = O.prototype.getEvents.call(this);
+                var t = I.prototype.getEvents.call(this);
                 return this.options.permanent || (t.preclick = this.close), t
             },
             _initLayout: function() {
                 var t = "leaflet-tooltip " + (this.options.className || "") + " leaflet-zoom-" + (this._zoomAnimated ? "animated" : "hide");
-                this._contentNode = this._container = b("div", t)
+                this._contentNode = this._container = P("div", t), this._container.setAttribute("role", "tooltip"), this._container.setAttribute("id", "leaflet-tooltip-" + h(this))
             },
             _updateLayout: function() {},
             _adjustPan: function() {},
             _setPosition: function(t) {
-                var i, e = this._map,
+                var e, i = this._map,
                     n = this._container,
-                    o = e.latLngToContainerPoint(e.getCenter()),
-                    e = e.layerPointToContainerPoint(t),
+                    o = i.latLngToContainerPoint(i.getCenter()),
+                    i = i.layerPointToContainerPoint(t),
                     s = this.options.direction,
                     r = n.offsetWidth,
                     a = n.offsetHeight,
-                    h = _(this.options.offset),
+                    h = m(this.options.offset),
                     l = this._getAnchor(),
-                    e = "top" === s ? (i = r / 2, a) : "bottom" === s ? (i = r / 2, 0) : (i = "center" === s ? r / 2 : "right" === s ? 0 : "left" === s ? r : e.x < o.x ? (s = "right", 0) : (s = "left", r + 2 * (h.x + l.x)), a / 2);
-                t = t.subtract(_(i, e, !0)).add(h).add(l), M(n, "leaflet-tooltip-right"), M(n, "leaflet-tooltip-left"), M(n, "leaflet-tooltip-top"), M(n, "leaflet-tooltip-bottom"), z(n, "leaflet-tooltip-" + s), Z(n, t)
+                    i = "top" === s ? (e = r / 2, a) : "bottom" === s ? (e = r / 2, 0) : (e = "center" === s ? r / 2 : "right" === s ? 0 : "left" === s ? r : i.x < o.x ? (s = "right", 0) : (s = "left", r + 2 * (h.x + l.x)), a / 2);
+                t = t.subtract(m(e, i, !0)).add(h).add(l), z(n, "leaflet-tooltip-right"), z(n, "leaflet-tooltip-left"), z(n, "leaflet-tooltip-top"), z(n, "leaflet-tooltip-bottom"), M(n, "leaflet-tooltip-" + s), Z(n, t)
             },
             _updatePosition: function() {
                 var t = this._map.latLngToLayerPoint(this._latlng);
                 this._setPosition(t)
             },
             setOpacity: function(t) {
                 this.options.opacity = t, this._container && C(this._container, t)
             },
             _animateZoom: function(t) {
                 t = this._map._latLngToNewLayerPoint(this._latlng, t.zoom, t.center);
                 this._setPosition(t)
             },
             _getAnchor: function() {
-                return _(this._source && this._source._getTooltipAnchor && !this.options.sticky ? this._source._getTooltipAnchor() : [0, 0])
+                return m(this._source && this._source._getTooltipAnchor && !this.options.sticky ? this._source._getTooltipAnchor() : [0, 0])
             }
         })),
-        Be = (A.include({
-            openTooltip: function(t, i, e) {
-                return this._initOverlay(Ee, t, i, e).openOn(this), this
+        Xi = (O.include({
+            openTooltip: function(t, e, i) {
+                return this._initOverlay(Ji, t, e, i).openOn(this), this
             },
             closeTooltip: function(t) {
                 return t.close(), this
             }
-        }), o.include({
-            bindTooltip: function(t, i) {
-                return this._tooltip && this.isTooltipOpen() && this.unbindTooltip(), this._tooltip = this._initOverlay(Ee, this._tooltip, t, i), this._initTooltipInteractions(), this._tooltip.options.permanent && this._map && this._map.hasLayer(this) && this.openTooltip(), this
+        }), y.include({
+            bindTooltip: function(t, e) {
+                return this._tooltip && this.isTooltipOpen() && this.unbindTooltip(), this._tooltip = this._initOverlay(Ji, this._tooltip, t, e), this._initTooltipInteractions(), this._tooltip.options.permanent && this._map && this._map.hasLayer(this) && this.openTooltip(), this
             },
             unbindTooltip: function() {
                 return this._tooltip && (this._initTooltipInteractions(!0), this.closeTooltip(), this._tooltip = null), this
             },
             _initTooltipInteractions: function(t) {
-                var i, e;
-                !t && this._tooltipHandlersAdded || (i = t ? "off" : "on", e = {
+                var e, i;
+                !t && this._tooltipHandlersAdded || (e = t ? "off" : "on", i = {
                     remove: this.closeTooltip,
                     move: this._moveTooltip
-                }, this._tooltip.options.permanent ? e.add = this._openTooltip : (e.mouseover = this._openTooltip, e.mouseout = this.closeTooltip, e.click = this._openTooltip), this._tooltip.options.sticky && (e.mousemove = this._moveTooltip), this[i](e), this._tooltipHandlersAdded = !t)
+                }, this._tooltip.options.permanent ? i.add = this._openTooltip : (i.mouseover = this._openTooltip, i.mouseout = this.closeTooltip, i.click = this._openTooltip, this._map ? this._addFocusListeners() : i.add = this._addFocusListeners), this._tooltip.options.sticky && (i.mousemove = this._moveTooltip), this[e](i), this._tooltipHandlersAdded = !t)
             },
             openTooltip: function(t) {
-                return this._tooltip && this._tooltip._prepareOpen(t) && this._tooltip.openOn(this._map), this
+                return this._tooltip && this._tooltip._prepareOpen(t) && (this._tooltip.openOn(this._map), this.getElement ? this._setAriaDescribedByOnLayer(this) : this.eachLayer && this.eachLayer(this._setAriaDescribedByOnLayer, this)), this
             },
             closeTooltip: function() {
                 if (this._tooltip) return this._tooltip.close()
             },
             toggleTooltip: function() {
                 return this._tooltip && this._tooltip.toggle(this), this
             },
@@ -3469,43 +3549,58 @@
             },
             setTooltipContent: function(t) {
                 return this._tooltip && this._tooltip.setContent(t), this
             },
             getTooltip: function() {
                 return this._tooltip
             },
+            _addFocusListeners: function() {
+                this.getElement ? this._addFocusListenersOnLayer(this) : this.eachLayer && this.eachLayer(this._addFocusListenersOnLayer, this)
+            },
+            _addFocusListenersOnLayer: function(t) {
+                S(t.getElement(), "focus", function() {
+                    this._tooltip._source = t, this.openTooltip()
+                }, this), S(t.getElement(), "blur", this.closeTooltip, this)
+            },
+            _setAriaDescribedByOnLayer: function(t) {
+                t.getElement().setAttribute("aria-describedby", this._tooltip._container.id)
+            },
             _openTooltip: function(t) {
                 !this._tooltip || !this._map || this._map.dragging && this._map.dragging.moving() || (this._tooltip._source = t.layer || t.target, this.openTooltip(this._tooltip.options.sticky ? t.latlng : void 0))
             },
             _moveTooltip: function(t) {
-                var i = t.latlng;
-                this._tooltip.options.sticky && t.originalEvent && (t = this._map.mouseEventToContainerPoint(t.originalEvent), t = this._map.containerPointToLayerPoint(t), i = this._map.layerPointToLatLng(t)), this._tooltip.setLatLng(i)
+                var e = t.latlng;
+                this._tooltip.options.sticky && t.originalEvent && (t = this._map.mouseEventToContainerPoint(t.originalEvent), t = this._map.containerPointToLayerPoint(t), e = this._map.layerPointToLatLng(t)), this._tooltip.setLatLng(e)
             }
-        }), le.extend({
+        }), fi.extend({
             options: {
                 iconSize: [12, 12],
                 html: !1,
                 bgPos: null,
                 className: "leaflet-div-icon"
             },
             createIcon: function(t) {
                 var t = t && "DIV" === t.tagName ? t : document.createElement("div"),
-                    i = this.options;
-                return i.html instanceof Element ? (mi(t), t.appendChild(i.html)) : t.innerHTML = !1 !== i.html ? i.html : "", i.bgPos && (i = _(i.bgPos), t.style.backgroundPosition = -i.x + "px " + -i.y + "px"), this._setIconStyles(t, "icon"), t
+                    e = this.options;
+                return e.html instanceof Element ? (fe(t), t.appendChild(e.html)) : t.innerHTML = !1 !== e.html ? e.html : "", e.bgPos && (e = m(e.bgPos), t.style.backgroundPosition = -e.x + "px " + -e.y + "px"), this._setIconStyles(t, "icon"), t
             },
             createShadow: function() {
                 return null
             }
         }));
-    le.Default = ue;
-    var Ae = o.extend({
+
+    function $i(t) {
+        return new Xi(t)
+    }
+    fi.Default = vi;
+    var Qi = y.extend({
         options: {
             tileSize: 256,
             opacity: 1,
-            updateWhenIdle: P.mobile,
+            updateWhenIdle: b.mobile,
             updateWhenZooming: !0,
             updateInterval: 200,
             zIndex: 1,
             bounds: null,
             minZoom: 0,
             maxZoom: void 0,
             maxNativeZoom: void 0,
@@ -3524,18 +3619,18 @@
         beforeAdd: function(t) {
             t._addZoomLimit(this)
         },
         onRemove: function(t) {
             this._removeAllTiles(), T(this._container), t._removeZoomLimit(this), this._container = null, this._tileZoom = void 0
         },
         bringToFront: function() {
-            return this._map && (fi(this._container), this._setAutoZIndex(Math.max)), this
+            return this._map && (ge(this._container), this._setAutoZIndex(Math.max)), this
         },
         bringToBack: function() {
-            return this._map && (gi(this._container), this._setAutoZIndex(Math.min)), this
+            return this._map && (ve(this._container), this._setAutoZIndex(Math.min)), this
         },
         getContainer: function() {
             return this._container
         },
         setOpacity: function(t) {
             return this.options.opacity = t, this._updateOpacity(), this
         },
@@ -3552,387 +3647,389 @@
         getEvents: function() {
             var t = {
                 viewprereset: this._invalidateAll,
                 viewreset: this._resetView,
                 zoom: this._resetView,
                 moveend: this._onMoveEnd
             };
-            return this.options.updateWhenIdle || (this._onMove || (this._onMove = j(this._onMoveEnd, this.options.updateInterval, this)), t.move = this._onMove), this._zoomAnimated && (t.zoomanim = this._animateZoom), t
+            return this.options.updateWhenIdle || (this._onMove || (this._onMove = H(this._onMoveEnd, this.options.updateInterval, this)), t.move = this._onMove), this._zoomAnimated && (t.zoomanim = this._animateZoom), t
         },
         createTile: function() {
             return document.createElement("div")
         },
         getTileSize: function() {
             var t = this.options.tileSize;
             return t instanceof p ? t : new p(t, t)
         },
         _updateZIndex: function() {
             this._container && void 0 !== this.options.zIndex && null !== this.options.zIndex && (this._container.style.zIndex = this.options.zIndex)
         },
         _setAutoZIndex: function(t) {
-            for (var i, e = this.getPane().children, n = -t(-1 / 0, 1 / 0), o = 0, s = e.length; o < s; o++) i = e[o].style.zIndex, e[o] !== this._container && i && (n = t(n, +i));
+            for (var e, i = this.getPane().children, n = -t(-1 / 0, 1 / 0), o = 0, s = i.length; o < s; o++) e = i[o].style.zIndex, i[o] !== this._container && e && (n = t(n, +e));
             isFinite(n) && (this.options.zIndex = n + t(-1, 1), this._updateZIndex())
         },
         _updateOpacity: function() {
-            if (this._map && !P.ielt9) {
+            if (this._map && !b.ielt9) {
                 C(this._container, this.options.opacity);
-                var t, i = +new Date,
-                    e = !1,
+                var t, e = +new Date,
+                    i = !1,
                     n = !1;
                 for (t in this._tiles) {
                     var o, s = this._tiles[t];
-                    s.current && s.loaded && (o = Math.min(1, (i - s.loaded) / 200), C(s.el, o), o < 1 ? e = !0 : (s.active ? n = !0 : this._onOpaqueTile(s), s.active = !0))
+                    s.current && s.loaded && (o = Math.min(1, (e - s.loaded) / 200), C(s.el, o), o < 1 ? i = !0 : (s.active ? n = !0 : this._onOpaqueTile(s), s.active = !0))
                 }
-                n && !this._noPrune && this._pruneTiles(), e && (r(this._fadeFrame), this._fadeFrame = x(this._updateOpacity, this))
+                n && !this._noPrune && this._pruneTiles(), i && (r(this._fadeFrame), this._fadeFrame = x(this._updateOpacity, this))
             }
         },
         _onOpaqueTile: u,
         _initContainer: function() {
-            this._container || (this._container = b("div", "leaflet-layer " + (this.options.className || "")), this._updateZIndex(), this.options.opacity < 1 && this._updateOpacity(), this.getPane().appendChild(this._container))
+            this._container || (this._container = P("div", "leaflet-layer " + (this.options.className || "")), this._updateZIndex(), this.options.opacity < 1 && this._updateOpacity(), this.getPane().appendChild(this._container))
         },
         _updateLevels: function() {
             var t = this._tileZoom,
-                i = this.options.maxZoom;
+                e = this.options.maxZoom;
             if (void 0 !== t) {
-                for (var e in this._levels) e = Number(e), this._levels[e].el.children.length || e === t ? (this._levels[e].el.style.zIndex = i - Math.abs(t - e), this._onUpdateLevel(e)) : (T(this._levels[e].el), this._removeTilesAtZoom(e), this._onRemoveLevel(e), delete this._levels[e]);
+                for (var i in this._levels) i = Number(i), this._levels[i].el.children.length || i === t ? (this._levels[i].el.style.zIndex = e - Math.abs(t - i), this._onUpdateLevel(i)) : (T(this._levels[i].el), this._removeTilesAtZoom(i), this._onRemoveLevel(i), delete this._levels[i]);
                 var n = this._levels[t],
                     o = this._map;
-                return n || ((n = this._levels[t] = {}).el = b("div", "leaflet-tile-container leaflet-zoom-animated", this._container), n.el.style.zIndex = i, n.origin = o.project(o.unproject(o.getPixelOrigin()), t).round(), n.zoom = t, this._setZoomTransform(n, o.getCenter(), o.getZoom()), u(n.el.offsetWidth), this._onCreateLevel(n)), this._level = n
+                return n || ((n = this._levels[t] = {}).el = P("div", "leaflet-tile-container leaflet-zoom-animated", this._container), n.el.style.zIndex = e, n.origin = o.project(o.unproject(o.getPixelOrigin()), t).round(), n.zoom = t, this._setZoomTransform(n, o.getCenter(), o.getZoom()), u(n.el.offsetWidth), this._onCreateLevel(n)), this._level = n
             }
         },
         _onUpdateLevel: u,
         _onRemoveLevel: u,
         _onCreateLevel: u,
         _pruneTiles: function() {
             if (this._map) {
-                var t, i, e, n = this._map.getZoom();
+                var t, e, i, n = this._map.getZoom();
                 if (n > this.options.maxZoom || n < this.options.minZoom) this._removeAllTiles();
                 else {
-                    for (t in this._tiles)(e = this._tiles[t]).retain = e.current;
-                    for (t in this._tiles)(e = this._tiles[t]).current && !e.active && (i = e.coords, this._retainParent(i.x, i.y, i.z, i.z - 5) || this._retainChildren(i.x, i.y, i.z, i.z + 2));
+                    for (t in this._tiles)(i = this._tiles[t]).retain = i.current;
+                    for (t in this._tiles)(i = this._tiles[t]).current && !i.active && (e = i.coords, this._retainParent(e.x, e.y, e.z, e.z - 5) || this._retainChildren(e.x, e.y, e.z, e.z + 2));
                     for (t in this._tiles) this._tiles[t].retain || this._removeTile(t)
                 }
             }
         },
         _removeTilesAtZoom: function(t) {
-            for (var i in this._tiles) this._tiles[i].coords.z === t && this._removeTile(i)
+            for (var e in this._tiles) this._tiles[e].coords.z === t && this._removeTile(e)
         },
         _removeAllTiles: function() {
             for (var t in this._tiles) this._removeTile(t)
         },
         _invalidateAll: function() {
             for (var t in this._levels) T(this._levels[t].el), this._onRemoveLevel(Number(t)), delete this._levels[t];
             this._removeAllTiles(), this._tileZoom = void 0
         },
-        _retainParent: function(t, i, e, n) {
+        _retainParent: function(t, e, i, n) {
             var t = Math.floor(t / 2),
-                i = Math.floor(i / 2),
-                e = e - 1,
-                o = new p(+t, +i),
-                o = (o.z = e, this._tileCoordsToKey(o)),
+                e = Math.floor(e / 2),
+                i = i - 1,
+                o = new p(+t, +e),
+                o = (o.z = i, this._tileCoordsToKey(o)),
                 o = this._tiles[o];
-            return o && o.active ? o.retain = !0 : (o && o.loaded && (o.retain = !0), n < e && this._retainParent(t, i, e, n))
+            return o && o.active ? o.retain = !0 : (o && o.loaded && (o.retain = !0), n < i && this._retainParent(t, e, i, n))
         },
-        _retainChildren: function(t, i, e, n) {
+        _retainChildren: function(t, e, i, n) {
             for (var o = 2 * t; o < 2 * t + 2; o++)
-                for (var s = 2 * i; s < 2 * i + 2; s++) {
+                for (var s = 2 * e; s < 2 * e + 2; s++) {
                     var r = new p(o, s),
-                        r = (r.z = e + 1, this._tileCoordsToKey(r)),
+                        r = (r.z = i + 1, this._tileCoordsToKey(r)),
                         r = this._tiles[r];
-                    r && r.active ? r.retain = !0 : (r && r.loaded && (r.retain = !0), e + 1 < n && this._retainChildren(o, s, e + 1, n))
+                    r && r.active ? r.retain = !0 : (r && r.loaded && (r.retain = !0), i + 1 < n && this._retainChildren(o, s, i + 1, n))
                 }
         },
         _resetView: function(t) {
             t = t && (t.pinch || t.flyTo);
             this._setView(this._map.getCenter(), this._map.getZoom(), t, t)
         },
         _animateZoom: function(t) {
             this._setView(t.center, t.zoom, !0, t.noUpdate)
         },
         _clampZoom: function(t) {
-            var i = this.options;
-            return void 0 !== i.minNativeZoom && t < i.minNativeZoom ? i.minNativeZoom : void 0 !== i.maxNativeZoom && i.maxNativeZoom < t ? i.maxNativeZoom : t
+            var e = this.options;
+            return void 0 !== e.minNativeZoom && t < e.minNativeZoom ? e.minNativeZoom : void 0 !== e.maxNativeZoom && e.maxNativeZoom < t ? e.maxNativeZoom : t
         },
-        _setView: function(t, i, e, n) {
-            var o = Math.round(i),
+        _setView: function(t, e, i, n) {
+            var o = Math.round(e),
                 o = void 0 !== this.options.maxZoom && o > this.options.maxZoom || void 0 !== this.options.minZoom && o < this.options.minZoom ? void 0 : this._clampZoom(o),
                 s = this.options.updateWhenZooming && o !== this._tileZoom;
-            n && !s || (this._tileZoom = o, this._abortLoading && this._abortLoading(), this._updateLevels(), this._resetGrid(), void 0 !== o && this._update(t), e || this._pruneTiles(), this._noPrune = !!e), this._setZoomTransforms(t, i)
+            n && !s || (this._tileZoom = o, this._abortLoading && this._abortLoading(), this._updateLevels(), this._resetGrid(), void 0 !== o && this._update(t), i || this._pruneTiles(), this._noPrune = !!i), this._setZoomTransforms(t, e)
         },
-        _setZoomTransforms: function(t, i) {
-            for (var e in this._levels) this._setZoomTransform(this._levels[e], t, i)
+        _setZoomTransforms: function(t, e) {
+            for (var i in this._levels) this._setZoomTransform(this._levels[i], t, e)
         },
-        _setZoomTransform: function(t, i, e) {
-            var n = this._map.getZoomScale(e, t.zoom),
-                i = t.origin.multiplyBy(n).subtract(this._map._getNewPixelOrigin(i, e)).round();
-            P.any3d ? Pi(t.el, i, n) : Z(t.el, i)
+        _setZoomTransform: function(t, e, i) {
+            var n = this._map.getZoomScale(i, t.zoom),
+                e = t.origin.multiplyBy(n).subtract(this._map._getNewPixelOrigin(e, i)).round();
+            b.any3d ? Pe(t.el, e, n) : Z(t.el, e)
         },
         _resetGrid: function() {
             var t = this._map,
-                i = t.options.crs,
-                e = this._tileSize = this.getTileSize(),
+                e = t.options.crs,
+                i = this._tileSize = this.getTileSize(),
                 n = this._tileZoom,
                 o = this._map.getPixelWorldBounds(this._tileZoom);
-            o && (this._globalTileRange = this._pxBoundsToTileRange(o)), this._wrapX = i.wrapLng && !this.options.noWrap && [Math.floor(t.project([0, i.wrapLng[0]], n).x / e.x), Math.ceil(t.project([0, i.wrapLng[1]], n).x / e.y)], this._wrapY = i.wrapLat && !this.options.noWrap && [Math.floor(t.project([i.wrapLat[0], 0], n).y / e.x), Math.ceil(t.project([i.wrapLat[1], 0], n).y / e.y)]
+            o && (this._globalTileRange = this._pxBoundsToTileRange(o)), this._wrapX = e.wrapLng && !this.options.noWrap && [Math.floor(t.project([0, e.wrapLng[0]], n).x / i.x), Math.ceil(t.project([0, e.wrapLng[1]], n).x / i.y)], this._wrapY = e.wrapLat && !this.options.noWrap && [Math.floor(t.project([e.wrapLat[0], 0], n).y / i.x), Math.ceil(t.project([e.wrapLat[1], 0], n).y / i.y)]
         },
         _onMoveEnd: function() {
             this._map && !this._map._animatingZoom && this._update()
         },
         _getTiledPixelBounds: function(t) {
-            var i = this._map,
-                e = i._animatingZoom ? Math.max(i._animateToZoom, i.getZoom()) : i.getZoom(),
-                e = i.getZoomScale(e, this._tileZoom),
-                t = i.project(t, this._tileZoom).floor(),
-                i = i.getSize().divideBy(2 * e);
-            return new m(t.subtract(i), t.add(i))
+            var e = this._map,
+                i = e._animatingZoom ? Math.max(e._animateToZoom, e.getZoom()) : e.getZoom(),
+                i = e.getZoomScale(i, this._tileZoom),
+                t = e.project(t, this._tileZoom).floor(),
+                e = e.getSize().divideBy(2 * i);
+            return new f(t.subtract(e), t.add(e))
         },
         _update: function(t) {
-            var i = this._map;
-            if (i) {
-                var e = this._clampZoom(i.getZoom());
-                if (void 0 === t && (t = i.getCenter()), void 0 !== this._tileZoom) {
-                    var n, i = this._getTiledPixelBounds(t),
-                        o = this._pxBoundsToTileRange(i),
+            var e = this._map;
+            if (e) {
+                var i = this._clampZoom(e.getZoom());
+                if (void 0 === t && (t = e.getCenter()), void 0 !== this._tileZoom) {
+                    var n, e = this._getTiledPixelBounds(t),
+                        o = this._pxBoundsToTileRange(e),
                         s = o.getCenter(),
                         r = [],
-                        i = this.options.keepBuffer,
-                        a = new m(o.getBottomLeft().subtract([i, -i]), o.getTopRight().add([i, -i]));
+                        e = this.options.keepBuffer,
+                        a = new f(o.getBottomLeft().subtract([e, -e]), o.getTopRight().add([e, -e]));
                     if (!(isFinite(o.min.x) && isFinite(o.min.y) && isFinite(o.max.x) && isFinite(o.max.y))) throw new Error("Attempted to load an infinite number of tiles");
                     for (n in this._tiles) {
                         var h = this._tiles[n].coords;
                         h.z === this._tileZoom && a.contains(new p(h.x, h.y)) || (this._tiles[n].current = !1)
                     }
-                    if (1 < Math.abs(e - this._tileZoom)) this._setView(t, e);
+                    if (1 < Math.abs(i - this._tileZoom)) this._setView(t, i);
                     else {
                         for (var l = o.min.y; l <= o.max.y; l++)
                             for (var u = o.min.x; u <= o.max.x; u++) {
                                 var c, d = new p(u, l);
                                 d.z = this._tileZoom, this._isValidTile(d) && ((c = this._tiles[this._tileCoordsToKey(d)]) ? c.current = !0 : r.push(d))
                             }
-                        if (r.sort(function(t, i) {
-                                return t.distanceTo(s) - i.distanceTo(s)
+                        if (r.sort(function(t, e) {
+                                return t.distanceTo(s) - e.distanceTo(s)
                             }), 0 !== r.length) {
                             this._loading || (this._loading = !0, this.fire("loading"));
                             for (var _ = document.createDocumentFragment(), u = 0; u < r.length; u++) this._addTile(r[u], _);
                             this._level.el.appendChild(_)
                         }
                     }
                 }
             }
         },
         _isValidTile: function(t) {
-            var i = this._map.options.crs;
-            if (!i.infinite) {
-                var e = this._globalTileRange;
-                if (!i.wrapLng && (t.x < e.min.x || t.x > e.max.x) || !i.wrapLat && (t.y < e.min.y || t.y > e.max.y)) return !1
-            }
-            if (!this.options.bounds) return !0;
-            i = this._tileCoordsToBounds(t);
-            return g(this.options.bounds).overlaps(i)
+            var e = this._map.options.crs;
+            if (!e.infinite) {
+                var i = this._globalTileRange;
+                if (!e.wrapLng && (t.x < i.min.x || t.x > i.max.x) || !e.wrapLat && (t.y < i.min.y || t.y > i.max.y)) return !1
+            }
+            return !this.options.bounds || (e = this._tileCoordsToBounds(t), g(this.options.bounds).overlaps(e))
         },
         _keyToBounds: function(t) {
             return this._tileCoordsToBounds(this._keyToTileCoords(t))
         },
         _tileCoordsToNwSe: function(t) {
-            var i = this._map,
-                e = this.getTileSize(),
-                n = t.scaleBy(e),
-                e = n.add(e);
-            return [i.unproject(n, t.z), i.unproject(e, t.z)]
+            var e = this._map,
+                i = this.getTileSize(),
+                n = t.scaleBy(i),
+                i = n.add(i);
+            return [e.unproject(n, t.z), e.unproject(i, t.z)]
         },
         _tileCoordsToBounds: function(t) {
             t = this._tileCoordsToNwSe(t), t = new s(t[0], t[1]);
             return t = this.options.noWrap ? t : this._map.wrapLatLngBounds(t)
         },
         _tileCoordsToKey: function(t) {
             return t.x + ":" + t.y + ":" + t.z
         },
         _keyToTileCoords: function(t) {
             var t = t.split(":"),
-                i = new p(+t[0], +t[1]);
-            return i.z = +t[2], i
+                e = new p(+t[0], +t[1]);
+            return e.z = +t[2], e
         },
         _removeTile: function(t) {
-            var i = this._tiles[t];
-            i && (T(i.el), delete this._tiles[t], this.fire("tileunload", {
-                tile: i.el,
+            var e = this._tiles[t];
+            e && (T(e.el), delete this._tiles[t], this.fire("tileunload", {
+                tile: e.el,
                 coords: this._keyToTileCoords(t)
             }))
         },
         _initTile: function(t) {
-            z(t, "leaflet-tile");
-            var i = this.getTileSize();
-            t.style.width = i.x + "px", t.style.height = i.y + "px", t.onselectstart = u, t.onmousemove = u, P.ielt9 && this.options.opacity < 1 && C(t, this.options.opacity)
+            M(t, "leaflet-tile");
+            var e = this.getTileSize();
+            t.style.width = e.x + "px", t.style.height = e.y + "px", t.onselectstart = u, t.onmousemove = u, b.ielt9 && this.options.opacity < 1 && C(t, this.options.opacity)
         },
-        _addTile: function(t, i) {
-            var e = this._getTilePos(t),
+        _addTile: function(t, e) {
+            var i = this._getTilePos(t),
                 n = this._tileCoordsToKey(t),
                 o = this.createTile(this._wrapCoords(t), a(this._tileReady, this, t));
-            this._initTile(o), this.createTile.length < 2 && x(a(this._tileReady, this, t, null, o)), Z(o, e), this._tiles[n] = {
+            this._initTile(o), this.createTile.length < 2 && x(a(this._tileReady, this, t, null, o)), Z(o, i), this._tiles[n] = {
                 el: o,
                 coords: t,
                 current: !0
-            }, i.appendChild(o), this.fire("tileloadstart", {
+            }, e.appendChild(o), this.fire("tileloadstart", {
                 tile: o,
                 coords: t
             })
         },
-        _tileReady: function(t, i, e) {
-            i && this.fire("tileerror", {
-                error: i,
-                tile: e,
+        _tileReady: function(t, e, i) {
+            e && this.fire("tileerror", {
+                error: e,
+                tile: i,
                 coords: t
             });
             var n = this._tileCoordsToKey(t);
-            (e = this._tiles[n]) && (e.loaded = +new Date, this._map._fadeAnimated ? (C(e.el, 0), r(this._fadeFrame), this._fadeFrame = x(this._updateOpacity, this)) : (e.active = !0, this._pruneTiles()), i || (z(e.el, "leaflet-tile-loaded"), this.fire("tileload", {
-                tile: e.el,
+            (i = this._tiles[n]) && (i.loaded = +new Date, this._map._fadeAnimated ? (C(i.el, 0), r(this._fadeFrame), this._fadeFrame = x(this._updateOpacity, this)) : (i.active = !0, this._pruneTiles()), e || (M(i.el, "leaflet-tile-loaded"), this.fire("tileload", {
+                tile: i.el,
                 coords: t
-            })), this._noTilesToLoad() && (this._loading = !1, this.fire("load"), P.ielt9 || !this._map._fadeAnimated ? x(this._pruneTiles, this) : setTimeout(a(this._pruneTiles, this), 250)))
+            })), this._noTilesToLoad() && (this._loading = !1, this.fire("load"), b.ielt9 || !this._map._fadeAnimated ? x(this._pruneTiles, this) : setTimeout(a(this._pruneTiles, this), 250)))
         },
         _getTilePos: function(t) {
             return t.scaleBy(this.getTileSize()).subtract(this._level.origin)
         },
         _wrapCoords: function(t) {
-            var i = new p(this._wrapX ? H(t.x, this._wrapX) : t.x, this._wrapY ? H(t.y, this._wrapY) : t.y);
-            return i.z = t.z, i
+            var e = new p(this._wrapX ? F(t.x, this._wrapX) : t.x, this._wrapY ? F(t.y, this._wrapY) : t.y);
+            return e.z = t.z, e
         },
         _pxBoundsToTileRange: function(t) {
-            var i = this.getTileSize();
-            return new m(t.min.unscaleBy(i).floor(), t.max.unscaleBy(i).ceil().subtract([1, 1]))
+            var e = this.getTileSize();
+            return new f(t.min.unscaleBy(e).floor(), t.max.unscaleBy(e).ceil().subtract([1, 1]))
         },
         _noTilesToLoad: function() {
             for (var t in this._tiles)
                 if (!this._tiles[t].loaded) return !1;
             return !0
         }
     });
-    var Ie = Ae.extend({
+
+    function tn(t) {
+        return new Qi(t)
+    }
+    var en = Qi.extend({
         options: {
             minZoom: 0,
             maxZoom: 18,
             subdomains: "abc",
             errorTileUrl: "",
             zoomOffset: 0,
             tms: !1,
             zoomReverse: !1,
             detectRetina: !1,
             crossOrigin: !1,
             referrerPolicy: !1
         },
-        initialize: function(t, i) {
-            this._url = t, (i = c(this, i)).detectRetina && P.retina && 0 < i.maxZoom && (i.tileSize = Math.floor(i.tileSize / 2), i.zoomReverse ? (i.zoomOffset--, i.minZoom++) : (i.zoomOffset++, i.maxZoom--), i.minZoom = Math.max(0, i.minZoom)), "string" == typeof i.subdomains && (i.subdomains = i.subdomains.split("")), this.on("tileunload", this._onTileRemove)
+        initialize: function(t, e) {
+            this._url = t, (e = c(this, e)).detectRetina && b.retina && 0 < e.maxZoom ? (e.tileSize = Math.floor(e.tileSize / 2), e.zoomReverse ? (e.zoomOffset--, e.minZoom = Math.min(e.maxZoom, e.minZoom + 1)) : (e.zoomOffset++, e.maxZoom = Math.max(e.minZoom, e.maxZoom - 1)), e.minZoom = Math.max(0, e.minZoom)) : e.zoomReverse ? e.minZoom = Math.min(e.maxZoom, e.minZoom) : e.maxZoom = Math.max(e.minZoom, e.maxZoom), "string" == typeof e.subdomains && (e.subdomains = e.subdomains.split("")), this.on("tileunload", this._onTileRemove)
         },
-        setUrl: function(t, i) {
-            return this._url === t && void 0 === i && (i = !0), this._url = t, i || this.redraw(), this
+        setUrl: function(t, e) {
+            return this._url === t && void 0 === e && (e = !0), this._url = t, e || this.redraw(), this
         },
-        createTile: function(t, i) {
-            var e = document.createElement("img");
-            return S(e, "load", a(this._tileOnLoad, this, i, e)), S(e, "error", a(this._tileOnError, this, i, e)), !this.options.crossOrigin && "" !== this.options.crossOrigin || (e.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), "string" == typeof this.options.referrerPolicy && (e.referrerPolicy = this.options.referrerPolicy), e.alt = "", e.setAttribute("role", "presentation"), e.src = this.getTileUrl(t), e
+        createTile: function(t, e) {
+            var i = document.createElement("img");
+            return S(i, "load", a(this._tileOnLoad, this, e, i)), S(i, "error", a(this._tileOnError, this, e, i)), !this.options.crossOrigin && "" !== this.options.crossOrigin || (i.crossOrigin = !0 === this.options.crossOrigin ? "" : this.options.crossOrigin), "string" == typeof this.options.referrerPolicy && (i.referrerPolicy = this.options.referrerPolicy), i.alt = "", i.src = this.getTileUrl(t), i
         },
         getTileUrl: function(t) {
-            var i = {
-                r: P.retina ? "@2x" : "",
+            var e = {
+                r: b.retina ? "@2x" : "",
                 s: this._getSubdomain(t),
                 x: t.x,
                 y: t.y,
                 z: this._getZoomForUrl()
             };
-            return this._map && !this._map.options.crs.infinite && (t = this._globalTileRange.max.y - t.y, this.options.tms && (i.y = t), i["-y"] = t), q(this._url, l(i, this.options))
+            return this._map && !this._map.options.crs.infinite && (t = this._globalTileRange.max.y - t.y, this.options.tms && (e.y = t), e["-y"] = t), q(this._url, l(e, this.options))
         },
-        _tileOnLoad: function(t, i) {
-            P.ielt9 ? setTimeout(a(t, this, null, i), 0) : t(null, i)
+        _tileOnLoad: function(t, e) {
+            b.ielt9 ? setTimeout(a(t, this, null, e), 0) : t(null, e)
         },
-        _tileOnError: function(t, i, e) {
+        _tileOnError: function(t, e, i) {
             var n = this.options.errorTileUrl;
-            n && i.getAttribute("src") !== n && (i.src = n), t(e, i)
+            n && e.getAttribute("src") !== n && (e.src = n), t(i, e)
         },
         _onTileRemove: function(t) {
             t.tile.onload = null
         },
         _getZoomForUrl: function() {
             var t = this._tileZoom,
-                i = this.options.maxZoom;
-            return (t = this.options.zoomReverse ? i - t : t) + this.options.zoomOffset
+                e = this.options.maxZoom;
+            return (t = this.options.zoomReverse ? e - t : t) + this.options.zoomOffset
         },
         _getSubdomain: function(t) {
             t = Math.abs(t.x + t.y) % this.options.subdomains.length;
             return this.options.subdomains[t]
         },
         _abortLoading: function() {
-            var t, i, e;
-            for (t in this._tiles) this._tiles[t].coords.z !== this._tileZoom && ((e = this._tiles[t].el).onload = u, e.onerror = u, e.complete || (e.src = K, i = this._tiles[t].coords, T(e), delete this._tiles[t], this.fire("tileabort", {
-                tile: e,
-                coords: i
+            var t, e, i;
+            for (t in this._tiles) this._tiles[t].coords.z !== this._tileZoom && ((i = this._tiles[t].el).onload = u, i.onerror = u, i.complete || (i.src = Y, e = this._tiles[t].coords, T(i), delete this._tiles[t], this.fire("tileabort", {
+                tile: i,
+                coords: e
             })))
         },
         _removeTile: function(t) {
-            var i = this._tiles[t];
-            if (i) return i.el.setAttribute("src", K), Ae.prototype._removeTile.call(this, t)
+            var e = this._tiles[t];
+            if (e) return e.el.setAttribute("src", Y), Qi.prototype._removeTile.call(this, t)
         },
-        _tileReady: function(t, i, e) {
-            if (this._map && (!e || e.getAttribute("src") !== K)) return Ae.prototype._tileReady.call(this, t, i, e)
+        _tileReady: function(t, e, i) {
+            if (this._map && (!i || i.getAttribute("src") !== Y)) return Qi.prototype._tileReady.call(this, t, e, i)
         }
     });
 
-    function Oe(t, i) {
-        return new Ie(t, i)
+    function nn(t, e) {
+        return new en(t, e)
     }
-    var Re = Ie.extend({
+    var on = en.extend({
         defaultWmsParams: {
             service: "WMS",
             request: "GetMap",
             layers: "",
             styles: "",
             format: "image/jpeg",
             transparent: !1,
             version: "1.1.1"
         },
         options: {
             crs: null,
             uppercase: !1
         },
-        initialize: function(t, i) {
+        initialize: function(t, e) {
             this._url = t;
-            var e, n = l({}, this.defaultWmsParams);
-            for (e in i) e in this.options || (n[e] = i[e]);
-            var t = (i = c(this, i)).detectRetina && P.retina ? 2 : 1,
+            var i, n = l({}, this.defaultWmsParams);
+            for (i in e) i in this.options || (n[i] = e[i]);
+            var t = (e = c(this, e)).detectRetina && b.retina ? 2 : 1,
                 o = this.getTileSize();
             n.width = o.x * t, n.height = o.y * t, this.wmsParams = n
         },
         onAdd: function(t) {
             this._crs = this.options.crs || t.options.crs, this._wmsVersion = parseFloat(this.wmsParams.version);
-            var i = 1.3 <= this._wmsVersion ? "crs" : "srs";
-            this.wmsParams[i] = this._crs.code, Ie.prototype.onAdd.call(this, t)
+            var e = 1.3 <= this._wmsVersion ? "crs" : "srs";
+            this.wmsParams[e] = this._crs.code, en.prototype.onAdd.call(this, t)
         },
         getTileUrl: function(t) {
-            var i = this._tileCoordsToNwSe(t),
-                e = this._crs,
-                e = f(e.project(i[0]), e.project(i[1])),
-                i = e.min,
-                e = e.max,
-                i = (1.3 <= this._wmsVersion && this._crs === re ? [i.y, i.x, e.y, e.x] : [i.x, i.y, e.x, e.y]).join(","),
-                e = Ie.prototype.getTileUrl.call(this, t);
-            return e + U(this.wmsParams, e, this.options.uppercase) + (this.options.uppercase ? "&BBOX=" : "&bbox=") + i
+            var e = this._tileCoordsToNwSe(t),
+                i = this._crs,
+                i = _(i.project(e[0]), i.project(e[1])),
+                e = i.min,
+                i = i.max,
+                e = (1.3 <= this._wmsVersion && this._crs === _i ? [e.y, e.x, i.y, i.x] : [e.x, e.y, i.x, i.y]).join(","),
+                i = en.prototype.getTileUrl.call(this, t);
+            return i + V(this.wmsParams, i, this.options.uppercase) + (this.options.uppercase ? "&BBOX=" : "&bbox=") + e
         },
-        setParams: function(t, i) {
-            return l(this.wmsParams, t), i || this.redraw(), this
+        setParams: function(t, e) {
+            return l(this.wmsParams, t), e || this.redraw(), this
         }
     });
-    Ie.WMS = Re, Oe.wms = function(t, i) {
-        return new Re(t, i)
+    en.WMS = on, nn.wms = function(t, e) {
+        return new on(t, e)
     };
-    var Ne = o.extend({
+    var sn = y.extend({
             options: {
                 padding: .1
             },
             initialize: function(t) {
                 c(this, t), h(this), this._layers = this._layers || {}
             },
             onAdd: function() {
-                this._container || (this._initContainer(), this._zoomAnimated && z(this._container, "leaflet-zoom-animated")), this.getPane().appendChild(this._container), this._update(), this.on("update", this._updatePaths, this)
+                this._container || (this._initContainer(), this._zoomAnimated && M(this._container, "leaflet-zoom-animated")), this.getPane().appendChild(this._container), this._update(), this.on("update", this._updatePaths, this)
             },
             onRemove: function() {
                 this.off("update", this._updatePaths, this), this._destroyContainer()
             },
             getEvents: function() {
                 var t = {
                     viewreset: this._reset,
@@ -3944,50 +4041,50 @@
             },
             _onAnimZoom: function(t) {
                 this._updateTransform(t.center, t.zoom)
             },
             _onZoom: function() {
                 this._updateTransform(this._map.getCenter(), this._map.getZoom())
             },
-            _updateTransform: function(t, i) {
-                var e = this._map.getZoomScale(i, this._zoom),
+            _updateTransform: function(t, e) {
+                var i = this._map.getZoomScale(e, this._zoom),
                     n = this._map.getSize().multiplyBy(.5 + this.options.padding),
-                    o = this._map.project(this._center, i),
-                    n = n.multiplyBy(-e).add(o).subtract(this._map._getNewPixelOrigin(t, i));
-                P.any3d ? Pi(this._container, n, e) : Z(this._container, n)
+                    o = this._map.project(this._center, e),
+                    n = n.multiplyBy(-i).add(o).subtract(this._map._getNewPixelOrigin(t, e));
+                b.any3d ? Pe(this._container, n, i) : Z(this._container, n)
             },
             _reset: function() {
                 for (var t in this._update(), this._updateTransform(this._center, this._zoom), this._layers) this._layers[t]._reset()
             },
             _onZoomEnd: function() {
                 for (var t in this._layers) this._layers[t]._project()
             },
             _updatePaths: function() {
                 for (var t in this._layers) this._layers[t]._update()
             },
             _update: function() {
                 var t = this.options.padding,
-                    i = this._map.getSize(),
-                    e = this._map.containerPointToLayerPoint(i.multiplyBy(-t)).round();
-                this._bounds = new m(e, e.add(i.multiplyBy(1 + 2 * t)).round()), this._center = this._map.getCenter(), this._zoom = this._map.getZoom()
+                    e = this._map.getSize(),
+                    i = this._map.containerPointToLayerPoint(e.multiplyBy(-t)).round();
+                this._bounds = new f(i, i.add(e.multiplyBy(1 + 2 * t)).round()), this._center = this._map.getCenter(), this._zoom = this._map.getZoom()
             }
         }),
-        De = Ne.extend({
+        rn = sn.extend({
             options: {
                 tolerance: 0
             },
             getEvents: function() {
-                var t = Ne.prototype.getEvents.call(this);
+                var t = sn.prototype.getEvents.call(this);
                 return t.viewprereset = this._onViewPreReset, t
             },
             _onViewPreReset: function() {
                 this._postponeUpdatePaths = !0
             },
             onAdd: function() {
-                Ne.prototype.onAdd.call(this), this._draw()
+                sn.prototype.onAdd.call(this), this._draw()
             },
             _initContainer: function() {
                 var t = this._container = document.createElement("canvas");
                 S(t, "mousemove", this._onMouseMove, this), S(t, "click dblclick mousedown mouseup contextmenu", this._onClick, this), S(t, "mouseout", this._handleMouseOut, this), t._leaflet_disable_events = !0, this._ctx = t.getContext("2d")
             },
             _destroyContainer: function() {
                 r(this._redrawRequest), delete this._ctx, T(this._container), E(this._container), delete this._container
@@ -3995,629 +4092,686 @@
             _updatePaths: function() {
                 if (!this._postponeUpdatePaths) {
                     for (var t in this._redrawBounds = null, this._layers) this._layers[t]._update();
                     this._redraw()
                 }
             },
             _update: function() {
-                var t, i, e, n;
-                this._map._animatingZoom && this._bounds || (Ne.prototype._update.call(this), t = this._bounds, i = this._container, e = t.getSize(), n = P.retina ? 2 : 1, Z(i, t.min), i.width = n * e.x, i.height = n * e.y, i.style.width = e.x + "px", i.style.height = e.y + "px", P.retina && this._ctx.scale(2, 2), this._ctx.translate(-t.min.x, -t.min.y), this.fire("update"))
+                var t, e, i, n;
+                this._map._animatingZoom && this._bounds || (sn.prototype._update.call(this), t = this._bounds, e = this._container, i = t.getSize(), n = b.retina ? 2 : 1, Z(e, t.min), e.width = n * i.x, e.height = n * i.y, e.style.width = i.x + "px", e.style.height = i.y + "px", b.retina && this._ctx.scale(2, 2), this._ctx.translate(-t.min.x, -t.min.y), this.fire("update"))
             },
             _reset: function() {
-                Ne.prototype._reset.call(this), this._postponeUpdatePaths && (this._postponeUpdatePaths = !1, this._updatePaths())
+                sn.prototype._reset.call(this), this._postponeUpdatePaths && (this._postponeUpdatePaths = !1, this._updatePaths())
             },
             _initPath: function(t) {
                 this._updateDashArray(t);
                 t = (this._layers[h(t)] = t)._order = {
                     layer: t,
                     prev: this._drawLast,
                     next: null
                 };
                 this._drawLast && (this._drawLast.next = t), this._drawLast = t, this._drawFirst = this._drawFirst || this._drawLast
             },
             _addPath: function(t) {
                 this._requestRedraw(t)
             },
             _removePath: function(t) {
-                var i = t._order,
-                    e = i.next,
-                    i = i.prev;
-                e ? e.prev = i : this._drawLast = i, i ? i.next = e : this._drawFirst = e, delete t._order, delete this._layers[h(t)], this._requestRedraw(t)
+                var e = t._order,
+                    i = e.next,
+                    e = e.prev;
+                i ? i.prev = e : this._drawLast = e, e ? e.next = i : this._drawFirst = i, delete t._order, delete this._layers[h(t)], this._requestRedraw(t)
             },
             _updatePath: function(t) {
                 this._extendRedrawBounds(t), t._project(), t._update(), this._requestRedraw(t)
             },
             _updateStyle: function(t) {
                 this._updateDashArray(t), this._requestRedraw(t)
             },
             _updateDashArray: function(t) {
                 if ("string" == typeof t.options.dashArray) {
-                    for (var i, e = t.options.dashArray.split(/[, ]+/), n = [], o = 0; o < e.length; o++) {
-                        if (i = Number(e[o]), isNaN(i)) return;
-                        n.push(i)
+                    for (var e, i = t.options.dashArray.split(/[, ]+/), n = [], o = 0; o < i.length; o++) {
+                        if (e = Number(i[o]), isNaN(e)) return;
+                        n.push(e)
                     }
                     t.options._dashArray = n
                 } else t.options._dashArray = t.options.dashArray
             },
             _requestRedraw: function(t) {
                 this._map && (this._extendRedrawBounds(t), this._redrawRequest = this._redrawRequest || x(this._redraw, this))
             },
             _extendRedrawBounds: function(t) {
-                var i;
-                t._pxBounds && (i = (t.options.weight || 0) + 1, this._redrawBounds = this._redrawBounds || new m, this._redrawBounds.extend(t._pxBounds.min.subtract([i, i])), this._redrawBounds.extend(t._pxBounds.max.add([i, i])))
+                var e;
+                t._pxBounds && (e = (t.options.weight || 0) + 1, this._redrawBounds = this._redrawBounds || new f, this._redrawBounds.extend(t._pxBounds.min.subtract([e, e])), this._redrawBounds.extend(t._pxBounds.max.add([e, e])))
             },
             _redraw: function() {
                 this._redrawRequest = null, this._redrawBounds && (this._redrawBounds.min._floor(), this._redrawBounds.max._ceil()), this._clear(), this._draw(), this._redrawBounds = null
             },
             _clear: function() {
-                var t, i = this._redrawBounds;
-                i ? (t = i.getSize(), this._ctx.clearRect(i.min.x, i.min.y, t.x, t.y)) : (this._ctx.save(), this._ctx.setTransform(1, 0, 0, 1, 0, 0), this._ctx.clearRect(0, 0, this._container.width, this._container.height), this._ctx.restore())
+                var t, e = this._redrawBounds;
+                e ? (t = e.getSize(), this._ctx.clearRect(e.min.x, e.min.y, t.x, t.y)) : (this._ctx.save(), this._ctx.setTransform(1, 0, 0, 1, 0, 0), this._ctx.clearRect(0, 0, this._container.width, this._container.height), this._ctx.restore())
             },
             _draw: function() {
-                var t, i, e = this._redrawBounds;
-                this._ctx.save(), e && (i = e.getSize(), this._ctx.beginPath(), this._ctx.rect(e.min.x, e.min.y, i.x, i.y), this._ctx.clip()), this._drawing = !0;
-                for (var n = this._drawFirst; n; n = n.next) t = n.layer, (!e || t._pxBounds && t._pxBounds.intersects(e)) && t._updatePath();
+                var t, e, i = this._redrawBounds;
+                this._ctx.save(), i && (e = i.getSize(), this._ctx.beginPath(), this._ctx.rect(i.min.x, i.min.y, e.x, e.y), this._ctx.clip()), this._drawing = !0;
+                for (var n = this._drawFirst; n; n = n.next) t = n.layer, (!i || t._pxBounds && t._pxBounds.intersects(i)) && t._updatePath();
                 this._drawing = !1, this._ctx.restore()
             },
-            _updatePoly: function(t, i) {
+            _updatePoly: function(t, e) {
                 if (this._drawing) {
-                    var e, n, o, s, r = t._parts,
+                    var i, n, o, s, r = t._parts,
                         a = r.length,
                         h = this._ctx;
                     if (a) {
-                        for (h.beginPath(), e = 0; e < a; e++) {
-                            for (n = 0, o = r[e].length; n < o; n++) s = r[e][n], h[n ? "lineTo" : "moveTo"](s.x, s.y);
-                            i && h.closePath()
+                        for (h.beginPath(), i = 0; i < a; i++) {
+                            for (n = 0, o = r[i].length; n < o; n++) s = r[i][n], h[n ? "lineTo" : "moveTo"](s.x, s.y);
+                            e && h.closePath()
                         }
                         this._fillStroke(h, t)
                     }
                 }
             },
             _updateCircle: function(t) {
-                var i, e, n, o;
-                this._drawing && !t._empty() && (i = t._point, e = this._ctx, n = Math.max(Math.round(t._radius), 1), 1 != (o = (Math.max(Math.round(t._radiusY), 1) || n) / n) && (e.save(), e.scale(1, o)), e.beginPath(), e.arc(i.x, i.y / o, n, 0, 2 * Math.PI, !1), 1 != o && e.restore(), this._fillStroke(e, t))
+                var e, i, n, o;
+                this._drawing && !t._empty() && (e = t._point, i = this._ctx, n = Math.max(Math.round(t._radius), 1), 1 != (o = (Math.max(Math.round(t._radiusY), 1) || n) / n) && (i.save(), i.scale(1, o)), i.beginPath(), i.arc(e.x, e.y / o, n, 0, 2 * Math.PI, !1), 1 != o && i.restore(), this._fillStroke(i, t))
             },
-            _fillStroke: function(t, i) {
-                var e = i.options;
-                e.fill && (t.globalAlpha = e.fillOpacity, t.fillStyle = e.fillColor || e.color, t.fill(e.fillRule || "evenodd")), e.stroke && 0 !== e.weight && (t.setLineDash && t.setLineDash(i.options && i.options._dashArray || []), t.globalAlpha = e.opacity, t.lineWidth = e.weight, t.strokeStyle = e.color, t.lineCap = e.lineCap, t.lineJoin = e.lineJoin, t.stroke())
+            _fillStroke: function(t, e) {
+                var i = e.options;
+                i.fill && (t.globalAlpha = i.fillOpacity, t.fillStyle = i.fillColor || i.color, t.fill(i.fillRule || "evenodd")), i.stroke && 0 !== i.weight && (t.setLineDash && t.setLineDash(e.options && e.options._dashArray || []), t.globalAlpha = i.opacity, t.lineWidth = i.weight, t.strokeStyle = i.color, t.lineCap = i.lineCap, t.lineJoin = i.lineJoin, t.stroke())
             },
             _onClick: function(t) {
-                for (var i, e, n = this._map.mouseEventToLayerPoint(t), o = this._drawFirst; o; o = o.next)(i = o.layer).options.interactive && i._containsPoint(n) && (("click" === t.type || "preclick" === t.type) && this._map._draggableMoved(i) || (e = i));
-                this._fireEvent(!!e && [e], t)
+                for (var e, i, n = this._map.mouseEventToLayerPoint(t), o = this._drawFirst; o; o = o.next)(e = o.layer).options.interactive && e._containsPoint(n) && (("click" === t.type || "preclick" === t.type) && this._map._draggableMoved(e) || (i = e));
+                this._fireEvent(!!i && [i], t)
             },
             _onMouseMove: function(t) {
-                var i;
-                !this._map || this._map.dragging.moving() || this._map._animatingZoom || (i = this._map.mouseEventToLayerPoint(t), this._handleMouseHover(t, i))
+                var e;
+                !this._map || this._map.dragging.moving() || this._map._animatingZoom || (e = this._map.mouseEventToLayerPoint(t), this._handleMouseHover(t, e))
             },
             _handleMouseOut: function(t) {
-                var i = this._hoveredLayer;
-                i && (M(this._container, "leaflet-interactive"), this._fireEvent([i], t, "mouseout"), this._hoveredLayer = null, this._mouseHoverThrottled = !1)
+                var e = this._hoveredLayer;
+                e && (z(this._container, "leaflet-interactive"), this._fireEvent([e], t, "mouseout"), this._hoveredLayer = null, this._mouseHoverThrottled = !1)
             },
-            _handleMouseHover: function(t, i) {
+            _handleMouseHover: function(t, e) {
                 if (!this._mouseHoverThrottled) {
-                    for (var e, n, o = this._drawFirst; o; o = o.next)(e = o.layer).options.interactive && e._containsPoint(i) && (n = e);
-                    n !== this._hoveredLayer && (this._handleMouseOut(t), n && (z(this._container, "leaflet-interactive"), this._fireEvent([n], t, "mouseover"), this._hoveredLayer = n)), this._fireEvent(!!this._hoveredLayer && [this._hoveredLayer], t), this._mouseHoverThrottled = !0, setTimeout(a(function() {
+                    for (var i, n, o = this._drawFirst; o; o = o.next)(i = o.layer).options.interactive && i._containsPoint(e) && (n = i);
+                    n !== this._hoveredLayer && (this._handleMouseOut(t), n && (M(this._container, "leaflet-interactive"), this._fireEvent([n], t, "mouseover"), this._hoveredLayer = n)), this._fireEvent(!!this._hoveredLayer && [this._hoveredLayer], t), this._mouseHoverThrottled = !0, setTimeout(a(function() {
                         this._mouseHoverThrottled = !1
                     }, this), 32)
                 }
             },
-            _fireEvent: function(t, i, e) {
-                this._map._fireDOMEvent(i, e || i.type, t)
+            _fireEvent: function(t, e, i) {
+                this._map._fireDOMEvent(e, i || e.type, t)
             },
             _bringToFront: function(t) {
-                var i, e, n = t._order;
-                n && (i = n.next, e = n.prev, i && ((i.prev = e) ? e.next = i : i && (this._drawFirst = i), n.prev = this._drawLast, (this._drawLast.next = n).next = null, this._drawLast = n, this._requestRedraw(t)))
+                var e, i, n = t._order;
+                n && (e = n.next, i = n.prev, e && ((e.prev = i) ? i.next = e : e && (this._drawFirst = e), n.prev = this._drawLast, (this._drawLast.next = n).next = null, this._drawLast = n, this._requestRedraw(t)))
             },
             _bringToBack: function(t) {
-                var i, e, n = t._order;
-                n && (i = n.next, (e = n.prev) && ((e.next = i) ? i.prev = e : e && (this._drawLast = e), n.prev = null, n.next = this._drawFirst, this._drawFirst.prev = n, this._drawFirst = n, this._requestRedraw(t)))
+                var e, i, n = t._order;
+                n && (e = n.next, (i = n.prev) && ((i.next = e) ? e.prev = i : i && (this._drawLast = i), n.prev = null, n.next = this._drawFirst, this._drawFirst.prev = n, this._drawFirst = n, this._requestRedraw(t)))
             }
         });
 
-    function je(t) {
-        return P.canvas ? new De(t) : null
+    function an(t) {
+        return b.canvas ? new rn(t) : null
     }
-    var He = function() {
+    var hn = function() {
             try {
                 return document.namespaces.add("lvml", "urn:schemas-microsoft-com:vml"),
                     function(t) {
                         return document.createElement("<lvml:" + t + ' class="lvml">')
                     }
             } catch (t) {}
             return function(t) {
                 return document.createElement("<" + t + ' xmlns="urn:schemas-microsoft.com:vml" class="lvml">')
             }
         }(),
-        Mt = {
+        zt = {
             _initContainer: function() {
-                this._container = b("div", "leaflet-vml-container")
+                this._container = P("div", "leaflet-vml-container")
             },
             _update: function() {
-                this._map._animatingZoom || (Ne.prototype._update.call(this), this.fire("update"))
+                this._map._animatingZoom || (sn.prototype._update.call(this), this.fire("update"))
             },
             _initPath: function(t) {
-                var i = t._container = He("shape");
-                z(i, "leaflet-vml-shape " + (this.options.className || "")), i.coordsize = "1 1", t._path = He("path"), i.appendChild(t._path), this._updateStyle(t), this._layers[h(t)] = t
+                var e = t._container = hn("shape");
+                M(e, "leaflet-vml-shape " + (this.options.className || "")), e.coordsize = "1 1", t._path = hn("path"), e.appendChild(t._path), this._updateStyle(t), this._layers[h(t)] = t
             },
             _addPath: function(t) {
-                var i = t._container;
-                this._container.appendChild(i), t.options.interactive && t.addInteractiveTarget(i)
+                var e = t._container;
+                this._container.appendChild(e), t.options.interactive && t.addInteractiveTarget(e)
             },
             _removePath: function(t) {
-                var i = t._container;
-                T(i), t.removeInteractiveTarget(i), delete this._layers[h(t)]
+                var e = t._container;
+                T(e), t.removeInteractiveTarget(e), delete this._layers[h(t)]
             },
             _updateStyle: function(t) {
-                var i = t._stroke,
-                    e = t._fill,
+                var e = t._stroke,
+                    i = t._fill,
                     n = t.options,
                     o = t._container;
-                o.stroked = !!n.stroke, o.filled = !!n.fill, n.stroke ? (i = i || (t._stroke = He("stroke")), o.appendChild(i), i.weight = n.weight + "px", i.color = n.color, i.opacity = n.opacity, n.dashArray ? i.dashStyle = d(n.dashArray) ? n.dashArray.join(" ") : n.dashArray.replace(/( *, *)/g, " ") : i.dashStyle = "", i.endcap = n.lineCap.replace("butt", "flat"), i.joinstyle = n.lineJoin) : i && (o.removeChild(i), t._stroke = null), n.fill ? (e = e || (t._fill = He("fill")), o.appendChild(e), e.color = n.fillColor || n.color, e.opacity = n.fillOpacity) : e && (o.removeChild(e), t._fill = null)
+                o.stroked = !!n.stroke, o.filled = !!n.fill, n.stroke ? (e = e || (t._stroke = hn("stroke")), o.appendChild(e), e.weight = n.weight + "px", e.color = n.color, e.opacity = n.opacity, n.dashArray ? e.dashStyle = d(n.dashArray) ? n.dashArray.join(" ") : n.dashArray.replace(/( *, *)/g, " ") : e.dashStyle = "", e.endcap = n.lineCap.replace("butt", "flat"), e.joinstyle = n.lineJoin) : e && (o.removeChild(e), t._stroke = null), n.fill ? (i = i || (t._fill = hn("fill")), o.appendChild(i), i.color = n.fillColor || n.color, i.opacity = n.fillOpacity) : i && (o.removeChild(i), t._fill = null)
             },
             _updateCircle: function(t) {
-                var i = t._point.round(),
-                    e = Math.round(t._radius),
-                    n = Math.round(t._radiusY || e);
-                this._setPath(t, t._empty() ? "M0 0" : "AL " + i.x + "," + i.y + " " + e + "," + n + " 0,23592600")
+                var e = t._point.round(),
+                    i = Math.round(t._radius),
+                    n = Math.round(t._radiusY || i);
+                this._setPath(t, t._empty() ? "M0 0" : "AL " + e.x + "," + e.y + " " + i + "," + n + " 0,23592600")
             },
-            _setPath: function(t, i) {
-                t._path.v = i
+            _setPath: function(t, e) {
+                t._path.v = e
             },
             _bringToFront: function(t) {
-                fi(t._container)
+                ge(t._container)
             },
             _bringToBack: function(t) {
-                gi(t._container)
+                ve(t._container)
             }
         },
-        We = P.vml ? He : ct,
-        Fe = Ne.extend({
+        ln = b.vml ? hn : ct,
+        un = sn.extend({
             _initContainer: function() {
-                this._container = We("svg"), this._container.setAttribute("pointer-events", "none"), this._rootGroup = We("g"), this._container.appendChild(this._rootGroup)
+                this._container = ln("svg"), this._container.setAttribute("pointer-events", "none"), this._rootGroup = ln("g"), this._container.appendChild(this._rootGroup)
             },
             _destroyContainer: function() {
                 T(this._container), E(this._container), delete this._container, delete this._rootGroup, delete this._svgSize
             },
             _update: function() {
-                var t, i, e;
-                this._map._animatingZoom && this._bounds || (Ne.prototype._update.call(this), i = (t = this._bounds).getSize(), e = this._container, this._svgSize && this._svgSize.equals(i) || (this._svgSize = i, e.setAttribute("width", i.x), e.setAttribute("height", i.y)), Z(e, t.min), e.setAttribute("viewBox", [t.min.x, t.min.y, i.x, i.y].join(" ")), this.fire("update"))
+                var t, e, i;
+                this._map._animatingZoom && this._bounds || (sn.prototype._update.call(this), e = (t = this._bounds).getSize(), i = this._container, this._svgSize && this._svgSize.equals(e) || (this._svgSize = e, i.setAttribute("width", e.x), i.setAttribute("height", e.y)), Z(i, t.min), i.setAttribute("viewBox", [t.min.x, t.min.y, e.x, e.y].join(" ")), this.fire("update"))
             },
             _initPath: function(t) {
-                var i = t._path = We("path");
-                t.options.className && z(i, t.options.className), t.options.interactive && z(i, "leaflet-interactive"), this._updateStyle(t), this._layers[h(t)] = t
+                var e = t._path = ln("path");
+                t.options.className && M(e, t.options.className), t.options.interactive && M(e, "leaflet-interactive"), this._updateStyle(t), this._layers[h(t)] = t
             },
             _addPath: function(t) {
                 this._rootGroup || this._initContainer(), this._rootGroup.appendChild(t._path), t.addInteractiveTarget(t._path)
             },
             _removePath: function(t) {
                 T(t._path), t.removeInteractiveTarget(t._path), delete this._layers[h(t)]
             },
             _updatePath: function(t) {
                 t._project(), t._update()
             },
             _updateStyle: function(t) {
-                var i = t._path,
+                var e = t._path,
                     t = t.options;
-                i && (t.stroke ? (i.setAttribute("stroke", t.color), i.setAttribute("stroke-opacity", t.opacity), i.setAttribute("stroke-width", t.weight), i.setAttribute("stroke-linecap", t.lineCap), i.setAttribute("stroke-linejoin", t.lineJoin), t.dashArray ? i.setAttribute("stroke-dasharray", t.dashArray) : i.removeAttribute("stroke-dasharray"), t.dashOffset ? i.setAttribute("stroke-dashoffset", t.dashOffset) : i.removeAttribute("stroke-dashoffset")) : i.setAttribute("stroke", "none"), t.fill ? (i.setAttribute("fill", t.fillColor || t.color), i.setAttribute("fill-opacity", t.fillOpacity), i.setAttribute("fill-rule", t.fillRule || "evenodd")) : i.setAttribute("fill", "none"))
+                e && (t.stroke ? (e.setAttribute("stroke", t.color), e.setAttribute("stroke-opacity", t.opacity), e.setAttribute("stroke-width", t.weight), e.setAttribute("stroke-linecap", t.lineCap), e.setAttribute("stroke-linejoin", t.lineJoin), t.dashArray ? e.setAttribute("stroke-dasharray", t.dashArray) : e.removeAttribute("stroke-dasharray"), t.dashOffset ? e.setAttribute("stroke-dashoffset", t.dashOffset) : e.removeAttribute("stroke-dashoffset")) : e.setAttribute("stroke", "none"), t.fill ? (e.setAttribute("fill", t.fillColor || t.color), e.setAttribute("fill-opacity", t.fillOpacity), e.setAttribute("fill-rule", t.fillRule || "evenodd")) : e.setAttribute("fill", "none"))
             },
-            _updatePoly: function(t, i) {
-                this._setPath(t, dt(t._parts, i))
+            _updatePoly: function(t, e) {
+                this._setPath(t, dt(t._parts, e))
             },
             _updateCircle: function(t) {
-                var i = t._point,
-                    e = Math.max(Math.round(t._radius), 1),
-                    n = "a" + e + "," + (Math.max(Math.round(t._radiusY), 1) || e) + " 0 1,0 ",
-                    i = t._empty() ? "M0 0" : "M" + (i.x - e) + "," + i.y + n + 2 * e + ",0 " + n + 2 * -e + ",0 ";
-                this._setPath(t, i)
+                var e = t._point,
+                    i = Math.max(Math.round(t._radius), 1),
+                    n = "a" + i + "," + (Math.max(Math.round(t._radiusY), 1) || i) + " 0 1,0 ",
+                    e = t._empty() ? "M0 0" : "M" + (e.x - i) + "," + e.y + n + 2 * i + ",0 " + n + 2 * -i + ",0 ";
+                this._setPath(t, e)
             },
-            _setPath: function(t, i) {
-                t._path.setAttribute("d", i)
+            _setPath: function(t, e) {
+                t._path.setAttribute("d", e)
             },
             _bringToFront: function(t) {
-                fi(t._path)
+                ge(t._path)
             },
             _bringToBack: function(t) {
-                gi(t._path)
+                ve(t._path)
             }
         });
 
-    function Ue(t) {
-        return P.svg || P.vml ? new Fe(t) : null
+    function cn(t) {
+        return b.svg || b.vml ? new un(t) : null
     }
-    P.vml && Fe.include(Mt), A.include({
+    b.vml && un.include(zt), O.include({
         getRenderer: function(t) {
             t = (t = t.options.renderer || this._getPaneRenderer(t.options.pane) || this.options.renderer || this._renderer) || (this._renderer = this._createRenderer());
             return this.hasLayer(t) || this.addLayer(t), t
         },
         _getPaneRenderer: function(t) {
-            if ("overlayPane" === t || void 0 === t) return !1;
-            var i = this._paneRenderers[t];
-            return void 0 === i && (i = this._createRenderer({
+            var e;
+            return "overlayPane" !== t && void 0 !== t && (void 0 === (e = this._paneRenderers[t]) && (e = this._createRenderer({
                 pane: t
-            }), this._paneRenderers[t] = i), i
+            }), this._paneRenderers[t] = e), e)
         },
         _createRenderer: function(t) {
-            return this.options.preferCanvas && je(t) || Ue(t)
+            return this.options.preferCanvas && an(t) || cn(t)
         }
     });
-    var Ve = ge.extend({
-        initialize: function(t, i) {
-            ge.prototype.initialize.call(this, this._boundsToLatLngs(t), i)
+    var dn = Zi.extend({
+        initialize: function(t, e) {
+            Zi.prototype.initialize.call(this, this._boundsToLatLngs(t), e)
         },
         setBounds: function(t) {
             return this.setLatLngs(this._boundsToLatLngs(t))
         },
         _boundsToLatLngs: function(t) {
             return [(t = g(t)).getSouthWest(), t.getNorthWest(), t.getNorthEast(), t.getSouthEast()]
         }
     });
-    Fe.create = We, Fe.pointsToPath = dt, ve.geometryToLayer = ye, ve.coordsToLatLng = we, ve.coordsToLatLngs = Pe, ve.latLngToCoords = be, ve.latLngsToCoords = Le, ve.getFeature = Te, ve.asFeature = ze, A.mergeOptions({
+
+    function _n(t, e) {
+        return new dn(t, e)
+    }
+    un.create = ln, un.pointsToPath = dt, Ei.geometryToLayer = ki, Ei.coordsToLatLng = Bi, Ei.coordsToLatLngs = Ai, Ei.latLngToCoords = Ii, Ei.latLngsToCoords = Ri, Ei.getFeature = Ni, Ei.asFeature = Di, O.mergeOptions({
         boxZoom: !0
     });
-    var _t = n.extend({
-            initialize: function(t) {
-                this._map = t, this._container = t._container, this._pane = t._panes.overlayPane, this._resetStateTimeout = 0, t.on("unload", this._destroy, this)
-            },
-            addHooks: function() {
-                S(this._container, "mousedown", this._onMouseDown, this)
-            },
-            removeHooks: function() {
-                E(this._container, "mousedown", this._onMouseDown, this)
-            },
-            moved: function() {
-                return this._moved
-            },
-            _destroy: function() {
-                T(this._pane), delete this._pane
-            },
-            _resetState: function() {
-                this._resetStateTimeout = 0, this._moved = !1
-            },
-            _clearDeferredResetState: function() {
-                0 !== this._resetStateTimeout && (clearTimeout(this._resetStateTimeout), this._resetStateTimeout = 0)
-            },
-            _onMouseDown: function(t) {
-                if (!t.shiftKey || 1 !== t.which && 1 !== t.button) return !1;
-                this._clearDeferredResetState(), this._resetState(), ri(), Li(), this._startPoint = this._map.mouseEventToContainerPoint(t), S(document, {
-                    contextmenu: Ri,
-                    mousemove: this._onMouseMove,
-                    mouseup: this._onMouseUp,
-                    keydown: this._onKeyDown
-                }, this)
-            },
-            _onMouseMove: function(t) {
-                this._moved || (this._moved = !0, this._box = b("div", "leaflet-zoom-box", this._container), z(this._container, "leaflet-crosshair"), this._map.fire("boxzoomstart")), this._point = this._map.mouseEventToContainerPoint(t);
-                var t = new m(this._point, this._startPoint),
-                    i = t.getSize();
-                Z(this._box, t.min), this._box.style.width = i.x + "px", this._box.style.height = i.y + "px"
-            },
-            _finish: function() {
-                this._moved && (T(this._box), M(this._container, "leaflet-crosshair")), ai(), Ti(), E(document, {
-                    contextmenu: Ri,
-                    mousemove: this._onMouseMove,
-                    mouseup: this._onMouseUp,
-                    keydown: this._onKeyDown
-                }, this)
-            },
-            _onMouseUp: function(t) {
-                1 !== t.which && 1 !== t.button || (this._finish(), this._moved && (this._clearDeferredResetState(), this._resetStateTimeout = setTimeout(a(this._resetState, this), 0), t = new s(this._map.containerPointToLatLng(this._startPoint), this._map.containerPointToLatLng(this._point)), this._map.fitBounds(t).fire("boxzoomend", {
-                    boxZoomBounds: t
-                })))
-            },
-            _onKeyDown: function(t) {
-                27 === t.keyCode && (this._finish(), this._clearDeferredResetState(), this._resetState())
-            }
-        }),
-        Ct = (A.addInitHook("addHandler", "boxZoom", _t), A.mergeOptions({
-            doubleClickZoom: !0
-        }), n.extend({
-            addHooks: function() {
-                this._map.on("dblclick", this._onDoubleClick, this)
-            },
-            removeHooks: function() {
-                this._map.off("dblclick", this._onDoubleClick, this)
-            },
-            _onDoubleClick: function(t) {
-                var i = this._map,
-                    e = i.getZoom(),
-                    n = i.options.zoomDelta,
-                    e = t.originalEvent.shiftKey ? e - n : e + n;
-                "center" === i.options.doubleClickZoom ? i.setZoom(e) : i.setZoomAround(t.containerPoint, e)
-            }
-        })),
-        Zt = (A.addInitHook("addHandler", "doubleClickZoom", Ct), A.mergeOptions({
-            dragging: !0,
-            inertia: !0,
-            inertiaDeceleration: 3400,
-            inertiaMaxSpeed: 1 / 0,
-            easeLinearity: .2,
-            worldCopyJump: !1,
-            maxBoundsViscosity: 0
-        }), n.extend({
-            addHooks: function() {
-                var t;
-                this._draggable || (t = this._map, this._draggable = new Xi(t._mapPane, t._container), this._draggable.on({
-                    dragstart: this._onDragStart,
-                    drag: this._onDrag,
-                    dragend: this._onDragEnd
-                }, this), this._draggable.on("predrag", this._onPreDragLimit, this), t.options.worldCopyJump && (this._draggable.on("predrag", this._onPreDragWrap, this), t.on("zoomend", this._onZoomEnd, this), t.whenReady(this._onZoomEnd, this))), z(this._map._container, "leaflet-grab leaflet-touch-drag"), this._draggable.enable(), this._positions = [], this._times = []
-            },
-            removeHooks: function() {
-                M(this._map._container, "leaflet-grab"), M(this._map._container, "leaflet-touch-drag"), this._draggable.disable()
-            },
-            moved: function() {
-                return this._draggable && this._draggable._moved
-            },
-            moving: function() {
-                return this._draggable && this._draggable._moving
-            },
-            _onDragStart: function() {
-                var t, i = this._map;
-                i._stop(), this._map.options.maxBounds && this._map.options.maxBoundsViscosity ? (t = g(this._map.options.maxBounds), this._offsetLimit = f(this._map.latLngToContainerPoint(t.getNorthWest()).multiplyBy(-1), this._map.latLngToContainerPoint(t.getSouthEast()).multiplyBy(-1).add(this._map.getSize())), this._viscosity = Math.min(1, Math.max(0, this._map.options.maxBoundsViscosity))) : this._offsetLimit = null, i.fire("movestart").fire("dragstart"), i.options.inertia && (this._positions = [], this._times = [])
-            },
-            _onDrag: function(t) {
-                var i, e;
-                this._map.options.inertia && (i = this._lastTime = +new Date, e = this._lastPos = this._draggable._absPos || this._draggable._newPos, this._positions.push(e), this._times.push(i), this._prunePositions(i)), this._map.fire("move", t).fire("drag", t)
-            },
-            _prunePositions: function(t) {
-                for (; 1 < this._positions.length && 50 < t - this._times[0];) this._positions.shift(), this._times.shift()
-            },
-            _onZoomEnd: function() {
-                var t = this._map.getSize().divideBy(2),
-                    i = this._map.latLngToLayerPoint([0, 0]);
-                this._initialWorldOffset = i.subtract(t).x, this._worldWidth = this._map.getPixelWorldBounds().getSize().x
-            },
-            _viscousLimit: function(t, i) {
-                return t - (t - i) * this._viscosity
-            },
-            _onPreDragLimit: function() {
-                var t, i;
-                this._viscosity && this._offsetLimit && (t = this._draggable._newPos.subtract(this._draggable._startPos), i = this._offsetLimit, t.x < i.min.x && (t.x = this._viscousLimit(t.x, i.min.x)), t.y < i.min.y && (t.y = this._viscousLimit(t.y, i.min.y)), t.x > i.max.x && (t.x = this._viscousLimit(t.x, i.max.x)), t.y > i.max.y && (t.y = this._viscousLimit(t.y, i.max.y)), this._draggable._newPos = this._draggable._startPos.add(t))
-            },
-            _onPreDragWrap: function() {
-                var t = this._worldWidth,
-                    i = Math.round(t / 2),
-                    e = this._initialWorldOffset,
-                    n = this._draggable._newPos.x,
-                    o = (n - i + e) % t + i - e,
-                    n = (n + i + e) % t - i - e,
-                    t = Math.abs(o + e) < Math.abs(n + e) ? o : n;
-                this._draggable._absPos = this._draggable._newPos.clone(), this._draggable._newPos.x = t
-            },
-            _onDragEnd: function(t) {
-                var i, e, n, o, s = this._map,
-                    r = s.options,
-                    a = !r.inertia || t.noInertia || this._times.length < 2;
-                s.fire("dragend", t), a ? s.fire("moveend") : (this._prunePositions(+new Date), t = this._lastPos.subtract(this._positions[0]), a = (this._lastTime - this._times[0]) / 1e3, i = r.easeLinearity, a = (t = t.multiplyBy(i / a)).distanceTo([0, 0]), e = Math.min(r.inertiaMaxSpeed, a), t = t.multiplyBy(e / a), n = e / (r.inertiaDeceleration * i), (o = t.multiplyBy(-n / 2).round()).x || o.y ? (o = s._limitOffset(o, s.options.maxBounds), x(function() {
-                    s.panBy(o, {
-                        duration: n,
-                        easeLinearity: i,
-                        noMoveStart: !0,
-                        animate: !0
-                    })
-                })) : s.fire("moveend"))
-            }
-        })),
-        St = (A.addInitHook("addHandler", "dragging", Zt), A.mergeOptions({
-            keyboard: !0,
-            keyboardPanDelta: 80
-        }), n.extend({
-            keyCodes: {
-                left: [37],
-                right: [39],
-                down: [40],
-                up: [38],
-                zoomIn: [187, 107, 61, 171],
-                zoomOut: [189, 109, 54, 173]
-            },
-            initialize: function(t) {
-                this._map = t, this._setPanDelta(t.options.keyboardPanDelta), this._setZoomDelta(t.options.zoomDelta)
-            },
-            addHooks: function() {
-                var t = this._map._container;
-                t.tabIndex <= 0 && (t.tabIndex = "0"), S(t, {
-                    focus: this._onFocus,
-                    blur: this._onBlur,
-                    mousedown: this._onMouseDown
-                }, this), this._map.on({
-                    focus: this._addHooks,
-                    blur: this._removeHooks
-                }, this)
-            },
-            removeHooks: function() {
-                this._removeHooks(), E(this._map._container, {
-                    focus: this._onFocus,
-                    blur: this._onBlur,
-                    mousedown: this._onMouseDown
-                }, this), this._map.off({
-                    focus: this._addHooks,
-                    blur: this._removeHooks
-                }, this)
-            },
-            _onMouseDown: function() {
-                var t, i, e;
-                this._focused || (e = document.body, t = document.documentElement, i = e.scrollTop || t.scrollTop, e = e.scrollLeft || t.scrollLeft, this._map._container.focus(), window.scrollTo(e, i))
-            },
-            _onFocus: function() {
-                this._focused = !0, this._map.fire("focus")
-            },
-            _onBlur: function() {
-                this._focused = !1, this._map.fire("blur")
-            },
-            _setPanDelta: function(t) {
-                for (var i = this._panKeys = {}, e = this.keyCodes, n = 0, o = e.left.length; n < o; n++) i[e.left[n]] = [-1 * t, 0];
-                for (n = 0, o = e.right.length; n < o; n++) i[e.right[n]] = [t, 0];
-                for (n = 0, o = e.down.length; n < o; n++) i[e.down[n]] = [0, t];
-                for (n = 0, o = e.up.length; n < o; n++) i[e.up[n]] = [0, -1 * t]
-            },
-            _setZoomDelta: function(t) {
-                for (var i = this._zoomKeys = {}, e = this.keyCodes, n = 0, o = e.zoomIn.length; n < o; n++) i[e.zoomIn[n]] = t;
-                for (n = 0, o = e.zoomOut.length; n < o; n++) i[e.zoomOut[n]] = -t
-            },
-            _addHooks: function() {
-                S(document, "keydown", this._onKeyDown, this)
-            },
-            _removeHooks: function() {
-                E(document, "keydown", this._onKeyDown, this)
-            },
-            _onKeyDown: function(t) {
-                if (!(t.altKey || t.ctrlKey || t.metaKey)) {
-                    var i, e = t.keyCode,
-                        n = this._map;
-                    if (e in this._panKeys) n._panAnim && n._panAnim._inProgress || (i = this._panKeys[e], t.shiftKey && (i = _(i).multiplyBy(3)), n.panBy(i), n.options.maxBounds && n.panInsideBounds(n.options.maxBounds));
-                    else if (e in this._zoomKeys) n.setZoom(n.getZoom() + (t.shiftKey ? 3 : 1) * this._zoomKeys[e]);
-                    else {
-                        if (27 !== e || !n._popup || !n._popup.options.closeOnEscapeKey) return;
-                        n.closePopup()
-                    }
-                    Ri(t)
+    _t = o.extend({
+        initialize: function(t) {
+            this._map = t, this._container = t._container, this._pane = t._panes.overlayPane, this._resetStateTimeout = 0, t.on("unload", this._destroy, this)
+        },
+        addHooks: function() {
+            S(this._container, "mousedown", this._onMouseDown, this)
+        },
+        removeHooks: function() {
+            E(this._container, "mousedown", this._onMouseDown, this)
+        },
+        moved: function() {
+            return this._moved
+        },
+        _destroy: function() {
+            T(this._pane), delete this._pane
+        },
+        _resetState: function() {
+            this._resetStateTimeout = 0, this._moved = !1
+        },
+        _clearDeferredResetState: function() {
+            0 !== this._resetStateTimeout && (clearTimeout(this._resetStateTimeout), this._resetStateTimeout = 0)
+        },
+        _onMouseDown: function(t) {
+            if (!t.shiftKey || 1 !== t.which && 1 !== t.button) return !1;
+            this._clearDeferredResetState(), this._resetState(), ae(), Te(), this._startPoint = this._map.mouseEventToContainerPoint(t), S(document, {
+                contextmenu: De,
+                mousemove: this._onMouseMove,
+                mouseup: this._onMouseUp,
+                keydown: this._onKeyDown
+            }, this)
+        },
+        _onMouseMove: function(t) {
+            this._moved || (this._moved = !0, this._box = P("div", "leaflet-zoom-box", this._container), M(this._container, "leaflet-crosshair"), this._map.fire("boxzoomstart")), this._point = this._map.mouseEventToContainerPoint(t);
+            var t = new f(this._point, this._startPoint),
+                e = t.getSize();
+            Z(this._box, t.min), this._box.style.width = e.x + "px", this._box.style.height = e.y + "px"
+        },
+        _finish: function() {
+            this._moved && (T(this._box), z(this._container, "leaflet-crosshair")), he(), Me(), E(document, {
+                contextmenu: De,
+                mousemove: this._onMouseMove,
+                mouseup: this._onMouseUp,
+                keydown: this._onKeyDown
+            }, this)
+        },
+        _onMouseUp: function(t) {
+            1 !== t.which && 1 !== t.button || (this._finish(), this._moved && (this._clearDeferredResetState(), this._resetStateTimeout = setTimeout(a(this._resetState, this), 0), t = new s(this._map.containerPointToLatLng(this._startPoint), this._map.containerPointToLatLng(this._point)), this._map.fitBounds(t).fire("boxzoomend", {
+                boxZoomBounds: t
+            })))
+        },
+        _onKeyDown: function(t) {
+            27 === t.keyCode && (this._finish(), this._clearDeferredResetState(), this._resetState())
+        }
+    }), O.addInitHook("addHandler", "boxZoom", _t), O.mergeOptions({
+        doubleClickZoom: !0
+    }), Ct = o.extend({
+        addHooks: function() {
+            this._map.on("dblclick", this._onDoubleClick, this)
+        },
+        removeHooks: function() {
+            this._map.off("dblclick", this._onDoubleClick, this)
+        },
+        _onDoubleClick: function(t) {
+            var e = this._map,
+                i = e.getZoom(),
+                n = e.options.zoomDelta,
+                i = t.originalEvent.shiftKey ? i - n : i + n;
+            "center" === e.options.doubleClickZoom ? e.setZoom(i) : e.setZoomAround(t.containerPoint, i)
+        }
+    }), O.addInitHook("addHandler", "doubleClickZoom", Ct), O.mergeOptions({
+        dragging: !0,
+        inertia: !0,
+        inertiaDeceleration: 3400,
+        inertiaMaxSpeed: 1 / 0,
+        easeLinearity: .2,
+        worldCopyJump: !1,
+        maxBoundsViscosity: 0
+    }), Zt = o.extend({
+        addHooks: function() {
+            var t;
+            this._draggable || (t = this._map, this._draggable = new ti(t._mapPane, t._container), this._draggable.on({
+                dragstart: this._onDragStart,
+                drag: this._onDrag,
+                dragend: this._onDragEnd
+            }, this), this._draggable.on("predrag", this._onPreDragLimit, this), t.options.worldCopyJump && (this._draggable.on("predrag", this._onPreDragWrap, this), t.on("zoomend", this._onZoomEnd, this), t.whenReady(this._onZoomEnd, this))), M(this._map._container, "leaflet-grab leaflet-touch-drag"), this._draggable.enable(), this._positions = [], this._times = []
+        },
+        removeHooks: function() {
+            z(this._map._container, "leaflet-grab"), z(this._map._container, "leaflet-touch-drag"), this._draggable.disable()
+        },
+        moved: function() {
+            return this._draggable && this._draggable._moved
+        },
+        moving: function() {
+            return this._draggable && this._draggable._moving
+        },
+        _onDragStart: function() {
+            var t, e = this._map;
+            e._stop(), this._map.options.maxBounds && this._map.options.maxBoundsViscosity ? (t = g(this._map.options.maxBounds), this._offsetLimit = _(this._map.latLngToContainerPoint(t.getNorthWest()).multiplyBy(-1), this._map.latLngToContainerPoint(t.getSouthEast()).multiplyBy(-1).add(this._map.getSize())), this._viscosity = Math.min(1, Math.max(0, this._map.options.maxBoundsViscosity))) : this._offsetLimit = null, e.fire("movestart").fire("dragstart"), e.options.inertia && (this._positions = [], this._times = [])
+        },
+        _onDrag: function(t) {
+            var e, i;
+            this._map.options.inertia && (e = this._lastTime = +new Date, i = this._lastPos = this._draggable._absPos || this._draggable._newPos, this._positions.push(i), this._times.push(e), this._prunePositions(e)), this._map.fire("move", t).fire("drag", t)
+        },
+        _prunePositions: function(t) {
+            for (; 1 < this._positions.length && 50 < t - this._times[0];) this._positions.shift(), this._times.shift()
+        },
+        _onZoomEnd: function() {
+            var t = this._map.getSize().divideBy(2),
+                e = this._map.latLngToLayerPoint([0, 0]);
+            this._initialWorldOffset = e.subtract(t).x, this._worldWidth = this._map.getPixelWorldBounds().getSize().x
+        },
+        _viscousLimit: function(t, e) {
+            return t - (t - e) * this._viscosity
+        },
+        _onPreDragLimit: function() {
+            var t, e;
+            this._viscosity && this._offsetLimit && (t = this._draggable._newPos.subtract(this._draggable._startPos), e = this._offsetLimit, t.x < e.min.x && (t.x = this._viscousLimit(t.x, e.min.x)), t.y < e.min.y && (t.y = this._viscousLimit(t.y, e.min.y)), t.x > e.max.x && (t.x = this._viscousLimit(t.x, e.max.x)), t.y > e.max.y && (t.y = this._viscousLimit(t.y, e.max.y)), this._draggable._newPos = this._draggable._startPos.add(t))
+        },
+        _onPreDragWrap: function() {
+            var t = this._worldWidth,
+                e = Math.round(t / 2),
+                i = this._initialWorldOffset,
+                n = this._draggable._newPos.x,
+                o = (n - e + i) % t + e - i,
+                n = (n + e + i) % t - e - i,
+                t = Math.abs(o + i) < Math.abs(n + i) ? o : n;
+            this._draggable._absPos = this._draggable._newPos.clone(), this._draggable._newPos.x = t
+        },
+        _onDragEnd: function(t) {
+            var e, i, n, o, s = this._map,
+                r = s.options,
+                a = !r.inertia || t.noInertia || this._times.length < 2;
+            s.fire("dragend", t), !a && (this._prunePositions(+new Date), t = this._lastPos.subtract(this._positions[0]), a = (this._lastTime - this._times[0]) / 1e3, e = r.easeLinearity, a = (t = t.multiplyBy(e / a)).distanceTo([0, 0]), i = Math.min(r.inertiaMaxSpeed, a), t = t.multiplyBy(i / a), n = i / (r.inertiaDeceleration * e), (o = t.multiplyBy(-n / 2).round()).x || o.y) ? (o = s._limitOffset(o, s.options.maxBounds), x(function() {
+                s.panBy(o, {
+                    duration: n,
+                    easeLinearity: e,
+                    noMoveStart: !0,
+                    animate: !0
+                })
+            })) : s.fire("moveend")
+        }
+    }), O.addInitHook("addHandler", "dragging", Zt), O.mergeOptions({
+        keyboard: !0,
+        keyboardPanDelta: 80
+    }), St = o.extend({
+        keyCodes: {
+            left: [37],
+            right: [39],
+            down: [40],
+            up: [38],
+            zoomIn: [187, 107, 61, 171],
+            zoomOut: [189, 109, 54, 173]
+        },
+        initialize: function(t) {
+            this._map = t, this._setPanDelta(t.options.keyboardPanDelta), this._setZoomDelta(t.options.zoomDelta)
+        },
+        addHooks: function() {
+            var t = this._map._container;
+            t.tabIndex <= 0 && (t.tabIndex = "0"), S(t, {
+                focus: this._onFocus,
+                blur: this._onBlur,
+                mousedown: this._onMouseDown
+            }, this), this._map.on({
+                focus: this._addHooks,
+                blur: this._removeHooks
+            }, this)
+        },
+        removeHooks: function() {
+            this._removeHooks(), E(this._map._container, {
+                focus: this._onFocus,
+                blur: this._onBlur,
+                mousedown: this._onMouseDown
+            }, this), this._map.off({
+                focus: this._addHooks,
+                blur: this._removeHooks
+            }, this)
+        },
+        _onMouseDown: function() {
+            var t, e, i;
+            this._focused || (i = document.body, t = document.documentElement, e = i.scrollTop || t.scrollTop, i = i.scrollLeft || t.scrollLeft, this._map._container.focus(), window.scrollTo(i, e))
+        },
+        _onFocus: function() {
+            this._focused = !0, this._map.fire("focus")
+        },
+        _onBlur: function() {
+            this._focused = !1, this._map.fire("blur")
+        },
+        _setPanDelta: function(t) {
+            for (var e = this._panKeys = {}, i = this.keyCodes, n = 0, o = i.left.length; n < o; n++) e[i.left[n]] = [-1 * t, 0];
+            for (n = 0, o = i.right.length; n < o; n++) e[i.right[n]] = [t, 0];
+            for (n = 0, o = i.down.length; n < o; n++) e[i.down[n]] = [0, t];
+            for (n = 0, o = i.up.length; n < o; n++) e[i.up[n]] = [0, -1 * t]
+        },
+        _setZoomDelta: function(t) {
+            for (var e = this._zoomKeys = {}, i = this.keyCodes, n = 0, o = i.zoomIn.length; n < o; n++) e[i.zoomIn[n]] = t;
+            for (n = 0, o = i.zoomOut.length; n < o; n++) e[i.zoomOut[n]] = -t
+        },
+        _addHooks: function() {
+            S(document, "keydown", this._onKeyDown, this)
+        },
+        _removeHooks: function() {
+            E(document, "keydown", this._onKeyDown, this)
+        },
+        _onKeyDown: function(t) {
+            if (!(t.altKey || t.ctrlKey || t.metaKey)) {
+                var e, i = t.keyCode,
+                    n = this._map;
+                if (i in this._panKeys) n._panAnim && n._panAnim._inProgress || (e = this._panKeys[i], t.shiftKey && (e = m(e).multiplyBy(3)), n.panBy(e), n.options.maxBounds && n.panInsideBounds(n.options.maxBounds));
+                else if (i in this._zoomKeys) n.setZoom(n.getZoom() + (t.shiftKey ? 3 : 1) * this._zoomKeys[i]);
+                else {
+                    if (27 !== i || !n._popup || !n._popup.options.closeOnEscapeKey) return;
+                    n.closePopup()
                 }
+                De(t)
             }
-        })),
-        kt = (A.addInitHook("addHandler", "keyboard", St), A.mergeOptions({
-            scrollWheelZoom: !0,
-            wheelDebounceTime: 40,
-            wheelPxPerZoomLevel: 60
-        }), n.extend({
-            addHooks: function() {
-                S(this._map._container, "wheel", this._onWheelScroll, this), this._delta = 0
-            },
-            removeHooks: function() {
-                E(this._map._container, "wheel", this._onWheelScroll, this)
-            },
-            _onWheelScroll: function(t) {
-                var i = ji(t),
-                    e = this._map.options.wheelDebounceTime,
-                    i = (this._delta += i, this._lastMousePos = this._map.mouseEventToContainerPoint(t), this._startTime || (this._startTime = +new Date), Math.max(e - (+new Date - this._startTime), 0));
-                clearTimeout(this._timer), this._timer = setTimeout(a(this._performZoom, this), i), Ri(t)
-            },
-            _performZoom: function() {
-                var t = this._map,
-                    i = t.getZoom(),
-                    e = this._map.options.zoomSnap || 0,
-                    n = (t._stop(), this._delta / (4 * this._map.options.wheelPxPerZoomLevel)),
-                    n = 4 * Math.log(2 / (1 + Math.exp(-Math.abs(n)))) / Math.LN2,
-                    e = e ? Math.ceil(n / e) * e : n,
-                    n = t._limitZoom(i + (0 < this._delta ? e : -e)) - i;
-                this._delta = 0, this._startTime = null, n && ("center" === t.options.scrollWheelZoom ? t.setZoom(i + n) : t.setZoomAround(this._lastMousePos, i + n))
-            }
-        })),
-        Et = (A.addInitHook("addHandler", "scrollWheelZoom", kt), A.mergeOptions({
-            tapHold: P.touchNative && P.safari && P.mobile,
-            tapTolerance: 15
-        }), n.extend({
-            addHooks: function() {
-                S(this._map._container, "touchstart", this._onDown, this)
-            },
-            removeHooks: function() {
-                E(this._map._container, "touchstart", this._onDown, this)
-            },
-            _onDown: function(t) {
-                var i;
-                clearTimeout(this._holdTimeout), 1 === t.touches.length && (i = t.touches[0], this._startPos = this._newPos = new p(i.clientX, i.clientY), this._holdTimeout = setTimeout(a(function() {
-                    this._cancel(), this._isTapValid() && (S(document, "touchend", B), S(document, "touchend touchcancel", this._cancelClickPrevent), this._simulateEvent("contextmenu", i))
-                }, this), 600), S(document, "touchend touchcancel contextmenu", this._cancel, this), S(document, "touchmove", this._onMove, this))
-            },
-            _cancelClickPrevent: function t() {
-                E(document, "touchend", B), E(document, "touchend touchcancel", t)
-            },
-            _cancel: function() {
-                clearTimeout(this._holdTimeout), E(document, "touchend touchcancel contextmenu", this._cancel, this), E(document, "touchmove", this._onMove, this)
-            },
-            _onMove: function(t) {
-                t = t.touches[0];
-                this._newPos = new p(t.clientX, t.clientY)
-            },
-            _isTapValid: function() {
-                return this._newPos.distanceTo(this._startPos) <= this._map.options.tapTolerance
-            },
-            _simulateEvent: function(t, i) {
-                t = new MouseEvent(t, {
-                    bubbles: !0,
-                    cancelable: !0,
-                    view: window,
-                    screenX: i.screenX,
-                    screenY: i.screenY,
-                    clientX: i.clientX,
-                    clientY: i.clientY
-                });
-                t._simulated = !0, i.target.dispatchEvent(t)
-            }
-        })),
-        Bt = (A.addInitHook("addHandler", "tapHold", Et), A.mergeOptions({
-            touchZoom: P.touch,
-            bounceAtZoomLimits: !0
-        }), n.extend({
-            addHooks: function() {
-                z(this._map._container, "leaflet-touch-zoom"), S(this._map._container, "touchstart", this._onTouchStart, this)
-            },
-            removeHooks: function() {
-                M(this._map._container, "leaflet-touch-zoom"), E(this._map._container, "touchstart", this._onTouchStart, this)
-            },
-            _onTouchStart: function(t) {
-                var i, e, n = this._map;
-                !t.touches || 2 !== t.touches.length || n._animatingZoom || this._zooming || (i = n.mouseEventToContainerPoint(t.touches[0]), e = n.mouseEventToContainerPoint(t.touches[1]), this._centerPoint = n.getSize()._divideBy(2), this._startLatLng = n.containerPointToLatLng(this._centerPoint), "center" !== n.options.touchZoom && (this._pinchStartLatLng = n.containerPointToLatLng(i.add(e)._divideBy(2))), this._startDist = i.distanceTo(e), this._startZoom = n.getZoom(), this._moved = !1, this._zooming = !0, n._stop(), S(document, "touchmove", this._onTouchMove, this), S(document, "touchend touchcancel", this._onTouchEnd, this), B(t))
-            },
-            _onTouchMove: function(t) {
-                if (t.touches && 2 === t.touches.length && this._zooming) {
-                    var i = this._map,
-                        e = i.mouseEventToContainerPoint(t.touches[0]),
-                        n = i.mouseEventToContainerPoint(t.touches[1]),
-                        o = e.distanceTo(n) / this._startDist;
-                    if (this._zoom = i.getScaleZoom(o, this._startZoom), !i.options.bounceAtZoomLimits && (this._zoom < i.getMinZoom() && o < 1 || this._zoom > i.getMaxZoom() && 1 < o) && (this._zoom = i._limitZoom(this._zoom)), "center" === i.options.touchZoom) {
-                        if (this._center = this._startLatLng, 1 == o) return
-                    } else {
-                        e = e._add(n)._divideBy(2)._subtract(this._centerPoint);
-                        if (1 == o && 0 === e.x && 0 === e.y) return;
-                        this._center = i.unproject(i.project(this._pinchStartLatLng, this._zoom).subtract(e), this._zoom)
-                    }
-                    this._moved || (i._moveStart(!0, !1), this._moved = !0), r(this._animRequest);
-                    n = a(i._move, i, this._center, this._zoom, {
-                        pinch: !0,
-                        round: !1
-                    });
-                    this._animRequest = x(n, this, !0), B(t)
+        }
+    }), O.addInitHook("addHandler", "keyboard", St), O.mergeOptions({
+        scrollWheelZoom: !0,
+        wheelDebounceTime: 40,
+        wheelPxPerZoomLevel: 60
+    }), Et = o.extend({
+        addHooks: function() {
+            S(this._map._container, "wheel", this._onWheelScroll, this), this._delta = 0
+        },
+        removeHooks: function() {
+            E(this._map._container, "wheel", this._onWheelScroll, this)
+        },
+        _onWheelScroll: function(t) {
+            var e = We(t),
+                i = this._map.options.wheelDebounceTime,
+                e = (this._delta += e, this._lastMousePos = this._map.mouseEventToContainerPoint(t), this._startTime || (this._startTime = +new Date), Math.max(i - (+new Date - this._startTime), 0));
+            clearTimeout(this._timer), this._timer = setTimeout(a(this._performZoom, this), e), De(t)
+        },
+        _performZoom: function() {
+            var t = this._map,
+                e = t.getZoom(),
+                i = this._map.options.zoomSnap || 0,
+                n = (t._stop(), this._delta / (4 * this._map.options.wheelPxPerZoomLevel)),
+                n = 4 * Math.log(2 / (1 + Math.exp(-Math.abs(n)))) / Math.LN2,
+                i = i ? Math.ceil(n / i) * i : n,
+                n = t._limitZoom(e + (0 < this._delta ? i : -i)) - e;
+            this._delta = 0, this._startTime = null, n && ("center" === t.options.scrollWheelZoom ? t.setZoom(e + n) : t.setZoomAround(this._lastMousePos, e + n))
+        }
+    }), O.addInitHook("addHandler", "scrollWheelZoom", Et), O.mergeOptions({
+        tapHold: b.touchNative && b.safari && b.mobile,
+        tapTolerance: 15
+    }), kt = o.extend({
+        addHooks: function() {
+            S(this._map._container, "touchstart", this._onDown, this)
+        },
+        removeHooks: function() {
+            E(this._map._container, "touchstart", this._onDown, this)
+        },
+        _onDown: function(t) {
+            var e;
+            clearTimeout(this._holdTimeout), 1 === t.touches.length && (e = t.touches[0], this._startPos = this._newPos = new p(e.clientX, e.clientY), this._holdTimeout = setTimeout(a(function() {
+                this._cancel(), this._isTapValid() && (S(document, "touchend", k), S(document, "touchend touchcancel", this._cancelClickPrevent), this._simulateEvent("contextmenu", e))
+            }, this), 600), S(document, "touchend touchcancel contextmenu", this._cancel, this), S(document, "touchmove", this._onMove, this))
+        },
+        _cancelClickPrevent: function t() {
+            E(document, "touchend", k), E(document, "touchend touchcancel", t)
+        },
+        _cancel: function() {
+            clearTimeout(this._holdTimeout), E(document, "touchend touchcancel contextmenu", this._cancel, this), E(document, "touchmove", this._onMove, this)
+        },
+        _onMove: function(t) {
+            t = t.touches[0];
+            this._newPos = new p(t.clientX, t.clientY)
+        },
+        _isTapValid: function() {
+            return this._newPos.distanceTo(this._startPos) <= this._map.options.tapTolerance
+        },
+        _simulateEvent: function(t, e) {
+            t = new MouseEvent(t, {
+                bubbles: !0,
+                cancelable: !0,
+                view: window,
+                screenX: e.screenX,
+                screenY: e.screenY,
+                clientX: e.clientX,
+                clientY: e.clientY
+            });
+            t._simulated = !0, e.target.dispatchEvent(t)
+        }
+    }), O.addInitHook("addHandler", "tapHold", kt), O.mergeOptions({
+        touchZoom: b.touch,
+        bounceAtZoomLimits: !0
+    }), Ot = o.extend({
+        addHooks: function() {
+            M(this._map._container, "leaflet-touch-zoom"), S(this._map._container, "touchstart", this._onTouchStart, this)
+        },
+        removeHooks: function() {
+            z(this._map._container, "leaflet-touch-zoom"), E(this._map._container, "touchstart", this._onTouchStart, this)
+        },
+        _onTouchStart: function(t) {
+            var e, i, n = this._map;
+            !t.touches || 2 !== t.touches.length || n._animatingZoom || this._zooming || (e = n.mouseEventToContainerPoint(t.touches[0]), i = n.mouseEventToContainerPoint(t.touches[1]), this._centerPoint = n.getSize()._divideBy(2), this._startLatLng = n.containerPointToLatLng(this._centerPoint), "center" !== n.options.touchZoom && (this._pinchStartLatLng = n.containerPointToLatLng(e.add(i)._divideBy(2))), this._startDist = e.distanceTo(i), this._startZoom = n.getZoom(), this._moved = !1, this._zooming = !0, n._stop(), S(document, "touchmove", this._onTouchMove, this), S(document, "touchend touchcancel", this._onTouchEnd, this), k(t))
+        },
+        _onTouchMove: function(t) {
+            if (t.touches && 2 === t.touches.length && this._zooming) {
+                var e = this._map,
+                    i = e.mouseEventToContainerPoint(t.touches[0]),
+                    n = e.mouseEventToContainerPoint(t.touches[1]),
+                    o = i.distanceTo(n) / this._startDist;
+                if (this._zoom = e.getScaleZoom(o, this._startZoom), !e.options.bounceAtZoomLimits && (this._zoom < e.getMinZoom() && o < 1 || this._zoom > e.getMaxZoom() && 1 < o) && (this._zoom = e._limitZoom(this._zoom)), "center" === e.options.touchZoom) {
+                    if (this._center = this._startLatLng, 1 == o) return
+                } else {
+                    i = i._add(n)._divideBy(2)._subtract(this._centerPoint);
+                    if (1 == o && 0 === i.x && 0 === i.y) return;
+                    this._center = e.unproject(e.project(this._pinchStartLatLng, this._zoom).subtract(i), this._zoom)
                 }
-            },
-            _onTouchEnd: function() {
-                this._moved && this._zooming ? (this._zooming = !1, r(this._animRequest), E(document, "touchmove", this._onTouchMove, this), E(document, "touchend touchcancel", this._onTouchEnd, this), this._map.options.zoomAnimation ? this._map._animateZoom(this._center, this._map._limitZoom(this._zoom), !0, this._map.options.zoomSnap) : this._map._resetView(this._center, this._map._limitZoom(this._zoom))) : this._zooming = !1
+                this._moved || (e._moveStart(!0, !1), this._moved = !0), r(this._animRequest);
+                n = a(e._move, e, this._center, this._zoom, {
+                    pinch: !0,
+                    round: !1
+                }, void 0);
+                this._animRequest = x(n, this, !0), k(t)
             }
-        })),
-        qe = (A.addInitHook("addHandler", "touchZoom", Bt), A.BoxZoom = _t, A.DoubleClickZoom = Ct, A.Drag = Zt, A.Keyboard = St, A.ScrollWheelZoom = kt, A.TapHold = Et, A.TouchZoom = Bt, t.Bounds = m, t.Browser = P, t.CRS = ot, t.Canvas = De, t.Circle = me, t.CircleMarker = pe, t.Class = it, t.Control = I, t.DivIcon = Be, t.DivOverlay = O, t.DomEvent = mt, t.DomUtil = pt, t.Draggable = Xi, t.Evented = et, t.FeatureGroup = he, t.GeoJSON = ve, t.GridLayer = Ae, t.Handler = n, t.Icon = le, t.ImageOverlay = Ce, t.LatLng = v, t.LatLngBounds = s, t.Layer = o, t.LayerGroup = ae, t.LineUtil = gt, t.Map = A, t.Marker = de, t.Mixin = ft, t.Path = _e, t.Point = p, t.PolyUtil = vt, t.Polygon = ge, t.Polyline = fe, t.Popup = ke, t.PosAnimation = Wi, t.Projection = wt, t.Rectangle = Ve, t.Renderer = Ne, t.SVG = Fe, t.SVGOverlay = Se, t.TileLayer = Ie, t.Tooltip = Ee, t.Transformation = at, t.Util = tt, t.VideoOverlay = Ze, t.bind = a, t.bounds = f, t.canvas = je, t.circle = function(t, i, e) {
-            return new me(t, i, e)
-        }, t.circleMarker = function(t, i) {
-            return new pe(t, i)
-        }, t.control = Fi, t.divIcon = function(t) {
-            return new Be(t)
-        }, t.extend = l, t.featureGroup = function(t, i) {
-            return new he(t, i)
-        }, t.geoJSON = Me, t.geoJson = zt, t.gridLayer = function(t) {
-            return new Ae(t)
-        }, t.icon = function(t) {
-            return new le(t)
-        }, t.imageOverlay = function(t, i, e) {
-            return new Ce(t, i, e)
-        }, t.latLng = w, t.latLngBounds = g, t.layerGroup = function(t, i) {
-            return new ae(t, i)
-        }, t.map = function(t, i) {
-            return new A(t, i)
-        }, t.marker = function(t, i) {
-            return new de(t, i)
-        }, t.point = _, t.polygon = function(t, i) {
-            return new ge(t, i)
-        }, t.polyline = function(t, i) {
-            return new fe(t, i)
-        }, t.popup = function(t, i) {
-            return new ke(t, i)
-        }, t.rectangle = function(t, i) {
-            return new Ve(t, i)
-        }, t.setOptions = c, t.stamp = h, t.svg = Ue, t.svgOverlay = function(t, i, e) {
-            return new Se(t, i, e)
-        }, t.tileLayer = Oe, t.tooltip = function(t, i) {
-            return new Ee(t, i)
-        }, t.transformation = ht, t.version = "1.8.0", t.videoOverlay = function(t, i, e) {
-            return new Ze(t, i, e)
-        }, window.L);
-    t.noConflict = function() {
-        return window.L = qe, this
-    }, window.L = t
-});
+        },
+        _onTouchEnd: function() {
+            this._moved && this._zooming ? (this._zooming = !1, r(this._animRequest), E(document, "touchmove", this._onTouchMove, this), E(document, "touchend touchcancel", this._onTouchEnd, this), this._map.options.zoomAnimation ? this._map._animateZoom(this._center, this._map._limitZoom(this._zoom), !0, this._map.options.zoomSnap) : this._map._resetView(this._center, this._map._limitZoom(this._zoom))) : this._zooming = !1
+        }
+    });
+    O.addInitHook("addHandler", "touchZoom", Ot), O.BoxZoom = _t, O.DoubleClickZoom = Ct, O.Drag = Zt, O.Keyboard = St, O.ScrollWheelZoom = Et, O.TapHold = kt, O.TouchZoom = Ot;
+    var pn = l({
+            __proto__: null,
+            version: R,
+            Control: B,
+            control: qe,
+            Class: e,
+            Handler: o,
+            extend: l,
+            bind: a,
+            stamp: h,
+            setOptions: c,
+            Browser: b,
+            Evented: it,
+            Mixin: ft,
+            Util: et,
+            PosAnimation: Ve,
+            Draggable: ti,
+            DomEvent: mt,
+            DomUtil: pt,
+            Point: p,
+            point: m,
+            Bounds: f,
+            bounds: _,
+            Transformation: at,
+            transformation: ht,
+            LineUtil: gt,
+            PolyUtil: vt,
+            LatLng: v,
+            latLng: w,
+            LatLngBounds: s,
+            latLngBounds: g,
+            CRS: ot,
+            Projection: wt,
+            Layer: y,
+            LayerGroup: pi,
+            layerGroup: ci,
+            FeatureGroup: mi,
+            featureGroup: di,
+            ImageOverlay: Fi,
+            imageOverlay: Hi,
+            VideoOverlay: Wi,
+            videoOverlay: Ui,
+            SVGOverlay: Vi,
+            svgOverlay: Gi,
+            DivOverlay: I,
+            Popup: Yi,
+            popup: qi,
+            Tooltip: Ji,
+            tooltip: Ki,
+            icon: gi,
+            DivIcon: Xi,
+            divIcon: $i,
+            Marker: xi,
+            marker: wi,
+            Icon: fi,
+            GridLayer: Qi,
+            gridLayer: tn,
+            TileLayer: en,
+            tileLayer: nn,
+            Renderer: sn,
+            Canvas: rn,
+            canvas: an,
+            Path: bi,
+            CircleMarker: Pi,
+            circleMarker: Li,
+            Circle: Ti,
+            circle: Mi,
+            Polyline: zi,
+            polyline: Ci,
+            Polygon: Zi,
+            polygon: Si,
+            Rectangle: dn,
+            rectangle: _n,
+            SVG: un,
+            svg: cn,
+            GeoJSON: Ei,
+            geoJSON: ji,
+            geoJson: Mt,
+            Map: O,
+            map: Ge
+        }, {
+            noConflict: gn
+        }),
+        mn = function() {
+            if ("undefined" != typeof globalThis) return globalThis;
+            if ("undefined" != typeof self) return self;
+            if ("undefined" != typeof window) return window;
+            if ("undefined" == typeof global) throw new Error("Unable to locate global object.");
+            return global
+        }(),
+        fn = mn.L;
+
+    function gn() {
+        return mn.L = fn, pn
+    }
+    mn.L = pn, t.Bounds = f, t.Browser = b, t.CRS = ot, t.Canvas = rn, t.Circle = Ti, t.CircleMarker = Pi, t.Class = e, t.Control = B, t.DivIcon = Xi, t.DivOverlay = I, t.DomEvent = mt, t.DomUtil = pt, t.Draggable = ti, t.Evented = it, t.FeatureGroup = mi, t.GeoJSON = Ei, t.GridLayer = Qi, t.Handler = o, t.Icon = fi, t.ImageOverlay = Fi, t.LatLng = v, t.LatLngBounds = s, t.Layer = y, t.LayerGroup = pi, t.LineUtil = gt, t.Map = O, t.Marker = xi, t.Mixin = ft, t.Path = bi, t.Point = p, t.PolyUtil = vt, t.Polygon = Zi, t.Polyline = zi, t.Popup = Yi, t.PosAnimation = Ve, t.Projection = wt, t.Rectangle = dn, t.Renderer = sn, t.SVG = un, t.SVGOverlay = Vi, t.TileLayer = en, t.Tooltip = Ji, t.Transformation = at, t.Util = et, t.VideoOverlay = Wi, t.bind = a, t.bounds = _, t.canvas = an, t.circle = Mi, t.circleMarker = Li, t.control = qe, t.default = pn, t.divIcon = $i, t.extend = l, t.featureGroup = di, t.geoJSON = ji, t.geoJson = Mt, t.gridLayer = tn, t.icon = gi, t.imageOverlay = Hi, t.latLng = w, t.latLngBounds = g, t.layerGroup = ci, t.map = Ge, t.marker = wi, t.noConflict = gn, t.point = m, t.polygon = Si, t.polyline = Ci, t.popup = qi, t.rectangle = _n, t.setOptions = c, t.stamp = h, t.svg = cn, t.svgOverlay = Gi, t.tileLayer = nn, t.tooltip = Ki, t.transformation = ht, t.version = R, t.videoOverlay = Ui
+});
+//# sourceMappingURL=leaflet.js.map
```

### Comparing `clld-9.2.1/src/clld/web/static/js/oms.min.js` & `clld-9.2.2/src/clld/web/static/js/oms.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/raphael.min.js` & `clld-9.2.2/src/clld/web/static/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/select2.js` & `clld-9.2.2/src/clld/web/static/js/select2.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/static/js/tree.jquery.js` & `clld-9.2.2/src/clld/web/static/js/tree.jquery.js`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/subscribers.py` & `clld-9.2.2/src/clld/web/subscribers.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/app.mako` & `clld-9.2.2/src/clld/web/templates/app.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/combination/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/combination/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/combined.mako` & `clld-9.2.2/src/clld/web/templates/combined.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/contact.mako` & `clld-9.2.2/src/clld/web/templates/contact.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/contribution/md_txt.mako` & `clld-9.2.2/src/clld/web/templates/contribution/md_txt.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/contributor/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/contributor/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/dataset/rdf.mako` & `clld-9.2.2/src/clld/web/templates/dataset/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/datatable.mako` & `clld-9.2.2/src/clld/web/templates/datatable.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/download.mako` & `clld-9.2.2/src/clld/web/templates/download.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/index_atom.mako` & `clld-9.2.2/src/clld/web/templates/index_atom.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/index_rdf.mako` & `clld-9.2.2/src/clld/web/templates/index_rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/language/kml.mako` & `clld-9.2.2/src/clld/web/templates/language/kml.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/language/map_html.mako` & `clld-9.2.2/src/clld/web/templates/language/map_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/language/rdf.mako` & `clld-9.2.2/src/clld/web/templates/language/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/language/snippet_html.mako` & `clld-9.2.2/src/clld/web/templates/language/snippet_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/map.mako` & `clld-9.2.2/src/clld/web/templates/map.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/multiselect.mako` & `clld-9.2.2/src/clld/web/templates/multiselect.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/olac.mako` & `clld-9.2.2/src/clld/web/templates/olac.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/olac_archive.mako` & `clld-9.2.2/src/clld/web/templates/olac_archive.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/olac_record.mako` & `clld-9.2.2/src/clld/web/templates/olac_record.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/parameter/rdf.mako` & `clld-9.2.2/src/clld/web/templates/parameter/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/parameter/snippet_html.mako` & `clld-9.2.2/src/clld/web/templates/parameter/snippet_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/resource_rdf.mako` & `clld-9.2.2/src/clld/web/templates/resource_rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/sentence/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/sentence/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/sentence/rdf.mako` & `clld-9.2.2/src/clld/web/templates/sentence/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/source/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/source/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/source/rdf.mako` & `clld-9.2.2/src/clld/web/templates/source/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/source/snippet_html.mako` & `clld-9.2.2/src/clld/web/templates/source/snippet_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/unit/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/unit/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/unitparameter/rdf.mako` & `clld-9.2.2/src/clld/web/templates/unitparameter/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/unitvalue/rdf.mako` & `clld-9.2.2/src/clld/web/templates/unitvalue/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/util.mako` & `clld-9.2.2/src/clld/web/templates/util.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/value/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/value/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/value/rdf.mako` & `clld-9.2.2/src/clld/web/templates/value/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/value/snippet_html.mako` & `clld-9.2.2/src/clld/web/templates/value/snippet_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/valueset/detail_html.mako` & `clld-9.2.2/src/clld/web/templates/valueset/detail_html.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/templates/valueset/rdf.mako` & `clld-9.2.2/src/clld/web/templates/valueset/rdf.mako`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/component.py` & `clld-9.2.2/src/clld/web/util/component.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/concepticon.py` & `clld-9.2.2/src/clld/web/util/concepticon.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/doi.py` & `clld-9.2.2/src/clld/web/util/doi.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/downloadwidget.py` & `clld-9.2.2/src/clld/web/util/downloadwidget.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/glottolog.py` & `clld-9.2.2/src/clld/web/util/glottolog.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/helpers.py` & `clld-9.2.2/src/clld/web/util/helpers.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/multiselect.py` & `clld-9.2.2/src/clld/web/util/multiselect.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/util/pager.py` & `clld-9.2.2/src/clld/web/util/pager.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/views/__init__.py` & `clld-9.2.2/src/clld/web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/views/olac.py` & `clld-9.2.2/src/clld/web/views/olac.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld/web/views/sitemap.py` & `clld-9.2.2/src/clld/web/views/sitemap.py`

 * *Files identical despite different names*

### Comparing `clld-9.2.1/src/clld.egg-info/PKG-INFO` & `clld-9.2.2/src/clld.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: clld
-Version: 9.2.1
+Version: 9.2.2
 Summary: Python library supporting the development of cross-linguistic databases
 Home-page: https://clld.org
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache Software License
 Description: # clld
         
         The `clld` toolkit - a web framework for the publication of
         [Cross-Linguistic Linked Data](https://clld.org).
         
         Documentation for the code base and its use is available at http://clld.readthedocs.org/en/latest/. The source for this documentation is in the `docs` directory.
         
         [![Build Status](https://github.com/clld/clld/workflows/tests/badge.svg)](https://github.com/clld/clld/actions?query=workflow%3Atests)
-        [![codecov](https://codecov.io/gh/clld/clld/branch/master/graph/badge.svg)](https://codecov.io/gh/clld/clld)
         [![Requirements Status](https://requires.io/github/clld/clld/requirements.svg?branch=master)](https://requires.io/github/clld/clld/requirements/?branch=master)
         [![PyPI](https://img.shields.io/pypi/v/clld.svg)](https://pypi.python.org/pypi/clld)
         [![Documentation Status](http://readthedocs.org/projects/clld/badge/?version=latest)](http://clld.readthedocs.io/en/latest/?badge=latest)
         
         
         ## Cite
         
@@ -92,14 +91,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
```

### Comparing `clld-9.2.1/src/clld.egg-info/SOURCES.txt` & `clld-9.2.2/src/clld.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 src/clld/__init__.py
 src/clld/__main__.py
 src/clld/appconf.ini
 src/clld/cliutil.py
 src/clld/config.py
```

