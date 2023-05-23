# Comparing `tmp/devpi-server-6.8.0.tar.gz` & `tmp/devpi-server-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-server-6.8.0.tar", last modified: Mon Dec  5 10:10:57 2022, max compression
+gzip compressed data, was "devpi-server-6.9.0.tar", last modified: Tue May 23 14:32:20 2023, max compression
```

## Comparing `devpi-server-6.8.0.tar` & `devpi-server-6.9.0.tar`

### file list

```diff
@@ -1,161 +1,165 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.985041 devpi-server-6.8.0/
--rw-r--r--   0 fschulze   (501) staff       (20)      138 2022-12-05 10:10:52.000000 devpi-server-6.8.0/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    69898 2022-12-05 10:10:52.000000 devpi-server-6.8.0/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2022-12-05 10:10:52.000000 devpi-server-6.8.0/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      188 2022-12-05 10:10:52.000000 devpi-server-6.8.0/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     6373 2022-12-05 10:10:57.985167 devpi-server-6.8.0/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     2033 2022-12-05 10:10:52.000000 devpi-server-6.8.0/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.959917 devpi-server-6.8.0/devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       82 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/__main__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7260 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1195 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/auth_basic.py
--rw-r--r--   0 fschulze   (501) staff       (20)      958 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/auth_devpi.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.965917 devpi-server-6.8.0/devpi_server/cfg/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)      213 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/crontab.template
--rw-r--r--   0 fschulze   (501) staff       (20)      430 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/devpi.service.template
--rw-r--r--   0 fschulze   (501) staff       (20)      455 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/launchd-macos.txt.template
--rw-r--r--   0 fschulze   (501) staff       (20)      619 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      237 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/nginx-devpi-caching-location.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      330 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      341 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/nginx-devpi-caching-server.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     2065 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/nginx-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      140 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/supervisor-devpi.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)      283 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/supervisord.conf.template
--rw-r--r--   0 fschulze   (501) staff       (20)     1694 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/cfg/windows-service.txt.template
--rwxr-xr-x   0 fschulze   (501) staff       (20)    36728 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)      643 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/exceptions.py
--rw-r--r--   0 fschulze   (501) staff       (20)    10169 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8831 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3579 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/fsck.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6962 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8555 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    28103 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1916 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/init.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5921 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/interfaces.py
--rw-r--r--   0 fschulze   (501) staff       (20)    30087 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    24210 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/keyfs_sqlite.py
--rw-r--r--   0 fschulze   (501) staff       (20)    11313 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2865 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/keyfs_types.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3751 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/log.py
--rwxr-xr-x   0 fschulze   (501) staff       (20)    25869 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)      794 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/middleware.py
--rw-r--r--   0 fschulze   (501) staff       (20)    38823 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/mirror.py
--rwxr-xr-x   0 fschulze   (501) staff       (20)    73864 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3668 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1642 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/passwd.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7035 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    51772 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1589 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/sizeof.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9110 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)    74942 2022-12-05 10:10:52.000000 devpi-server-6.8.0/devpi_server/views.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.962029 devpi-server-6.8.0/devpi_server.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     6373 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     4729 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)     1007 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      235 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       51 2022-12-05 10:10:57.000000 devpi-server-6.8.0/devpi_server.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      549 2022-12-05 10:10:52.000000 devpi-server-6.8.0/pyproject.toml
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.966192 devpi-server-6.8.0/pytest_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)      863 2022-12-05 10:10:52.000000 devpi-server-6.8.0/pytest_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       86 2022-12-05 10:10:57.985589 devpi-server-6.8.0/setup.cfg
--rwxr-xr-x   0 fschulze   (501) staff       (20)     4487 2022-12-05 10:10:52.000000 devpi-server-6.8.0/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.977806 devpi-server-6.8.0/test_devpi_server/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    46069 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)      504 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/example.py
--rw-r--r--   0 fschulze   (501) staff       (20)    20813 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/functional.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.947327 devpi-server-6.8.0/test_devpi_server/importexportdata/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.978134 devpi-server-6.8.0/test_devpi_server/importexportdata/badindexname/
--rw-r--r--   0 fschulze   (501) staff       (20)      698 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/badindexname/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.978602 devpi-server-6.8.0/test_devpi_server/importexportdata/badusername/
--rw-r--r--   0 fschulze   (501) staff       (20)      719 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/badusername/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.978875 devpi-server-6.8.0/test_devpi_server/importexportdata/basescycle/
--rw-r--r--   0 fschulze   (501) staff       (20)      659 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/basescycle/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.979158 devpi-server-6.8.0/test_devpi_server/importexportdata/createdmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      423 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/createdmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.979437 devpi-server-6.8.0/test_devpi_server/importexportdata/deletedbase/
--rw-r--r--   0 fschulze   (501) staff       (20)     1603 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/deletedbase/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.979716 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/
--rw-r--r--   0 fschulze   (501) staff       (20)     1413 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.943390 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.943591 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/pypi/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.943705 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.980047 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
--rw-r--r--   0 fschulze   (501) staff       (20)      780 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.980332 devpi-server-6.8.0/test_devpi_server/importexportdata/modifiedpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      648 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.980714 devpi-server-6.8.0/test_devpi_server/importexportdata/nocreatedmodified/
--rw-r--r--   0 fschulze   (501) staff       (20)      485 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.980995 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/
--rw-r--r--   0 fschulze   (501) staff       (20)     1610 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.944482 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.944600 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.981279 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.981557 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/
--rw-r--r--   0 fschulze   (501) staff       (20)     2299 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.945098 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.945377 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.981839 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.982252 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        8 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.982529 devpi-server-6.8.0/test_devpi_server/importexportdata/norootpypi/
--rw-r--r--   0 fschulze   (501) staff       (20)      340 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/norootpypi/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.982805 devpi-server-6.8.0/test_devpi_server/importexportdata/nouser/
--rw-r--r--   0 fschulze   (501) staff       (20)      198 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/nouser/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.983093 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/
--rw-r--r--   0 fschulze   (501) staff       (20)     1581 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.946195 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/user/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.946307 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.983535 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.983818 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/
--rw-r--r--   0 fschulze   (501) staff       (20)     1538 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.946768 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.946882 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.947165 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.984102 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
--rw-r--r--   0 fschulze   (501) staff       (20)        7 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.984402 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
--rw-r--r--   0 fschulze   (501) staff       (20)        2 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:57.984811 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_upload_default/
--rw-r--r--   0 fschulze   (501) staff       (20)      650 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
--rw-r--r--   0 fschulze   (501) staff       (20)     3040 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6106 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/simpypi.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9275 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2401 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_authcheck.py
--rw-r--r--   0 fschulze   (501) staff       (20)    17684 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1064 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16223 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_filestore.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4355 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_fileutil.py
--rw-r--r--   0 fschulze   (501) staff       (20)      623 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_genconfig.py
--rw-r--r--   0 fschulze   (501) staff       (20)    47340 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_importexport.py
--rw-r--r--   0 fschulze   (501) staff       (20)    31907 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_keyfs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2877 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_keyfs_sqlite_fs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4069 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_log.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13816 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)    50832 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_mirror.py
--rw-r--r--   0 fschulze   (501) staff       (20)    81168 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_model.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1711 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_mythread.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1038 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_nginx_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9617 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_permissions.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4485 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_readonly.py
--rw-r--r--   0 fschulze   (501) staff       (20)    54879 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3133 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_replica_functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1790 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)    16607 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_stage_customizer.py
--rw-r--r--   0 fschulze   (501) staff       (20)     5066 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_streaming.py
--rw-r--r--   0 fschulze   (501) staff       (20)      664 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_streaming_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)      669 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_streaming_replica.py
--rw-r--r--   0 fschulze   (501) staff       (20)      681 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_streaming_replica_nginx.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4932 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_view_auth.py
--rw-r--r--   0 fschulze   (501) staff       (20)   105490 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_views.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3101 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_views_patch.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9464 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_views_push_external.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8899 2022-12-05 10:10:52.000000 devpi-server-6.8.0/test_devpi_server/test_views_status.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1434 2022-12-05 10:10:52.000000 devpi-server-6.8.0/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454745 devpi-server-6.9.0/
+-rw-r--r--   0 fschulze   (501) staff       (20)      138 2023-05-23 14:32:14.000000 devpi-server-6.9.0/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    70739 2023-05-23 14:32:14.000000 devpi-server-6.9.0/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-05-23 14:32:14.000000 devpi-server-6.9.0/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      188 2023-05-23 14:32:14.000000 devpi-server-6.9.0/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     6946 2023-05-23 14:32:20.454864 devpi-server-6.9.0/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     2033 2023-05-23 14:32:14.000000 devpi-server-6.9.0/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.419010 devpi-server-6.9.0/devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       82 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/__main__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7260 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1195 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth_basic.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      958 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/auth_devpi.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.426238 devpi-server-6.9.0/devpi_server/cfg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      213 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/crontab.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      430 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/devpi.service.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      455 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/launchd-macos.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      619 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      237 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-location.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      330 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      341 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-server.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     2065 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/nginx-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      140 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/supervisor-devpi.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)      283 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/supervisord.conf.template
+-rw-r--r--   0 fschulze   (501) staff       (20)     1694 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/cfg/windows-service.txt.template
+-rw-r--r--   0 fschulze   (501) staff       (20)    36715 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      643 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/exceptions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    10069 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8841 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3579 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/fsck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6962 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8555 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    28123 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1926 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/init.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5921 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/interfaces.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    30064 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    24238 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_sqlite.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    11289 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2865 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/keyfs_types.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3751 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    26268 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      952 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/middleware.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    39630 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    74949 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3668 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1642 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/passwd.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7018 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    52077 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1589 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/sizeof.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.426654 devpi-server-6.9.0/devpi_server/vendor/
+-rw-r--r--   0 fschulze   (501) staff       (20)     5030 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/vendor/_pip.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9110 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    75198 2023-05-23 14:32:14.000000 devpi-server-6.9.0/devpi_server/views.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.421715 devpi-server-6.9.0/devpi_server.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     6946 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     4838 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1007 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)      235 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       51 2023-05-23 14:32:20.000000 devpi-server-6.9.0/devpi_server.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      549 2023-05-23 14:32:14.000000 devpi-server-6.9.0/pyproject.toml
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.427025 devpi-server-6.9.0/pytest_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)      863 2023-05-23 14:32:14.000000 devpi-server-6.9.0/pytest_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-05-23 14:32:20.455296 devpi-server-6.9.0/setup.cfg
+-rwxr-xr-x   0 fschulze   (501) staff       (20)     4518 2023-05-23 14:32:14.000000 devpi-server-6.9.0/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.445440 devpi-server-6.9.0/test_devpi_server/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    46442 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      504 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/example.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/functional.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.398379 devpi-server-6.9.0/test_devpi_server/importexportdata/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.445852 devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/
+-rw-r--r--   0 fschulze   (501) staff       (20)      698 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.446250 devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/
+-rw-r--r--   0 fschulze   (501) staff       (20)      719 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.446622 devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/
+-rw-r--r--   0 fschulze   (501) staff       (20)      659 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.447031 devpi-server-6.9.0/test_devpi_server/importexportdata/createdmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      423 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/createdmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.447440 devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1603 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448023 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1413 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394524 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394646 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.394766 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448575 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/
+-rw-r--r--   0 fschulze   (501) staff       (20)      780 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.448954 devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      648 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.449333 devpi-server-6.9.0/test_devpi_server/importexportdata/nocreatedmodified/
+-rw-r--r--   0 fschulze   (501) staff       (20)      485 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/nocreatedmodified/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.449707 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1610 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.395564 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.395680 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450095 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450472 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/
+-rw-r--r--   0 fschulze   (501) staff       (20)     2299 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.396145 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.396426 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.450854 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello-pkg/hello.pkg-1.1.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451235 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        8 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/root/dev/hello.pkg/hello.pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451609 devpi-server-6.9.0/test_devpi_server/importexportdata/norootpypi/
+-rw-r--r--   0 fschulze   (501) staff       (20)      340 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/norootpypi/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.451982 devpi-server-6.9.0/test_devpi_server/importexportdata/nouser/
+-rw-r--r--   0 fschulze   (501) staff       (20)      198 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/nouser/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.452346 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1581 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397219 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397335 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.452725 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/user/dev/pkg/pkg-1.0.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.453086 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1538 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397796 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.397911 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.398213 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.453472 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/
+-rw-r--r--   0 fschulze   (501) staff       (20)        7 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/0.9/hello-0.9.tar.gz
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454054 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/
+-rw-r--r--   0 fschulze   (501) staff       (20)        2 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/root/dev/hello/sha256=ed7002b439e9ac845f22357d822bac1444730fbdb6016d3ec9432297b9ec9f73/hello-0.9.tar.gz.toxresult0
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-05-23 14:32:20.454428 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/
+-rw-r--r--   0 fschulze   (501) staff       (20)      650 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json
+-rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/simpypi.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9275 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2401 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_authcheck.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    17566 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1064 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16223 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_filestore.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4355 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_fileutil.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      623 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_genconfig.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    47791 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_importexport.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    31905 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_keyfs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2877 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_keyfs_sqlite_fs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3965 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_log.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13794 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    51665 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mirror.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8945 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mirror_no_project_list.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    81466 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_model.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1711 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_mythread.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3112 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1210 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_nginx_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9617 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_permissions.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4527 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_readonly.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    56091 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3305 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_replica_functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1790 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    16607 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_stage_customizer.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     5214 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      664 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      669 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_replica.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      681 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_streaming_replica_nginx.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4932 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_view_auth.py
+-rw-r--r--   0 fschulze   (501) staff       (20)   105730 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3101 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_patch.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9465 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_push_external.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8899 2023-05-23 14:32:14.000000 devpi-server-6.9.0/test_devpi_server/test_views_status.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1514 2023-05-23 14:32:14.000000 devpi-server-6.9.0/tox.ini
```

### Comparing `devpi-server-6.8.0/CHANGELOG` & `devpi-server-6.9.0/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 
 
 .. towncrier release notes start
 
