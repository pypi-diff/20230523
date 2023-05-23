# Comparing `tmp/typecode-30.0.0.tar.gz` & `tmp/typecode-30.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typecode-30.0.0.tar", last modified: Mon May  9 21:59:31 2022, max compression
+gzip compressed data, was "typecode-30.0.1.tar", last modified: Tue May 23 00:27:25 2023, max compression
```

## Comparing `typecode-30.0.0.tar` & `typecode-30.0.1.tar`

### file list

```diff
@@ -1,786 +1,785 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.744150 typecode-30.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-09 21:59:18.000000 typecode-30.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.636142 typecode-30.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.644142 typecode-30.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-05-09 21:59:18.000000 typecode-30.0.0/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-05-09 21:59:18.000000 typecode-30.0.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-05-09 21:59:18.000000 typecode-30.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-09 21:59:18.000000 typecode-30.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-05-09 21:59:18.000000 typecode-30.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-05-09 21:59:18.000000 typecode-30.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-05-09 21:59:18.000000 typecode-30.0.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-09 21:59:18.000000 typecode-30.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-05-09 21:59:18.000000 typecode-30.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-05-09 21:59:31.744150 typecode-30.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-05-09 21:59:18.000000 typecode-30.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-05-09 21:59:18.000000 typecode-30.0.0/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-09 21:59:18.000000 typecode-30.0.0/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-05-09 21:59:18.000000 typecode-30.0.0/azure-pipelines.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)     6157 2022-05-09 21:59:18.000000 typecode-30.0.0/configure
--rw-r--r--   0 runner    (1001) docker     (121)     7109 2022-05-09 21:59:18.000000 typecode-30.0.0/configure.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.644142 typecode-30.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.648143 typecode-30.0.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.648143 typecode-30.0.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.648143 typecode-30.0.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8022 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.648143 typecode-30.0.0/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (121)    10245 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-05-09 21:59:18.000000 typecode-30.0.0/docs/source/skeleton-usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.636142 typecode-30.0.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.648143 typecode-30.0.0/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.652143 typecode-30.0.0/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3745 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8210 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)     9595 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     6141 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)    75791 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-05-09 21:59:18.000000 typecode-30.0.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-05-09 21:59:18.000000 typecode-30.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-09 21:59:18.000000 typecode-30.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2022-05-09 21:59:18.000000 typecode-30.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-05-09 21:59:31.744150 typecode-30.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-05-09 21:59:18.000000 typecode-30.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.636142 typecode-30.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.652143 typecode-30.0.0/src/typecode/
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.652143 typecode-30.0.0/src/typecode/_vendor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/bsd-new.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.656144 typecode-30.0.0/src/typecode/_vendor/pygments/
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19808 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.656144 typecode-30.0.0/src/typecode/_vendor/pygments/filters/
--rw-r--r--   0 runner    (1001) docker     (121)    40336 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.656144 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3348 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0 runner    (1001) docker     (121)    33527 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/html.py
--rw-r--r--   0 runner    (1001) docker     (121)    21236 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/img.py
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/irc.py
--rw-r--r--   0 runner    (1001) docker     (121)    18968 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/latex.py
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/other.py
--rw-r--r--   0 runner    (1001) docker     (121)     5048 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7330 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/svg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4730 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)    11177 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0 runner    (1001) docker     (121)    31586 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.684146 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/
--rw-r--r--   0 runner    (1001) docker     (121)    11351 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27311 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_asy_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    14018 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_cl_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    39962 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_cocoa_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    17881 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_csound_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)   134534 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_lasso_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     8297 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_lua_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    68577 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)    24737 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mql_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    24534 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mysql_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    48362 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_openedge_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)   154365 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_php_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_postgres_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    52418 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_scilab_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    27091 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_sourcemod_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    10481 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_stan_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    25228 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_stata_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    15484 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_tsql_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1682 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_usd_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)     4249 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_vbscript_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    57090 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_vim_builtins.py
--rw-r--r--   0 runner    (1001) docker     (121)    11511 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/actionscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/agile.py
--rw-r--r--   0 runner    (1001) docker     (121)     7788 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/algebra.py
--rw-r--r--   0 runner    (1001) docker     (121)     2597 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ambient.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ampl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/apl.py
--rw-r--r--   0 runner    (1001) docker     (121)    11165 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/archetype.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/arrow.py
--rw-r--r--   0 runner    (1001) docker     (121)    39443 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/asm.py
--rw-r--r--   0 runner    (1001) docker     (121)    19674 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/automation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2943 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/bare.py
--rw-r--r--   0 runner    (1001) docker     (121)    27671 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/boa.py
--rw-r--r--   0 runner    (1001) docker     (121)    28056 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/business.py
--rw-r--r--   0 runner    (1001) docker     (121)    15119 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/c_cpp.py
--rw-r--r--   0 runner    (1001) docker     (121)    24984 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/c_like.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/capnproto.py
--rw-r--r--   0 runner    (1001) docker     (121)     3979 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/chapel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/compiled.py
--rw-r--r--   0 runner    (1001) docker     (121)    33763 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/configs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/console.py
--rw-r--r--   0 runner    (1001) docker     (121)    15741 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/crystal.py
--rw-r--r--   0 runner    (1001) docker     (121)    16947 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/csound.py
--rw-r--r--   0 runner    (1001) docker     (121)    31700 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/css.py
--rw-r--r--   0 runner    (1001) docker     (121)     9732 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/d.py
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dalvik.py
--rw-r--r--   0 runner    (1001) docker     (121)    23963 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     4025 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/devicetree.py
--rw-r--r--   0 runner    (1001) docker     (121)     4919 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/diff.py
--rw-r--r--   0 runner    (1001) docker     (121)    28066 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dotnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    35883 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dsls.py
--rw-r--r--   0 runner    (1001) docker     (121)    10368 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dylan.py
--rw-r--r--   0 runner    (1001) docker     (121)     6304 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ecl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/eiffel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/elm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5186 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/email.py
--rw-r--r--   0 runner    (1001) docker     (121)    19021 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/erlang.py
--rw-r--r--   0 runner    (1001) docker     (121)    10207 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/esoteric.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ezhil.py
--rw-r--r--   0 runner    (1001) docker     (121)    17894 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/factor.py
--rw-r--r--   0 runner    (1001) docker     (121)    10016 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/fantom.py
--rw-r--r--   0 runner    (1001) docker     (121)     9442 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/felix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/floscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     7176 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/forth.py
--rw-r--r--   0 runner    (1001) docker     (121)     9931 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/fortran.py
--rw-r--r--   0 runner    (1001) docker     (121)    26271 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/foxpro.py
--rw-r--r--   0 runner    (1001) docker     (121)    27154 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/freefem.py
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)    11180 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/gdscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/go.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/grammar_notation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    39013 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)    32284 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/haskell.py
--rw-r--r--   0 runner    (1001) docker     (121)    31004 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/haxe.py
--rw-r--r--   0 runner    (1001) docker     (121)    22379 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/hdl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3541 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/hexdump.py
--rw-r--r--   0 runner    (1001) docker     (121)    20174 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/html.py
--rw-r--r--   0 runner    (1001) docker     (121)    15282 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/idl.py
--rw-r--r--   0 runner    (1001) docker     (121)    30643 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/igor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3151 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/inferno.py
--rw-r--r--   0 runner    (1001) docker     (121)    12900 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/installers.py
--rw-r--r--   0 runner    (1001) docker     (121)    56704 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/int_fiction.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/iolang.py
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/j.py
--rw-r--r--   0 runner    (1001) docker     (121)    60880 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/javascript.py
--rw-r--r--   0 runner    (1001) docker     (121)    13928 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/julia.py
--rw-r--r--   0 runner    (1001) docker     (121)    71060 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/jvm.py
--rw-r--r--   0 runner    (1001) docker     (121)   141435 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/lisp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7467 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/make.py
--rw-r--r--   0 runner    (1001) docker     (121)    26919 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/markup.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/math.py
--rw-r--r--   0 runner    (1001) docker     (121)    31947 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/matlab.py
--rw-r--r--   0 runner    (1001) docker     (121)     8026 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/mime.py
--rw-r--r--   0 runner    (1001) docker     (121)    35352 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ml.py
--rw-r--r--   0 runner    (1001) docker     (121)    13476 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/modeling.py
--rw-r--r--   0 runner    (1001) docker     (121)    53141 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/modula2.py
--rw-r--r--   0 runner    (1001) docker     (121)     6341 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/monte.py
--rw-r--r--   0 runner    (1001) docker     (121)     9245 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/mosel.py
--rw-r--r--   0 runner    (1001) docker     (121)    64020 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ncl.py
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nimrod.py
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nit.py
--rw-r--r--   0 runner    (1001) docker     (121)     4065 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nix.py
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/oberon.py
--rw-r--r--   0 runner    (1001) docker     (121)    22862 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/objective.py
--rw-r--r--   0 runner    (1001) docker     (121)     3033 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ooc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/other.py
--rw-r--r--   0 runner    (1001) docker     (121)     2771 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/parasail.py
--rw-r--r--   0 runner    (1001) docker     (121)    26091 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    32717 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pascal.py
--rw-r--r--   0 runner    (1001) docker     (121)     8303 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pawn.py
--rw-r--r--   0 runner    (1001) docker     (121)    39154 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/perl.py
--rw-r--r--   0 runner    (1001) docker     (121)    12639 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/php.py
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pointless.py
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pony.py
--rw-r--r--   0 runner    (1001) docker     (121)    12331 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/praat.py
--rw-r--r--   0 runner    (1001) docker     (121)    12441 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/prolog.py
--rw-r--r--   0 runner    (1001) docker     (121)     4791 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/promql.py
--rw-r--r--   0 runner    (1001) docker     (121)    51192 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/qvt.py
--rw-r--r--   0 runner    (1001) docker     (121)     6235 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/r.py
--rw-r--r--   0 runner    (1001) docker     (121)    15848 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)    18658 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rebol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     5108 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ride.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rnc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/roboconf.py
--rw-r--r--   0 runner    (1001) docker     (121)    18470 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/robotframework.py
--rw-r--r--   0 runner    (1001) docker     (121)    22437 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ruby.py
--rw-r--r--   0 runner    (1001) docker     (121)     8269 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rust.py
--rw-r--r--   0 runner    (1001) docker     (121)     9483 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/scdoc.py
--rw-r--r--   0 runner    (1001) docker     (121)    70124 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/scripting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sgf.py
--rw-r--r--   0 runner    (1001) docker     (121)    35968 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/shell.py
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sieve.py
--rw-r--r--   0 runner    (1001) docker     (121)     8557 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/slash.py
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/smalltalk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/smv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/snobol.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/solidity.py
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/special.py
--rw-r--r--   0 runner    (1001) docker     (121)    34135 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sql.py
--rw-r--r--   0 runner    (1001) docker     (121)     6489 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/stata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/supercollider.py
--rw-r--r--   0 runner    (1001) docker     (121)     5449 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/tcl.py
--rw-r--r--   0 runner    (1001) docker     (121)    71787 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     9943 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/teraterm.py
--rw-r--r--   0 runner    (1001) docker     (121)    10783 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     6172 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/textedit.py
--rw-r--r--   0 runner    (1001) docker     (121)    15267 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/textfmts.py
--rw-r--r--   0 runner    (1001) docker     (121)    19404 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/theorem.py
--rw-r--r--   0 runner    (1001) docker     (121)    10212 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/tnt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1580 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/trafficscript.py
--rw-r--r--   0 runner    (1001) docker     (121)     8258 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/typoscript.py
--rw-r--r--   0 runner    (1001) docker     (121)    18570 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/unicon.py
--rw-r--r--   0 runner    (1001) docker     (121)     6096 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/urbi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/usd.py
--rw-r--r--   0 runner    (1001) docker     (121)     7301 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/varnish.py
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/verification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/web.py
--rw-r--r--   0 runner    (1001) docker     (121)    10531 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/webidl.py
--rw-r--r--   0 runner    (1001) docker     (121)    40122 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/webmisc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4045 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/whiley.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/x10.py
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/xorg.py
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/yang.py
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/lexers/zig.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/modeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/regexopt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     4669 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (121)     6048 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/style.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/src/typecode/_vendor/pygments/styles/
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/abap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/algol.py
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/algol_nu.py
--rw-r--r--   0 runner    (1001) docker     (121)     4525 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/arduino.py
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/autumn.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/borland.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/bw.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/colorful.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/emacs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/friendly.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/fruity.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/igor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2381 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/inkpot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/lovelace.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/manni.py
--rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/monokai.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/murphy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/native.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/paraiso_dark.py
--rw-r--r--   0 runner    (1001) docker     (121)     5679 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/paraiso_light.py
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/pastie.py
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/perldoc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/rainbow_dash.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/rrt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/sas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3989 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/solarized.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/stata_dark.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/stata_light.py
--rw-r--r--   0 runner    (1001) docker     (121)     7130 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/tango.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/trac.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/vim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/vs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/styles/xcode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6167 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    63224 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/unistring.py
--rw-r--r--   0 runner    (1001) docker     (121)     9147 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/_vendor/pygments.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/bsd-new.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/bsd-simplified.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    27411 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/contenttype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/extractible.py
--rw-r--r--   0 runner    (1001) docker     (121)    14024 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/magic2.py
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/magic2.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)    40494 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/mimetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/mimetypes.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/mit.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/public-domain.LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    11260 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)    69785 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers_mapping.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/pygments_lexers_mapping.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     9785 2022-05-09 21:59:18.000000 typecode-30.0.0/src/typecode/python.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.652143 typecode-30.0.0/src/typecode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-05-09 21:59:30.000000 typecode-30.0.0/src/typecode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    29698 2022-05-09 21:59:31.000000 typecode-30.0.0/src/typecode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 21:59:30.000000 typecode-30.0.0/src/typecode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 21:59:30.000000 typecode-30.0.0/src/typecode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-05-09 21:59:31.000000 typecode-30.0.0/src/typecode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-09 21:59:31.000000 typecode-30.0.0/src/typecode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/contenttype/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/tests/data/contenttype/archive/
--rw-r--r--   0 runner    (1001) docker     (121)     9367 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/archive/crashing-squashfs
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/archive/sqfs-gz.sqs
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/archive/sqfs-lzo.sqs
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/archive/sqfs-xz.sqs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/tests/data/contenttype/certificate/
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/certificate/CERTIFICATE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/contenttype/code/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/tests/data/contenttype/code/c/
--rw-r--r--   0 runner    (1001) docker     (121)    37290 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/code/c/c_code.c
--rw-r--r--   0 runner    (1001) docker     (121)    37290 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/code/c/some.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.688146 typecode-30.0.0/tests/data/contenttype/code/python/
--rw-r--r--   0 runner    (1001) docker     (121)     1189 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/code/python/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/contenttype/compiled/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/compiled/java/
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/compiled/java/CommonViewerSiteFactory.class
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/compiled/java/old.class
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/compiled/linux/
--rw-r--r--   0 runner    (1001) docker     (121)   373403 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/compiled/linux/libnetsnmpagent.so.5
--rw-r--r--   0 runner    (1001) docker     (121)   186532 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/compiled/linux/libssl.so.0.9.7
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/compiled/python/
--rw-r--r--   0 runner    (1001) docker     (121)     7376 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/compiled/python/compiled.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/contenttype/doc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/doc/postscript/
--rw-r--r--   0 runner    (1001) docker     (121)    12388 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/doc/postscript/Image1.eps
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/links/
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/links/links.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/media/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/media/Image1.img
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/package/
--rw-r--r--   0 runner    (1001) docker     (121)    54216 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/package/libjama-dev_1.2.4-2_all.deb
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/package/package.json
--rw-r--r--   0 runner    (1001) docker     (121)    37728 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/package/wget-el_0.5.0-8_all.deb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.640142 typecode-30.0.0/tests/data/contenttype/size/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/size/dir/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/a.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/b.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/a.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/b.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/subsub/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/subsub/a.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub1/subsub/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/size/dir/sub2/
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/size/dir/sub2/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/text/
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/text/wildtest.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.692146 typecode-30.0.0/tests/data/contenttype/unicode/
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/unicode/unicode.zip
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/contenttype/unicode/unicode2.zip
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.696146 typecode-30.0.0/tests/data/extractible/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/a.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)     9367 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/crashing-squashfs
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/dbase.fdt
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/e.tar
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/e.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/e.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)    42754 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/file_4.26-1.diff.gz
--rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/posixnotgnu.tar
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/sqfs-gz.sqs
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/sqfs-lzo.sqs
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/sqfs-xz.sqs
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/test.tar.lzma
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/test.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/test.zip
--rw-r--r--   0 runner    (1001) docker     (121)     8845 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/extractible/win-archive.lib
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.696146 typecode-30.0.0/tests/data/filetest/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.700147 typecode-30.0.0/tests/data/filetest/archive/
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/a.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/a.tar.gz.yml
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/dbase.fdt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/dbase.fdt.yml
--rw-r--r--   0 runner    (1001) docker     (121)    10240 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar.bz2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar.gz.yml
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/e.tar.yml
--rw-r--r--   0 runner    (1001) docker     (121)    42754 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/file_4.26-1.diff.gz
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/file_4.26-1.diff.gz.yml
--rw-r--r--   0 runner    (1001) docker     (121)    35328 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/posixnotgnu.tar
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/posixnotgnu.tar.yml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.tar.lzma
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.tar.lzma.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.tar.xz
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.tar.xz.yml
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.zip
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/test.zip.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8845 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/win-archive.lib
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/archive/win-archive.lib.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.700147 typecode-30.0.0/tests/data/filetest/binary/
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/data.fdt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/data.fdt.yml
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/dbase.fdt
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/dbase.fdt.yml
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/jruby_time_zone_TimeOfDay.dat
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/jruby_time_zone_TimeOfDay.dat.yml
--rw-r--r--   0 runner    (1001) docker     (121)   129600 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/pixelstream.rgb
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/pixelstream.rgb.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/windows.dll
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary/windows.dll.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.704147 typecode-30.0.0/tests/data/filetest/binary-random/
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_0
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_0.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_1
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_1.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_2
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_2.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_3
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_3.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_4
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_4.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_5
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_5.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_6
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_6.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_7
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_7.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_8
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/binary-random/binary_random_8.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.704147 typecode-30.0.0/tests/data/filetest/build/
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/Makefile.inc
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/Makefile.inc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/Makefile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/ar-ER.css.map
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/ar-ER.css.map.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/ar-ER.js.map
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/ar-ER.js.map.yml
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/binary.js.map
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/binary.js.map.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/build.xml
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/build.xml.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2492 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/documentation.dsp
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/documentation.dsp.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.704147 typecode-30.0.0/tests/data/filetest/build/m/
--rw-r--r--   0 runner    (1001) docker     (121)     2888 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/m/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/m/Makefile.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/pom.pom
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/pom.pom.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6129 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/pom.xml
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/build/pom.xml.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.704147 typecode-30.0.0/tests/data/filetest/certificate/
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/certificate/ECLIPSE.RSA
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/certificate/ECLIPSE.RSA.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.644142 typecode-30.0.0/tests/data/filetest/code/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.704147 typecode-30.0.0/tests/data/filetest/code/assembly/
--rw-r--r--   0 runner    (1001) docker     (121)    32452 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/assembly/bcopy.s
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/assembly/bcopy.s.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.708147 typecode-30.0.0/tests/data/filetest/code/c/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/CcccDevStudioAddIn.rc2
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/CcccDevStudioAddIn.rc2.yml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/SIMPLE.C
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/SIMPLE.C.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/TEST.H
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/TEST.H.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8440 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/TEST_LOWERCASE.h
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/TEST_LOWERCASE.h.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/cpu.c
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/cpu.c.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/main.c
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/main.c.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3297 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/mm.c
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/mm.c.yml
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/netdb.h
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/netdb.h.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/pci.c
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/pci.c.yml
--rw-r--r--   0 runner    (1001) docker     (121)    18253 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/pci_v3.c
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/pci_v3.c.yml
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/resource.h
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/c/resource.h.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.708147 typecode-30.0.0/tests/data/filetest/code/cpp/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/StdAfx.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/StdAfx.cpp.yml
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/non_ascii.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/non_ascii.cpp.yml
--rw-r--r--   0 runner    (1001) docker     (121)    13670 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/stacktrace.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/stacktrace.cpp.yml
--rw-r--r--   0 runner    (1001) docker     (121)    69358 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/string.CPP
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/cpp/string.CPP.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.708147 typecode-30.0.0/tests/data/filetest/code/groff/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/groff/example.ms
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/groff/example.ms.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/code/java/
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/Appender.java
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/Appender.java.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/ChartTiming1.java
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/ChartTiming1.java.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/CommonViewerSiteFactory.jad
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/CommonViewerSiteFactory.jad.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/Logger.JAVA
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/Logger.JAVA.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/contenttype.java
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/java/contenttype.java.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/code/js/
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/js/a.js
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/js/a.js.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/code/python/
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/python/__init__.py.yml
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/python/contenttype.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/python/contenttype.py.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/code/scala/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/scala/ABOUT
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/scala/ABOUT.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/scala/Applicative.scala
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/code/scala/Applicative.scala.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.644142 typecode-30.0.0/tests/data/filetest/compiled/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/compiled/flash/
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/a.swf
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/a.swf.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/b.swf
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/b.swf.yml
--rw-r--r--   0 runner    (1001) docker     (121)   207900 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/compiled/linux/
--rw-r--r--   0 runner    (1001) docker     (121)    22887 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/linux/i686-shash
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/linux/i686-shash.yml
--rw-r--r--   0 runner    (1001) docker     (121)    19446 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/linux/x86_64-shash
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/linux/x86_64-shash.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.712147 typecode-30.0.0/tests/data/filetest/compiled/win/
--rw-r--r--   0 runner    (1001) docker     (121)    45056 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/win/file.exe
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/win/file.exe.yml
--rw-r--r--   0 runner    (1001) docker     (121)    72192 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/win/zlib1.dll
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/compiled/win/zlib1.dll.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.720148 typecode-30.0.0/tests/data/filetest/config/
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/config.conf
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/config.conf.yml
--rw-r--r--   0 runner    (1001) docker     (121)    14466 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/defconfig-ar531x-jffs2
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/defconfig-ar531x-jffs2.yml
--rw-r--r--   0 runner    (1001) docker     (121)   338561 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/eclipse_configuration_3u.cfs
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/eclipse_configuration_3u.cfs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/wrapper.conf
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/config/wrapper.conf.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.720148 typecode-30.0.0/tests/data/filetest/data/
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARM
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARM.yml
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARN
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARN.yml
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARZ
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.ARZ.yml
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/mysql-arch.yml
--rw-r--r--   0 runner    (1001) docker     (121)    10000 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/nulls.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/data/nulls.txt.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.720148 typecode-30.0.0/tests/data/filetest/debug/
--rw-r--r--   0 runner    (1001) docker     (121)   863232 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/debug/QTMovieWin.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/debug/QTMovieWin.pdb.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.644142 typecode-30.0.0/tests/data/filetest/doc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.724148 typecode-30.0.0/tests/data/filetest/doc/html/
--rw-r--r--   0 runner    (1001) docker     (121)    49584 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/Label.html
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/Label.html.yml
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/a.htm
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/a.htm.yml
--rw-r--r--   0 runner    (1001) docker     (121)   434697 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/allclasses-frame.html
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/allclasses-frame.html.yml
--rw-r--r--   0 runner    (1001) docker     (121)    23689 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/contenttype.html
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/html/contenttype.html.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.724148 typecode-30.0.0/tests/data/filetest/doc/office/
--rw-r--r--   0 runner    (1001) docker     (121)   100864 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/Glitch-ERD.vsd
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/Glitch-ERD.vsd.yml
--rw-r--r--   0 runner    (1001) docker     (121)    24015 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/document
--rw-r--r--   0 runner    (1001) docker     (121)    24015 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/document.doc
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/document.doc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/document.yml
--rw-r--r--   0 runner    (1001) docker     (121)    13824 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/excel.xls
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/excel.xls.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8276 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/excel.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/excel.xlsx.yml
--rw-r--r--   0 runner    (1001) docker     (121)     9216 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/power.ppt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/power.ppt.yml
--rw-r--r--   0 runner    (1001) docker     (121)    28876 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/power.pptx
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/power.pptx.yml
--rw-r--r--   0 runner    (1001) docker     (121)    31232 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/word.doc
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/word.doc.yml
--rw-r--r--   0 runner    (1001) docker     (121)    11868 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/word.docx
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/office/word.docx.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.728149 typecode-30.0.0/tests/data/filetest/doc/pdf/
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/a.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/a.pdf.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/notpdf.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/notpdf.pdf.yml
--rw-r--r--   0 runner    (1001) docker     (121)    29133 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/pdf.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/pdf/pdf.pdf.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.728149 typecode-30.0.0/tests/data/filetest/doc/postscript/
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/postscript/a.ps
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/postscript/a.ps.yml
--rw-r--r--   0 runner    (1001) docker     (121)   232479 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/postscript/doc.ps
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/postscript/doc.ps.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.728149 typecode-30.0.0/tests/data/filetest/doc/xml/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/simple.xml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/simple.xml.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/some.xml
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/some.xml.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2396 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/somespring.xml
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/doc/xml/somespring.xml.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.736149 typecode-30.0.0/tests/data/filetest/media/
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image-ascii.pgm
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image-ascii.pgm.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image.pgm
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image.pgm.yml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.bmp.yml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.dib
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.dib.yml
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.emf
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.emf.yml
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.gif
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.gif.yml
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ico
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ico.yml
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.iff
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.iff.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jif
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jif.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jpeg
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jpeg.yml
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.jpg.yml
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.pbm
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.pbm.yml
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.pcx
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.pcx.yml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ppm
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ppm.yml
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.psd
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.psd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.psp
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.psp.yml
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ras
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.ras.yml
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.tga
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.tga.yml
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.tif
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.tif.yml
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.wmf
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Image1.wmf.yml
--rw-r--r--   0 runner    (1001) docker     (121)    12053 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie.wmv
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie.wmv.yml
--rw-r--r--   0 runner    (1001) docker     (121)    43620 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie_0001.wmv
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie_0001.wmv.yml
--rw-r--r--   0 runner    (1001) docker     (121)    46372 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie_0002.wmv
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/Movie_0002.wmv.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/TBarLrge.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/TBarLrge.bmp.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/TBarMedm.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/TBarMedm.bmp.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.aif
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.aif.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8246 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.aiff
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.aiff.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8216 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.au
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.au.yml
--rw-r--r--   0 runner    (1001) docker     (121)   156277 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.avi
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.avi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.flac
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.flac.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.mp2
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.mp2.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2507 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.mp3
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.mp3.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5323 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.ogg
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.ogg.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.pdf
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.pdf.yml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.png
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.png.yml
--rw-r--r--   0 runner    (1001) docker     (121)    81644 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.theo.ogg
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.theo.ogg.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.wav
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a.wav.yml
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a4.mp4
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a4.mp4.yml
--rw-r--r--   0 runner    (1001) docker     (121)   238534 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a4.mpg
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/a4.mpg.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/drawing.svg
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/drawing.svg.yml
--rw-r--r--   0 runner    (1001) docker     (121)    10416 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/mov.wvm.wmv
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/media/mov.wvm.wmv.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.740149 typecode-30.0.0/tests/data/filetest/package/
--rw-r--r--   0 runner    (1001) docker     (121)    38037 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg.yml
--rw-r--r--   0 runner    (1001) docker     (121)    30122 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/ant-jsch-1.7.0.jar
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/ant-jsch-1.7.0.jar.yml
--rw-r--r--   0 runner    (1001) docker     (121)    30122 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/ant.zip
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/ant.zip.yml
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/c.war
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/c.war.yml
--rw-r--r--   0 runner    (1001) docker     (121)   301056 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/rubygems-update-1.4.1.gem
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/rubygems-update-1.4.1.gem.yml
--rw-r--r--   0 runner    (1001) docker     (121)   614846 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.740149 typecode-30.0.0/tests/data/filetest/script/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/build_w32vc.bat
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/build_w32vc.bat.yml
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/install
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/install.yml
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/makelinks
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/makelinks.yml
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/test.sh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/zip_src.bat
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/script/zip_src.bat.yml
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/test.sh
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/test.sh.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.744150 typecode-30.0.0/tests/data/filetest/text/
--rw-r--r--   0 runner    (1001) docker     (121)    18691 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/COPYING.yml
--rw-r--r--   0 runner    (1001) docker     (121)    82295 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/CREDITS
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/CREDITS.yml
--rwxr-xr-x   0 runner    (1001) docker     (121)    76402 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/ChangeLog.yml
--rw-r--r--   0 runner    (1001) docker     (121)    17982 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/GPL.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/GPL.txt.yml
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/crashing-a.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/crashing-a.txt.yml
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/crashing-z.txt
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/crashing-z.txt.yml
--rw-r--r--   0 runner    (1001) docker     (121)    65454 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/windowserver.log
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/windowserver.log.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/x11-xconsortium_text.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/data/filetest/text/x11-xconsortium_text.txt.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/filetype_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16586 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_contenttype.py
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1578 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_extractible.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_magic2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-05-09 21:59:18.000000 typecode-30.0.0/tests/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-09 21:59:31.744150 typecode-30.0.0/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-09 21:59:18.000000 typecode-30.0.0/thirdparty/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-05-09 21:59:18.000000 typecode-30.0.0/typecode.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.262997 typecode-30.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-23 00:27:12.000000 typecode-30.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.090997 typecode-30.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-23 00:27:12.000000 typecode-30.0.1/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-23 00:27:12.000000 typecode-30.0.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-23 00:27:12.000000 typecode-30.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-23 00:27:12.000000 typecode-30.0.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-23 00:27:12.000000 typecode-30.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1909 2023-05-23 00:27:12.000000 typecode-30.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3422 2023-05-23 00:27:12.000000 typecode-30.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-23 00:27:12.000000 typecode-30.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-23 00:27:12.000000 typecode-30.0.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-23 00:27:12.000000 typecode-30.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     3870 2023-05-23 00:27:25.262997 typecode-30.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2724 2023-05-23 00:27:12.000000 typecode-30.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-23 00:27:12.000000 typecode-30.0.1/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-23 00:27:12.000000 typecode-30.0.1/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-23 00:27:12.000000 typecode-30.0.1/azure-pipelines.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6339 2023-05-23 00:27:12.000000 typecode-30.0.1/configure
+-rw-r--r--   0 runner    (1001) docker     (122)     6959 2023-05-23 00:27:12.000000 typecode-30.0.1/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     8022 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.106997 typecode-30.0.1/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (122)    10245 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5491 2023-05-23 00:27:12.000000 typecode-30.0.1/docs/source/skeleton-usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.090997 typecode-30.0.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.110997 typecode-30.0.1/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1240 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1215 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1022 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.114997 typecode-30.0.1/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3744 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9486 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9699 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2776 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2266 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4497 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2839 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6418 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6704 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     6152 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75931 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-23 00:27:12.000000 typecode-30.0.1/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-05-23 00:27:12.000000 typecode-30.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      402 2023-05-23 00:27:12.000000 typecode-30.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1504 2023-05-23 00:27:12.000000 typecode-30.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-05-23 00:27:25.262997 typecode-30.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-23 00:27:12.000000 typecode-30.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.090997 typecode-30.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.118997 typecode-30.0.1/src/typecode/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.118997 typecode-30.0.1/src/typecode/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/bsd-new.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.122997 typecode-30.0.1/src/typecode/_vendor/pygments/
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19808 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/console.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1962 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.122997 typecode-30.0.1/src/typecode/_vendor/pygments/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)    40336 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.126997 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33527 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21236 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/img.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18968 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5204 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/other.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5048 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7330 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11177 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31586 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.170997 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/
+-rw-r--r--   0 runner    (1001) docker     (122)    11351 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27311 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_asy_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14018 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_cl_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39962 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_cocoa_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17881 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_csound_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)   134534 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_lasso_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8297 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_lua_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68577 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24737 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mql_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24534 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mysql_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48362 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_openedge_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)   154365 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_php_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12225 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_postgres_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52418 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_scilab_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27091 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_sourcemod_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10481 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_stan_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25228 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_stata_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15484 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_tsql_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_usd_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4249 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_vbscript_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57090 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_vim_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11511 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/actionscript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/agile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7788 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ambient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4157 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ampl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3306 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/apl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11165 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/archetype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39443 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/asm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19674 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/automation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2943 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/bare.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27671 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4004 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/boa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/business.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/c_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24984 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/c_like.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/capnproto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/chapel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6419 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/clean.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/compiled.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33763 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/configs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4154 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/console.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15741 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/crystal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16947 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/csound.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31700 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9732 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4454 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dalvik.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23963 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4025 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/devicetree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4919 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28066 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dotnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35883 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dsls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10368 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dylan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ecl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2516 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/eiffel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3037 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/elm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5186 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/email.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19021 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/erlang.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10207 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/esoteric.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ezhil.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17894 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/factor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10016 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/fantom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9442 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/felix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2701 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/floscript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7176 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/forth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9931 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26271 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/foxpro.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27154 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/freefem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/functional.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11180 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/gdscript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/go.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7975 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/grammar_notation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2790 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39013 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32284 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/haskell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31004 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/haxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22379 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/hdl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3541 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20174 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15282 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/idl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30643 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/igor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3151 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/inferno.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12900 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/installers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56704 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/int_fiction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1945 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/iolang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4561 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/j.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60880 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13928 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/julia.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71060 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)   141435 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/lisp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7467 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/make.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26919 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/markup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/math.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31947 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/matlab.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8026 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/mime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35352 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ml.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13476 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53141 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/modula2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/monte.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9245 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/mosel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64020 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ncl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5178 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nimrod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2777 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4065 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4269 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/oberon.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22862 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/objective.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ooc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/other.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2771 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/parasail.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26091 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32717 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pascal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8303 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39154 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/perl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12639 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/php.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2026 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pointless.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pony.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12331 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/praat.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12441 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/prolog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4791 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/promql.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51192 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/python.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6130 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/qvt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6235 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/r.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15848 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18658 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rebol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2960 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5108 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ride.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rnc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2104 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/roboconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18470 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/robotframework.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ruby.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8269 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rust.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9483 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2302 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/scdoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70124 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/scripting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sgf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35968 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8557 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/slash.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7250 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/smalltalk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2827 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/smv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2790 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/snobol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/solidity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/special.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34135 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/stata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3751 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/supercollider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71787 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9943 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/teraterm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10783 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6172 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/textedit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15267 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/textfmts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19404 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/theorem.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10212 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/tnt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/trafficscript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8258 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/typoscript.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18570 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/unicon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6096 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/urbi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3543 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/usd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7301 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/varnish.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3966 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/verification.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/web.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10531 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/webidl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40122 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/webmisc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4045 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/whiley.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2005 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/x10.py
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/xorg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4581 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/yang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3997 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/lexers/zig.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1010 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/modeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1734 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3094 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/regexopt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3115 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4669 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/style.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.174997 typecode-30.0.1/src/typecode/_vendor/pygments/styles/
+-rw-r--r--   0 runner    (1001) docker     (122)     2906 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/abap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2297 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/algol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2312 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/algol_nu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4525 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/arduino.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/autumn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/borland.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1389 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/bw.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2812 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/colorful.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2520 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/emacs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/friendly.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/fruity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/igor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2381 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/inkpot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3207 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/lovelace.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/manni.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5120 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/monokai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/murphy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1972 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/native.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5675 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/paraiso_dark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5679 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/paraiso_light.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/pastie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/perldoc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/rainbow_dash.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/rrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3989 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/solarized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1279 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/stata_dark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/stata_light.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7130 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/tango.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/trac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2010 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/vim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/vs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1535 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/styles/xcode.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)    63224 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/unistring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9147 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1923 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/_vendor/pygments.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    11356 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/bsd-new.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/bsd-simplified.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    27411 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/extractible.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14029 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/magic2.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/magic2.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)    40494 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/mimetypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      389 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/mimetypes.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/mit.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/public-domain.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11260 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    69785 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1138 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers_mapping.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)     1890 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/pygments_lexers_mapping.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     9785 2023-05-23 00:27:12.000000 typecode-30.0.1/src/typecode/python.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.118997 typecode-30.0.1/src/typecode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3870 2023-05-23 00:27:24.000000 typecode-30.0.1/src/typecode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    29685 2023-05-23 00:27:25.000000 typecode-30.0.1/src/typecode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 00:27:24.000000 typecode-30.0.1/src/typecode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 00:27:24.000000 typecode-30.0.1/src/typecode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      313 2023-05-23 00:27:24.000000 typecode-30.0.1/src/typecode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 00:27:24.000000 typecode-30.0.1/src/typecode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/contenttype/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/data/contenttype/archive/
+-rw-r--r--   0 runner    (1001) docker     (122)     9367 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/archive/crashing-squashfs
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/archive/sqfs-gz.sqs
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/archive/sqfs-lzo.sqs
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/archive/sqfs-xz.sqs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/data/contenttype/certificate/
+-rw-r--r--   0 runner    (1001) docker     (122)     5688 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/certificate/CERTIFICATE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/contenttype/code/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/data/contenttype/code/c/
+-rw-r--r--   0 runner    (1001) docker     (122)    37290 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/code/c/c_code.c
+-rw-r--r--   0 runner    (1001) docker     (122)    37290 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/code/c/some.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/data/contenttype/code/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/code/python/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/contenttype/compiled/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.178997 typecode-30.0.1/tests/data/contenttype/compiled/java/
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/compiled/java/CommonViewerSiteFactory.class
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/compiled/java/old.class
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/compiled/linux/
+-rw-r--r--   0 runner    (1001) docker     (122)   373403 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/compiled/linux/libnetsnmpagent.so.5
+-rw-r--r--   0 runner    (1001) docker     (122)   186532 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/compiled/linux/libssl.so.0.9.7
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/compiled/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     7376 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/compiled/python/compiled.zip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/contenttype/doc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/doc/postscript/
+-rw-r--r--   0 runner    (1001) docker     (122)    12388 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/doc/postscript/Image1.eps
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/links/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/links/links.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/media/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/media/Image1.img
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/package/
+-rw-r--r--   0 runner    (1001) docker     (122)    54216 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/package/libjama-dev_1.2.4-2_all.deb
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/package/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)    37728 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/package/wget-el_0.5.0-8_all.deb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.094997 typecode-30.0.1/tests/data/contenttype/size/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/size/dir/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/b.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.182997 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/b.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.186997 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/subsub/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/subsub/a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub1/subsub/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.186997 typecode-30.0.1/tests/data/contenttype/size/dir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (122)        2 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/size/dir/sub2/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.186997 typecode-30.0.1/tests/data/contenttype/text/
+-rw-r--r--   0 runner    (1001) docker     (122)     4233 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/text/wildtest.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.186997 typecode-30.0.1/tests/data/contenttype/unicode/
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/unicode/unicode.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/contenttype/unicode/unicode2.zip
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.190997 typecode-30.0.1/tests/data/extractible/
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/a.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)     9367 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/crashing-squashfs
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/dbase.fdt
+-rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/e.tar
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/e.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/e.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    42754 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/file_4.26-1.diff.gz
+-rw-r--r--   0 runner    (1001) docker     (122)    35328 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/posixnotgnu.tar
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/sqfs-gz.sqs
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/sqfs-lzo.sqs
+-rw-r--r--   0 runner    (1001) docker     (122)     4096 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/sqfs-xz.sqs
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/test.tar.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/test.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/test.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/extractible/win-archive.lib
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.190997 typecode-30.0.1/tests/data/filetest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.194997 typecode-30.0.1/tests/data/filetest/archive/
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/a.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/a.tar.gz.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/dbase.fdt
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/dbase.fdt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    10240 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar.bz2.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar.gz.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/e.tar.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    42754 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/file_4.26-1.diff.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/file_4.26-1.diff.gz.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    35328 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/posixnotgnu.tar
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/posixnotgnu.tar.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.tar.lzma
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.tar.lzma.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.tar.xz.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      177 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/test.zip.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/win-archive.lib
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/archive/win-archive.lib.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.194997 typecode-30.0.1/tests/data/filetest/binary/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/data.fdt
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/data.fdt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/dbase.fdt
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/dbase.fdt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/jruby_time_zone_TimeOfDay.dat
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/jruby_time_zone_TimeOfDay.dat.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   129600 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/pixelstream.rgb
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/pixelstream.rgb.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3394 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/windows.dll
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary/windows.dll.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.198997 typecode-30.0.1/tests/data/filetest/binary-random/
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_0
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_0.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_1
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_1.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_2
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_2.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_3
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_3.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_4
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_4.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_5
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_5.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_6
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_6.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_7
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_7.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_8
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/binary-random/binary_random_8.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.202997 typecode-30.0.1/tests/data/filetest/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      502 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/Makefile.inc
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/Makefile.inc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/Makefile.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/ar-ER.css.map
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/ar-ER.css.map.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1605 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/ar-ER.js.map
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/ar-ER.js.map.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/binary.js.map
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/binary.js.map.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4161 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/build.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/build.xml.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/documentation.dsp
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/documentation.dsp.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.202997 typecode-30.0.1/tests/data/filetest/build/m/
+-rw-r--r--   0 runner    (1001) docker     (122)     2888 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/m/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/m/Makefile.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/pom.pom
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/pom.pom.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/pom.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/build/pom.xml.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.202997 typecode-30.0.1/tests/data/filetest/certificate/
+-rw-r--r--   0 runner    (1001) docker     (122)     3487 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/certificate/ECLIPSE.RSA
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/certificate/ECLIPSE.RSA.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.098997 typecode-30.0.1/tests/data/filetest/code/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.206997 typecode-30.0.1/tests/data/filetest/code/assembly/
+-rw-r--r--   0 runner    (1001) docker     (122)    32452 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/assembly/bcopy.s
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/assembly/bcopy.s.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.210997 typecode-30.0.1/tests/data/filetest/code/c/
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/CcccDevStudioAddIn.rc2
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/CcccDevStudioAddIn.rc2.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/SIMPLE.C
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/SIMPLE.C.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/TEST.H
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/TEST.H.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/TEST_LOWERCASE.h
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/TEST_LOWERCASE.h.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3044 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/cpu.c
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/cpu.c.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/main.c
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/main.c.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/mm.c
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/mm.c.yml
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/netdb.h
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/netdb.h.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/pci.c
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/pci.c.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    18253 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/pci_v3.c
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/pci_v3.c.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/resource.h
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/c/resource.h.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.210997 typecode-30.0.1/tests/data/filetest/code/cpp/
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/StdAfx.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/StdAfx.cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/non_ascii.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/non_ascii.cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    13670 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/stacktrace.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/stacktrace.cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    69358 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/string.CPP
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/cpp/string.CPP.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.210997 typecode-30.0.1/tests/data/filetest/code/groff/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/groff/example.ms
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/groff/example.ms.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.214997 typecode-30.0.1/tests/data/filetest/code/java/
+-rw-r--r--   0 runner    (1001) docker     (122)     3647 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/Appender.java
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/Appender.java.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4116 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/ChartTiming1.java
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/ChartTiming1.java.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/CommonViewerSiteFactory.jad
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/CommonViewerSiteFactory.jad.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6800 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/Logger.JAVA
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/Logger.JAVA.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/contenttype.java
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/java/contenttype.java.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.214997 typecode-30.0.1/tests/data/filetest/code/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/js/a.js
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/js/a.js.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.214997 typecode-30.0.1/tests/data/filetest/code/python/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/python/__init__.py.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/python/contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/python/contenttype.py.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.214997 typecode-30.0.1/tests/data/filetest/code/scala/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/scala/ABOUT
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/scala/ABOUT.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4500 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/scala/Applicative.scala
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/code/scala/Applicative.scala.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.098997 typecode-30.0.1/tests/data/filetest/compiled/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.218997 typecode-30.0.1/tests/data/filetest/compiled/flash/
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/a.swf
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/a.swf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/b.swf
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/b.swf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   207900 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.218997 typecode-30.0.1/tests/data/filetest/compiled/linux/
+-rw-r--r--   0 runner    (1001) docker     (122)    22887 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/linux/i686-shash
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/linux/i686-shash.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    19446 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/linux/x86_64-shash
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/linux/x86_64-shash.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.218997 typecode-30.0.1/tests/data/filetest/compiled/win/
+-rw-r--r--   0 runner    (1001) docker     (122)    45056 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/win/file.exe
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/win/file.exe.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    72192 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/win/zlib1.dll
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/compiled/win/zlib1.dll.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.222997 typecode-30.0.1/tests/data/filetest/config/
+-rw-r--r--   0 runner    (1001) docker     (122)     4005 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/config.conf
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/config.conf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    14466 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/defconfig-ar531x-jffs2
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/defconfig-ar531x-jffs2.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   338561 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/eclipse_configuration_3u.cfs
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/eclipse_configuration_3u.cfs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4005 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/wrapper.conf
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/config/wrapper.conf.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.222997 typecode-30.0.1/tests/data/filetest/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARM
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARM.yml
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARN
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARN.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARZ
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.ARZ.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/mysql-arch.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    10000 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/nulls.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/data/nulls.txt.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.226997 typecode-30.0.1/tests/data/filetest/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)   863232 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/debug/QTMovieWin.pdb
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/debug/QTMovieWin.pdb.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.098997 typecode-30.0.1/tests/data/filetest/doc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.226997 typecode-30.0.1/tests/data/filetest/doc/html/
+-rw-r--r--   0 runner    (1001) docker     (122)    49584 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/Label.html
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/Label.html.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/a.htm
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/a.htm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   434697 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/allclasses-frame.html
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/allclasses-frame.html.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    23689 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/contenttype.html
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/html/contenttype.html.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.230997 typecode-30.0.1/tests/data/filetest/doc/office/
+-rw-r--r--   0 runner    (1001) docker     (122)   100864 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/Glitch-ERD.vsd
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/Glitch-ERD.vsd.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    24015 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/document
+-rw-r--r--   0 runner    (1001) docker     (122)    24015 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/document.doc
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/document.doc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      233 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/document.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    13824 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/excel.xls
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/excel.xls.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8276 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/excel.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)      310 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/excel.xlsx.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     9216 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/power.ppt
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/power.ppt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    28876 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/power.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/power.pptx.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    31232 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/word.doc
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/word.doc.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    11868 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/word.docx
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/office/word.docx.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.230997 typecode-30.0.1/tests/data/filetest/doc/pdf/
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/a.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/a.pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/notpdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/notpdf.pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    29133 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/pdf.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/pdf/pdf.pdf.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.234997 typecode-30.0.1/tests/data/filetest/doc/postscript/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/postscript/a.ps
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/postscript/a.ps.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   232479 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/postscript/doc.ps
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/postscript/doc.ps.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.234997 typecode-30.0.1/tests/data/filetest/doc/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/simple.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/simple.xml.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/some.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/some.xml.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/somespring.xml
+-rw-r--r--   0 runner    (1001) docker     (122)      201 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/doc/xml/somespring.xml.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.250997 typecode-30.0.1/tests/data/filetest/media/
+-rw-r--r--   0 runner    (1001) docker     (122)     5458 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image-ascii.pgm
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image-ascii.pgm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1478 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image.pgm
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image.pgm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.bmp
+-rw-r--r--   0 runner    (1001) docker     (122)      291 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.bmp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.dib
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.dib.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.emf
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.emf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.gif
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.gif.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ico.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.iff
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.iff.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jif
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jif.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jpeg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jpg
+-rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.jpg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.pbm
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.pbm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.pcx
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.pcx.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ppm
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ppm.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.psd
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.psd.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.psp
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.psp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ras
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.ras.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      543 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.tga
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.tga.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.tif
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.tif.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.wmf
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Image1.wmf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12053 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie.wmv
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie.wmv.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    43620 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie_0001.wmv
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie_0001.wmv.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    46372 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie_0002.wmv
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/Movie_0002.wmv.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/TBarLrge.bmp
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/TBarLrge.bmp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/TBarMedm.bmp
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/TBarMedm.bmp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.aif
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.aif.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.aiff
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.aiff.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8216 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.au
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.au.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   156277 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.avi
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.avi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4036 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.flac
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.flac.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2088 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.mp2
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.mp2.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.mp3
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.mp3.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     5323 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.ogg
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.ogg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.png
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.png.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    81644 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.theo.ogg
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.theo.ogg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.wav
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a.wav.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a4.mp4
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a4.mp4.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   238534 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a4.mpg
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/a4.mpg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/drawing.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/drawing.svg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    10416 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/mov.wvm.wmv
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/media/mov.wvm.wmv.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.254997 typecode-30.0.1/tests/data/filetest/package/
+-rw-r--r--   0 runner    (1001) docker     (122)    38037 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    30122 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/ant-jsch-1.7.0.jar
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/ant-jsch-1.7.0.jar.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    30122 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/ant.zip
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/ant.zip.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/c.war
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/c.war.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   301056 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/rubygems-update-1.4.1.gem
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/rubygems-update-1.4.1.gem.yml
+-rw-r--r--   0 runner    (1001) docker     (122)   614846 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.258997 typecode-30.0.1/tests/data/filetest/script/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/build_w32vc.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/build_w32vc.bat.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/install
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/install.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/makelinks
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/makelinks.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/test.sh.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/zip_src.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/script/zip_src.bat.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/test.sh.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 00:27:25.258997 typecode-30.0.1/tests/data/filetest/text/
+-rw-r--r--   0 runner    (1001) docker     (122)    18691 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/COPYING
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/COPYING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    82295 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/CREDITS.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)    76402 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/ChangeLog.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    17982 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/GPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/GPL.txt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/crashing-a.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/crashing-a.txt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/crashing-z.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/crashing-z.txt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    65454 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/windowserver.log
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/windowserver.log.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1355 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/x11-xconsortium_text.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/data/filetest/text/x11-xconsortium_text.txt.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8771 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/filetype_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16586 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3898 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_extractible.py
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_magic2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-23 00:27:12.000000 typecode-30.0.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-05-23 00:27:12.000000 typecode-30.0.1/typecode.ABOUT
```

### Comparing `typecode-30.0.0/.github/workflows/docs-ci.yml` & `typecode-30.0.1/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/.gitignore` & `typecode-30.0.1/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Python compiled files
 *.py[cod]
 
 # virtualenv and other misc bits
