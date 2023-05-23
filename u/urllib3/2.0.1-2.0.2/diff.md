# Comparing `tmp/urllib3-2.0.1.tar.gz` & `tmp/urllib3-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Apr 30 06:04:47 2023, max compression
+gzip compressed data, last modified: Wed May  3 22:26:56 2023, max compression
```

## Comparing `urllib3-2.0.1.tar` & `urllib3-2.0.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    58021 2023-04-30 06:04:47.000000 urllib3-2.0.1/CHANGES.rst
--rw-r--r--   0        0        0      328 2023-04-30 06:04:47.000000 urllib3-2.0.1/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/Makefile
--rw-r--r--   0        0        0    21359 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/advanced-usage.rst
--rw-r--r--   0        0        0       59 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/changelog.rst
--rw-r--r--   0        0        0     3795 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/conf.py
--rw-r--r--   0        0        0     9500 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/contributing.rst
--rw-r--r--   0        0        0     3836 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/index.rst
--rw-r--r--   0        0        0     4513 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/make.bat
--rw-r--r--   0        0        0       72 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     1818 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/sponsors.rst
--rw-r--r--   0        0        0    16385 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/user-guide.rst
--rw-r--r--   0        0        0    12502 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0     7872 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/logo.png
--rw-r--r--   0        0        0      516 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/images/logo.svg
--rw-r--r--   0        0        0      226 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/index.rst
--rw-r--r--   0        0        0      316 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      408 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      338 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      788 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      555 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      233 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      295 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/pyopenssl.rst
--rw-r--r--   0        0        0     1431 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/securetransport.rst
--rw-r--r--   0        0        0      124 2023-04-30 06:04:47.000000 urllib3-2.0.1/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/__init__.py
--rw-r--r--   0        0        0    13109 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     5420 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9839 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/server.py
--rw-r--r--   0        0        0    11171 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2023-04-30 06:04:47.000000 urllib3-2.0.1/dummyserver/certs/server.key
--rw-r--r--   0        0        0     5028 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/__init__.py
--rw-r--r--   0        0        0     5651 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_base_connection.py
--rw-r--r--   0        0        0    15561 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_collections.py
--rw-r--r--   0        0        0     7756 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/_version.py
--rw-r--r--   0        0        0    33511 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/connection.py
--rw-r--r--   0        0        0    42961 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9289 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/exceptions.py
--rw-r--r--   0        0        0    11026 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/filepost.py
--rw-r--r--   0        0        0    22160 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/py.typed
--rw-r--r--   0        0        0    39769 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19437 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34121 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7715 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    14452 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    16220 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0     1051 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8111 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/response.py
--rw-r--r--   0        0        0    18375 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    18540 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9045 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10529 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2023-04-30 06:04:47.000000 urllib3-2.0.1/src/urllib3/util/wait.py
--rw-r--r--   0        0        0    10763 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/__init__.py
--rw-r--r--   0        0        0    11211 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/conftest.py
--rw-r--r--   0        0        0     6222 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/port_helpers.py
--rw-r--r--   0        0        0    13035 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_collections.py
--rw-r--r--   0        0        0      692 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_compatibility.py
--rw-r--r--   0        0        0    10737 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_connection.py
--rw-r--r--   0        0        0    22772 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_connectionpool.py
--rw-r--r--   0        0        0     2164 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_exceptions.py
--rw-r--r--   0        0        0     4438 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_fields.py
--rw-r--r--   0        0        0     3751 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_filepost.py
--rw-r--r--   0        0        0      978 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_no_ssl.py
--rw-r--r--   0        0        0    17765 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_proxymanager.py
--rw-r--r--   0        0        0      761 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_queue_monkeypatch.py
--rw-r--r--   0        0        0    44819 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_response.py
--rw-r--r--   0        0        0    16568 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_retry.py
--rw-r--r--   0        0        0     7281 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_ssl.py
--rw-r--r--   0        0        0    20750 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_ssltransport.py
--rw-r--r--   0        0        0    43233 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_util.py
--rw-r--r--   0        0        0     5999 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/test_wait.py
--rw-r--r--   0        0        0     1211 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/tz_stub.py
--rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0     3007 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_pyopenssl.py
--rw-r--r--   0        0        0     1988 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_pyopenssl_dependencies.py
--rw-r--r--   0        0        0     1690 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_securetransport.py
--rw-r--r--   0        0        0    25908 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0    10678 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3827 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56860 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0    43609 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    22082 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    33489 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    84327 2023-04-30 06:04:47.000000 urllib3-2.0.1/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0       85 2023-04-30 06:04:47.000000 urllib3-2.0.1/.gitignore
--rw-r--r--   0        0        0     1115 2023-04-30 06:04:47.000000 urllib3-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4393 2023-04-30 06:04:47.000000 urllib3-2.0.1/README.md
--rw-r--r--   0        0        0     4069 2023-04-30 06:04:47.000000 urllib3-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6621 2023-04-30 06:04:47.000000 urllib3-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    58603 2023-05-03 22:26:56.000000 urllib3-2.0.2/CHANGES.rst
+-rw-r--r--   0        0        0      328 2023-05-03 22:26:56.000000 urllib3-2.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/Makefile
+-rw-r--r--   0        0        0    21359 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/advanced-usage.rst
+-rw-r--r--   0        0        0       59 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/changelog.rst
+-rw-r--r--   0        0        0     3795 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/conf.py
+-rw-r--r--   0        0        0     9500 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/contributing.rst
+-rw-r--r--   0        0        0     3836 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/index.rst
+-rw-r--r--   0        0        0     4513 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/make.bat
+-rw-r--r--   0        0        0       72 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     1818 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/sponsors.rst
+-rw-r--r--   0        0        0    16385 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/user-guide.rst
+-rw-r--r--   0        0        0    12502 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0     7872 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/logo.svg
+-rw-r--r--   0        0        0      226 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/index.rst
+-rw-r--r--   0        0        0      316 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      408 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      338 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      788 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      555 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      233 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      295 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/pyopenssl.rst
+-rw-r--r--   0        0        0     1431 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/securetransport.rst
+-rw-r--r--   0        0        0      124 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13109 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     5420 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9839 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/server.py
+-rw-r--r--   0        0        0    11171 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     5028 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/__init__.py
+-rw-r--r--   0        0        0     5651 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    15561 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     7756 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_version.py
+-rw-r--r--   0        0        0    33511 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/connection.py
+-rw-r--r--   0        0        0    42961 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9289 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0    11026 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    22160 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/py.typed
+-rw-r--r--   0        0        0    39802 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19437 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34121 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7715 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    14452 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    16220 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0     1051 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8111 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    18375 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    18540 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9045 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10529 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10763 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/__init__.py
+-rw-r--r--   0        0        0    11211 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/conftest.py
+-rw-r--r--   0        0        0     6222 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/port_helpers.py
+-rw-r--r--   0        0        0    13035 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_collections.py
+-rw-r--r--   0        0        0      692 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_compatibility.py
+-rw-r--r--   0        0        0    10737 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_connection.py
+-rw-r--r--   0        0        0    22772 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_connectionpool.py
+-rw-r--r--   0        0        0     2164 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_exceptions.py
+-rw-r--r--   0        0        0     4438 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_fields.py
+-rw-r--r--   0        0        0     3751 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_no_ssl.py
+-rw-r--r--   0        0        0    17765 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_proxymanager.py
+-rw-r--r--   0        0        0      761 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_queue_monkeypatch.py
+-rw-r--r--   0        0        0    44819 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_response.py
+-rw-r--r--   0        0        0    16568 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_retry.py
+-rw-r--r--   0        0        0     7281 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_ssl.py
+-rw-r--r--   0        0        0    20750 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43233 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_util.py
+-rw-r--r--   0        0        0     5999 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_wait.py
+-rw-r--r--   0        0        0     1211 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0     3007 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_pyopenssl.py
+-rw-r--r--   0        0        0     1988 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_pyopenssl_dependencies.py
+-rw-r--r--   0        0        0     1690 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_securetransport.py
+-rw-r--r--   0        0        0    25908 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0    10678 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3827 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    56860 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0    43609 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    22082 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    33489 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    85953 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0       85 2023-05-03 22:26:56.000000 urllib3-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1115 2023-05-03 22:26:56.000000 urllib3-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4363 2023-05-03 22:26:56.000000 urllib3-2.0.2/README.md
+-rw-r--r--   0        0        0     4069 2023-05-03 22:26:56.000000 urllib3-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6591 2023-05-03 22:26:56.000000 urllib3-2.0.2/PKG-INFO
```

### Comparing `urllib3-2.0.1/CHANGES.rst` & `urllib3-2.0.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-2.0.1 (2023-04-30)
+2.0.2 (2023-05-03)
 ==================
 