+6.9.0 (2023-05-23)
+==================
+
+Features
+--------
+
+- Support export directory layout for ``--replica-file-search-path`` option.
+
+- Fix #931: Add ``mirror_no_project_list`` setting for mirror indexes that have no full project list like google cloud artifacts or if you want to prevent downloading the full list for huge indexes like PyPI.
+
+
+Bug Fixes
+---------
+
+- Keep a reference to async tasks to avoid their removal mid execution.
+
+- Support changed default of ``enforce_content_length`` in urllib3 >= 2.
+
+- Fix #934: Properly set PATH_INFO when outside URL is used with sub-path.
+
+- Fix #945: Adapt FatalError to be usable as an async HTTP response when updating a project on a mirror.
+
+- Fix wrong hash metadata introduced in 6.5.0 for toxresults which prevents replication. The metadata can be fixed by an export/import cycle.
+
+
 6.8.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Fix #929: Cache normalized project names per transaction on mirror index instances.
```

### Comparing `devpi-server-6.8.0/LICENSE` & `devpi-server-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/PKG-INFO` & `devpi-server-6.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.8.0
+Version: 6.9.0
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,39 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.0 (2023-05-23)
+==================
+
+Features
+--------
+
+- Support export directory layout for ``--replica-file-search-path`` option.
+
+- Fix #931: Add ``mirror_no_project_list`` setting for mirror indexes that have no full project list like google cloud artifacts or if you want to prevent downloading the full list for huge indexes like PyPI.
+
+
+Bug Fixes
+---------
+
+- Keep a reference to async tasks to avoid their removal mid execution.
+
+- Support changed default of ``enforce_content_length`` in urllib3 >= 2.
+
+- Fix #934: Properly set PATH_INFO when outside URL is used with sub-path.
+
+- Fix #945: Adapt FatalError to be usable as an async HTTP response when updating a project on a mirror.
+
+- Fix wrong hash metadata introduced in 6.5.0 for toxresults which prevents replication. The metadata can be fixed by an export/import cycle.
+
+
 6.8.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Fix #929: Cache normalized project names per transaction on mirror index instances.
@@ -179,18 +204,7 @@
 
 - Fix #895: store and return content of data-yanked.
 
 - Fix #908: include basic auth from ``mirror_url`` when fetching packages.
 
 - Fix #914: switch to write transaction as late as possible when streaming a file from a mirror.
 
-
-6.5.1 (2022-04-25)
-==================
-
-Bug Fixes
----------
-
-- Fix traceback when trying to delete already deleted release or toxresult.
-
-- Preserve index config settings of plugins during import instead of aborting, even if the plugin isn't installed during import.
-
```

### Comparing `devpi-server-6.8.0/README.rst` & `devpi-server-6.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/auth.py` & `devpi-server-6.9.0/devpi_server/auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/auth_basic.py` & `devpi-server-6.9.0/devpi_server/auth_basic.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/auth_devpi.py` & `devpi-server-6.9.0/devpi_server/auth_devpi.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template` & `devpi-server-6.9.0/devpi_server/cfg/nginx-devpi-caching-http.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/cfg/nginx-devpi.conf.template` & `devpi-server-6.9.0/devpi_server/cfg/nginx-devpi.conf.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/cfg/windows-service.txt.template` & `devpi-server-6.9.0/devpi_server/cfg/windows-service.txt.template`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/config.py` & `devpi-server-6.9.0/devpi_server/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
     if args.configfile:
         config_file = args.configfile
     else:
         config_file = find_config_file()
     try:
         config_options = load_config_file(config_file)
     except InvalidConfigError as e:
-        log.error("Error in config file '%s':\n  %s" % (
+        log.error("Error in config file '%s':\n  %s" % (  # noqa: TRY400
             config_file, e))
         sys.exit(4)
     defaultget = partial(
         default_getter,
         config_options=config_options,
         environ=os.environ)
     parser.post_process_actions(defaultget=defaultget)
@@ -878,20 +878,19 @@
         return (
             self.storage_info['name'] == 'sqlite'
             and not self.serverdir.join(".sqlite").exists()
         )
 
     @cached_property
     def secretfile(self):
-        import warnings
         if not self.args.secretfile:
             secretfile = self.serverdir.join('.secret')
             if not secretfile.check(file=True):
                 return None
-            warnings.warn(
+            log.warn(
                 "Using deprecated existing secret file at '%s', use "
                 "--secretfile to explicitly provide the location." % secretfile)
             return secretfile
         return py.path.local(
             os.path.expanduser(self.args.secretfile))
 
     def get_validated_secret(self):
```

### Comparing `devpi-server-6.8.0/devpi_server/exceptions.py` & `devpi-server-6.9.0/devpi_server/exceptions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/filestore.py` & `devpi-server-6.9.0/devpi_server/filestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,23 +135,20 @@
     def get_file_entry_from_key(self, key, meta=_nodefault, readonly=True):
         return FileEntry(key, meta=meta, readonly=readonly)
 
     def store(self, user, index, basename, content_or_file, dir_hash_spec=None):
         # dir_hash_spec is set for toxresult files
         if dir_hash_spec is None:
             dir_hash_spec = get_default_hash_spec(content_or_file)
-        # prevent hashing twice
-        hash_spec = dir_hash_spec
         hashdir_a, hashdir_b = make_splitdir(dir_hash_spec)
         key = self.keyfs.STAGEFILE(
             user=user, index=index,
             hashdir_a=hashdir_a, hashdir_b=hashdir_b, filename=basename)
         entry = FileEntry(key, readonly=False)
-        entry.file_set_content(
-            content_or_file, hash_spec=hash_spec)
+        entry.file_set_content(content_or_file)
         return entry
 
 
 def metaprop(name):
     def fget(self):
         if self.meta is not None:
             return self.meta.get(name)
```

### Comparing `devpi-server-6.8.0/devpi_server/fileutil.py` & `devpi-server-6.9.0/devpi_server/fileutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,17 +256,18 @@
             nonlocal count
             count += len(data)
             if count > maxlen:
                 raise _SizeError
 
     try:
         _dump(write, obj)
-        return count
     except _SizeError:
         return None
+    else:
+        return count
 
 
 def dumps(obj):
     fp = BytesIO()
     _dump(fp.write, obj)
     return fp.getvalue()
```

### Comparing `devpi-server-6.8.0/devpi_server/fsck.py` & `devpi-server-6.9.0/devpi_server/fsck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/genconfig.py` & `devpi-server-6.9.0/devpi_server/genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/hookspecs.py` & `devpi-server-6.9.0/devpi_server/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/importexport.py` & `devpi-server-6.9.0/devpi_server/importexport.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,19 +83,20 @@
         parser.add_argument("directory")
         config = parseoptions(pluginmanager, argv, parser=parser)
         configure_cli_logging(config.args)
         if not config.path_nodeinfo.exists():
             fatal("The path '%s' contains no devpi-server data, use devpi-init to initialize." % config.serverdir)
         xom = xom_from_config(config)
         do_export(config.args.directory, xom)
-        return 0
     except Fatal as e:
         tw = py.io.TerminalWriter(sys.stderr)
         tw.line("fatal: %s" % e.args[0], red=True)
         return 1
+    else:
+        return 0
 
 
 def do_import(path, xom):
     logging.basicConfig(level=logging.INFO, format='%(message)s')
     path = py.path.local(path)
     tw = py.io.TerminalWriter()
 
@@ -147,19 +148,20 @@
         if not (sdir.exists() and len(sdir.listdir()) >= 2):
             set_state_version(config, DATABASE_VERSION)
         xom = xom_from_config(config, init=True)
         if config.args.wait_for_events:
             xom.thread_pool.start_one(xom.keyfs.notifier)
         init_default_indexes(xom)
         do_import(config.args.directory, xom)
-        return 0
     except Fatal as e:
         tw = py.io.TerminalWriter(sys.stderr)
         tw.line("fatal: %s" % e.args[0], red=True)
         return 1
+    else:
+        return 0
 
 
 class Exporter:
     DUMPVERSION = "2"
 
     def __init__(self, tw, xom):
         self.tw = tw
```

### Comparing `devpi-server-6.8.0/devpi_server/init.py` & `devpi-server-6.9.0/devpi_server/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,12 +41,13 @@
         if config.path_nodeinfo.exists():
             fatal("The path '%s' already contains devpi-server data." % config.serverdir)
         sdir = config.serverdir
         if not (sdir.exists() and len(sdir.listdir()) >= 2):
             set_state_version(config, DATABASE_VERSION)
         xom = xom_from_config(config, init=True)
         init_default_indexes(xom)
-        return 0
     except Fatal as e:
         tw = py.io.TerminalWriter(sys.stderr)
         tw.line("fatal: %s" % e.args[0], red=True)
         return 1
+    else:
+        return 0
```

### Comparing `devpi-server-6.8.0/devpi_server/interfaces.py` & `devpi-server-6.9.0/devpi_server/interfaces.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/keyfs.py` & `devpi-server-6.9.0/devpi_server/keyfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             return conn.last_changelog_serial
 
     def get_last_commit_timestamp(self):
         return self._storage.last_commit_timestamp
 
     @property
     def tx(self):
-        return getattr(self._threadlocal, "tx")
+        return self._threadlocal.tx
 
     def add_key(self, name, path, type):
         assert isinstance(path, str)
         if "{" in path:
             key = PTypedKey(self, path, type, name)
         else:
             key = TypedKey(self, path, type, name)
@@ -457,15 +457,14 @@
             raise RuntimeError("no transaction entry at %s" % (last_serial))
         keyname, back_serial, val = tup
         yield (last_serial, back_serial, val)
         last_serial = back_serial
 
     # we could not find any change below at_serial which means
     # the key didn't exist at that point in time
-    return
 
 
 def iter_relpaths_at(self, typedkeys, at_serial):
     keynames = frozenset(k.name for k in typedkeys)
     seen = set()
     for serial in range(at_serial, -1, -1):
         raw_entry = self.get_raw_changelog_entry(serial)
```

### Comparing `devpi-server-6.8.0/devpi_server/keyfs_sqlite.py` & `devpi-server-6.9.0/devpi_server/keyfs_sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,14 @@
         # with the first successful one
         try:
             # the uri keyword is only supported from Python 3.4 onwards and
             # possibly other Python implementations
             conn = self._get_sqlconn_uri_kw(uri)
             # remember for next time
             self._get_sqlconn = self._get_sqlconn_uri_kw
-            return conn
         except TypeError as e:
             if e.args and 'uri' in e.args[0] and 'keyword argument' in e.args[0]:
                 threadlog.warn(
                     "The uri keyword for 'sqlite3.connect' isn't supported by "
                     "this Python version.")
             else:
                 raise
@@ -392,31 +391,34 @@
             threadlog.warn(
                 "The installed version of sqlite3 doesn't seem to support "
                 "the uri keyword for 'sqlite3.connect'.")
         except sqlite3.NotSupportedError:
             threadlog.warn(
                 "The installed version of sqlite3 doesn't support the uri "
                 "keyword for 'sqlite3.connect'.")
+        else:
+            return conn
         try:
             # sqlite3 might be compiled with default URI support
             conn = self._get_sqlconn_uri(uri)
             # remember for next time
             self._get_sqlconn = self._get_sqlconn_uri
-            return conn
         except sqlite3.OperationalError as e:
             # log the error and switch to using the path
             threadlog.warn("%s" % e)
             threadlog.warn(
                 "Opening the sqlite3 db without options in URI. There is a "
                 "higher possibility of read/write conflicts between "
                 "threads, causing slowdowns due to retries.")
             conn = self._get_sqlconn_path(uri)
             # remember for next time
             self._get_sqlconn = self._get_sqlconn_path
             return conn
+        else:
+            return conn
 
     def get_connection(self, closing=True, write=False, timeout=30):
         # we let the database serialize all writers at connection time
         # to play it very safe (we don't have massive amounts of writes).
         mode = "ro"
         if write:
             mode = "rw"
```

### Comparing `devpi-server-6.8.0/devpi_server/keyfs_sqlite_fs.py` & `devpi-server-6.9.0/devpi_server/keyfs_sqlite_fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,17 +274,16 @@
         if suffix is not None:
             suffix_len = len(suffix)
             dst = path[:-suffix_len]
             if os.path.exists(path):
                 rename(path, dst)
                 threadlog.warn("completed file-commit from crashed tx: %s",
                                dst)