+/src/*.egg-info
 *.egg-info
 /dist
 /build
 /bin
 /lib
 /scripts
 /Scripts
```

### Comparing `typecode-30.0.0/CHANGELOG.rst` & `typecode-30.0.1/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Release notes
 =============
 
+Version 30.0.1
+-----------------
+
+- Upgrade skeleton
+- Fix ctypes import
+- Bump dependencies
+
+
 Version 30.0.0
 -----------------
 
 - Drop Calver
 - Fix minor bugs
 - Upgrade dependencies
 - Adopt black style
```

### Comparing `typecode-30.0.0/CODE_OF_CONDUCT.rst` & `typecode-30.0.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/PKG-INFO` & `typecode-30.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: typecode
-Version: 30.0.0
+Version: 30.0.1
 Summary: Comprehensive filetype and mimetype detection using libmagic and Pygments.
 Home-page: https://github.com/nexB/typecode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,filetype,mimetype,libmagic,scancode-toolkit,typecode,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: apache-2.0.LICENSE
 License-File: NOTICE
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
+License-File: CODE_OF_CONDUCT.rst
 
 ========
 TypeCode
 ========
 
 - license: Apache-2.0
 - copyright: copyright (c) nexB. Inc. and others
@@ -106,9 +106,7 @@
 
   - Update the version of pygments in ``pyproject.toml``
   - Run ``vendy``
   - Update the src/typecpde/pygments_lexers_mapping.py
     and src/typecode/pygments_lexers.py scripts accordingly, including their
     ABOUT files
 
-
-
```

### Comparing `typecode-30.0.0/README.rst` & `typecode-30.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/apache-2.0.LICENSE` & `typecode-30.0.1/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/appveyor.yml` & `typecode-30.0.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/azure-pipelines.yml` & `typecode-30.0.1/azure-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -5,52 +5,52 @@
 # These jobs are using VMs with Azure-provided Python builds
 ################################################################################
 
 jobs:
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: ubuntu18_cpython
-          image_name: ubuntu-18.04
-          python_versions: ['3.6', '3.7', '3.8', '3.9', '3.10']
+          job_name: ubuntu20_cpython
+          image_name: ubuntu-20.04
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: ubuntu20_cpython
-          image_name: ubuntu-20.04
-          python_versions: ['3.6', '3.7', '3.8', '3.9', '3.10']
+          job_name: ubuntu22_cpython
+          image_name: ubuntu-22.04
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: macos1015_cpython
-          image_name: macos-10.15
-          python_versions: ['3.6', '3.7', '3.8', '3.9', '3.10']
+          job_name: macos11_cpython
+          image_name: macos-11
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-posix.yml
       parameters:
-          job_name: macos11_cpython
-          image_name: macos-11
-          python_versions: ['3.7', '3.8', '3.9', '3.10']
+          job_name: macos12_cpython
+          image_name: macos-12
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv/bin/pytest -n 2 -vvs
 
     - template: etc/ci/azure-win.yml
       parameters:
           job_name: win2019_cpython
           image_name: windows-2019
-          python_versions: ['3.6', '3.7', '3.8', '3.9', '3.10']
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv\Scripts\pytest -n 2 -vvs
 
     - template: etc/ci/azure-win.yml
       parameters:
           job_name: win2022_cpython
           image_name: windows-2022
-          python_versions: ['3.7', '3.8', '3.9', '3.10']
+          python_versions: ['3.7', '3.8', '3.9', '3.10', '3.11']
           test_suites:
               all: venv\Scripts\pytest -n 2 -vvs
```

### Comparing `typecode-30.0.0/configure` & `typecode-30.0.1/configure`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 DEV_REQUIREMENTS="--editable .[full,testing] --constraint requirements.txt --constraint requirements-dev.txt"
 DOCS_REQUIREMENTS="--editable .[docs] --constraint requirements.txt"
 
 # where we create a virtualenv
 VIRTUALENV_DIR=venv
 
 # Cleanable files and directories to delete with the --clean option
-CLEANABLE="build venv"
+CLEANABLE="build dist venv .cache .eggs"
 
 # extra  arguments passed to pip
 PIP_EXTRA_ARGS=" "
 
 # the URL to download virtualenv.pyz if needed
 VIRTUALENV_PYZ_URL=https://bootstrap.pypa.io/virtualenv.pyz
 ################################
@@ -49,20 +49,27 @@
 ################################
 # Current directory where this script lives
 CFG_ROOT_DIR="$( cd "$( dirname "${BASH_SOURCE[0]}" )" && pwd )"
 CFG_BIN_DIR=$CFG_ROOT_DIR/$VIRTUALENV_DIR/bin
 
 
 ################################
+# Install with or without and index. With "--no-index" this is using only local wheels
+# This is an offline mode with no index and no network operations
+# NO_INDEX="--no-index "
+NO_INDEX=""
+
+
+################################
 # Thirdparty package locations and index handling
-# Find packages from the local thirdparty directory or from thirdparty.aboutcode.org
-if [ -d "$CFG_ROOT_DIR/thirdparty" ]; then
-    PIP_EXTRA_ARGS="--find-links $CFG_ROOT_DIR/thirdparty"
+# Find packages from the local thirdparty directory if present
+THIRDPARDIR=$CFG_ROOT_DIR/thirdparty
+if [[ "$(echo $THIRDPARDIR/*.whl)x" != "$THIRDPARDIR/*.whlx" ]]; then
+    PIP_EXTRA_ARGS="$NO_INDEX --find-links $THIRDPARDIR"
 fi
-PIP_EXTRA_ARGS="$PIP_EXTRA_ARGS --find-links https://thirdparty.aboutcode.org/pypi/simple/links.html"
 
 
 ################################
 # Set the quiet flag to empty if not defined
 if [[ "$CFG_QUIET" == "" ]]; then
     CFG_QUIET=" "
 fi
@@ -179,14 +186,15 @@
                 clean ) find_python && clean;;
                 dev   ) CFG_REQUIREMENTS="$DEV_REQUIREMENTS";;
                 docs   ) CFG_REQUIREMENTS="$DOCS_REQUIREMENTS";;
             esac;;
     esac
 done
 
+
 PIP_EXTRA_ARGS="$PIP_EXTRA_ARGS"
 
 find_python
 create_virtualenv "$VIRTUALENV_DIR"
 install_packages "$CFG_REQUIREMENTS"
 . "$CFG_BIN_DIR/activate"
```

### Comparing `typecode-30.0.0/configure.bat` & `typecode-30.0.1/configure.bat`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 set "DEV_REQUIREMENTS=--editable .[full,testing] --constraint requirements.txt --constraint requirements-dev.txt"
 set "DOCS_REQUIREMENTS=--editable .[docs] --constraint requirements.txt"
 
 @rem # where we create a virtualenv
 set "VIRTUALENV_DIR=venv"
 
 @rem # Cleanable files and directories to delete with the --clean option
-set "CLEANABLE=build venv"
+set "CLEANABLE=build dist venv .cache .eggs"
 
 @rem # extra  arguments passed to pip
 set "PIP_EXTRA_ARGS= "
 
 @rem # the URL to download virtualenv.pyz if needed
 set VIRTUALENV_PYZ_URL=https://bootstrap.pypa.io/virtualenv.pyz
 @rem ################################
@@ -48,32 +48,30 @@
 @rem # Current directory where this script lives
 set CFG_ROOT_DIR=%~dp0
 set "CFG_BIN_DIR=%CFG_ROOT_DIR%\%VIRTUALENV_DIR%\Scripts"
 
 
 @rem ################################
 @rem # Thirdparty package locations and index handling
-@rem # Find packages from the local thirdparty directory or from thirdparty.aboutcode.org
+@rem # Find packages from the local thirdparty directory
 if exist "%CFG_ROOT_DIR%\thirdparty" (
     set PIP_EXTRA_ARGS=--find-links "%CFG_ROOT_DIR%\thirdparty"
 )
-set "PIP_EXTRA_ARGS=%PIP_EXTRA_ARGS% --find-links https://thirdparty.aboutcode.org/pypi/simple/links.html"
 
 
 @rem ################################
 @rem # Set the quiet flag to empty if not defined
 if not defined CFG_QUIET (
     set "CFG_QUIET= "
 )
 
 
 @rem ################################
 @rem # Main command line entry point
 set "CFG_REQUIREMENTS=%REQUIREMENTS%"
-set "NO_INDEX=--no-index"
 
 :again
 if not "%1" == "" (
     if "%1" EQU "--help"   (goto cli_help)
     if "%1" EQU "--clean"  (goto clean)
     if "%1" EQU "--dev"    (
         set "CFG_REQUIREMENTS=%DEV_REQUIREMENTS%"
```

### Comparing `typecode-30.0.0/docs/Makefile` & `typecode-30.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/docs/make.bat` & `typecode-30.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/docs/source/_static/theme_overrides.css` & `typecode-30.0.1/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/docs/source/conf.py` & `typecode-30.0.1/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-'sphinx.ext.intersphinx',
+    "sphinx.ext.intersphinx",
 ]
 
 # This points to aboutcode.readthedocs.io
 # In case of "undefined label" ERRORS check docs on intersphinx to troubleshoot
 # Link was created at commit - https://github.com/nexB/aboutcode/commit/faea9fcf3248f8f198844fe34d43833224ac4a83
 
 intersphinx_mapping = {
-    'aboutcode': ('https://aboutcode.readthedocs.io/en/latest/', None),
-    'scancode-workbench': ('https://scancode-workbench.readthedocs.io/en/develop/', None),
+    "aboutcode": ("https://aboutcode.readthedocs.io/en/latest/", None),
+    "scancode-workbench": ("https://scancode-workbench.readthedocs.io/en/develop/", None),
 }
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
@@ -58,27 +58,25 @@
 html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
-master_doc = 'index'
+master_doc = "index"
 
 html_context = {
     "display_github": True,
     "github_user": "nexB",
     "github_repo": "nexb-skeleton",
     "github_version": "develop",  # branch
     "conf_py_path": "/docs/source/",  # path in the checkout to the docs root
 }
 
-html_css_files = [
-    '_static/theme_overrides.css'
-    ]
+html_css_files = ["_static/theme_overrides.css"]
 
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
 html_show_sphinx = True
 
 # Define CSS and HTML abbreviations used in .rst files.  These are examples.
 # .. role:: is used to refer to styles defined in _static/theme_overrides.css and is used like this: :red:`text`
```

### Comparing `typecode-30.0.0/docs/source/contribute/contrib_doc.rst` & `typecode-30.0.1/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/docs/source/skeleton-usage.rst` & `typecode-30.0.1/docs/source/skeleton-usage.rst`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/azure-container-deb.yml` & `typecode-30.0.1/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/azure-container-rpm.yml` & `typecode-30.0.1/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/azure-posix.yml` & `typecode-30.0.1/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/azure-win.yml` & `typecode-30.0.1/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/macports-ci` & `typecode-30.0.1/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/macports-ci.ABOUT` & `typecode-30.0.1/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/ci/mit.LICENSE` & `typecode-30.0.1/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/README.rst` & `typecode-30.0.1/etc/scripts/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,28 @@
     virtualenv as instructed below (This is to avoid injecting requirements
     specific to the tools used here in the main requirements).
 
   * For other usages, the tools here can run either in their own isolated
     virtualenv or in the the main configured development virtualenv.
     These requireements need to be installed::
 
-        pip install --requirement etc/release/requirements.txt
+        pip install --requirement etc/scripts/requirements.txt
 
 TODO: we need to pin the versions of these tools
 
 
 
 Generate or update pip requirement files
 ----------------------------------------
 
 Scripts
 ~~~~~~~
 
 **gen_requirements.py**: create/update requirements files from currently
-  installed requirements. 
+  installed requirements.
 
 **gen_requirements_dev.py** does the same but can subtract the main requirements
   to get extra requirements used in only development.
 
 
 Usage
 ~~~~~
@@ -46,24 +46,24 @@
 The sequence of commands to run are:
 
 
 * Start with these to generate the main pip requirements file::
 
     ./configure --clean
     ./configure
-    python etc/release/gen_requirements.py --site-packages-dir <path to site-packages dir>
+    python etc/scripts/gen_requirements.py --site-packages-dir <path to site-packages dir>
 
 * You can optionally install or update extra main requirements after the
   ./configure step such that these are included in the generated main requirements.
 
 * Optionally, generate a development pip requirements file by running these::
 
     ./configure --clean
     ./configure --dev
-    python etc/release/gen_requirements_dev.py --site-packages-dir <path to site-packages dir>
+    python etc/scripts/gen_requirements_dev.py --site-packages-dir <path to site-packages dir>
 
 * You can optionally install or update extra dev requirements after the
   ./configure step such that these are included in the generated dev
   requirements.
 
 Notes: we generate development requirements after the main as this step requires
 the main requirements.txt to be up-to-date first. See **gen_requirements.py and
```

### Comparing `typecode-30.0.0/etc/scripts/check_thirdparty.py` & `typecode-30.0.1/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/fetch_thirdparty.py` & `typecode-30.0.1/etc/scripts/fetch_thirdparty.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # See https://github.com/nexB/skeleton for support or download.
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
 
 import itertools
 import os
 import sys
+from collections import defaultdict
 
 import click
 
 import utils_thirdparty
 import utils_requirements
 
 TRACE = False
@@ -106,27 +107,62 @@
     help="PyPI index URL(s) to use for wheels and sources, in order of preferences.",
 )
 @click.option(
     "--use-cached-index",
     is_flag=True,
     help="Use on disk cached PyPI indexes list of packages and versions and do not refetch if present.",
 )
-
+@click.option(
+    "--sdist-only",
+    "sdist_only",
+    type=str,
+    metavar="SDIST",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that come only in sdist format (no wheels). "
+         "The command will not fail and exit if no wheel exists for these names",
+)
+@click.option(
+    "--wheel-only",
+    "wheel_only",
+    type=str,
+    metavar="WHEEL",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that come only in wheel format (no sdist). "
+         "The command will not fail and exit if no sdist exists for these names",
+)
+@click.option(
+    "--no-dist",
+    "no_dist",
+    type=str,
+    metavar="DIST",
+    default=tuple(),
+    show_default=False,
+    multiple=True,
+    help="Package name(s) that do not come either in wheel or sdist format. "
+         "The command will not fail and exit if no distribution exists for these names",
+)
 @click.help_option("-h", "--help")
 def fetch_thirdparty(
     requirements_files,
     specifiers,
     latest_version,
     dest_dir,
     python_versions,
     operating_systems,
     wheels,
     sdists,
     index_urls,
     use_cached_index,
+    sdist_only,
+    wheel_only,
+    no_dist,
 ):
     """
     Download to --dest THIRDPARTY_DIR the PyPI wheels, source distributions,
     and their ABOUT metadata, license and notices files.
 
     Download the PyPI packages listed in the combination of:
     - the pip requirements --requirements REQUIREMENT-FILE(s),
@@ -201,66 +237,70 @@
         else:
             repo = utils_thirdparty.PypiSimpleRepository(
                 index_url=index_url,
                 use_cached_index=use_cached_index,
             )
             repos.append(repo)
 
-    wheels_fetched = []
-    wheels_not_found = []
-
-    sdists_fetched = []
-    sdists_not_found = []
+    wheels_or_sdist_not_found = defaultdict(list)
 
     for name, version in sorted(required_name_versions):
         nv = name, version
         print(f"Processing: {name} @ {version}")
         if wheels:
             for environment in environments:
+
                 if TRACE:
                     print(f"  ==> Fetching wheel for envt: {environment}")
-                fwfns = utils_thirdparty.download_wheel(
+
+                fetched = utils_thirdparty.download_wheel(
                     name=name,
                     version=version,
                     environment=environment,
                     dest_dir=dest_dir,
                     repos=repos,
                 )
-                if fwfns:
-                    wheels_fetched.extend(fwfns)
-                else:
-                    wheels_not_found.append(f"{name}=={version} for: {environment}")
+                if not fetched:
+                    wheels_or_sdist_not_found[f"{name}=={version}"].append(environment)
                     if TRACE:
                         print(f"      NOT FOUND")
 
-        if sdists:
+        if (sdists or
+            (f"{name}=={version}" in wheels_or_sdist_not_found and name in sdist_only)
+         ):
             if TRACE:
                 print(f"  ==> Fetching sdist: {name}=={version}")
+
             fetched = utils_thirdparty.download_sdist(
                 name=name,
                 version=version,
                 dest_dir=dest_dir,
                 repos=repos,
             )
-            if fetched:
-                sdists_fetched.append(fetched)
-            else:
-                sdists_not_found.append(f"{name}=={version}")
+            if not fetched:
+                wheels_or_sdist_not_found[f"{name}=={version}"].append("sdist")
                 if TRACE:
                     print(f"      NOT FOUND")
 
-    if wheels and wheels_not_found:
-        print(f"==> MISSING WHEELS")
-        for wh in wheels_not_found:
-            print(f"  {wh}")
-
-    if sdists and sdists_not_found:
-        print(f"==> MISSING SDISTS")
-        for sd in sdists_not_found:
-            print(f"  {sd}")
+    mia = []
+    for nv, dists in wheels_or_sdist_not_found.items():
+        name, _, version = nv.partition("==")
+        if name in no_dist:
+            continue
+        sdist_missing = sdists and "sdist" in dists and not name in wheel_only
+        if sdist_missing:
+            mia.append(f"SDist missing: {nv} {dists}")
+        wheels_missing = wheels and any(d for d in dists if d != "sdist") and not name in sdist_only
+        if wheels_missing:
+            mia.append(f"Wheels missing: {nv} {dists}")
+
+    if mia:
+        for m in mia:
+            print(m)
+        raise Exception(mia)
 
     print(f"==> FETCHING OR CREATING ABOUT AND LICENSE FILES")
     utils_thirdparty.fetch_abouts_and_licenses(dest_dir=dest_dir, use_cached_index=use_cached_index)
     utils_thirdparty.clean_about_files(dest_dir=dest_dir)
 
     # check for problems
     print(f"==> CHECK FOR PROBLEMS")
```

### Comparing `typecode-30.0.0/etc/scripts/gen_pypi_simple.py` & `typecode-30.0.1/etc/scripts/gen_pypi_simple.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,15 +114,15 @@
   <head>
     <meta name="pypi:repository-version" content="1.0">
     <title>Links for {pkg_name}</title>
   </head>
   <body>"""
     document.append(header)
 
-    for package in packages:
+    for package in sorted(packages, key=lambda p: p.archive_file):
         document.append(package.simple_index_entry(base_url))
 
     footer = """  </body>
 </html>
 """
     document.append(footer)
     return "\n".join(document)
@@ -137,16 +137,16 @@
 <html>
   <head>
     <title>Links for all packages</title>
   </head>
   <body>"""
     document.append(header)
 
-    for _name, packages in packages_by_package_name.items():
-        for package in packages:
+    for _name, packages in sorted(packages_by_package_name.items(), key=lambda i: i[0]):
+        for package in sorted(packages, key=lambda p: p.archive_file):
             document.append(package.simple_index_entry(base_url))
 
     footer = """  </body>
 </html>
 """
     document.append(footer)
     return "\n".join(document)
```

### Comparing `typecode-30.0.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `typecode-30.0.1/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/gen_requirements.py` & `typecode-30.0.1/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/gen_requirements_dev.py` & `typecode-30.0.1/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `typecode-30.0.1/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/test_utils_pypi_supported_tags.py` & `typecode-30.0.1/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `typecode-30.0.1/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/utils_dejacode.py` & `typecode-30.0.1/etc/scripts/utils_dejacode.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import io
 import os
 import zipfile
 
 import requests
 import saneyaml
 
-from packaging import version as packaging_version
+from packvers import version as packaging_version
 
 """
 Utility to create and retrieve package and ABOUT file data from DejaCode.
 """
 
 DEJACODE_API_KEY = os.environ.get("DEJACODE_API_KEY", "")
 DEJACODE_API_URL = os.environ.get("DEJACODE_API_URL", "")
```

### Comparing `typecode-30.0.0/etc/scripts/utils_pip_compatibility_tags.py` & `typecode-30.0.1/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
 WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 import re
 
-from packaging.tags import (
+from packvers.tags import (
     compatible_tags,
     cpython_tags,
     generic_tags,
     interpreter_name,
     interpreter_version,
     mac_platforms,
 )
```

### Comparing `typecode-30.0.0/etc/scripts/utils_pypi_supported_tags.py` & `typecode-30.0.1/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `typecode-30.0.1/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/etc/scripts/utils_requirements.py` & `typecode-30.0.1/etc/scripts/utils_requirements.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Copyright (c) nexB Inc. and others. All rights reserved.
 # ScanCode is a trademark of nexB Inc.
 # SPDX-License-Identifier: Apache-2.0
 # See http://www.apache.org/licenses/LICENSE-2.0 for the license text.
 # See https://github.com/nexB/skeleton for support or download.
 # See https://aboutcode.org for more information about nexB OSS projects.
 #
+
+import os
 import re
 import subprocess
 
 """
 Utilities to manage requirements files and call pip.
 NOTE: this should use ONLY the standard library and not import anything else
 because this is used for boostrapping with no requirements installed.
```

### Comparing `typecode-30.0.0/etc/scripts/utils_thirdparty.py` & `typecode-30.0.1/etc/scripts/utils_thirdparty.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 import license_expression
 import packageurl
 import requests
 import saneyaml
 from commoncode import fileutils
 from commoncode.hash import multi_checksums
 from commoncode.text import python_safe_name
-from packaging import tags as packaging_tags
-from packaging import version as packaging_version
+from packvers import tags as packaging_tags
+from packvers import version as packaging_version
 
 import utils_pip_compatibility_tags
 
 """
 Utilities to manage Python thirparty libraries source, binaries and metadata in
 local directories and remote repositories.
 
@@ -111,18 +111,17 @@
 """
 
 TRACE = False
 TRACE_DEEP = False
 TRACE_ULTRA_DEEP = False
 
 # Supported environments
-PYTHON_VERSIONS = "36", "37", "38", "39", "310"
+PYTHON_VERSIONS = "37", "38", "39", "310"
 
 PYTHON_DOT_VERSIONS_BY_VER = {
-    "36": "3.6",
     "37": "3.7",
     "38": "3.8",
     "39": "3.9",
     "310": "3.10",
 }
 
 
@@ -130,15 +129,14 @@
     """
     Return a dot version from a plain, non-dot version.
     """
     return PYTHON_DOT_VERSIONS_BY_VER[version]
 
 
 ABIS_BY_PYTHON_VERSION = {
-    "36": ["cp36", "cp36m", "abi3"],
     "37": ["cp37", "cp37m", "abi3"],
     "38": ["cp38", "cp38m", "abi3"],
     "39": ["cp39", "cp39m", "abi3"],
     "310": ["cp310", "cp310m", "abi3"],
 }
 
 PLATFORMS_BY_OS = {
@@ -307,14 +305,15 @@
 
         if fetched_sdist_filename:
             # do not futher fetch from other repos if we find in first, typically PyPI
             break
 
     return fetched_sdist_filename
 
+
 ################################################################################
 #
 # Core models
 #
 ################################################################################
 
 
@@ -907,15 +906,15 @@
         raw_data = email.message_from_string(pkginfo_text)
 
         classifiers = raw_data.get_all("Classifier") or []
 
         declared_license = [raw_data["License"]] + [
             c for c in classifiers if c.startswith("License")
         ]
-        license_expression = compute_normalized_license_expression(declared_license)
+        license_expression = get_license_expression(declared_license)
         other_classifiers = [c for c in classifiers if not c.startswith("License")]
 
         holder = raw_data["Author"]
         holder_contact = raw_data["Author-email"]
         copyright_statement = f"Copyright (c) {holder} <{holder_contact}>"
 
         pkginfo_data = dict(
@@ -1060,24 +1059,24 @@
     ):
         return False
 
     # all char versions
     if version.isalpha():
         return False
 
-    # non-pep 440 version    
+    # non-pep 440 version
     if "-" in version:
         return False
 
-    # single version    
+    # single version
     if version.isdigit() and len(version) == 1:
         return False
 
-    # r1 version    
-    if len(version) == 2 and version[0]=="r" and version[1].isdigit():
+    # r1 version
+    if len(version) == 2 and version[0] == "r" and version[1].isdigit():
         return False
 
     # dotless version (but calver is OK)
     if "." not in version and len(version) < 3:
         return False
 
     # version with dashes selenium-2.0-dev-9429.tar.gz
@@ -1332,18 +1331,18 @@
     def package_from_dists(cls, dists):
         """
         Return a new PypiPackage built from an iterable of Wheels and Sdist
         objects all for the same package name and version.
 
         For example:
         >>> w1 = Wheel(name='bitarray', version='0.8.1', build='',
-        ...    python_versions=['cp36'], abis=['cp36m'],
+        ...    python_versions=['cp38'], abis=['cp38m'],
         ...    platforms=['linux_x86_64'])
         >>> w2 = Wheel(name='bitarray', version='0.8.1', build='',
-        ...    python_versions=['cp36'], abis=['cp36m'],
+        ...    python_versions=['cp38'], abis=['cp38m'],
         ...    platforms=['macosx_10_9_x86_64', 'macosx_10_10_x86_64'])
         >>> sd = Sdist(name='bitarray', version='0.8.1')
         >>> package = PypiPackage.package_from_dists(dists=[w1, w2, sd])
         >>> assert package.name == 'bitarray'
         >>> assert package.version == '0.8.1'
         >>> assert package.sdist == sd
         >>> assert package.wheels == [w1, w2]
@@ -1584,14 +1583,15 @@
                 version=self.python_version or None,
                 impl=self.implementation or None,
                 platforms=self.platforms or None,
                 abis=self.abis or None,
             )
         )
 
+
 ################################################################################
 #
 # PyPI repo and link index for package wheels and sources
 #
 ################################################################################
 
 
@@ -1625,15 +1625,17 @@
         default=attr.Factory(set),
         metadata=dict(help="A set of already fetched package normalized names."),
     )
 
     use_cached_index = attr.ib(
         type=bool,
         default=False,
-        metadata=dict(help="If True, use any existing on-disk cached PyPI index files. Otherwise, fetch and cache."),
+        metadata=dict(
+            help="If True, use any existing on-disk cached PyPI index files. Otherwise, fetch and cache."
+        ),
     )
 
     def _get_package_versions_map(self, name):
         """
         Return a mapping of all available PypiPackage version for this package name.
         The mapping may be empty. It is ordered by version from oldest to newest
         """
@@ -1670,14 +1672,15 @@
     def get_package_version(self, name, version=None):
         """
         Return the PypiPackage with name and version or None.
         Return the latest PypiPackage version if version is None.
         """
         if not version:
             versions = list(self._get_package_versions_map(name).values())
+            # return the latest version
             return versions and versions[-1]
         else:
             return self._get_package_versions_map(name).get(version)
 
     def fetch_links(self, normalized_name):
         """
         Return a list of download link URLs found in a PyPI simple index for package
@@ -1720,15 +1723,17 @@
         default=attr.Factory(list),
         metadata=dict(help="List of links available in this repo"),
     )
 
     use_cached_index = attr.ib(
         type=bool,
         default=False,
-        metadata=dict(help="If True, use any existing on-disk cached index files. Otherwise, fetch and cache."),
+        metadata=dict(
+            help="If True, use any existing on-disk cached index files. Otherwise, fetch and cache."
+        ),
     )
 
     def __attrs_post_init__(self):
         if not self.links:
             self.links = self.find_links()
 
     def find_links(self, _CACHE=[]):
@@ -1786,27 +1791,29 @@
 
     @classmethod
     def from_url(cls, url=ABOUT_BASE_URL, _LINKS_REPO={}, use_cached_index=False):
         if url not in _LINKS_REPO:
             _LINKS_REPO[url] = cls(url=url, use_cached_index=use_cached_index)
         return _LINKS_REPO[url]
 
+
 ################################################################################
 # Globals for remote repos to be lazily created and cached on first use for the
 # life of the session together with some convenience functions.
 ################################################################################
 
 
 def get_local_packages(directory=THIRDPARTY_DIR):
     """
     Return the list of all PypiPackage objects built from a local directory. Return
     an empty list if the package cannot be found.
     """
     return list(PypiPackage.packages_from_dir(directory=directory))
 
+
 ################################################################################
 #
 # Basic file and URL-based operations using a persistent file-based Cache
 #
 ################################################################################
 
 
@@ -1949,14 +1956,15 @@
     )
     output = os.path.join(dest_dir, filename)
     wmode = "w" if as_text else "wb"
     with open(output, wmode) as fo:
         fo.write(content)
     return content
 
+
 ################################################################################
 #
 # Functions to update or fetch ABOUT and license files
 #
 ################################################################################
 
 
@@ -2047,15 +2055,17 @@
                         # if has key data we may look to improve later, but we can move on
                         if local_dist.has_key_metadata():
                             break
 
                 # if has key data we may look to improve later, but we can move on
                 if local_dist.has_key_metadata():
                     local_dist.save_about_and_notice_files(dest_dir=dest_dir)
-                    local_dist.fetch_license_files(dest_dir=dest_dir, use_cached_index=use_cached_index)
+                    local_dist.fetch_license_files(
+                        dest_dir=dest_dir, use_cached_index=use_cached_index
+                    )
                     continue
 
             # lets try to fetch remotely
             local_dist.load_remote_about_data()
 
             # if has key data we may look to improve later, but we can move on
             if local_dist.has_key_metadata():
@@ -2085,15 +2095,17 @@
                         # if has key data we may look to improve later, but we can move on
                         if local_dist.has_key_metadata():
                             break
 
                 # if has key data we may look to improve later, but we can move on
                 if local_dist.has_key_metadata():
                     local_dist.save_about_and_notice_files(dest_dir=dest_dir)
-                    local_dist.fetch_license_files(dest_dir=dest_dir, use_cached_index=use_cached_index)
+                    local_dist.fetch_license_files(
+                        dest_dir=dest_dir, use_cached_index=use_cached_index
+                    )
                     continue
 
             # try to get data from pkginfo (no license though)
             local_dist.load_pkginfo_data(dest_dir=dest_dir)
 
             # FIXME: save as this is the last resort for now in all cases
             # if local_dist.has_key_metadata() or not local_dist.has_key_metadata():
@@ -2103,14 +2115,15 @@
 
             if not local_dist.has_key_metadata():
                 print(f"Unable to add essential ABOUT data for: {local_dist}")
             if lic_errs:
                 lic_errs = "\n".join(lic_errs)
                 print(f"Failed to fetch some licenses:: {lic_errs}")
 
+
 ################################################################################
 #
 # Functions to build new Python wheels including native on multiple OSes
 #
 ################################################################################
 
 
@@ -2206,14 +2219,15 @@
         print(error)
         print()
         print("###########################################################################")
 
     downloaded = existing ^ set(os.listdir(dest_dir))
     return sorted(downloaded), error
 
+
 ################################################################################
 #
 # Functions to check for problems
 #
 ################################################################################
 
 
@@ -2254,21 +2268,21 @@
                 print(f"   Invalid checksums in file://{abpth}")
             if not dist.sha1 and dist.md5:
                 print(f"   Missing checksums in file://{abpth}")
 
     check_about(dest_dir=dest_dir)
 
 
-def compute_normalized_license_expression(declared_licenses):
+def get_license_expression(declared_licenses):
     """
     Return a normalized license expression or None.
     """
     if not declared_licenses:
         return
     try:
-        from packagedcode import pypi
+        from packagedcode.licensing import get_only_expression_from_extracted_license
 
-        return pypi.compute_normalized_license(declared_licenses)
+        return get_only_expression_from_extracted_license(declared_licenses)
     except ImportError:
         # Scancode is not installed, clean and join all the licenses
         lics = [python_safe_name(l).lower() for l in declared_licenses]
         return " AND ".join(lics).lower()
```

### Comparing `typecode-30.0.0/etc/scripts/utils_thirdparty.py.ABOUT` & `typecode-30.0.1/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/pyproject.toml` & `typecode-30.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/requirements.txt` & `typecode-30.0.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 commoncode==30.2.0
 construct==2.10.68
 container-inspector==31.0.0
 cryptography==36.0.2
 debian-inspector==30.0.0
 dockerfile-parse==1.2.0
 dparse2==0.6.1
-extractcode==30.0.0
+extractcode==31.0.0
 extractcode-7z==16.5.210531
 extractcode-libarchive==3.5.1.210531
 fasteners==0.17.3
 fingerprints==1.0.3
 ftfy==6.0.3
 future==0.18.2
 gemfileparser==0.8.0
 html5lib==1.1
 idna==3.3
 importlib-metadata==4.8.3
 inflection==0.5.1
-intbitset==3.0.1
+intbitset==3.0.2
 isodate==0.6.1
 jaraco.functools==3.4.0
 javaproperties==0.8.1
 Jinja2==3.0.3
 jsonstreams==0.6.0
 license-expression==21.6.14
 lxml==4.8.0
@@ -40,15 +40,15 @@
 more-itertools==8.13.0
 normality==2.3.3
 packagedcode-msitools==0.101.210706
 packageurl-python==0.9.9
 packaging==21.3
 parameter-expansion-patched==0.3.1
 patch==1.16
-pdfminer.six==20220506
+pdfminer-six==20220506
 pefile==2021.9.3
 pip-requirements-parser==31.2.0
 pkginfo2==30.0.0
 pluggy==1.0.0
 plugincode==30.0.0
 ply==3.11
 publicsuffix2==2.20191221
@@ -57,15 +57,15 @@
 pygmars==0.7.0
 Pygments==2.12.0
 pymaven-patch==0.3.0
 pyparsing==3.0.8
 pytz==2022.1
 PyYAML==6.0
 rdflib==5.0.0
-regipy==2.2.2
+regipy==2.3.1
 requests==2.27.1
 rpm-inspector-rpm==4.16.1.3.210404
 saneyaml==0.5.2
 six==1.16.0
 soupsieve==2.3.1
 spdx-tools==0.7.0a3
 text-unidecode==1.3
```

### Comparing `typecode-30.0.0/setup.cfg` & `typecode-30.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = typecode
+version = 30.0.1
 license = Apache-2.0
 description = Comprehensive filetype and mimetype detection using libmagic and Pygments.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/nexB/typecode
 author = nexB. Inc. and others
 author_email = info@aboutcode.org
@@ -28,23 +29,24 @@
 	typecode
 	utilities
 license_files = 
 	apache-2.0.LICENSE
 	NOTICE
 	AUTHORS.rst
 	CHANGELOG.rst
+	CODE_OF_CONDUCT.rst
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
 zip_safe = false
 setup_requires = setuptools_scm[toml] >= 4
-python_requires = >=3.6.*
+python_requires = >=3.7
 install_requires = 
 	attrs >= 18.1, !=20.1.0
 	binaryornot
 	commoncode >= 30.2.0
 	pdfminer.six >= 20200101
 	plugincode >= 30.0.0
 
@@ -53,21 +55,24 @@
 
 [options.extras_require]
 full = 
 	typecode_libmagic >= 5.39.210223
 testing = 
 	pytest >= 6, != 7.0.0
 	pytest-xdist >= 2
-	aboutcode-toolkit >= 6.0.0
+	aboutcode-toolkit >= 8.0.0
+	pycodestyle >= 2.8.0
+	twine
 	black
 	twine
 	saneyaml
 	vendy
+	isort
 docs = 
-	Sphinx >= 3.3.1
+	Sphinx == 6.2.1
 	sphinx-rtd-theme >= 0.5.0
 	doc8 >= 0.8.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `typecode-30.0.0/src/typecode/__init__.py` & `typecode-30.0.1/src/typecode/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/apache-2.0.LICENSE` & `typecode-30.0.1/src/typecode/_vendor/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/bsd-new.LICENSE` & `typecode-30.0.1/src/typecode/_vendor/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/LICENSE` & `typecode-30.0.1/src/typecode/_vendor/pygments/LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/__init__.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/cmdline.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/console.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/filter.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/filters/__init__.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatter.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/__init__.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/_mapping.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/bbcode.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/html.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/img.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/irc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/latex.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/other.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/rtf.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/svg.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/terminal.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/formatters/terminal256.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexer.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/__init__.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_asy_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_cl_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_cocoa_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_csound_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_lasso_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_lua_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mapping.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mql_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_mysql_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_openedge_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_php_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_postgres_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_scilab_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_sourcemod_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_stan_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_stata_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_tsql_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_usd_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_vbscript_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/_vim_builtins.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/actionscript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/agile.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/algebra.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ambient.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ampl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/apl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/archetype.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/arrow.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/asm.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/automation.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/bare.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/basic.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/bibtex.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/boa.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/business.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/c_cpp.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/c_like.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/capnproto.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/chapel.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/clean.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/compiled.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/configs.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/console.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/crystal.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/csound.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/css.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/d.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dalvik.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/data.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/devicetree.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/diff.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dotnet.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dsls.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/dylan.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ecl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/eiffel.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/elm.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/email.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/erlang.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/esoteric.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ezhil.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/factor.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/fantom.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/felix.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/floscript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/forth.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/fortran.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/foxpro.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/freefem.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/functional.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/gdscript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/go.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/grammar_notation.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/graph.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/graphics.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/haskell.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/haxe.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/hdl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/hexdump.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/html.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/idl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/igor.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/inferno.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/installers.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/int_fiction.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/iolang.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/j.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/javascript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/julia.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/jvm.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/lisp.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/make.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/markup.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/math.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/matlab.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/mime.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ml.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/modeling.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/modula2.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/monte.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/mosel.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ncl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nimrod.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nit.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/nix.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/oberon.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/objective.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ooc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/other.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/parasail.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/parsers.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pascal.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pawn.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/perl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/php.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pointless.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/pony.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/praat.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/prolog.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/promql.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/python.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/qvt.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/r.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rdf.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rebol.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/resource.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ride.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rnc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/roboconf.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/robotframework.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/ruby.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/rust.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sas.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/scdoc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/scripting.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sgf.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/shell.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sieve.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/slash.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/smalltalk.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/smv.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/snobol.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/solidity.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/special.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/sql.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/stata.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/supercollider.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/tcl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/templates.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/teraterm.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/testing.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/text.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/textedit.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/textfmts.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/theorem.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/tnt.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/trafficscript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/typoscript.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/unicon.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/urbi.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/usd.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/varnish.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/verification.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/web.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/webidl.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/webmisc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/whiley.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/x10.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/xorg.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/yang.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/lexers/zig.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/modeline.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/plugin.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/regexopt.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/scanner.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/sphinxext.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/style.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/__init__.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/abap.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/algol.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/algol_nu.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/arduino.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/autumn.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/borland.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/bw.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/colorful.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/default.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/emacs.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/friendly.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/fruity.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/igor.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/inkpot.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/lovelace.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/manni.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/monokai.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/murphy.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/native.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/paraiso_dark.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/paraiso_light.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/pastie.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/perldoc.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/rainbow_dash.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/rrt.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/sas.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/solarized.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/stata_dark.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/stata_light.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/tango.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/trac.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/vim.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/vs.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/styles/xcode.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/token.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/unistring.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments/util.py` & `typecode-30.0.1/src/typecode/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments.ABOUT` & `typecode-30.0.1/src/typecode/_vendor/pygments.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/_vendor/pygments.NOTICE` & `typecode-30.0.1/src/typecode/_vendor/pygments.NOTICE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/apache-2.0.LICENSE` & `typecode-30.0.1/src/typecode/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/bsd-new.LICENSE` & `typecode-30.0.1/src/typecode/bsd-new.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/bsd-simplified.LICENSE` & `typecode-30.0.1/src/typecode/bsd-simplified.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/contenttype.py` & `typecode-30.0.1/src/typecode/contenttype.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/entropy.py` & `typecode-30.0.1/src/typecode/entropy.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/extractible.py` & `typecode-30.0.1/src/typecode/extractible.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/magic2.py` & `typecode-30.0.1/src/typecode/magic2.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import ctypes
+import ctypes.util
 import glob
 import os
 import sys
 import warnings
 
 from commoncode import command
 from commoncode.system import on_windows
```

### Comparing `typecode-30.0.0/src/typecode/mimetypes.py` & `typecode-30.0.1/src/typecode/mimetypes.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/mit.LICENSE` & `typecode-30.0.1/src/typecode/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers.py` & `typecode-30.0.1/src/typecode/pygments_lexers.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers.py.ABOUT` & `typecode-30.0.1/src/typecode/pygments_lexers.py.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers.py.NOTICE` & `typecode-30.0.1/src/typecode/pygments_lexers.py.NOTICE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers_mapping.py` & `typecode-30.0.1/src/typecode/pygments_lexers_mapping.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers_mapping.py.ABOUT` & `typecode-30.0.1/src/typecode/pygments_lexers_mapping.py.ABOUT`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/pygments_lexers_mapping.py.NOTICE` & `typecode-30.0.1/src/typecode/pygments_lexers_mapping.py.NOTICE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode/python.LICENSE` & `typecode-30.0.1/src/typecode/python.LICENSE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/src/typecode.egg-info/PKG-INFO` & `typecode-30.0.1/src/typecode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: typecode
-Version: 30.0.0
+Version: 30.0.1
 Summary: Comprehensive filetype and mimetype detection using libmagic and Pygments.
 Home-page: https://github.com/nexB/typecode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: open source,filetype,mimetype,libmagic,scancode-toolkit,typecode,utilities
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.*
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: full
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: apache-2.0.LICENSE
 License-File: NOTICE
 License-File: AUTHORS.rst
 License-File: CHANGELOG.rst
+License-File: CODE_OF_CONDUCT.rst
 
 ========
 TypeCode
 ========
 
 - license: Apache-2.0
 - copyright: copyright (c) nexB. Inc. and others
@@ -106,9 +106,7 @@
 
   - Update the version of pygments in ``pyproject.toml``
   - Run ``vendy``
   - Update the src/typecpde/pygments_lexers_mapping.py
     and src/typecode/pygments_lexers.py scripts accordingly, including their
     ABOUT files
 
-
-
```

### Comparing `typecode-30.0.0/src/typecode.egg-info/SOURCES.txt` & `typecode-30.0.1/src/typecode.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitattributes
 .gitignore
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 MANIFEST.in
+Makefile
 NOTICE
 README.rst
 apache-2.0.LICENSE
 appveyor.yml
 azure-pipelines.yml
 configure
 configure.bat
@@ -698,9 +699,8 @@
 tests/data/filetest/text/crashing-a.txt
 tests/data/filetest/text/crashing-a.txt.yml
 tests/data/filetest/text/crashing-z.txt
 tests/data/filetest/text/crashing-z.txt.yml
 tests/data/filetest/text/windowserver.log
 tests/data/filetest/text/windowserver.log.yml
 tests/data/filetest/text/x11-xconsortium_text.txt
-tests/data/filetest/text/x11-xconsortium_text.txt.yml
-thirdparty/README.rst
+tests/data/filetest/text/x11-xconsortium_text.txt.yml
```

### Comparing `typecode-30.0.0/tests/data/contenttype/archive/crashing-squashfs` & `typecode-30.0.1/tests/data/contenttype/archive/crashing-squashfs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/archive/sqfs-gz.sqs` & `typecode-30.0.1/tests/data/contenttype/archive/sqfs-gz.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/archive/sqfs-lzo.sqs` & `typecode-30.0.1/tests/data/contenttype/archive/sqfs-lzo.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/archive/sqfs-xz.sqs` & `typecode-30.0.1/tests/data/contenttype/archive/sqfs-xz.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/certificate/CERTIFICATE` & `typecode-30.0.1/tests/data/contenttype/certificate/CERTIFICATE`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/code/c/c_code.c` & `typecode-30.0.1/tests/data/contenttype/code/c/c_code.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/code/c/some.c` & `typecode-30.0.1/tests/data/contenttype/code/c/some.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/code/python/extract.py` & `typecode-30.0.1/tests/data/contenttype/code/python/extract.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/compiled/java/CommonViewerSiteFactory.class` & `typecode-30.0.1/tests/data/contenttype/compiled/java/CommonViewerSiteFactory.class`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/compiled/java/old.class` & `typecode-30.0.1/tests/data/contenttype/compiled/java/old.class`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/compiled/linux/libnetsnmpagent.so.5` & `typecode-30.0.1/tests/data/contenttype/compiled/linux/libnetsnmpagent.so.5`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/compiled/linux/libssl.so.0.9.7` & `typecode-30.0.1/tests/data/contenttype/compiled/linux/libssl.so.0.9.7`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/compiled/python/compiled.zip` & `typecode-30.0.1/tests/data/contenttype/compiled/python/compiled.zip`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/doc/postscript/Image1.eps` & `typecode-30.0.1/tests/data/contenttype/doc/postscript/Image1.eps`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/package/libjama-dev_1.2.4-2_all.deb` & `typecode-30.0.1/tests/data/contenttype/package/libjama-dev_1.2.4-2_all.deb`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/package/package.json` & `typecode-30.0.1/tests/data/contenttype/package/package.json`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/package/wget-el_0.5.0-8_all.deb` & `typecode-30.0.1/tests/data/contenttype/package/wget-el_0.5.0-8_all.deb`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/text/wildtest.txt` & `typecode-30.0.1/tests/data/contenttype/text/wildtest.txt`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/unicode/unicode.zip` & `typecode-30.0.1/tests/data/contenttype/unicode/unicode.zip`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/contenttype/unicode/unicode2.zip` & `typecode-30.0.1/tests/data/contenttype/unicode/unicode2.zip`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/crashing-squashfs` & `typecode-30.0.1/tests/data/extractible/crashing-squashfs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/e.tar` & `typecode-30.0.1/tests/data/extractible/e.tar`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/file_4.26-1.diff.gz` & `typecode-30.0.1/tests/data/extractible/file_4.26-1.diff.gz`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/posixnotgnu.tar` & `typecode-30.0.1/tests/data/extractible/posixnotgnu.tar`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/sqfs-gz.sqs` & `typecode-30.0.1/tests/data/extractible/sqfs-gz.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/sqfs-lzo.sqs` & `typecode-30.0.1/tests/data/extractible/sqfs-lzo.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/sqfs-xz.sqs` & `typecode-30.0.1/tests/data/extractible/sqfs-xz.sqs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/test.tar.xz` & `typecode-30.0.1/tests/data/extractible/test.tar.xz`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/extractible/win-archive.lib` & `typecode-30.0.1/tests/data/extractible/win-archive.lib`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/archive/e.tar` & `typecode-30.0.1/tests/data/filetest/archive/e.tar`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/archive/file_4.26-1.diff.gz` & `typecode-30.0.1/tests/data/filetest/archive/file_4.26-1.diff.gz`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/archive/posixnotgnu.tar` & `typecode-30.0.1/tests/data/filetest/archive/posixnotgnu.tar`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/archive/test.tar.xz` & `typecode-30.0.1/tests/data/filetest/archive/test.tar.xz`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/archive/win-archive.lib` & `typecode-30.0.1/tests/data/filetest/archive/win-archive.lib`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary/pixelstream.rgb` & `typecode-30.0.1/tests/data/filetest/binary/pixelstream.rgb`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary/windows.dll` & `typecode-30.0.1/tests/data/filetest/binary/windows.dll`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_0` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_0`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_1` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_1`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_2` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_2`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_3` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_3`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_4` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_4`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_5` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_5`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_6` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_6`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_7` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_7`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/binary-random/binary_random_8` & `typecode-30.0.1/tests/data/filetest/binary-random/binary_random_8`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/Makefile.inc` & `typecode-30.0.1/tests/data/filetest/build/Makefile.inc`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/ar-ER.css.map` & `typecode-30.0.1/tests/data/filetest/build/ar-ER.css.map`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/ar-ER.js.map` & `typecode-30.0.1/tests/data/filetest/build/ar-ER.js.map`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/binary.js.map` & `typecode-30.0.1/tests/data/filetest/build/binary.js.map`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/build.xml` & `typecode-30.0.1/tests/data/filetest/build/build.xml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/documentation.dsp` & `typecode-30.0.1/tests/data/filetest/build/documentation.dsp`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/m/Makefile` & `typecode-30.0.1/tests/data/filetest/build/m/Makefile`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/pom.pom` & `typecode-30.0.1/tests/data/filetest/build/pom.pom`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/build/pom.xml` & `typecode-30.0.1/tests/data/filetest/build/pom.xml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/certificate/ECLIPSE.RSA` & `typecode-30.0.1/tests/data/filetest/certificate/ECLIPSE.RSA`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/assembly/bcopy.s` & `typecode-30.0.1/tests/data/filetest/code/assembly/bcopy.s`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/TEST.H` & `typecode-30.0.1/tests/data/filetest/code/c/TEST.H`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/TEST_LOWERCASE.h` & `typecode-30.0.1/tests/data/filetest/code/c/TEST_LOWERCASE.h`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/cpu.c` & `typecode-30.0.1/tests/data/filetest/code/c/cpu.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/main.c` & `typecode-30.0.1/tests/data/filetest/code/c/main.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/mm.c` & `typecode-30.0.1/tests/data/filetest/code/c/mm.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/pci.c` & `typecode-30.0.1/tests/data/filetest/code/c/pci.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/c/pci_v3.c` & `typecode-30.0.1/tests/data/filetest/code/c/pci_v3.c`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/cpp/stacktrace.cpp` & `typecode-30.0.1/tests/data/filetest/code/cpp/stacktrace.cpp`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/cpp/string.CPP` & `typecode-30.0.1/tests/data/filetest/code/cpp/string.CPP`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/java/Appender.java` & `typecode-30.0.1/tests/data/filetest/code/java/Appender.java`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/java/ChartTiming1.java` & `typecode-30.0.1/tests/data/filetest/code/java/ChartTiming1.java`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/java/CommonViewerSiteFactory.jad` & `typecode-30.0.1/tests/data/filetest/code/java/CommonViewerSiteFactory.jad`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/java/Logger.JAVA` & `typecode-30.0.1/tests/data/filetest/code/java/Logger.JAVA`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/java/contenttype.java` & `typecode-30.0.1/tests/data/filetest/code/java/contenttype.java`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/code/scala/Applicative.scala` & `typecode-30.0.1/tests/data/filetest/code/scala/Applicative.scala`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/flash/a.swf` & `typecode-30.0.1/tests/data/filetest/compiled/flash/a.swf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/flash/b.swf` & `typecode-30.0.1/tests/data/filetest/compiled/flash/b.swf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr` & `typecode-30.0.1/tests/data/filetest/compiled/flash/flash-haloclassic.swc.incr`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/linux/i686-shash` & `typecode-30.0.1/tests/data/filetest/compiled/linux/i686-shash`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/linux/x86_64-shash` & `typecode-30.0.1/tests/data/filetest/compiled/linux/x86_64-shash`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/win/file.exe` & `typecode-30.0.1/tests/data/filetest/compiled/win/file.exe`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/compiled/win/zlib1.dll` & `typecode-30.0.1/tests/data/filetest/compiled/win/zlib1.dll`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/config/config.conf` & `typecode-30.0.1/tests/data/filetest/config/config.conf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/config/defconfig-ar531x-jffs2` & `typecode-30.0.1/tests/data/filetest/config/defconfig-ar531x-jffs2`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/config/eclipse_configuration_3u.cfs` & `typecode-30.0.1/tests/data/filetest/config/eclipse_configuration_3u.cfs`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/config/wrapper.conf` & `typecode-30.0.1/tests/data/filetest/config/wrapper.conf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/data/mysql-arch` & `typecode-30.0.1/tests/data/filetest/data/mysql-arch`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/debug/QTMovieWin.pdb` & `typecode-30.0.1/tests/data/filetest/debug/QTMovieWin.pdb`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/html/Label.html` & `typecode-30.0.1/tests/data/filetest/doc/html/Label.html`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/html/a.htm` & `typecode-30.0.1/tests/data/filetest/doc/html/a.htm`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/html/allclasses-frame.html` & `typecode-30.0.1/tests/data/filetest/doc/html/allclasses-frame.html`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/html/contenttype.html` & `typecode-30.0.1/tests/data/filetest/doc/html/contenttype.html`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/Glitch-ERD.vsd` & `typecode-30.0.1/tests/data/filetest/doc/office/Glitch-ERD.vsd`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/document` & `typecode-30.0.1/tests/data/filetest/doc/office/document`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/document.doc` & `typecode-30.0.1/tests/data/filetest/doc/office/document.doc`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/excel.xls` & `typecode-30.0.1/tests/data/filetest/doc/office/excel.xls`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/excel.xlsx` & `typecode-30.0.1/tests/data/filetest/doc/office/excel.xlsx`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/power.ppt` & `typecode-30.0.1/tests/data/filetest/doc/office/power.ppt`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/power.pptx` & `typecode-30.0.1/tests/data/filetest/doc/office/power.pptx`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/word.doc` & `typecode-30.0.1/tests/data/filetest/doc/office/word.doc`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/office/word.docx` & `typecode-30.0.1/tests/data/filetest/doc/office/word.docx`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/pdf/a.pdf` & `typecode-30.0.1/tests/data/filetest/doc/pdf/a.pdf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/pdf/notpdf.pdf` & `typecode-30.0.1/tests/data/filetest/doc/pdf/notpdf.pdf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/pdf/pdf.pdf` & `typecode-30.0.1/tests/data/filetest/doc/pdf/pdf.pdf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/postscript/a.ps` & `typecode-30.0.1/tests/data/filetest/doc/postscript/a.ps`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/postscript/doc.ps` & `typecode-30.0.1/tests/data/filetest/doc/postscript/doc.ps`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/xml/some.xml` & `typecode-30.0.1/tests/data/filetest/doc/xml/some.xml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/doc/xml/somespring.xml` & `typecode-30.0.1/tests/data/filetest/doc/xml/somespring.xml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Image-ascii.pgm` & `typecode-30.0.1/tests/data/filetest/media/Image-ascii.pgm`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Image.pgm` & `typecode-30.0.1/tests/data/filetest/media/Image.pgm`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Image1.psp` & `typecode-30.0.1/tests/data/filetest/media/Image1.psp`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Image1.tga` & `typecode-30.0.1/tests/data/filetest/media/Image1.tga`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie.wmv` & `typecode-30.0.1/tests/data/filetest/media/Movie.wmv`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie.wmv.yml` & `typecode-30.0.1/tests/data/filetest/media/Movie.wmv.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie_0001.wmv` & `typecode-30.0.1/tests/data/filetest/media/Movie_0001.wmv`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie_0001.wmv.yml` & `typecode-30.0.1/tests/data/filetest/media/Movie_0001.wmv.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie_0002.wmv` & `typecode-30.0.1/tests/data/filetest/media/Movie_0002.wmv`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/Movie_0002.wmv.yml` & `typecode-30.0.1/tests/data/filetest/media/Movie_0002.wmv.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/TBarLrge.bmp` & `typecode-30.0.1/tests/data/filetest/media/TBarLrge.bmp`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/TBarMedm.bmp` & `typecode-30.0.1/tests/data/filetest/media/TBarMedm.bmp`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.aif` & `typecode-30.0.1/tests/data/filetest/media/a.aif`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.aiff` & `typecode-30.0.1/tests/data/filetest/media/a.aiff`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.au` & `typecode-30.0.1/tests/data/filetest/media/a.au`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.avi` & `typecode-30.0.1/tests/data/filetest/media/a.avi`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.flac` & `typecode-30.0.1/tests/data/filetest/media/a.flac`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.mp2` & `typecode-30.0.1/tests/data/filetest/media/a.mp2`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.mp3` & `typecode-30.0.1/tests/data/filetest/media/a.mp3`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.ogg` & `typecode-30.0.1/tests/data/filetest/media/a.ogg`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.pdf` & `typecode-30.0.1/tests/data/filetest/media/a.pdf`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.theo.ogg` & `typecode-30.0.1/tests/data/filetest/media/a.theo.ogg`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a.wav` & `typecode-30.0.1/tests/data/filetest/media/a.wav`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/a4.mpg` & `typecode-30.0.1/tests/data/filetest/media/a4.mpg`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/drawing.svg` & `typecode-30.0.1/tests/data/filetest/media/drawing.svg`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/mov.wvm.wmv` & `typecode-30.0.1/tests/data/filetest/media/mov.wvm.wmv`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/media/mov.wvm.wmv.yml` & `typecode-30.0.1/tests/data/filetest/media/mov.wvm.wmv.yml`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg` & `typecode-30.0.1/tests/data/filetest/package/TicketImport-0.7a-py2.5.egg`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/ant-jsch-1.7.0.jar` & `typecode-30.0.1/tests/data/filetest/package/ant-jsch-1.7.0.jar`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/ant.zip` & `typecode-30.0.1/tests/data/filetest/package/ant.zip`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/c.war` & `typecode-30.0.1/tests/data/filetest/package/c.war`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/rubygems-update-1.4.1.gem` & `typecode-30.0.1/tests/data/filetest/package/rubygems-update-1.4.1.gem`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm` & `typecode-30.0.1/tests/data/filetest/package/wget-1.11.4-3.fc11.i586.rpm`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/script/build_w32vc.bat` & `typecode-30.0.1/tests/data/filetest/script/build_w32vc.bat`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/script/makelinks` & `typecode-30.0.1/tests/data/filetest/script/makelinks`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/COPYING` & `typecode-30.0.1/tests/data/filetest/text/COPYING`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/CREDITS` & `typecode-30.0.1/tests/data/filetest/text/CREDITS`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/ChangeLog` & `typecode-30.0.1/tests/data/filetest/text/ChangeLog`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/GPL.txt` & `typecode-30.0.1/tests/data/filetest/text/GPL.txt`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/windowserver.log` & `typecode-30.0.1/tests/data/filetest/text/windowserver.log`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/data/filetest/text/x11-xconsortium_text.txt` & `typecode-30.0.1/tests/data/filetest/text/x11-xconsortium_text.txt`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/filetype_test_utils.py` & `typecode-30.0.1/tests/filetype_test_utils.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/test_contenttype.py` & `typecode-30.0.1/tests/test_contenttype.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/test_entropy.py` & `typecode-30.0.1/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/test_extractible.py` & `typecode-30.0.1/tests/test_extractible.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/test_skeleton_codestyle.py` & `typecode-30.0.1/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/tests/test_types.py` & `typecode-30.0.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `typecode-30.0.0/typecode.ABOUT` & `typecode-30.0.1/typecode.ABOUT`

 * *Files identical despite different names*