-Fixes
------
+- Fixed ``HTTPResponse.stream()`` to continue yielding bytes if buffered decompressed data
+  was still available to be read even if the underlying socket is closed. This prevents
+  a compressed response from being truncated. (`#3009 <https://github.com/urllib3/urllib3/issues/3009>`__)
+
+
+2.0.1 (2023-04-30)
+==================
 
 - Fixed a socket leak when fingerprint or hostname verifications fail. (`#2991 <https://github.com/urllib3/urllib3/issues/2991>`__)
 - Fixed an error when ``HTTPResponse.read(0)`` was the first ``read`` call or when the internal response body buffer was otherwise empty. (`#2998 <https://github.com/urllib3/urllib3/issues/2998>`__)
 
 
 2.0.0 (2023-04-26)
 ==================
@@ -35,23 +40,24 @@
   function instead of the ``urllib3.request`` module (`#2269 <https://github.com/urllib3/urllib3/issues/2269>`__).
 * Removed support for SSLv3.0 from the ``urllib3.contrib.pyopenssl`` even when support is available from the compiled OpenSSL library (`#2233 <https://github.com/urllib3/urllib3/issues/2233>`__).
 * Removed the deprecated ``urllib3.contrib.ntlmpool`` module (`#2339 <https://github.com/urllib3/urllib3/issues/2339>`__).
 * Removed ``DEFAULT_CIPHERS``, ``HAS_SNI``, ``USE_DEFAULT_SSLCONTEXT_CIPHERS``, from the private module ``urllib3.util.ssl_`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
 * Removed ``urllib3.exceptions.SNIMissingWarning`` (`#2168 <https://github.com/urllib3/urllib3/issues/2168>`__).
 * Removed the ``_prepare_conn`` method from ``HTTPConnectionPool``. Previously this was only used to call ``HTTPSConnection.set_cert()`` by ``HTTPSConnectionPool`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Removed ``tls_in_tls_required`` property from ``HTTPSConnection``. This is now determined from the ``scheme`` parameter in ``HTTPConnection.set_tunnel()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
+* Removed the ``strict`` parameter/attribute from ``HTTPConnection``, ``HTTPSConnection``, ``HTTPConnectionPool``, ``HTTPSConnectionPool``, and ``HTTPResponse`` (`#2064 <https://github.com/urllib3/urllib3/issues/2064>`__).
 
 Deprecated
 ----------
 
 * Deprecated ``HTTPResponse.getheaders()`` and ``HTTPResponse.getheader()`` which will be removed in urllib3 v2.1.0. Instead use ``HTTPResponse.headers`` and ``HTTPResponse.headers.get(name, default)``. (`#1543 <https://github.com/urllib3/urllib3/issues/1543>`__, `#2814 <https://github.com/urllib3/urllib3/issues/2814>`__).
 * Deprecated ``urllib3.contrib.pyopenssl`` module which will be removed in urllib3 v2.1.0 (`#2691 <https://github.com/urllib3/urllib3/issues/2691>`__).
 * Deprecated ``urllib3.contrib.securetransport`` module which will be removed in urllib3 v2.1.0 (`#2692 <https://github.com/urllib3/urllib3/issues/2692>`__).
 * Deprecated ``ssl_version`` option in favor of ``ssl_minimum_version``. ``ssl_version`` will be removed in urllib3 v2.1.0 (`#2110 <https://github.com/urllib3/urllib3/issues/2110>`__).