-            else:
-                if not os.path.exists(dst):
-                    raise OSError("missing file %s" % dst)
+            elif not os.path.exists(dst):
+                raise OSError("missing file %s" % dst)
         else:
             try:
                 os.remove(path)  # was already removed
                 threadlog.warn("completed file-del from crashed tx: %s", path)
             except OSError:
                 pass
```

### Comparing `devpi-server-6.8.0/devpi_server/keyfs_types.py` & `devpi-server-6.9.0/devpi_server/keyfs_types.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/log.py` & `devpi-server-6.9.0/devpi_server/log.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/main.py` & `devpi-server-6.9.0/devpi_server/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         while 1:
             try:
                 self.loop.run_forever()
             except Exception:
                 threadlog.exception("Exception in asyncio event loop")
             finally:
                 threadlog.info("The asyncio event loop stopped")
-                return
+            return
 
     def thread_shutdown(self):
         loop = self.loop
         try:
             loop.call_soon_threadsafe(loop.stop)
         except RuntimeError:
             # the shutdown function may have been called already
@@ -216,14 +216,15 @@
     class Exiting(SystemExit):
         pass
 
     def __init__(self, config, httpget=None):
         self.config = config
         self.thread_pool = mythread.ThreadPool()
         self.async_thread = AsyncioLoopThread(self)
+        self.async_tasks = set()
         self.thread_pool.register(self.async_thread)
         if httpget is not None:
             self.httpget = httpget
             self.async_httpget = httpget.async_httpget
         self.log = threadlog
         self.polling_replicas = {}
         self._stagecache = {}
@@ -261,15 +262,19 @@
         future = self._run_coroutine_threadsafe(coroutine, timeout=timeout)
         exc = future.exception()
         if exc:
             raise exc
         return future.result()
 
     def create_task(self, coroutine):
-        asyncio.ensure_future(coroutine, loop=self.async_thread.loop)
+        task = asyncio.ensure_future(coroutine, loop=self.async_thread.loop)
+        # keep a strong reference
+        self.async_tasks.add(task)
+        # automatically remove the reference when done
+        task.add_done_callback(self.async_tasks.discard)
 
     def get_singleton(self, indexpath, key):
         """ return a per-xom singleton for the given indexpath and key
         or raise KeyError if no such singleton was set yet.
         """
         with self._stagecache_lock:
             return self._stagecache[indexpath][key]
@@ -426,15 +431,14 @@
             headers.update(extra_headers)
         try:
             resp = self._httpsession.get(
                 url, stream=True,
                 allow_redirects=allow_redirects,
                 headers=headers,
                 timeout=timeout or self.config.args.request_timeout)
-            return resp
         except OSError as e:
             location = get_caller_location()
             threadlog.warn(
                 "OS error during httpget of %s at %s: %s",
                 url, location, lazy_format_exception_only(e))
             return FatalResponse(url, repr(sys.exc_info()[1]))
         except exceptions.ConnectionError as e:
@@ -445,14 +449,16 @@
             return FatalResponse(url, repr(sys.exc_info()[1]))
         except self._httpsession.Errors as e:
             location = get_caller_location()
             threadlog.warn(
                 "HTTPError during httpget of %s at %s: %s",
                 url, location, lazy_format_exception_only(e))
             return FatalResponse(url, repr(sys.exc_info()[1]))
+        else:
+            return resp
 
     def view_deriver(self, view, info):
         if self.is_replica():
             if info.options.get('is_mutating', True):
                 from .model import ensure_list
                 from .replica import proxy_view_to_master
                 from .views import is_mutating_http_method
@@ -614,18 +620,24 @@
 
 class FatalResponse:
     status_code = -1
 
     def __init__(self, url, reason):
         self.url = url
         self.reason = reason
+        self.status = self.status_code
 
     def __repr__(self):
         return "%s(%r)" % (self.__class__.__name__, self.reason)
 
+    # an adapter to allow this to be used in async_httpget
+    def __iter__(self):
+        yield self
+        yield self.reason
+
     def close(self):
         pass
 
 
 def get_remote_ip(request):
     return request.headers.get("X-REAL-IP", request.client_addr)
```

### Comparing `devpi-server-6.8.0/devpi_server/middleware.py` & `devpi-server-6.9.0/devpi_server/middleware.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,10 @@
             # XXX memoize it for later access from replica thread
             # self.xom.current_outside_url = outside_url
             outside_url = urlparse(outside_url)
             environ['wsgi.url_scheme'] = outside_url.scheme
             environ['HTTP_HOST'] = outside_url.netloc
             if outside_url.path:
                 environ['SCRIPT_NAME'] = outside_url.path
+                if environ['PATH_INFO'].startswith(outside_url.path):
+                    environ['PATH_INFO'] = environ['PATH_INFO'][len(outside_url.path):]
         return self.app(environ, start_response)
```

### Comparing `devpi-server-6.8.0/devpi_server/mirror.py` & `devpi-server-6.9.0/devpi_server/mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 
 """
 
 import asyncio
 import time
 
 import re
-from devpi_common.vendor._pip import HTMLPage
 from devpi_common.url import URL
 from devpi_common.metadata import BasenameMeta
 from devpi_common.metadata import is_archive_of_project
 from devpi_common.metadata import parse_version
 from devpi_common.validation import normalize_name
 from functools import partial
 from html.parser import HTMLParser
 from .config import hookimpl
 from .exceptions import lazy_format_exception
 from .filestore import key_from_link
 from .model import BaseStageCustomizer
 from .model import BaseStage
+from .model import Unknown
 from .model import ensure_boolean
 from .model import join_links_data
 from .readonly import ensure_deeply_readonly
 from .log import threadlog
+from .vendor._pip import HTMLPage
 from .views import SIMPLE_API_V1_JSON
 from .views import make_uuid_headers
 import json
 import threading
 import weakref
 
 
@@ -232,23 +233,31 @@
 
     @property
     def mirror_url_auth(self):
         url = self.mirror_url
         return dict(username=url.username, password=url.password)
 
     @property
+    def no_project_list(self):
+        return self.ixconfig.get('mirror_no_project_list', False)
+
+    @property
     def use_external_url(self):
         return self.ixconfig.get('mirror_use_external_urls', False)
 
     def get_possible_indexconfig_keys(self):
         return tuple(dict(self.get_default_config_items())) + (
-            "custom_data", "description",
-            "mirror_url", "mirror_cache_expiry",
+            "custom_data",
+            "description",
+            "mirror_cache_expiry",
+            "mirror_no_project_list",
+            "mirror_url",
             "mirror_use_external_urls",
-            "mirror_web_url_fmt", "title")
+            "mirror_web_url_fmt",
+            "title")
 
     def get_default_config_items(self):
         return [("volatile", True)]
 
     def normalize_indexconfig_value(self, key, value):
         if key == "volatile":
             return ensure_boolean(value)
@@ -260,14 +269,16 @@
         if key == "mirror_cache_expiry":
             try:
                 value = int(value)
             except (TypeError, ValueError):
                 raise self.InvalidIndexconfig([
                     "'mirror_cache_expiry' option must be an integer"])
             return value
+        if key == "mirror_no_project_list":
+            return ensure_boolean(value)
         if key == "mirror_use_external_urls":
             return ensure_boolean(value)
         if key in ("custom_data", "description", "mirror_web_url_fmt", "title"):
             return value
 
     def delete(self):
         # delete all projects on this index
@@ -423,14 +434,18 @@
         """ Return the cached project names.
 
             Only for internal use which makes sure the data isn't modified.
         """
         if self.offline:
             threadlog.warn("offline mode: using stale projects list")
             return self._stale_list_projects_perstage()
+        if self.no_project_list:
+            # upstream of mirror configured as not having a project list
+            # return only locally known projects
+            return self._stale_list_projects_perstage()
         # try without lock first
         if not self.cache_projectnames.is_expired(self.cache_expiry):
             projects = self.cache_projectnames.get()
         else:
             with self._list_projects_perstage_lock:
                 # retry in case it was updated in another thread
                 if not self.cache_projectnames.is_expired(self.cache_expiry):
@@ -688,19 +703,23 @@
 
         if links is None:
             is_retrieval_expired = self.cache_retrieve_times.is_expired(
                 project, self.cache_expiry)
             if not is_retrieval_expired:
                 raise self.UpstreamNotFoundError(
                     "cached not found for project %s" % project)
-            elif not self.has_project_perstage(project):
-                # immediately cache the not found with no ETag
-                self.cache_retrieve_times.refresh(project, None)
-                raise self.UpstreamNotFoundError(
-                    "project %s not found" % project)
+            else:
+                exists = self.has_project_perstage(project)
+                if exists is Unknown and self.no_project_list:
+                    pass
+                elif not exists:
+                    # immediately cache the not found with no ETag
+                    self.cache_retrieve_times.refresh(project, None)
+                    raise self.UpstreamNotFoundError(
+                        "project %s not found" % project)
 
         newlinks_future = self.xom.create_future()
         # we need to set this up here, as these access the database and
         # the async loop has no transaction
         _key_from_link = partial(
             key_from_link, self.keyfs, user=self.user.name, index=self.index)
         try:
@@ -756,14 +775,18 @@
 
         return self._update_simplelinks(project, info, links, newlinks)
 
     def has_project_perstage(self, project):
         project = normalize_name(project)
         if self.is_project_cached(project):
             return True
+        if self.no_project_list:
+            if project in self._stale_list_projects_perstage():
+                return True
+            return Unknown
         # use the internal method to avoid a copy
         return project in self._list_projects_perstage()
 
     def list_versions_perstage(self, project):
         try:
             return set(x.version for x in self.get_simplelinks_perstage(project))
         except self.UpstreamNotFoundError:
```

### Comparing `devpi-server-6.8.0/devpi_server/model.py` & `devpi-server-6.9.0/devpi_server/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,27 @@
 from .log import threadlog
 from .readonly import get_mutable_deepcopy
 
 
 notset = object()
 
 
+class _Unknown:
+    __slots__ = ()
+
+    def __bool__(self):
+        return False
+
+    def __repr__(self):
+        return "<Unknown>"
+
+
+Unknown = _Unknown()
+
+
 def join_links_data(links, requires_python, yanked):
     # build list of (key, href, require_python, yanked) tuples
     result = []
     links = zip_longest(links, requires_python, yanked, fillvalue=None)
     for link, require_python, yanked in links:
         key, href = link
         result.append((key, href, require_python, yanked))
@@ -535,32 +548,29 @@
         """ Returns value normalized to the type stored in the database.
 
             A return value of None is treated as an error.
             Can raise InvalidIndexconfig.
             Will only be called for custom options, not for existing options
             of a private index.
             """
-        pass
 
     def validate_config(self, oldconfig, newconfig):
         """ Validates the index config.
 
             Can raise InvalidIndexconfig."""
-        pass
 
     def on_modified(self, request, oldconfig):
         """ Called after index was created or modified via a request.
 
             Can do further changes in the current transaction.
 
             Must use request.apifatal method to indicate errors instead
             of raising HTTPException responses.
 
             Other exceptions will be handled."""
-        pass
 
     def get_projects_filter_iter(self, projects):
         """ Called when a list of projects is returned.
 
             Returns None for no filtering, or an iterator returning
             True for items to keep and False for items to remove."""
         return None
@@ -626,14 +636,19 @@
 
     def append(self, item):
         self._links.append(item)
 
     def sort(self, *args, **kw):
         self._links.sort(*args, **kw)
 
+    def __repr__(self):
+        clsname = f"{self.__class__.__module__}.{self.__class__.__name__}"
+        content = ', '.join(repr(x) for x in self._links)
+        return f"<{clsname} stale={self.stale!r} [{content}]>"
+
 
 class BaseStage(object):
     InvalidIndex = InvalidIndex
     InvalidIndexconfig = InvalidIndexconfig
     InvalidUser = InvalidUser
     NotFound = NotFound
     UpstreamError = UpstreamError
@@ -937,38 +952,41 @@
         whitelist_inheritance = self.get_whitelist_inheritance()
         whitelist = None
         for stage in self.sro():
             if stage.ixconfig["type"] == "mirror":
                 if private_hit and not whitelisted:
                     # don't check the mirror for private packages
                     return dict(
-                        has_mirror_base=False,
+                        has_mirror_base=Unknown,
                         blocked_by_mirror_whitelist=stage.name)
                 in_index = stage.has_project_perstage(project)
+                if in_index is Unknown:
+                    return dict(
+                        has_mirror_base=Unknown,
+                        blocked_by_mirror_whitelist=None)
                 has_mirror_base = in_index and (not private_hit or whitelisted)
                 blocked_by_mirror_whitelist = in_index and private_hit and not whitelisted
                 return dict(
                     has_mirror_base=has_mirror_base,
                     blocked_by_mirror_whitelist=stage.name if blocked_by_mirror_whitelist else None)
             else:
                 in_index = stage.has_project_perstage(project)
             private_hit = private_hit or in_index
             stage_whitelist = set(
                 stage.ixconfig.get("mirror_whitelist", set()))
             if whitelist is None:
                 whitelist = stage_whitelist
+            elif whitelist_inheritance == "union":
+                whitelist = whitelist.union(stage_whitelist)
+            elif whitelist_inheritance == "intersection":
+                whitelist = whitelist.intersection(stage_whitelist)
             else:
-                if whitelist_inheritance == "union":
-                    whitelist = whitelist.union(stage_whitelist)
-                elif whitelist_inheritance == "intersection":
-                    whitelist = whitelist.intersection(stage_whitelist)
-                else:
-                    raise RuntimeError(
-                        "Unknown whitelist_inheritance setting '%s'"
-                        % whitelist_inheritance)
+                raise RuntimeError(
+                    "Unknown whitelist_inheritance setting '%s'"
+                    % whitelist_inheritance)
             if whitelisted or whitelist.intersection(('*', project)):
                 whitelisted = True
         return dict(
             has_mirror_base=False,
             blocked_by_mirror_whitelist=None)
 
     def has_mirror_base(self, project):
@@ -980,14 +998,16 @@
             return projects
         return frozenset(apply_filter_iter(projects, iterator))
 
     def has_project(self, project):
         if not self.filter_projects([project]):
             return False
         for stage, res in self.op_sro("has_project_perstage", project=project):
+            if res is Unknown:
+                return res
             if res:
                 return True
         return False
 
     def list_projects(self):
         result = []
         for stage, projects in self.op_sro("list_projects_perstage"):
@@ -1057,30 +1077,33 @@
                     threadlog.debug("private package %r whitelisted at stage %s",
                                     project, whitelisted.name)
             else:
                 stage_whitelist = set(
                     stage.ixconfig.get("mirror_whitelist", set()))
                 if whitelist is None:
                     whitelist = stage_whitelist
+                elif whitelist_inheritance == "union":
+                    whitelist = whitelist.union(stage_whitelist)
+                elif whitelist_inheritance == "intersection":
+                    whitelist = whitelist.intersection(stage_whitelist)
                 else:
-                    if whitelist_inheritance == "union":
-                        whitelist = whitelist.union(stage_whitelist)
-                    elif whitelist_inheritance == "intersection":
-                        whitelist = whitelist.intersection(stage_whitelist)
-                    else:
-                        raise RuntimeError(
-                            "Unknown whitelist_inheritance setting '%s'"
-                            % whitelist_inheritance)
+                    raise RuntimeError(
+                        "Unknown whitelist_inheritance setting '%s'"
+                        % whitelist_inheritance)
                 if whitelist.intersection(('*', project)):
                     whitelisted = stage
                 elif stage.has_project_perstage(project):
                     private_hit = True
 
             try:
-                if not stage.has_project_perstage(project):
+                exists = stage.has_project_perstage(project)
+                if not private_hit and exists is Unknown and stage.no_project_list:
+                    # direct fetching is allowed
+                    pass
+                elif not exists:
                     continue
                 res = getattr(stage, opname)(**kw)
                 yield stage, res
             except self.UpstreamError as exc:
                 # If we are currently checking ourself raise the error, it is fatal
                 if stage is self:
                     raise
@@ -1138,15 +1161,16 @@
             if not callable(method) and permission == 'upload':
                 method = getattr(
                     self.customizer, 'get_principals_for_pypi_submit', None)
                 if callable(method):
                     warnings.warn(
                         "The 'get_principals_for_pypi_submit' method is deprecated, "
                         "you should use 'get_principals_for_upload'. "
-                        "If you want to support older devpi-server versions, add an alias.")
+                        "If you want to support older devpi-server versions, add an alias.",
+                        stacklevel=1)
             if not callable(method):
                 raise AttributeError(
                     "The attribute %s with value %r of %r is not callable." % (
                         method_name, method, self.customizer))
             for principal in get_principals(method(restrict_modify=restrict_modify)):
                 acl.append((Allow, principal, permission))
                 if permission == 'upload':
@@ -1462,15 +1486,16 @@
         return last_serial
 
     # BBB old name for backward compatibility, remove with 6.0.0
     def get_last_change_serial(self, at_serial=None):
         warnings.warn(
             "The get_last_change_serial method is deprecated, "
             "use get_last_change_serial_perstage instead",
-            DeprecationWarning)
+            DeprecationWarning,
+            stacklevel=2)
         return self.get_last_change_serial_perstage(at_serial=at_serial)
 
 
 class StageCustomizer(BaseStageCustomizer):
     pass
 
 
@@ -1709,16 +1734,17 @@
             other = other.cmpval
         return self.cmpval < other
 
     def __getitem__(self, index):
         warnings.warn(
             "Item access for SimplelinkMeta is deprecated, "
             "use attributes instead.",
-            DeprecationWarning)
-        if index == 0:
+            DeprecationWarning,
+            stacklevel=2)
+        if index == 0:  # noqa: SIM116
             return self.key
         elif index == 1:
             return self.href
         elif index == 2:
             return self.require_python
         elif index == 3:
             return self.yanked
@@ -1775,14 +1801,23 @@
         if self.__cmpval is notset:
             self.__cmpval = (
                 parse_version(self.version),
                 normalize_name(self.name),
                 self.ext)
         return self.__cmpval
 
+    def __repr__(self):
+        clsname = f"{self.__class__.__module__}.{self.__class__.__name__}"
+        return (
+            f"<{clsname} "
+            f"key={self.key!r} "
+            f"href={self.href!r} "
+            f"require_python={self.require_python!r} "
+            f"yanked={self.yanked!r}>")
+
 
 def make_key_and_href(entry):
     # entry is either an ELink or a filestore.FileEntry instance.
     # both provide a "relpath" attribute which points to a file entry.
     href = entry.relpath
     if entry.hash_spec:
         href += "#" + entry.hash_spec
```

### Comparing `devpi-server-6.8.0/devpi_server/mythread.py` & `devpi-server-6.9.0/devpi_server/mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/passwd.py` & `devpi-server-6.9.0/devpi_server/passwd.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/readonly.py` & `devpi-server-6.9.0/devpi_server/readonly.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,13 +289,13 @@
 def _(val: tuple) -> tuple:
     return tuple(get_mutable_deepcopy(item) for item in val)
 
 
 def is_deeply_readonly(val: Any) -> bool:
     """ Return True if the value is either immutable or a readonly proxy
     (which ensures only reading of data is possible). """
-    return isinstance(val, ReadonlyView) or isinstance(val, _immutable)
+    return isinstance(val, (ReadonlyView, _immutable))
 
 
 def is_sequence(val: Any) -> bool:
     """ Return True if the value is a readonly or normal sequence (list, tuple)"""
     return isinstance(val, (SeqViewReadonly, list, tuple))
```

### Comparing `devpi-server-6.8.0/devpi_server/replica.py` & `devpi-server-6.9.0/devpi_server/replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
     @view_config(route_name="/+changelog/{serial}-")
     def get_multiple_changes(self):
         acceptable = self.request.accept.acceptable_offers(
             [REPLICA_CONTENT_TYPE, "application/octet-stream"])
         preferres_streaming = (
             (REPLICA_CONTENT_TYPE, 1.0) in acceptable
-            and not ("application/octet-stream", 1.0) in acceptable)
+            and ("application/octet-stream", 1.0) not in acceptable)
         if preferres_streaming:
             # a replica which accepts streams has a lower priority for
             # "application/octet-stream" as the old default "Accept: */*"
             return self.get_streaming_changes()
 
         self.verify_master()
 
@@ -430,15 +430,15 @@
                 allow_redirects=False,
                 auth=self.master_auth,
                 headers=headers,
                 stream=self.use_streaming,
                 timeout=self.REPLICA_REQUEST_TIMEOUT)
         except Exception as e:
             msg = ''.join(traceback.format_exception_only(e.__class__, e)).strip()
-            log.error("error fetching %s: %s", url, msg)
+            log.error("error fetching %s: %s", url, msg)  # noqa: TRY400
             return False
 
         with contextlib.closing(r):
             if r.status_code in (301, 302):
                 log.error(
                     "%s %s: redirect detected at %s to %s",
                     r.status_code, r.reason, url, r.headers.get('Location'))
@@ -471,15 +471,15 @@
                 # force exit of the process
                 os._exit(3)
 
             try:
                 remote_serial = int(r.headers["X-DEVPI-SERIAL"])
             except Exception as e:
                 msg = ''.join(traceback.format_exception_only(e.__class__, e)).strip()
-                log.error("error fetching %s: %s", url, msg)
+                log.error("error fetching %s: %s", url, msg)  # noqa: TRY400
                 return False
 
             if r.status_code == 200:
                 try:
                     handler(r)
                 except mythread.Shutdown:
                     raise
@@ -850,14 +850,21 @@
         return get_auth_serializer(self.xom.config)
 
     def find_pre_existing_file(self, entry):
         if self.file_search_path is None:
             return
         path = os.path.join(self.file_search_path, entry.relpath)
         if not os.path.exists(path):
+            # look for file in export layout
+            path = os.path.join(
+                self.file_search_path,
+                entry.user, entry.index,
+                entry.project, entry.version,
+                entry.basename)
+        if not os.path.exists(path):
             threadlog.debug("path for existing file not found: %s", path)
             return
         threadlog.debug("checking existing file: %s", path)
         f = open(path, "rb")
         hexdigest = get_file_hash(f, entry.hash_type)
         if hexdigest != entry.hash_value:
             f.close()
```

### Comparing `devpi-server-6.8.0/devpi_server/sizeof.py` & `devpi-server-6.9.0/devpi_server/sizeof.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/view_auth.py` & `devpi-server-6.9.0/devpi_server/view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/devpi_server/views.py` & `devpi-server-6.9.0/devpi_server/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from pyramid.response import Response
 from pyramid.security import forget
 from pyramid.threadlocal import RequestContext
 from pyramid.traversal import DefaultRootFactory
 from pyramid.view import exception_view_config
 from pyramid.view import view_config
 from urllib.parse import urlparse
+from urllib3.exceptions import IncompleteRead
 import itertools
 import json
 from devpi_common.request import new_requests_session
 from devpi_common.validation import normalize_name, is_valid_archive_name
 
 from .config import hookimpl
 from .filestore import BadGateway
@@ -180,15 +181,15 @@
     nodeinfo = registry["xom"].config.nodeinfo
 
     def request_log_handler(request):
         tag = f"[req{next(req_count)}]"
         log = thread_push_log(tag)
         try:
             request.log = log
-            log.info("%s %s" % (request.method, request.path,))
+            log.info("%s %s" % (request.method, request.path))
             now = time()
             response = handler(request)
             duration = time() - now
             rheaders = response.headers
             serial = rheaders.get("X-DEVPI-SERIAL")
             rheaders.update(meta_headers)
             uuid, master_uuid = make_uuid_headers(nodeinfo)
@@ -335,17 +336,16 @@
     if status["role"] == "REPLICA":
         master_serial = status["master-serial"]
         if master_serial is not None and master_serial > status["serial"]:
             if status["replica-in-sync-at"] is None or (now - status["replica-in-sync-at"]) > 300:
                 msgs.append(dict(status="fatal", msg="Replica is behind master for more than 5 minutes"))
             elif (now - status["replica-in-sync-at"]) > 60:
                 msgs.append(dict(status="warn", msg="Replica is behind master for more than 1 minute"))
-        else:
-            if len(status["replication-errors"]):
-                msgs.append(dict(status="fatal", msg="Unhandled replication errors"))
+        elif len(status["replication-errors"]):
+            msgs.append(dict(status="fatal", msg="Unhandled replication errors"))
         if status["replica-started-at"] is not None:
             last_update = status["update-from-master-at"]
             if last_update is None:
                 if (now - status["replica-started-at"]) > 300:
                     msgs.append(dict(status="fatal", msg="No contact to master for more than 5 minutes"))
                 elif (now - status["replica-started-at"]) > 60:
                     msgs.append(dict(status="warn", msg="No contact to master for more than 1 minute"))
@@ -727,19 +727,18 @@
             threadlog.error(e.msg)
             abort(self.request, 502, e.msg)
         # at this point we are sure we can produce the data without
         # depending on remote networks
         content_type = _select_simple_content_type(self.request)
         if content_type == SIMPLE_API_V1_JSON:
             app_iter = self._simple_list_all_json_v1(stage, stage_results)
+        elif is_requested_by_installer(self.request):
+            app_iter = self._simple_list_all_installer(stage, stage_results)
         else:
-            if is_requested_by_installer(self.request):
-                app_iter = self._simple_list_all_installer(stage, stage_results)
-            else:
-                app_iter = self._simple_list_all(stage, stage_results)
+            app_iter = self._simple_list_all(stage, stage_results)
         return Response(
             app_iter=buffered_iterator(app_iter),
             content_type=content_type,
             vary=set(["Accept", "User-Agent"]))
 
     def _simple_list_all(self, stage, stage_results):
         title = "%s: simple list (including inherited indices)" % (stage.name)
@@ -1595,15 +1594,18 @@
             threadlog.info("reading remote: %r, target %s", URL(r.url), entry.relpath)
             content_size = r.headers.get("content-length")
             err = None
 
             yield _headers_from_response(r)
 
             while 1:
-                data = r.raw.read(10240)
+                try:
+                    data = r.raw.read(10240)
+                except IncompleteRead as e:
+                    raise BadGateway(str(e)) from e
                 if not data:
                     break
                 filesize += len(data)
                 running_hash.update(data)
                 f.write(data)
                 yield data
 
@@ -1652,15 +1654,15 @@
                     # on Windows we need to close the file
                     # before the transaction closes
                     f.close()
         else:
             # the file was downloaded before but locally removed, so put
             # it back in place without creating a new serial
             # we need a direct write connection to use the io_file_* methods
-            if tx is not None:
+            if tx is not None:  # noqa: PLR5501
                 if not tx.write:
                     xom.keyfs.restart_as_write_transaction()
                 tx.conn.io_file_set(entry._storepath, f)
                 threadlog.debug(
                     "put missing file back into place: %s", entry._storepath)
             else:
                 with xom.keyfs.get_connection(write=True, timeout=300) as conn:
@@ -1708,15 +1710,18 @@
 
     f = entry.tx.conn.io_file_new_open(entry._storepath)
     with contextlib.closing(f):
         with contextlib.closing(r):
             yield _headers_from_response(r)
 
             while 1:
-                data = r.raw.read(10240)
+                try:
+                    data = r.raw.read(10240)
+                except IncompleteRead as e:
+                    raise BadGateway(str(e)) from e
                 if not data:
                     break
                 running_hash.update(data)
                 f.write(data)
                 yield data
 
         err = get_checksum_error(running_hash, entry.relpath, hash_spec)
```

### Comparing `devpi-server-6.8.0/devpi_server.egg-info/PKG-INFO` & `devpi-server-6.9.0/devpi_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-server
-Version: 6.8.0
+Version: 6.9.0
 Summary: devpi-server: reliable private and pypi.org caching server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/server/CHANGELOG
@@ -98,14 +98,39 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+6.9.0 (2023-05-23)
+==================
+
+Features
+--------
+
+- Support export directory layout for ``--replica-file-search-path`` option.
+
+- Fix #931: Add ``mirror_no_project_list`` setting for mirror indexes that have no full project list like google cloud artifacts or if you want to prevent downloading the full list for huge indexes like PyPI.
+
+
+Bug Fixes
+---------
+
+- Keep a reference to async tasks to avoid their removal mid execution.
+
+- Support changed default of ``enforce_content_length`` in urllib3 >= 2.
+
+- Fix #934: Properly set PATH_INFO when outside URL is used with sub-path.
+
+- Fix #945: Adapt FatalError to be usable as an async HTTP response when updating a project on a mirror.
+
+- Fix wrong hash metadata introduced in 6.5.0 for toxresults which prevents replication. The metadata can be fixed by an export/import cycle.
+
+
 6.8.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Fix #929: Cache normalized project names per transaction on mirror index instances.
@@ -179,18 +204,7 @@
 
 - Fix #895: store and return content of data-yanked.
 
 - Fix #908: include basic auth from ``mirror_url`` when fetching packages.
 
 - Fix #914: switch to write transaction as late as possible when streaming a file from a mirror.
 
-
-6.5.1 (2022-04-25)
-==================
-
-Bug Fixes
----------
-
-- Fix traceback when trying to delete already deleted release or toxresult.
-
-- Preserve index config settings of plugins during import instead of aborting, even if the plugin isn't installed during import.
-
```

### Comparing `devpi-server-6.8.0/devpi_server.egg-info/SOURCES.txt` & `devpi-server-6.9.0/devpi_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 devpi_server/cfg/nginx-devpi-caching-location.conf.template
 devpi_server/cfg/nginx-devpi-caching-proxy.conf.template
 devpi_server/cfg/nginx-devpi-caching-server.conf.template
 devpi_server/cfg/nginx-devpi.conf.template
 devpi_server/cfg/supervisor-devpi.conf.template
 devpi_server/cfg/supervisord.conf.template
 devpi_server/cfg/windows-service.txt.template
+devpi_server/vendor/_pip.py
 pytest_devpi_server/__init__.py
 test_devpi_server/__init__.py
 test_devpi_server/conftest.py
 test_devpi_server/example.py
 test_devpi_server/functional.py
 test_devpi_server/reqmock.py
 test_devpi_server/simpypi.py
@@ -73,16 +74,18 @@
 test_devpi_server/test_genconfig.py
 test_devpi_server/test_importexport.py
 test_devpi_server/test_keyfs.py
 test_devpi_server/test_keyfs_sqlite_fs.py
 test_devpi_server/test_log.py
 test_devpi_server/test_main.py
 test_devpi_server/test_mirror.py
+test_devpi_server/test_mirror_no_project_list.py
 test_devpi_server/test_model.py
 test_devpi_server/test_mythread.py
+test_devpi_server/test_nginx.py
 test_devpi_server/test_nginx_replica.py
 test_devpi_server/test_permissions.py
 test_devpi_server/test_readonly.py
 test_devpi_server/test_replica.py
 test_devpi_server/test_replica_functional.py
 test_devpi_server/test_reqmock.py
 test_devpi_server/test_stage_customizer.py
```

### Comparing `devpi-server-6.8.0/devpi_server.egg-info/entry_points.txt` & `devpi-server-6.9.0/devpi_server.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/pyproject.toml` & `devpi-server-6.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/pytest_devpi_server/__init__.py` & `devpi-server-6.9.0/pytest_devpi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/setup.py` & `devpi-server-6.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CHANGELOG = get_changelog()
 
     install_requires = ["py>=1.4.23",
                         "aiohttp!=4.0.0a0,!=4.0.0a1",
                         "argon2-cffi",
                         "attrs>=21.3.0",
                         "defusedxml",
-                        "devpi_common<4,>3.6.0",
+                        "devpi_common<5,>3.6.0",
                         "itsdangerous>=0.24",
                         "platformdirs",
                         "pyramid>=2",
                         "waitress>=1.0.1",
                         "repoze.lru>=0.6",
                         "passlib[argon2]",
                         "pluggy>=0.6.0,<2.0",
@@ -53,20 +53,21 @@
       url="https://devpi.net",
       project_urls={
         'Bug Tracker': 'https://github.com/devpi/devpi/issues',
         'Changelog': 'https://github.com/devpi/devpi/blob/main/server/CHANGELOG',
         'Documentation': 'https://doc.devpi.net',
         'Source Code': 'https://github.com/devpi/devpi'
       },
-      version='6.8.0',
+      version='6.9.0',
       maintainer="Florian Schulze",
       maintainer_email="mail@pyfidelity.com",
       packages=[
         'devpi_server',
         'devpi_server.cfg',
+        'devpi_server.vendor',
         'pytest_devpi_server',
         'test_devpi_server'],
       include_package_data=True,
       zip_safe=False,
       license="MIT",
       classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `devpi-server-6.8.0/test_devpi_server/conftest.py` & `devpi-server-6.9.0/test_devpi_server/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 
 import pytest
 import py
 import requests
 import socket
 import sys
 import time
+from .functional import MappMixin
 from .reqmock import reqmock, patch_reqsessionmock  # noqa
 from bs4 import BeautifulSoup
 from contextlib import closing
 from devpi_server import mirror
 from devpi_server.config import get_pluginmanager
 from devpi_server.main import XOM, parseoptions
 from devpi_common.validation import normalize_name
 from devpi_common.url import URL
 from devpi_server.log import threadlog, thread_clear_log
 from io import BytesIO
 from pyramid.authentication import b64encode
 from pyramid.httpexceptions import status_map
 from queue import Queue as BaseQueue
+from webtest import TestApp as TApp
+from webtest import TestResponse
 import hashlib
 
 
 @pytest.fixture(scope="session")
 def server_version():
     from devpi_server import __version__
     from devpi_common.metadata import parse_version
@@ -134,15 +137,15 @@
     names = request.fixturenames
     if ("xom" not in names and "keyfs" not in names) or (
             request.node.get_closest_marker("notransaction")):
         yield
         return
     keyfs = request.getfixturevalue("keyfs")
 
-    write = True if request.node.get_closest_marker("writetransaction") else False
+    write = bool(request.node.get_closest_marker("writetransaction"))
     keyfs.begin_transaction_in_thread(write=write)
     yield
     try:
         keyfs.rollback_transaction_in_thread()
     except AttributeError:  # already finished within the test
         pass
 
@@ -157,15 +160,14 @@
 def _speed_up_sqlite(cls):
     old = cls.ensure_tables_exist
 
     def make_unsynchronous(self, old=old):
         conn = old(self)
         with self.get_connection() as conn:
             conn._sqlconn.execute("PRAGMA synchronous=OFF")
-        return
 
     cls.ensure_tables_exist = make_unsynchronous
     return old
 
 
 @pytest.fixture(autouse=True, scope="session")
 def speed_up_sqlite():
@@ -206,15 +208,15 @@
 @pytest.fixture(scope="session")
 def storage(storage_info):
     return storage_info['storage']
 
 
 @pytest.fixture
 def makexom(request, gentmp, httpget, monkeypatch, storage_info):
-    def makexom(opts=(), httpget=httpget, plugins=()):
+    def makexom(opts=(), httpget=httpget, plugins=()):  # noqa: PLR0912
         from devpi_server import auth_basic
         from devpi_server import auth_devpi
         from devpi_server import model
         from devpi_server import replica
         from devpi_server import view_auth
         from devpi_server import views
         from devpi_server.interfaces import verify_connection_interface
@@ -481,15 +483,15 @@
     monkeypatch.setattr(
         mirror.MirrorStage, "mock_simple_projects",
         mock_simple_projects, raising=False)
 
     def mock_extfile(self, path, content, **kw):
         headers = {"content-length": len(content),
                    "content-type": mimetypes.guess_type(path),
-                   "last-modified": "today",}
+                   "last-modified": "today"}
         url = URL(self.mirror_url).joinpath(path)
         return self.xom.httpget.mockresponse(
             url.url, content=content, headers=headers, **kw)
     monkeypatch.setattr(
         mirror.MirrorStage, "mock_extfile", mock_extfile, raising=False)
 
 
@@ -505,17 +507,14 @@
 
 
 @pytest.fixture
 def mapp(makemapp, testapp):
     return makemapp(testapp)
 
 
-from .functional import MappMixin
-
-
 class Mapp(MappMixin):
     def __init__(self, testapp):
         self.testapp = testapp
         self.current_stage = ""
 
     def _getindexname(self, indexname):
         if not indexname:
@@ -813,15 +812,15 @@
         assert r.status_code == code
         return r
 
     def get_release_paths(self, project):
         r = self.get_simple(project)
         pkg_url = URL(r.request.url)
         paths = [pkg_url.joinpath(link["href"]).path
-                 for link in BeautifulSoup(r.body, "html.parser").findAll("a")]
+                 for link in BeautifulSoup(r.body, "html.parser").find_all("a")]
         return paths
 
     def upload_doc(self, basename, content, name, version, indexname=None,
                          code=200, waithooks=False):
         indexname = self._getindexname(indexname)
         form = {":action": "doc_upload", "name": name,
                 "content": Upload(basename, content)}
@@ -843,18 +842,14 @@
     def get_simple(self, project, code=200):
         r = self.testapp.get(self.api.simpleindex + project + '/',
                              expect_errors=True)
         assert r.status_code == code
         return r
 
 
-from webtest import TestApp as TApp
-from webtest import TestResponse
-
-
 @pytest.fixture
 def noiter(monkeypatch, request):
     l = []
 
     @property
     def body(self):
         if self.headers["Content-Type"] != "application/octet-stream":
@@ -1181,15 +1176,22 @@
     sendfile        on;
     keepalive_timeout 0;
     include nginx-devpi.conf;
 }
 """
 
 