-* Deprecated the ``strict`` parameter as it's not longer needed in Python 3.x. It will be removed in urllib3 v2.1.0 (`#2267 <https://github.com/urllib3/urllib3/issues/2267>`__)
+* Deprecated the ``strict`` parameter of ``PoolManager.connection_from_context()`` as it's not longer needed in Python 3.x. It will be removed in urllib3 v2.1.0 (`#2267 <https://github.com/urllib3/urllib3/issues/2267>`__)
 * Deprecated the ``NewConnectionError.pool`` attribute which will be removed in urllib3 v2.1.0 (`#2271 <https://github.com/urllib3/urllib3/issues/2271>`__).
 * Deprecated ``format_header_param_html5`` and ``format_header_param`` in favor of ``format_multipart_header_param`` (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
 * Deprecated ``RequestField.header_formatter`` parameter which will be removed in urllib3 v2.1.0 (`#2257 <https://github.com/urllib3/urllib3/issues/2257>`__).
 * Deprecated ``HTTPSConnection.set_cert()`` method. Instead pass parameters to the ``HTTPSConnection`` constructor (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 * Deprecated ``HTTPConnection.request_chunked()`` method which will be removed in urllib3 v2.1.0. Instead pass ``chunked=True`` to ``HTTPConnection.request()`` (`#1985 <https://github.com/urllib3/urllib3/issues/1985>`__).
 
 Added
```

### Comparing `urllib3-2.0.1/docs/Makefile` & `urllib3-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/advanced-usage.rst` & `urllib3-2.0.2/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/conf.py` & `urllib3-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/contributing.rst` & `urllib3-2.0.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/index.rst` & `urllib3-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/make.bat` & `urllib3-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/sponsors.rst` & `urllib3-2.0.2/docs/sponsors.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/user-guide.rst` & `urllib3-2.0.2/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/v2-migration-guide.rst` & `urllib3-2.0.2/docs/v2-migration-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/_static/banner.svg` & `urllib3-2.0.2/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/_static/banner_github.svg` & `urllib3-2.0.2/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/_static/dark-logo.svg` & `urllib3-2.0.2/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/images/demo-button.png` & `urllib3-2.0.2/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/images/favicon.png` & `urllib3-2.0.2/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/images/learn-more-button.png` & `urllib3-2.0.2/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/images/logo.png` & `urllib3-2.0.2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/images/logo.svg` & `urllib3-2.0.2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/reference/urllib3.response.rst` & `urllib3-2.0.2/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/reference/urllib3.util.rst` & `urllib3-2.0.2/docs/reference/urllib3.util.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/docs/reference/contrib/securetransport.rst` & `urllib3-2.0.2/docs/reference/contrib/securetransport.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/handlers.py` & `urllib3-2.0.2/dummyserver/handlers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/https_proxy.py` & `urllib3-2.0.2/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/proxy.py` & `urllib3-2.0.2/dummyserver/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/server.py` & `urllib3-2.0.2/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/testcase.py` & `urllib3-2.0.2/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/certs/cacert.key` & `urllib3-2.0.2/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/certs/cacert.pem` & `urllib3-2.0.2/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/certs/server.crt` & `urllib3-2.0.2/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/dummyserver/certs/server.key` & `urllib3-2.0.2/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/__init__.py` & `urllib3-2.0.2/src/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/_base_connection.py` & `urllib3-2.0.2/src/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/_collections.py` & `urllib3-2.0.2/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/_request_methods.py` & `urllib3-2.0.2/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/connection.py` & `urllib3-2.0.2/src/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/connectionpool.py` & `urllib3-2.0.2/src/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/exceptions.py` & `urllib3-2.0.2/src/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/fields.py` & `urllib3-2.0.2/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/filepost.py` & `urllib3-2.0.2/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/poolmanager.py` & `urllib3-2.0.2/src/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/response.py` & `urllib3-2.0.2/src/urllib3/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -927,15 +927,15 @@
         :param decode_content:
             If True, will attempt to decode the body based on the
             'content-encoding' header.
         """
         if self.chunked and self.supports_chunked_reads():
             yield from self.read_chunked(amt, decode_content=decode_content)
         else:
-            while not is_fp_closed(self._fp):
+            while not is_fp_closed(self._fp) or len(self._decoded_buffer) > 0:
                 data = self.read(amt=amt, decode_content=decode_content)
 
                 if data:
                     yield data
 
     # Overrides from io.IOBase
     def readable(self) -> bool:
```

### Comparing `urllib3-2.0.1/src/urllib3/contrib/pyopenssl.py` & `urllib3-2.0.2/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/contrib/securetransport.py` & `urllib3-2.0.2/src/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/contrib/socks.py` & `urllib3-2.0.2/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/contrib/_securetransport/bindings.py` & `urllib3-2.0.2/src/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/contrib/_securetransport/low_level.py` & `urllib3-2.0.2/src/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/__init__.py` & `urllib3-2.0.2/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/connection.py` & `urllib3-2.0.2/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/proxy.py` & `urllib3-2.0.2/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/request.py` & `urllib3-2.0.2/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/response.py` & `urllib3-2.0.2/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/retry.py` & `urllib3-2.0.2/src/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/ssl_.py` & `urllib3-2.0.2/src/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/ssl_match_hostname.py` & `urllib3-2.0.2/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/ssltransport.py` & `urllib3-2.0.2/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/timeout.py` & `urllib3-2.0.2/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/url.py` & `urllib3-2.0.2/src/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/util.py` & `urllib3-2.0.2/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/src/urllib3/util/wait.py` & `urllib3-2.0.2/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/__init__.py` & `urllib3-2.0.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/conftest.py` & `urllib3-2.0.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/port_helpers.py` & `urllib3-2.0.2/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_collections.py` & `urllib3-2.0.2/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_compatibility.py` & `urllib3-2.0.2/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_connection.py` & `urllib3-2.0.2/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_connectionpool.py` & `urllib3-2.0.2/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_exceptions.py` & `urllib3-2.0.2/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_fields.py` & `urllib3-2.0.2/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_filepost.py` & `urllib3-2.0.2/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_no_ssl.py` & `urllib3-2.0.2/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_poolmanager.py` & `urllib3-2.0.2/test/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_proxymanager.py` & `urllib3-2.0.2/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_queue_monkeypatch.py` & `urllib3-2.0.2/test/test_queue_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_response.py` & `urllib3-2.0.2/test/test_response.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_retry.py` & `urllib3-2.0.2/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_ssl.py` & `urllib3-2.0.2/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_ssltransport.py` & `urllib3-2.0.2/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_util.py` & `urllib3-2.0.2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/test_wait.py` & `urllib3-2.0.2/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/tz_stub.py` & `urllib3-2.0.2/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/contrib/duplicate_san.pem` & `urllib3-2.0.2/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/contrib/test_pyopenssl.py` & `urllib3-2.0.2/test/contrib/test_pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/contrib/test_pyopenssl_dependencies.py` & `urllib3-2.0.2/test/contrib/test_pyopenssl_dependencies.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/contrib/test_securetransport.py` & `urllib3-2.0.2/test/contrib/test_securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/contrib/test_socks.py` & `urllib3-2.0.2/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_chunked_transfer.py` & `urllib3-2.0.2/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_connection.py` & `urllib3-2.0.2/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_connectionpool.py` & `urllib3-2.0.2/test/with_dummyserver/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_https.py` & `urllib3-2.0.2/test/with_dummyserver/test_https.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_no_ssl.py` & `urllib3-2.0.2/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_poolmanager.py` & `urllib3-2.0.2/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3-2.0.2/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/test/with_dummyserver/test_socketlevel.py` & `urllib3-2.0.2/test/with_dummyserver/test_socketlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import shutil
 import socket
 import ssl
 import sys
 import tempfile
 import time
 import typing
+import zlib
 from collections import OrderedDict
 from pathlib import Path
 from test import (
     LONG_TIMEOUT,
     SHORT_TIMEOUT,
     notSecureTransport,
     notWindows,
@@ -1281,24 +1282,21 @@
 
 
 class TestSSL(SocketDummyServerTestCase):
     def test_ssl_failure_midway_through_conn(self) -> None:
         def socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
             sock2 = sock.dup()
-            try:
-                ssl_sock = original_ssl_wrap_socket(
-                    sock,
-                    server_side=True,
-                    keyfile=DEFAULT_CERTS["keyfile"],
-                    certfile=DEFAULT_CERTS["certfile"],
-                    ca_certs=DEFAULT_CA,
-                )
-            except ssl.SSLError:
-                return
+            ssl_sock = original_ssl_wrap_socket(
+                sock,
+                server_side=True,
+                keyfile=DEFAULT_CERTS["keyfile"],
+                certfile=DEFAULT_CERTS["certfile"],
+                ca_certs=DEFAULT_CA,
+            )
 
             buf = b""
             while not buf.endswith(b"\r\n\r\n"):
                 buf += ssl_sock.recv(65536)
 
             # Deliberately send from the non-SSL socket.
             sock2.send(
@@ -1308,18 +1306,19 @@
                 b"\r\n"
                 b"Hi"
             )
             sock2.close()
             ssl_sock.close()
 
         self._start_server(socket_handler)
-        with HTTPSConnectionPool(self.host, self.port) as pool:
-            with pytest.raises(MaxRetryError) as cm:
-                pool.request("GET", "/", retries=0)
-            assert isinstance(cm.value.reason, SSLError)
+        with HTTPSConnectionPool(self.host, self.port, ca_certs=DEFAULT_CA) as pool:
+            with pytest.raises(
+                SSLError, match=r"(wrong version number|record overflow)"
+            ):
+                pool.request("GET", "/", retries=False)
 
     @notSecureTransport()
     def test_ssl_read_timeout(self) -> None:
         timed_out = Event()
 
         def socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
@@ -1999,14 +1998,62 @@
             r = pool.request("GET", "/", timeout=LONG_TIMEOUT, preload_content=False)
 
             # Stream should read to the end.
             assert [b"hello, world"] == list(r.stream(None))
 
             done_event.set()
 
+    def test_large_compressed_stream(self) -> None:
+        done_event = Event()
+        expected_total_length = 296085
+
+        def socket_handler(listener: socket.socket) -> None:
+            compress = zlib.compressobj(6, zlib.DEFLATED, 16 + zlib.MAX_WBITS)
+            data = compress.compress(b"x" * expected_total_length)
+            data += compress.flush()
+
+            sock = listener.accept()[0]
+
+            buf = b""
+            while not buf.endswith(b"\r\n\r\n"):
+                buf += sock.recv(65536)
+
+            sock.sendall(
+                b"HTTP/1.1 200 OK\r\n"
+                b"Content-Length: %d\r\n"
+                b"Content-Encoding: gzip\r\n"
+                b"\r\n" % (len(data),) + data
+            )
+
+            done_event.wait(5)
+            sock.close()
+
+        self._start_server(socket_handler)
+
+        with HTTPConnectionPool(self.host, self.port, retries=False) as pool:
+            r = pool.request("GET", "/", timeout=LONG_TIMEOUT, preload_content=False)
+
+            # Chunks must all be equal or less than 10240
+            # and only the last chunk is allowed to be smaller
+            # than 10240.
+            total_length = 0
+            chunks_smaller_than_10240 = 0
+            for chunk in r.stream(10240, decode_content=True):
+                assert 0 < len(chunk) <= 10240
+                if len(chunk) < 10240:
+                    chunks_smaller_than_10240 += 1
+                else:
+                    assert chunks_smaller_than_10240 == 0
+                total_length += len(chunk)
+
+            assert chunks_smaller_than_10240 == 1
+            assert expected_total_length == total_length
+
+            done_event.set()
+
 
 class TestBadContentLength(SocketDummyServerTestCase):
     def test_enforce_content_length_get(self) -> None:
         done_event = Event()
 
         def socket_handler(listener: socket.socket) -> None:
             sock = listener.accept()[0]
```

### Comparing `urllib3-2.0.1/LICENSE.txt` & `urllib3-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/README.md` & `urllib3-2.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 - Proxy support for HTTP and SOCKS.
 - 100% test coverage.
 
 urllib3 is powerful and easy to use:
 
 ```python3
 >>> import urllib3
->>> http = urllib3.PoolManager()
->>> resp = http.request("GET", "http://httpbin.org/robots.txt")
+>>> resp = urllib3.request("GET", "http://httpbin.org/robots.txt")
 >>> resp.status
 200
 >>> resp.data
 b"User-agent: *\nDisallow: /deny\n"
 ```
 
 ## Installing
```

#### html2text {}

```diff
@@ -6,22 +6,22 @@
 urllib3 is a powerful, *user-friendly* HTTP client for Python. Much of the
 Python ecosystem already uses urllib3 and you should too. urllib3 brings many
 critical features that are missing from the Python standard libraries: - Thread
 safety. - Connection pooling. - Client-side SSL/TLS verification. - File
 uploads with multipart encoding. - Helpers for retrying requests and dealing
 with HTTP redirects. - Support for gzip, deflate, brotli, and zstd encoding. -
 Proxy support for HTTP and SOCKS. - 100% test coverage. urllib3 is powerful and
-easy to use: ```python3 >>> import urllib3 >>> http = urllib3.PoolManager() >>>
-resp = http.request("GET", "http://httpbin.org/robots.txt") >>> resp.status 200
->>> resp.data b"User-agent: *\nDisallow: /deny\n" ``` ## Installing urllib3 can
-be installed with [pip](https://pip.pypa.io): ```bash $ python -m pip install
-urllib3 ``` Alternatively, you can grab the latest source code from [GitHub]
-(https://github.com/urllib3/urllib3): ```bash $ git clone https://github.com/
-urllib3/urllib3.git $ cd urllib3 $ pip install . ``` ## Documentation urllib3
-has usage and reference documentation at [urllib3.readthedocs.io](https://
+easy to use: ```python3 >>> import urllib3 >>> resp = urllib3.request("GET",
+"http://httpbin.org/robots.txt") >>> resp.status 200 >>> resp.data b"User-
+agent: *\nDisallow: /deny\n" ``` ## Installing urllib3 can be installed with
+[pip](https://pip.pypa.io): ```bash $ python -m pip install urllib3 ```
+Alternatively, you can grab the latest source code from [GitHub](https://
+github.com/urllib3/urllib3): ```bash $ git clone https://github.com/urllib3/
+urllib3.git $ cd urllib3 $ pip install . ``` ## Documentation urllib3 has usage
+and reference documentation at [urllib3.readthedocs.io](https://
 urllib3.readthedocs.io). ## Community urllib3 has a [community Discord channel]
 (https://discord.gg/urllib3) for asking questions and collaborating with other
 contributors. Drop by and say hello ð ## Contributing urllib3 happily
 accepts contributions. Please see our [contributing documentation](https://
 urllib3.readthedocs.io/en/latest/contributing.html) for some tips on getting
 started. ## Security Disclosures To report a security vulnerability, please use
 the [Tidelift security contact](https://tidelift.com/security). Tidelift will
```

### Comparing `urllib3-2.0.1/pyproject.toml` & `urllib3-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.1/PKG-INFO` & `urllib3-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3
-Version: 2.0.1
+Version: 2.0.2
 Summary: HTTP library with thread-safe connection pooling, file post, and more.
 Project-URL: Changelog, https://github.com/urllib3/urllib3/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/urllib3/urllib3
 Project-URL: Issue tracker, https://github.com/urllib3/urllib3/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: Seth Michael Larson <sethmichaellarson@gmail.com>, Quentin Pradet <quentin@pradet.me>
@@ -75,16 +75,15 @@
 - Proxy support for HTTP and SOCKS.
 - 100% test coverage.
 
 urllib3 is powerful and easy to use:
 
 ```python3
 >>> import urllib3
->>> http = urllib3.PoolManager()
->>> resp = http.request("GET", "http://httpbin.org/robots.txt")
+>>> resp = urllib3.request("GET", "http://httpbin.org/robots.txt")
 >>> resp.status
 200
 >>> resp.data
 b"User-agent: *\nDisallow: /deny\n"
 ```
 
 ## Installing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urllib3 Version: 2.0.1 Summary: HTTP library with
+Metadata-Version: 2.1 Name: urllib3 Version: 2.0.2 Summary: HTTP library with
 thread-safe connection pooling, file post, and more. Project-URL: Changelog,
 https://github.com/urllib3/urllib3/blob/main/CHANGES.rst Project-URL:
 Documentation, https://urllib3.readthedocs.io Project-URL: Code, https://
 github.com/urllib3/urllib3 Project-URL: Issue tracker, https://github.com/
 urllib3/urllib3/issues Author-email: Andrey Petrov
 petrov@shazow.net> Maintainer-email: Seth Michael Larson
 gmail.com>, Quentin Pradet
@@ -38,22 +38,22 @@
 urllib3 is a powerful, *user-friendly* HTTP client for Python. Much of the
 Python ecosystem already uses urllib3 and you should too. urllib3 brings many
 critical features that are missing from the Python standard libraries: - Thread
 safety. - Connection pooling. - Client-side SSL/TLS verification. - File
 uploads with multipart encoding. - Helpers for retrying requests and dealing
 with HTTP redirects. - Support for gzip, deflate, brotli, and zstd encoding. -
 Proxy support for HTTP and SOCKS. - 100% test coverage. urllib3 is powerful and
-easy to use: ```python3 >>> import urllib3 >>> http = urllib3.PoolManager() >>>
-resp = http.request("GET", "http://httpbin.org/robots.txt") >>> resp.status 200
->>> resp.data b"User-agent: *\nDisallow: /deny\n" ``` ## Installing urllib3 can
-be installed with [pip](https://pip.pypa.io): ```bash $ python -m pip install
-urllib3 ``` Alternatively, you can grab the latest source code from [GitHub]
-(https://github.com/urllib3/urllib3): ```bash $ git clone https://github.com/
-urllib3/urllib3.git $ cd urllib3 $ pip install . ``` ## Documentation urllib3
-has usage and reference documentation at [urllib3.readthedocs.io](https://
+easy to use: ```python3 >>> import urllib3 >>> resp = urllib3.request("GET",
+"http://httpbin.org/robots.txt") >>> resp.status 200 >>> resp.data b"User-
+agent: *\nDisallow: /deny\n" ``` ## Installing urllib3 can be installed with
+[pip](https://pip.pypa.io): ```bash $ python -m pip install urllib3 ```
+Alternatively, you can grab the latest source code from [GitHub](https://
+github.com/urllib3/urllib3): ```bash $ git clone https://github.com/urllib3/
+urllib3.git $ cd urllib3 $ pip install . ``` ## Documentation urllib3 has usage
+and reference documentation at [urllib3.readthedocs.io](https://
 urllib3.readthedocs.io). ## Community urllib3 has a [community Discord channel]
 (https://discord.gg/urllib3) for asking questions and collaborating with other
 contributors. Drop by and say hello ð ## Contributing urllib3 happily
 accepts contributions. Please see our [contributing documentation](https://
 urllib3.readthedocs.io/en/latest/contributing.html) for some tips on getting
 started. ## Security Disclosures To report a security vulnerability, please use
 the [Tidelift security contact](https://tidelift.com/security). Tidelift will
```