-def _nginx_host_port(host, port, call_devpi_in_dir, server_directory):
+@pytest.fixture(scope="class")
+def adjust_nginx_conf_content():
+    def adjust_nginx_conf_content(content):
+        return content
+    return adjust_nginx_conf_content
+
+
+def _nginx_host_port(host, port, call_devpi_in_dir, server_directory, adjust_nginx_conf_content):
     # let xproc find the correct executable instead of py.test
     nginx = py.path.local.sysfind("nginx")
     if nginx is None:
         pytest.skip("No nginx executable found.")
     nginx = str(nginx)
 
     orig_dir = server_directory.chdir()
@@ -1205,14 +1207,15 @@
     nginx_directory = server_directory.join("gen-config")
     nginx_devpi_conf = nginx_directory.join("nginx-devpi.conf")
     nginx_port = get_open_port(host)
     nginx_devpi_conf_content = nginx_devpi_conf.read()
     nginx_devpi_conf_content = nginx_devpi_conf_content.replace(
         "listen 80;",
         "listen %s;" % nginx_port)
+    nginx_devpi_conf_content = adjust_nginx_conf_content(nginx_devpi_conf_content)
     nginx_devpi_conf.write(nginx_devpi_conf_content)
     nginx_conf = nginx_directory.join("nginx.conf")
     nginx_conf.write(nginx_conf_content)
     try:
         subprocess.check_output([
             nginx, "-t",
             "-c", nginx_conf.strpath,
@@ -1222,37 +1225,37 @@
         raise
     p = subprocess.Popen([
         nginx, "-c", nginx_conf.strpath, "-p", nginx_directory.strpath])
     return (p, nginx_port)
 
 
 @pytest.fixture(scope="class")
-def nginx_host_port(request, call_devpi_in_dir, server_directory):
+def nginx_host_port(request, call_devpi_in_dir, server_directory, adjust_nginx_conf_content):
     if sys.platform.startswith("win"):
         pytest.skip("no nginx on windows")
     # we need the skip above before master_host_port is called
     (host, port) = request.getfixturevalue("master_host_port")
     (p, nginx_port) = _nginx_host_port(
-        host, port, call_devpi_in_dir, server_directory)
+        host, port, call_devpi_in_dir, server_directory, adjust_nginx_conf_content)
     try:
         wait_for_port(host, nginx_port)
         yield (host, nginx_port)
     finally:
         p.terminate()
         p.wait()
 
 
 @pytest.fixture(scope="class")
-def nginx_replica_host_port(request, call_devpi_in_dir, server_directory):
+def nginx_replica_host_port(request, call_devpi_in_dir, server_directory, adjust_nginx_conf_content):
     if sys.platform.startswith("win"):
         pytest.skip("no nginx on windows")
     # we need the skip above before master_host_port is called
     (host, port) = request.getfixturevalue("replica_host_port")
     (p, nginx_port) = _nginx_host_port(
-        host, port, call_devpi_in_dir, server_directory)
+        host, port, call_devpi_in_dir, server_directory, adjust_nginx_conf_content)
     try:
         wait_for_port(host, nginx_port)
         yield (host, nginx_port)
     finally:
         p.terminate()
         p.wait()
 
@@ -1302,15 +1305,15 @@
 
 class Gen:
     def __init__(self):
         self._md5 = hashlib.md5()
 
     def pypi_package_link(self, pkgname, md5=True):
         link = "https://pypi.org/package/some/%s" % pkgname
-        if md5 == True:
+        if md5 is True:
             self._md5.update(link.encode("utf8"))  # basically random
             link += "#md5=%s" % self._md5.hexdigest()
         elif md5:
             link += "#md5=%s" % md5
         return URL(link)
```

### Comparing `devpi-server-6.8.0/test_devpi_server/functional.py` & `devpi-server-6.9.0/test_devpi_server/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,20 @@
     from urllib import quote as url_quote  # type: ignore
 
 
 class API:
     def __init__(self, d):
         self.__dict__ = d
 
+    def __repr__(self):
+        cls = self.__class__
+        name = "%s.%s" % (cls.__module__, cls.__name__)
+        return "<%s %r>" % (
+            name, self.__dict__.get('stagename', 'uninitialized'))
+
 
 class MappMixin:
     _usercount = 0
 
     def create_and_use(self, stagename=None, password="123", indexconfig=None):
         if stagename is None:
             stagename = self.get_new_stagename()
@@ -338,14 +344,35 @@
         link, = res['result']['1.0']['+links']
         assert len(link['log']) == 1
         assert link['log'][0]['what'] == 'upload'
         assert link['log'][0]['dst'] == '%s/dev' % username
 
 
 @pytest.mark.nomocking
+class TestProjectThings:
+    def test_toxresult(self, mapp):
+        import json
+        mapp.create_and_use('pruser1/dev')
+        content = mapp.makepkg("hello-1.0.tar.gz", b"content", "hello", "1.0")
+        mapp.upload_file_pypi("hello-1.0.tar.gz", content, "hello", "1.0")
+        (pkg_url,) = mapp.getreleaseslist("hello")
+        tox_result_data = dict(foo="bar")
+        mapp.upload_toxresult(pkg_url, json.dumps(tox_result_data))
+        info = mapp.getjson("/%s/hello" % mapp.api.stagename)
+        (toxresult_url,) = [
+            x["href"]
+            for x in info["result"]["1.0"]["+links"]
+            if "for_href" in x]
+        r = mapp.downloadrelease(200, pkg_url)
+        assert r == content
+        r = mapp.downloadrelease(200, toxresult_url)
+        assert json.loads(r.decode('utf-8')) == tox_result_data
+
+
+@pytest.mark.nomocking
 class TestMirrorIndexThings:
     def test_create_and_delete_mirror_index(self, mapp, simpypi):
         mapp.create_and_login_user('mirror1')
         indexname = mapp.auth[0] + "/mirror"
         assert indexname not in mapp.getindexlist()
         indexconfig = dict(
             type="mirror",
```

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/badindexname/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/badindexname/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/badusername/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/badusername/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/basescycle/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/basescycle/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/deletedbase/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/deletedbase/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz` & `devpi-server-6.9.0/test_devpi_server/importexportdata/mirrordata/root/pypi/dddttt/0.1.dev1/dddttt-0.1.dev1.tar.gz`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/modifiedpypi/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/normalization/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/normalization/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/normalization_merge/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/removedindexplugin/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_naming_scheme/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json` & `devpi-server-6.9.0/test_devpi_server/importexportdata/toxresult_upload_default/dataindex.json`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/reqmock.py` & `devpi-server-6.9.0/test_devpi_server/reqmock.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             response = self.url2reply.get((url, None))
             if response is None:
                 for (name, method), response in self.url2reply.items():
                     if method is None or method == request.method:
                         if fnmatch.fnmatch(request.url, name):
                             break
                 else:
-                    raise Exception("not mocked call to %s" % url)
+                    raise Exception("not mocked call to %s" % url)  # noqa: TRY002
         response.add_request(request)
         r = HTTPAdapter().build_response(request, response)
         return r
 
     def mockresponse(self, url, code, method=None, data=None, headers=None,
                      on_request=None, reason=None):
         if not url:
```

### Comparing `devpi-server-6.8.0/test_devpi_server/simpypi.py` & `devpi-server-6.9.0/test_devpi_server/simpypi.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
 class SimPyPI:
     def __init__(self, address):
         self.baseurl = "http://%s:%s" % address
         self.simpleurl = "%s/simple" % self.baseurl
         self.projects = {}
         self.files = {}
+        self.clear()
+
+    def clear(self):
         self.clear_log()
         self.clear_requests()
 
     def clear_log(self):
         self.log = []
 
     def clear_requests(self):
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_auth.py` & `devpi-server-6.9.0/test_devpi_server/test_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_authcheck.py` & `devpi-server-6.9.0/test_devpi_server/test_authcheck.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_config.py` & `devpi-server-6.9.0/test_devpi_server/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,14 @@
         assert config.secretfile is None
         assert config.basesecret != secret
         assert config.basesecret != prev_secret
         recs = caplog.getrecords(".*new random secret.*")
         assert len(recs) == 1
 
     def test_bbb_default_secretfile_location(self, caplog, recwarn, tmpdir):
-        import warnings
-        warnings.simplefilter("always")
         # setup secret file in old default location
         configdir = tmpdir.ensure_dir('config')
         configdir.chmod(0o700)
         p = configdir.join(".secret")
         secret = b"qwoieuqwelkj1234qwoieuqwelkj1234"
         p.write(secret)
         p.chmod(0o600)
@@ -102,16 +100,16 @@
         config = make_config(["devpi-server", "--serverdir", configdir.strpath])
         # the existing file should be used
         assert config.args.secretfile is None
         assert config.secretfile == str(p)
         assert config.basesecret == secret
         recs = caplog.getrecords(".*new random secret.*")
         assert len(recs) == 0
-        (warning,) = [x for x in recwarn if not isinstance(x, ResourceWarning)]
-        assert 'deprecated existing secret' in warning.message.args[0]
+        recs = caplog.getrecords(".*deprecated existing secret.*")
+        assert len(recs) == 1
 
     def test_secret_complexity(self, tmpdir):
         # create a secret file with too short secret
         configdir = tmpdir.ensure_dir('config')
         configdir.chmod(0o700)
         p = configdir.join("secret")
         secret = b"qwoieuqwelkj123"
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_conftest.py` & `devpi-server-6.9.0/test_devpi_server/test_conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_filestore.py` & `devpi-server-6.9.0/test_devpi_server/test_filestore.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_fileutil.py` & `devpi-server-6.9.0/test_devpi_server/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_genconfig.py` & `devpi-server-6.9.0/test_devpi_server/test_genconfig.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_importexport.py` & `devpi-server-6.9.0/test_devpi_server/test_importexport.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from devpi_server.config import hookimpl
 from devpi_server.importexport import Exporter
 from devpi_server.importexport import IndexTree
 from devpi_server.importexport import do_export, do_import
 from devpi_server.main import Fatal
 from devpi_common.archive import Archive, zip_dict
 from devpi_common.metadata import Version
+from devpi_common.types import parse_hash_spec
 from devpi_common.url import URL
 from io import BytesIO
 import importlib.resources
 
 import devpi_server
 
 
@@ -544,21 +545,27 @@
         with mapp.xom.keyfs.transaction(write=False):
             stage = mapp.xom.model.getstage('user/dev')
             assert stage is None
             userconfig = mapp.xom.model.get_user('user').get()
             assert userconfig['indexes'] == {}
 
     def test_upload_releasefile_with_toxresult(self, impexp, tox_result_data):
+        import hashlib
         mapp1 = impexp.mapp1
         api = mapp1.create_and_use()
         content = b'content'
         mapp1.upload_file_pypi("hello-1.0.tar.gz", content, "hello", "1.0")
         path, = mapp1.get_release_paths("hello")
         path = path.strip("/")
-        mapp1.upload_toxresult("/%s" % path, json.dumps(tox_result_data))
+        toxresult_dump = json.dumps(tox_result_data)
+        toxresult_hash = hashlib.sha256(toxresult_dump.encode("utf-8")).hexdigest()
+        r = mapp1.upload_toxresult("/%s" % path, toxresult_dump)
+        toxresult_link = mapp1.getjson(f'/{r.json["result"]}')["result"]
+        (hash_type, hash_value) = parse_hash_spec(toxresult_link["hash_spec"])
+        assert hash_value == toxresult_hash
         impexp.export()
         mapp2 = impexp.new_import()
         with mapp2.xom.keyfs.transaction(write=False):
             stage = mapp2.xom.model.getstage(api.stagename)
             links = stage.get_releaselinks("hello")
             assert len(links) == 1
             assert links[0].entry.file_get_content() == b"content"
@@ -570,14 +577,15 @@
             assert history_log[0]['dst'] == 'user1/dev'
             results = stage.get_toxresults(link)
             assert len(results) == 1
             assert results[0] == tox_result_data
             linkstore = stage.get_linkstore_perstage(
                 link.project, link.version)
             tox_link, = linkstore.get_links(rel="toxresult", for_entrypath=link)
+            assert tox_link.hash_value == toxresult_hash
             history_log = tox_link.get_logs()
             assert len(history_log) == 1
             assert history_log[0]['what'] == 'upload'
             assert history_log[0]['who'] == 'user1'
             assert history_log[0]['dst'] == 'user1/dev'
 
     def test_import_with_old_toxresult_naming_scheme(self, impexp):
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_keyfs.py` & `devpi-server-6.9.0/test_devpi_server/test_keyfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @pytest.fixture
 def keyfs(gentmp, pool, storage):
     keyfs = KeyFS(gentmp(), storage)
     pool.register(keyfs.notifier)
     yield keyfs
 
 
-@pytest.fixture(params=["direct", "a/b/c", ])
+@pytest.fixture(params=["direct", "a/b/c"])
 def key(request):
     return request.param
 
 
 @pytest.fixture
 def pool():
     pool = ThreadPool()
@@ -794,15 +794,15 @@
 
         # directly  modify the database without keyfs-transaction machinery
         with keyfs._storage.get_connection(write=True) as conn:
             with conn.write_transaction():
                 pass
 
         # check wait_tx_serial() call from the thread returned True
-        assert queue.get() == True
+        assert queue.get() is True
 
     def test_wait_tx_async_timeout(self, keyfs):
         wait_serial = keyfs.get_next_serial()
         assert not keyfs.wait_tx_serial(wait_serial, timeout=0.001, recheck=0.0001)
 
     def test_commit_serial(self, keyfs):
         with keyfs.transaction() as tx:
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_keyfs_sqlite_fs.py` & `devpi-server-6.9.0/test_devpi_server/test_keyfs_sqlite_fs.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_log.py` & `devpi-server-6.9.0/test_devpi_server/test_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         config = make_config(["devpi-server"])
         configure_logging(config.args)
 
         assert logging.getLogger().getEffectiveLevel() == logging.INFO
         level = logging.getLogger("requests.packages.urllib3").getEffectiveLevel()
         assert level == logging.ERROR
 
-    @pytest.mark.skipif("sys.version_info < (2,7)")
     def test_logger_cfg_json(self, tmpdir):
         logger_cfg = tmpdir.join("logging.json")
         logger_cfg.write(textwrap.dedent("""
             {
                 "version": 1,
                 "disable_existing_loggers": false,
                 "root": {
@@ -119,15 +118,14 @@
         """))
         config = make_config(["devpi-server", "--logger-cfg=%s" % logger_cfg])
         configure_logging(config.args)
 
         assert logging.getLogger().getEffectiveLevel() == logging.WARNING
         assert not logging.getLogger().handlers
 
-    @pytest.mark.skipif("sys.version_info < (2,7)")
     def test_logger_cfg_yaml(self, tmpdir):
         logger_cfg = tmpdir.join("logging.yml")
         logger_cfg.write(textwrap.dedent("""
             version: 1
             disable_existing_loggers: False
 
             root:
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_main.py` & `devpi-server-6.9.0/test_devpi_server/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         ["devpi-server", "--serverdir", serverdir.strpath])
 
 
 def test_pkgresources_version_matches_init():
     try:
         import importlib.metadata as importlib_metadata
     except ImportError:
-        import importlib_metadata as importlib_metadata
+        import importlib_metadata
     ver = devpi_server.__version__
     assert importlib_metadata.version("devpi-server") == ver
 
 
 def test_version(capfd):
     main(["devpi-server", "--version"])
     out, err = capfd.readouterr()
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_mirror.py` & `devpi-server-6.9.0/test_devpi_server/test_mirror.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from devpi_server.mirror import URL, parse_index
 from devpi_server.mirror import ProjectNamesCache, ProjectUpdateCache
 from test_devpi_server.simpypi import getmd5
 
 
 def getlinks(text):
     from bs4 import BeautifulSoup
-    return BeautifulSoup(text, "html.parser").findAll("a")
+    return BeautifulSoup(text, "html.parser").find_all("a")
 
 
 class TestIndexParsing:
     simplepy = URL("https://pypi.org/simple/py/")
 
     @pytest.mark.parametrize("hash_type,hash_value", [
         ("sha256", "090123"),
@@ -969,14 +969,41 @@
         yield
 
     monkeypatch.setattr(aiohttp.ClientSession, "get", async_httpget)
     r = await xom.async_httpget("http://notexists.qwe", allow_redirects=False)
     assert r.status_code == -1
 
 
+@pytest.mark.asyncio
+@pytest.mark.nomocking
+@pytest.mark.parametrize("exc", [
+    OSError,
+    aiohttp.ClientError])
+async def test_get_simplelinks_perstage_when_http_error(exc, pypistage, monkeypatch):
+    from contextlib import asynccontextmanager
+    from devpi_server.model import SimpleLinks
+
+    # to reach the code path in question, we must have cached links
+    links = [("key", "href", "req_py", "yanked")]
+
+    def mock_load_cache_links(project):
+        return (True, links, 42)
+
+    monkeypatch.setattr(pypistage, "_load_cache_links", mock_load_cache_links)
+
+    @asynccontextmanager
+    async def async_httpget(self, url, **kw):
+        raise exc()
+        yield
+
+    monkeypatch.setattr(aiohttp.ClientSession, "get", async_httpget)
+
+    assert pypistage.get_simplelinks_perstage("def_missing") == SimpleLinks(links)
+
+
 def test_is_project_cached(pypistage):
     assert not pypistage.is_project_cached("xyz")
     assert not pypistage.has_project("xyz")
     assert not pypistage.is_project_cached("xyz")
 
     pypistage.mock_simple("abc", text="")
     assert not pypistage.is_project_cached("abc")
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_model.py` & `devpi-server-6.9.0/test_devpi_server/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 
 from devpi_common.metadata import splitbasename
 from devpi_common.archive import Archive, zip_dict
 from devpi_server.config import hookimpl
 from devpi_server.model import InvalidIndexconfig
 from devpi_server.model import PrivateStage
+from devpi_server.model import Unknown
 from devpi_server.model import ensure_boolean
 from devpi_server.model import ensure_acl_list
 from devpi_server.model import ensure_list
 from devpi_server.model import run_passwd
 from devpi_server.model import StageCustomizer
 from io import BytesIO
 
@@ -96,29 +97,29 @@
         blocked_by_mirror_whitelist=None)
     stage2 = user.create_stage("stage2", bases=("root/pypi",))
     assert stage2.get_mirror_whitelist_info("pytest") == dict(
         has_mirror_base=True,
         blocked_by_mirror_whitelist=None)
     register_and_store(stage2, "pytest-1.1.tar.gz")
     assert stage2.get_mirror_whitelist_info("pytest") == dict(
-        has_mirror_base=False,
+        has_mirror_base=Unknown,
         blocked_by_mirror_whitelist='root/pypi')
     # now add to whitelist
     ixconfig = stage2.ixconfig.copy()
     ixconfig["mirror_whitelist"] = ["pytest"]
     stage2.modify(**ixconfig)
     assert stage2.get_mirror_whitelist_info("pytest") == dict(
         has_mirror_base=True,
         blocked_by_mirror_whitelist=None)
     # now remove from whitelist
     ixconfig = stage2.ixconfig.copy()
     ixconfig["mirror_whitelist"] = []
     stage2.modify(**ixconfig)
     assert stage2.get_mirror_whitelist_info("pytest") == dict(
-        has_mirror_base=False,
+        has_mirror_base=Unknown,
         blocked_by_mirror_whitelist='root/pypi')
     # and try "*"
     ixconfig = stage2.ixconfig.copy()
     ixconfig["mirror_whitelist"] = ["*"]
     stage2.modify(**ixconfig)
     assert stage2.get_mirror_whitelist_info("pytest") == dict(
         has_mirror_base=True,
@@ -134,15 +135,15 @@
     # test that getting the whitelist info doesn't reveal package name, see #451
     with mapp.xom.keyfs.transaction(write=False):
         with monkeypatch.context() as m:
             # make sure we get an error if data is fetched
             m.setattr(mapp.xom, 'httpget', None)
             stage = mapp.xom.model.getstage(api.stagename)
             info = stage.get_mirror_whitelist_info("pkg1")
-            assert info['has_mirror_base'] is False
+            assert info['has_mirror_base'] is Unknown
             assert info['blocked_by_mirror_whitelist'] == "root/pypi"
     mapp.use("root/pypi")
     mapp.xom.httpget.mockresponse(
         "https://pypi.org/simple/", text='<a href="pkg1"></a>')
     mapp.xom.httpget.mock_simple("pkg1", text="")
     mapp.get_simple("pkg1")
     with mapp.xom.keyfs.transaction(write=False):
@@ -152,15 +153,15 @@
             pypistage = mapp.xom.model.getstage("root/pypi")
             # expire the project data, otherwise we wouldn't fetch data
             # by accident
             pypistage.cache_retrieve_times.expire("pkg1")
             # now we check that we get correct info without fetching data
             stage = mapp.xom.model.getstage(api.stagename)
             info = stage.get_mirror_whitelist_info("pkg1")
-            assert info['has_mirror_base'] is False
+            assert info['has_mirror_base'] is Unknown
             assert info['blocked_by_mirror_whitelist'] == "root/pypi"
     # now we whitelist the package
     testapp.patch_json("/" + api.stagename, ["mirror_whitelist+=pkg1"])
     with mapp.xom.keyfs.transaction(write=False):
         stage = mapp.xom.model.getstage(api.stagename)
         info = stage.get_mirror_whitelist_info("pkg1")
         assert info['has_mirror_base'] is True
@@ -208,23 +209,23 @@
     def test_not_configured_index(self, model):
         stagename = "hello/world"
         assert model.getstage(stagename) is None
 
     def test_indexconfig_set_throws_on_unknown_base_index(self, stage, user):
         with pytest.raises(InvalidIndexconfig) as excinfo:
             user.create_stage(index="something",
-                              bases=("root/notexists", "root/notexists2"),)
+                              bases=("root/notexists", "root/notexists2"))
         messages = excinfo.value.messages
         assert len(messages) == 2
         assert "root/notexists" in messages[0]
         assert "root/notexists2" in messages[1]
 
     def test_indexconfig_set_throws_on_invalid_base_index(self, stage, user):
         with pytest.raises(InvalidIndexconfig) as excinfo:
-            user.create_stage(index="world3", bases=("root/dev/123",),)
+            user.create_stage(index="world3", bases=("root/dev/123",))
         messages = excinfo.value.messages
         assert len(messages) == 1
         assert "root/dev/123" in messages[0]
 
     def test_indexconfig_set_normalizes_bases(self, user):
         stage = user.create_stage(index="world", bases=("/root/pypi/",))
         assert stage.ixconfig["bases"] == ("root/pypi",)
@@ -1374,28 +1375,33 @@
         linkstore.create_linked_entry(
             rel="doczip", basename="proj1-1.0.doc.zip",
             content_or_file=b'123')
         link, = linkstore.get_links(rel="releasefile")
         assert link.entrypath.endswith("proj1-1.0.zip")
 
     def test_toxresult_create_remove(self, linkstore):
+        import hashlib
         linkstore.create_linked_entry(
             rel="releasefile", basename="proj1-1.0.zip",
             content_or_file=b'123')
         linkstore.create_linked_entry(
             rel="releasefile", basename="proj1-1.1.zip",
             content_or_file=b'456')
         (link1, link2) = linkstore.get_links(rel="releasefile")
         assert link1.entrypath.endswith("proj1-1.0.zip")
 
-        linkstore.new_reflink(rel="toxresult", content_or_file=b'123', for_entrypath=link1)
-        linkstore.new_reflink(rel="toxresult", content_or_file=b'456', for_entrypath=link2)
+        tox_content1 = b'tox123'
+        linkstore.new_reflink(rel="toxresult", content_or_file=tox_content1, for_entrypath=link1)
+        tox_content2 = b'tox456'
+        linkstore.new_reflink(rel="toxresult", content_or_file=tox_content2, for_entrypath=link2)
         rlink, = linkstore.get_links(rel="toxresult", for_entrypath=link1)
+        assert rlink.hash_value == hashlib.sha256(tox_content1).hexdigest()
         assert rlink.for_entrypath == link1.entrypath
         rlink, = linkstore.get_links(rel="toxresult", for_entrypath=link2)
+        assert rlink.hash_value == hashlib.sha256(tox_content2).hexdigest()
         assert rlink.for_entrypath == link2.entrypath
 
         link1_entry = link1.entry  # queried below
 
         # remove one release link, which should removes its toxresults
         # and check that the other release and its toxresult is still there
         linkstore.remove_links(rel="releasefile", basename="proj1-1.0.zip")
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_mythread.py` & `devpi-server-6.9.0/test_devpi_server/test_mythread.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_nginx_replica.py` & `devpi-server-6.9.0/test_devpi_server/test_nginx_replica.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .functional import TestProjectThings as BaseTestProjectThings
 from .functional import TestUserThings as BaseTestUserThings
 from .functional import TestIndexThings as BaseTestIndexThings
 from .functional import TestIndexPushThings as BaseTestIndexPushThings
 from .functional import TestMirrorIndexThings as BaseTestMirrorIndexThings
 import pytest
 
 
@@ -14,14 +15,19 @@
     try:
         yield app
     finally:
         app.xom.thread_pool.shutdown()
 
 
 @pytest.mark.skipif("not config.option.slow")
+class TestProjectThings(BaseTestProjectThings):
+    pass
+
+
+@pytest.mark.skipif("not config.option.slow")
 class TestUserThings(BaseTestUserThings):
     pass
 
 
 @pytest.mark.skipif("not config.option.slow")
 class TestIndexThings(BaseTestIndexThings):
     pass
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_permissions.py` & `devpi-server-6.9.0/test_devpi_server/test_permissions.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_readonly.py` & `devpi-server-6.9.0/test_devpi_server/test_readonly.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         d = {1: 2}
         r = ensure_deeply_readonly(d)
         assert r[1] == 2
         with pytest.raises(KeyError):
             r[2]
         assert len(r) == 1
         assert r == d
-        assert not (r != d)
+        assert not (r != d)  # noqa: SIM202 - we want to check __ne__
 
     def test_recursive(self) -> None:
         d: dict = {1: []}
         r = ensure_deeply_readonly(d)
         assert r[1] == []
         with pytest.raises(AttributeError):
             r[1].append(1)
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_replica.py` & `devpi-server-6.9.0/test_devpi_server/test_replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,14 +482,37 @@
         # now sync the replica, if the file is not found there will be an error
         # because httpget is mocked
         caplog.clear()
         replay(xom, replica_xom, events=False)
         replica_xom.replica_thread.wait()
         assert len(caplog.getrecords('checking existing file')) == 1
 
+    def test_use_existing_files_export_layout(self, caplog, make_replica_xom, mapp, monkeypatch, tmpdir, xom):
+        # this will be the folder to find existing files in the replica
+        existing_base = tmpdir.join('existing').ensure_dir()
+        # prepare data on master
+        mapp.create_and_use()
+        content1 = mapp.makepkg("hello-1.0.zip", b"content1", "hello", "1.0")
+        mapp.upload_file_pypi("hello-1.0.zip", content1, "hello", "1.0")
+        # get the path of the release in export layout
+        existing_path = existing_base.join(
+            mapp.api.stagename, "hello", "1.0", "hello-1.0.zip")
+        # create the file
+        existing_path.dirpath().ensure_dir()
+        existing_path.write_binary(content1)
+        # create the replica with the path to existing files
+        replica_xom = make_replica_xom(options=[
+            '--replica-file-search-path', existing_base.strpath])
+        # now sync the replica, if the file is not found there will be an error
+        # because httpget is mocked
+        caplog.clear()
+        replay(xom, replica_xom, events=False)
+        replica_xom.replica_thread.wait()
+        assert len(caplog.getrecords('checking existing file')) == 1
+
     @pytest.mark.storage_with_filesystem
     @pytest.mark.skipif(not hasattr(os, 'link'),
                         reason="OS doesn't support hard links")
     def test_hardlink(self, caplog, make_replica_xom, mapp, monkeypatch, tmpdir, xom):
         # this will be the folder to find existing files in the replica
         existing_base = tmpdir.join('existing').ensure_dir()
         # prepare data on master
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_replica_functional.py` & `devpi-server-6.9.0/test_devpi_server/test_replica_functional.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .functional import TestProjectThings as BaseTestProjectThings
 from .functional import TestUserThings as BaseTestUserThings
 from .functional import TestIndexThings as BaseTestIndexThings
 from .functional import TestIndexPushThings as BaseTestIndexPushThings
 from .functional import TestMirrorIndexThings as BaseTestMirrorIndexThings
 import pytest
 
 
@@ -19,14 +20,19 @@
 @pytest.fixture
 def mapp(replica_mapp):
     replica_mapp.xom.thread_pool.start_one(replica_mapp.xom.replica_thread)
     return replica_mapp
 
 
 @pytest.mark.skipif("not config.option.slow")
+class TestProjectThings(BaseTestProjectThings):
+    pass
+
+
+@pytest.mark.skipif("not config.option.slow")
 class TestUserThings(BaseTestUserThings):
     pass
 
 
 @pytest.mark.skipif("not config.option.slow")
 class TestIndexThings(BaseTestIndexThings):
     pass
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_reqmock.py` & `devpi-server-6.9.0/test_devpi_server/test_reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_stage_customizer.py` & `devpi-server-6.9.0/test_devpi_server/test_stage_customizer.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_streaming.py` & `devpi-server-6.9.0/test_devpi_server/test_streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                 break
             sleep(0.1)
         assert pkg_file.exists()
 
     @pytest.mark.parametrize("size_factor,pkg_version,pkg_name", [
         (2, '1.2', 'pkg3'), (0.5, '1.3', 'pkg4')])
     def test_streaming_differing_content_size(self, content_digest, files_directory, pkg_version, pkg_name, server_url_session, simpypi, size_factor, storage_info):
+        from requests.exceptions import ChunkedEncodingError
         if "storage_with_filesystem" not in storage_info.get('_test_markers', []):
             pytest.skip("The storage doesn't have marker 'storage_with_filesystem'.")
         (content, digest) = content_digest
         (url, s) = server_url_session
         pkgzip = f"{pkg_name}-{pkg_version}.zip"
         length = int(len(content) * size_factor)
         simpypi.add_release(pkg_name, pkgver='%s#sha256=%s' % (pkgzip, digest))
@@ -114,13 +115,16 @@
             stream = r.iter_content(1024)
             data = next(stream)
             assert data == b'deadbeaf' * 128
             part = next(stream)
             assert part == b'sandwich' * 128
             data = data + part
             assert r.headers['content-length'] == str(length)
-            for part in stream:
-                data = data + part
+            try:
+                for part in stream:
+                    data = data + part
+            except ChunkedEncodingError:
+                pass
             assert data == content[:length]
         pkg_file = files_directory.join(
             'root', 'pypi', '+f', digest[:3], digest[3:16], pkgzip)
         assert not pkg_file.exists()
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_streaming_nginx.py` & `devpi-server-6.9.0/test_devpi_server/test_streaming_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_streaming_replica.py` & `devpi-server-6.9.0/test_devpi_server/test_streaming_replica.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_streaming_replica_nginx.py` & `devpi-server-6.9.0/test_devpi_server/test_streaming_replica_nginx.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_view_auth.py` & `devpi-server-6.9.0/test_devpi_server/test_view_auth.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_views.py` & `devpi-server-6.9.0/test_devpi_server/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 from devpi_common.viewhelp import ViewLinkStore
 
 import devpi_server.views
 from devpi_server.config import hookimpl
 from devpi_server.views import tween_keyfs_transaction, make_uuid_headers
 from devpi_server.mirror import parse_index
 from io import BytesIO
-from .functional import TestUserThings, TestIndexThings, TestIndexPushThings  # noqa
-from .functional import TestMirrorIndexThings  # noqa
+from .functional import TestIndexThings  # noqa: F401
+from .functional import TestIndexPushThings  # noqa: F401
+from .functional import TestProjectThings  # noqa: F401
+from .functional import TestUserThings  # noqa: F401
+from .functional import TestMirrorIndexThings  # noqa: F401
 
 import devpi_server.filestore
 from devpi_server.filestore import get_default_hash_spec, make_splitdir
 
 proj = pytest.mark.parametrize("proj", [True, False])
 pytestmark = [pytest.mark.notransaction]
 
 
 def getlinks(text):
-    return BeautifulSoup(text, "html.parser").findAll("a")
+    return BeautifulSoup(text, "html.parser").find_all("a")
 
 
 def getfirstlink(text):
     return getlinks(text)[0]
 
 
 def getentry(testapp, path):
@@ -157,39 +160,39 @@
 
 def test_simple_project_requires_python(pypistage, testapp):
     name = "django"
     path = "/%s-2.0.tar.gz" % name
     pypistage.mock_simple(name, text='<a href="%s" data-requires-python="&gt;=3.4" />' % path)
     r = testapp.get("/root/pypi/+simple/%s/" % name)
     assert r.status_code == 200
-    links = BeautifulSoup(r.text, "html.parser").findAll("a")
+    links = BeautifulSoup(r.text, "html.parser").find_all("a")
     assert len(links) == 1
     assert links[0].get("href").endswith(path)
     assert links[0].get("data-requires-python") == '>=3.4'
 
 
 def test_simple_project_requires_python_empty(pypistage, testapp):
     name = "django"
     path = "/%s-2.0.tar.gz" % name
     pypistage.mock_simple(name, text='<a href="%s" data-requires-python="" />' % path)
     r = testapp.get("/root/pypi/+simple/%s/" % name)
     assert r.status_code == 200
-    links = BeautifulSoup(r.text, "html.parser").findAll("a")
+    links = BeautifulSoup(r.text, "html.parser").find_all("a")
     assert len(links) == 1
     assert links[0].get("href").endswith(path)
     assert links[0].get("data-requires-python") is None
 
 
 def test_simple_project_yanked(pypistage, testapp):
     name = "django"
     path = "/%s-2.0.tar.gz" % name
     pypistage.mock_simple(name, text='<a href="%s" data-yanked="" />' % path)
     r = testapp.get("/root/pypi/+simple/%s/" % name)
     assert r.status_code == 200
-    links = BeautifulSoup(r.text, "html.parser").findAll("a")
+    links = BeautifulSoup(r.text, "html.parser").find_all("a")
     assert len(links) == 1
     assert links[0].get("href").endswith(path)
     assert links[0].get("data-yanked") == ""
 
 
 def test_simple_project_yanked_true(pypistage, testapp):
     name = "django"
@@ -201,15 +204,15 @@
                     "yanked": True,
                     "filename": path,
                     "url": path,
                     "hashes": []}]}),
         headers={"content-type": "application/vnd.pypi.simple.v1+json"})
     r = testapp.get("/root/pypi/+simple/%s/" % name)
     assert r.status_code == 200
-    links = BeautifulSoup(r.text, "html.parser").findAll("a")
+    links = BeautifulSoup(r.text, "html.parser").find_all("a")
     assert len(links) == 1
     assert links[0].get("href").endswith(path)
     assert links[0].get("data-yanked") == ""
 
 
 def test_simple_list_all_redirect(pypistage, testapp):
     r = testapp.get("/root/pypi/+simple", follow=False)
@@ -1201,25 +1204,23 @@
         submit.metadata(metadata, code=200)
         mapp.getjson("/%s/pkg1" % submit.stagename, code=200)
         #assert location.endswith("/Pkg1")
 
 
 def test_submit_authorization(mapp, testapp):
     from base64 import b64encode
-    import sys
     api = mapp.create_and_use()
     testapp.auth = None
     data = {':action': 'submit', "name": "Pkg1", "version": "1.0"}
     r = testapp.post(api.index + '/', data, expect_errors=True)
     assert r.status_code == 401
     assert 'WWW-Authenticate' in r.headers
     basic_auth = '%s:%s' % (api.user, api.password)
     basic_auth = b"Basic " + b64encode(basic_auth.encode("ascii"))
-    if sys.version_info[0] >= 3:
-        basic_auth = basic_auth.decode("ascii")
+    basic_auth = basic_auth.decode("ascii")
     headers = {'Authorization': basic_auth}
     r = testapp.post(api.index + '/', data, headers=headers)
     assert r.status_code == 200
 
 
 def test_submit_without_trailing_slash(mapp, testapp):
     # the regular target URL for uploads ends in a slash, the target
@@ -2252,53 +2253,54 @@
     api = mapp.getapi()
     r = testapp.post(api.login, "qweqweqwe", expect_errors=True)
     assert r.status_code == 400
     r = testapp.post_json(api.login, {"qwelk": ""}, expect_errors=True)
     assert r.status_code == 400
 
 
-@pytest.mark.parametrize("headers, environ, outsideurl, expected", [
+@pytest.mark.parametrize("headers, environ, path, outsideurl, expected", [
     (
-        {"X-outside-url": "http://outside.com"}, {},
+        {"X-outside-url": "http://outside.com"}, {}, "",
         None, "http://outside.com"),
     (
-        {"X-outside-url": "http://outside.com/foo"}, {},
+        {"X-outside-url": "http://outside.com/foo"}, {}, "/foo",
         None, "http://outside.com/foo"),
     (
-        {"Host": "outside3.com"}, {},
+        {"Host": "outside3.com"}, {}, "",
         None, "http://outside3.com"),
     (
-        {"Host": "outside3.com"}, {'wsgi.url_scheme': 'https'},
+        {"Host": "outside3.com"}, {'wsgi.url_scheme': 'https'}, "",
         None, "https://outside3.com"),
     (
-        {"Host": "outside3.com:3141"}, {},
+        {"Host": "outside3.com:3141"}, {}, "",
         None, "http://outside3.com:3141"),
     (
-        {"Host": "outside3.com:3141"}, {'wsgi.url_scheme': 'https'},
+        {"Host": "outside3.com:3141"}, {'wsgi.url_scheme': 'https'}, "",
         None, "https://outside3.com:3141"),
     # x-outside-url header takes precedence over outside url option
     (
-        {"X-outside-url": "http://outside.com"}, {},
+        {"X-outside-url": "http://outside.com"}, {}, "",
         "http://outside2.com", "http://outside.com"),
     (
-        {"X-outside-url": "http://outside.com"}, {},
+        {"X-outside-url": "http://outside.com"}, {}, "",
         "http://outside2.com/foo", "http://outside.com"),
     # outside url option takes precedence over host and environ
     (
-        {"Host": "outside3.com"}, {},
+        {"Host": "outside3.com"}, {}, "",
         "http://out.com", "http://out.com"),
     (
-        {"Host": "outside3.com"}, {'wsgi.url_scheme': 'https'},
+        {"Host": "outside3.com"}, {'wsgi.url_scheme': 'https'}, "",
         "http://out.com", "http://out.com")])
-def test_outside_url_middleware(headers, environ, outsideurl, expected, testapp):
+def test_outside_url_middleware(headers, environ, path, outsideurl, expected, testapp):
     headers = dict((str(k), str(v)) for k, v in headers.items())
     environ = dict((str(k), str(v)) for k, v in environ.items())
     testapp.xom.config.args.outside_url = outsideurl
-    r = testapp.get('/+api', headers=headers, extra_environ=environ)
+    r = testapp.get(f'{path}/+api', headers=headers, extra_environ=environ)
     assert r.json['result']['login'] == "%s/+login" % expected
+    testapp.xget(200, path, headers=headers, extra_environ=environ, follow=False)
 
 
 class TestOfflineMode:
     @pytest.fixture
     def xom(self, makexom):
         return makexom(["--offline-mode"])
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_views_patch.py` & `devpi-server-6.9.0/test_devpi_server/test_views_patch.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/test_devpi_server/test_views_push_external.py` & `devpi-server-6.9.0/test_devpi_server/test_views_push_external.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pytest
 
 
 pytestmark = [pytest.mark.notransaction]
 
 
 def getfirstlink(text):
-    return BeautifulSoup(text, "html.parser").findAll("a")[0]
+    return BeautifulSoup(text, "html.parser").find_all("a")[0]
 
 
 def test_upload_and_push_external(mapp, testapp, reqmock):
     api = mapp.create_and_use()
     mapp.upload_file_pypi("pkg1-2.6.tgz", b"123", "pkg1", "2.6")
     zipcontent = zip_dict({"index.html": "<html/>"})
     mapp.upload_doc("pkg1.zip", zipcontent, "pkg1", "")
```

### Comparing `devpi-server-6.8.0/test_devpi_server/test_views_status.py` & `devpi-server-6.9.0/test_devpi_server/test_views_status.py`

 * *Files identical despite different names*

### Comparing `devpi-server-6.8.0/tox.ini` & `devpi-server-6.9.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 setenv =
     LANG = C
 
 commands=
     !keyfs_sqlite: py.test --instafail --slow {posargs}
     keyfs_sqlite: py.test --instafail --backend=devpi_server.keyfs_sqlite --slow {posargs}
 
+passenv = GITHUB_ACTIONS
+
 deps=
     webtest
     pytest
     pytest-asyncio
     pytest-flake8 < 1.1.0;python_version=="2.7"
     pytest-flake8;python_version!="2.7"
     flake8<5
+    pytest-github-actions-annotate-failures
     pytest-instafail
     pytest-timeout
-    beautifulsoup4
+    beautifulsoup4 != 4.12.1
     execnet
     importlib.metadata;python_version<"3.8"
 
 
 [pytest]
 addopts= -r a --flake8 -W once::DeprecationWarning -W ignore::DeprecationWarning:webob.acceptparse -W once::pytest.PytestDeprecationWarning -W once::ResourceWarning
 timeout = 60
```

