# Comparing `tmp/RBTools-4.0.tar.gz` & `tmp/RBTools-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RBTools-4.0.tar", last modified: Mon Oct 24 07:27:42 2022, max compression
+gzip compressed data, was "RBTools-4.1.tar", last modified: Tue May 23 21:07:43 2023, max compression
```

## Comparing `RBTools-4.0.tar` & `RBTools-4.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.234657 RBTools-4.0/
--rw-r--r--   0 chipx86    (501) staff       (20)     2158 2022-10-24 07:27:41.000000 RBTools-4.0/AUTHORS
--rw-r--r--   0 chipx86    (501) staff       (20)     1109 2022-10-24 07:27:41.000000 RBTools-4.0/COPYING
--rw-r--r--   0 chipx86    (501) staff       (20)      219 2022-10-24 07:27:41.000000 RBTools-4.0/INSTALL
--rw-r--r--   0 chipx86    (501) staff       (20)      200 2022-10-24 07:27:41.000000 RBTools-4.0/MANIFEST.in
--rw-r--r--   0 chipx86    (501) staff       (20)      219 2022-10-24 07:27:41.000000 RBTools-4.0/NEWS
--rw-r--r--   0 chipx86    (501) staff       (20)     6303 2022-10-24 07:27:42.234738 RBTools-4.0/PKG-INFO
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.211395 RBTools-4.0/RBTools.egg-info/
--rw-r--r--   0 chipx86    (501) staff       (20)     6303 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/PKG-INFO
--rw-r--r--   0 chipx86    (501) staff       (20)     4733 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/SOURCES.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        1 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/dependency_links.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      935 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/entry_points.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      139 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/requires.txt
--rw-r--r--   0 chipx86    (501) staff       (20)        8 2022-10-24 07:27:42.000000 RBTools-4.0/RBTools.egg-info/top_level.txt
--rw-r--r--   0 chipx86    (501) staff       (20)     5086 2022-10-24 07:27:41.000000 RBTools-4.0/README.md
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.211667 RBTools-4.0/contrib/
--rw-r--r--   0 chipx86    (501) staff       (20)      133 2022-10-24 07:27:41.000000 RBTools-4.0/contrib/P4Tool.txt
--rw-r--r--   0 chipx86    (501) staff       (20)      601 2022-10-24 07:27:41.000000 RBTools-4.0/contrib/README.P4Tool
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.207525 RBTools-4.0/contrib/installers/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.207570 RBTools-4.0/contrib/installers/windows/
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.211934 RBTools-4.0/contrib/installers/windows/scripts/
--rw-r--r--   0 chipx86    (501) staff       (20)      286 2022-10-24 07:27:41.000000 RBTools-4.0/contrib/installers/windows/scripts/get-version.py
--rw-r--r--   0 chipx86    (501) staff       (20)      351 2022-10-24 07:27:41.000000 RBTools-4.0/pytest.ini
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.212569 RBTools-4.0/rbtools/
--rw-r--r--   0 chipx86    (501) staff       (20)     1893 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.214772 RBTools-4.0/rbtools/api/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    30266 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/cache.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1582 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/capabilities.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7064 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/client.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1491 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/decode.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1246 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/decorators.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10107 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2575 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/factory.py
--rw-r--r--   0 chipx86    (501) staff       (20)    38266 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/request.py
--rw-r--r--   0 chipx86    (501) staff       (20)    55683 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/resource.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.216103 RBTools-4.0/rbtools/api/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5284 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/base.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1138 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/test_capabilities.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6553 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/test_errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2754 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/test_factory.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6804 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/test_http_request.py
--rw-r--r--   0 chipx86    (501) staff       (20)    27303 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/tests/test_resource.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.216500 RBTools-4.0/rbtools/api/transport/
--rw-r--r--   0 chipx86    (501) staff       (20)     5391 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/transport/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11333 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/transport/sync.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2490 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/api/utils.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.218728 RBTools-4.0/rbtools/clients/
--rw-r--r--   0 chipx86    (501) staff       (20)     8559 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.219515 RBTools-4.0/rbtools/clients/base/
--rw-r--r--   0 chipx86    (501) staff       (20)       69 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/base/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2239 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/base/patch.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8725 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/base/registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5684 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/base/repository.py
--rw-r--r--   0 chipx86    (501) staff       (20)    43216 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/base/scmclient.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18324 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/bazaar.py
--rw-r--r--   0 chipx86    (501) staff       (20)    85623 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/clearcase.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8472 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/cvs.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5929 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)    67557 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/git.py
--rw-r--r--   0 chipx86    (501) staff       (20)    48781 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/mercurial.py
--rw-r--r--   0 chipx86    (501) staff       (20)    86172 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/perforce.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13565 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/plastic.py
--rw-r--r--   0 chipx86    (501) staff       (20)    67967 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/sos.py
--rw-r--r--   0 chipx86    (501) staff       (20)    61029 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/svn.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.222557 RBTools-4.0/rbtools/clients/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)    15736 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7646 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_base_scmclient.py
--rw-r--r--   0 chipx86    (501) staff       (20)    36502 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_bzr.py
--rw-r--r--   0 chipx86    (501) staff       (20)    73740 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_clearcase.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12010 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_cvs.py
--rw-r--r--   0 chipx86    (501) staff       (20)    97458 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_git.py
--rw-r--r--   0 chipx86    (501) staff       (20)    75278 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_mercurial.py
--rw-r--r--   0 chipx86    (501) staff       (20)    31268 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_p4.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1448 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_plastic.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2838 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_scanning.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8252 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_scmclient_registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)   127141 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_sos.py
--rw-r--r--   0 chipx86    (501) staff       (20)    71161 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_svn.py
--rw-r--r--   0 chipx86    (501) staff       (20)    73825 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tests/test_tfs.py
--rw-r--r--   0 chipx86    (501) staff       (20)    49853 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/clients/tfs.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.226483 RBTools-4.0/rbtools/commands/
--rw-r--r--   0 chipx86    (501) staff       (20)    65716 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3965 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/alias.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1966 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/api_get.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3258 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/attach.py
--rw-r--r--   0 chipx86    (501) staff       (20)      937 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/clearcache.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2667 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/close.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.226850 RBTools-4.0/rbtools/commands/conf/
--rw-r--r--   0 chipx86    (501) staff       (20)      329 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/conf/_rbt-zsh-completion
--rw-r--r--   0 chipx86    (501) staff       (20)      527 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/conf/rbt-bash-completion
--rw-r--r--   0 chipx86    (501) staff       (20)     3520 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/diff.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3038 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/info.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7383 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/install.py
--rw-r--r--   0 chipx86    (501) staff       (20)    17872 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/land.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1608 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/list_repo_types.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1738 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/login.py
--rw-r--r--   0 chipx86    (501) staff       (20)      905 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/logout.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7749 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/main.py
--rw-r--r--   0 chipx86    (501) staff       (20)    26885 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/patch.py
--rw-r--r--   0 chipx86    (501) staff       (20)    67281 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/post.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3047 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/publish.py
--rw-r--r--   0 chipx86    (501) staff       (20)    14125 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/review.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3924 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/setup_completion.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10329 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/setup_repo.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6306 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/stamp.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8387 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/status.py
--rw-r--r--   0 chipx86    (501) staff       (20)    18475 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/status_update.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.227530 RBTools-4.0/rbtools/commands/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4018 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/tests/test_alias.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6498 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/tests/test_main.py
--rw-r--r--   0 chipx86    (501) staff       (20)    48852 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/tests/test_post.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5351 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/commands/tests/test_setup_repo.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9101 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/deprecation.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.227869 RBTools-4.0/rbtools/diffs/
--rw-r--r--   0 chipx86    (501) staff       (20)       90 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.228704 RBTools-4.0/rbtools/diffs/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    10469 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/test_apple_diff_tool.py
--rw-r--r--   0 chipx86    (501) staff       (20)    35136 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/test_diff_file_result.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6322 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/test_diff_tools_registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12957 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/test_gnu_diff_tool.py
--rw-r--r--   0 chipx86    (501) staff       (20)    17425 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tests/test_unified_diff_writer.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.229067 RBTools-4.0/rbtools/diffs/tools/
--rw-r--r--   0 chipx86    (501) staff       (20)       77 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.229410 RBTools-4.0/rbtools/diffs/tools/backends/
--rw-r--r--   0 chipx86    (501) staff       (20)       79 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/backends/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8434 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/backends/apple.py
--rw-r--r--   0 chipx86    (501) staff       (20)     7679 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/backends/gnu.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.229752 RBTools-4.0/rbtools/diffs/tools/base/
--rw-r--r--   0 chipx86    (501) staff       (20)      597 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/base/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    13031 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/base/diff_file_result.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5553 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/base/diff_tool.py
--rw-r--r--   0 chipx86    (501) staff       (20)     2711 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)     8535 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/tools/registry.py
--rw-r--r--   0 chipx86    (501) staff       (20)    12538 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/diffs/writers.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.229943 RBTools-4.0/rbtools/helpers/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/helpers/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)      599 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/helpers/hgext.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.230249 RBTools-4.0/rbtools/hooks/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/hooks/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4208 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/hooks/common.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4289 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/hooks/git.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.230704 RBTools-4.0/rbtools/testing/
--rw-r--r--   0 chipx86    (501) staff       (20)      280 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/__init__.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.231112 RBTools-4.0/rbtools/testing/api/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/api/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)    38570 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/api/payloads.py
--rw-r--r--   0 chipx86    (501) staff       (20)    35243 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/api/transport.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9376 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/commands.py
--rw-r--r--   0 chipx86    (501) staff       (20)    11619 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/testcase.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4262 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/testing/transport.py
--rw-r--r--   0 chipx86    (501) staff       (20)      637 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/tests.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.233368 RBTools-4.0/rbtools/utils/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     5018 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/aliases.py
--rwxr-xr-x   0 chipx86    (501) staff       (20)    22374 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/appdirs.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3860 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/checks.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3252 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/commands.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9128 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/console.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6022 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/diffs.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1272 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/encoding.py
--rw-r--r--   0 chipx86    (501) staff       (20)      900 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/errors.py
--rw-r--r--   0 chipx86    (501) staff       (20)     9753 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/filesystem.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1847 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/graphs.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1842 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/match_score.py
--rw-r--r--   0 chipx86    (501) staff       (20)    21837 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/process.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4184 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/repository.py
--rw-r--r--   0 chipx86    (501) staff       (20)    29283 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/review_request.py
--rw-r--r--   0 chipx86    (501) staff       (20)    16398 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/source_tree.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3157 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/streams.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1026 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/testbase.py
-drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:42.234533 RBTools-4.0/rbtools/utils/tests/
--rw-r--r--   0 chipx86    (501) staff       (20)        0 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/__init__.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3898 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_aliases.py
--rw-r--r--   0 chipx86    (501) staff       (20)     4140 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_buffered_iterator.py
--rw-r--r--   0 chipx86    (501) staff       (20)     1676 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_checks.py
--rw-r--r--   0 chipx86    (501) staff       (20)    16441 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_console.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3098 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_filesystem.py
--rw-r--r--   0 chipx86    (501) staff       (20)    17193 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_process.py
--rw-r--r--   0 chipx86    (501) staff       (20)     6116 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_repository.py
--rw-r--r--   0 chipx86    (501) staff       (20)    30360 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_review_request.py
--rw-r--r--   0 chipx86    (501) staff       (20)    17128 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/tests/test_source_tree.py
--rw-r--r--   0 chipx86    (501) staff       (20)     3375 2022-10-24 07:27:41.000000 RBTools-4.0/rbtools/utils/users.py
--rw-r--r--   0 chipx86    (501) staff       (20)      408 2022-10-24 07:27:42.234993 RBTools-4.0/setup.cfg
--rwxr-xr-x   0 chipx86    (501) staff       (20)     6791 2022-10-24 07:27:41.000000 RBTools-4.0/setup.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.839454 RBTools-4.1/
+-rw-r--r--   0 chipx86    (501) staff       (20)     2158 2023-05-23 21:07:43.000000 RBTools-4.1/AUTHORS
+-rw-r--r--   0 chipx86    (501) staff       (20)     1109 2023-05-23 21:07:43.000000 RBTools-4.1/COPYING
+-rw-r--r--   0 chipx86    (501) staff       (20)      219 2023-05-23 21:07:43.000000 RBTools-4.1/INSTALL
+-rw-r--r--   0 chipx86    (501) staff       (20)      200 2023-05-23 21:07:43.000000 RBTools-4.1/MANIFEST.in
+-rw-r--r--   0 chipx86    (501) staff       (20)      219 2023-05-23 21:07:43.000000 RBTools-4.1/NEWS
+-rw-r--r--   0 chipx86    (501) staff       (20)     6303 2023-05-23 21:07:43.839523 RBTools-4.1/PKG-INFO
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.819551 RBTools-4.1/RBTools.egg-info/
+-rw-r--r--   0 chipx86    (501) staff       (20)     6303 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/PKG-INFO
+-rw-r--r--   0 chipx86    (501) staff       (20)     4714 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/SOURCES.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        1 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/dependency_links.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      935 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/entry_points.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)      146 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/requires.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)        8 2023-05-23 21:07:43.000000 RBTools-4.1/RBTools.egg-info/top_level.txt
+-rw-r--r--   0 chipx86    (501) staff       (20)     5086 2023-05-23 21:07:43.000000 RBTools-4.1/README.md
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.816770 RBTools-4.1/contrib/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.819652 RBTools-4.1/contrib/P4V/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1419 2023-05-23 21:07:43.000000 RBTools-4.1/contrib/P4V/README.md
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.816811 RBTools-4.1/contrib/installers/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.816851 RBTools-4.1/contrib/installers/windows/
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.819765 RBTools-4.1/contrib/installers/windows/scripts/
+-rw-r--r--   0 chipx86    (501) staff       (20)      229 2023-05-23 21:07:43.000000 RBTools-4.1/contrib/installers/windows/scripts/get-version.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      351 2023-05-23 21:07:43.000000 RBTools-4.1/pytest.ini
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.820089 RBTools-4.1/rbtools/
+-rw-r--r--   0 chipx86    (501) staff       (20)     1893 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.821942 RBTools-4.1/rbtools/api/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    30382 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/cache.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1582 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/capabilities.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7064 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/client.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1491 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/decode.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1246 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/decorators.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17336 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2575 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/factory.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    41359 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/request.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    55475 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/resource.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.823034 RBTools-4.1/rbtools/api/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5243 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/base.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1138 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/test_capabilities.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17180 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/test_errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2713 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/test_factory.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6742 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/test_http_request.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    27233 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/tests/test_resource.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.823269 RBTools-4.1/rbtools/api/transport/
+-rw-r--r--   0 chipx86    (501) staff       (20)     5391 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/transport/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11333 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/transport/sync.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2490 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/api/utils.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.825309 RBTools-4.1/rbtools/clients/
+-rw-r--r--   0 chipx86    (501) staff       (20)     8518 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.826063 RBTools-4.1/rbtools/clients/base/
+-rw-r--r--   0 chipx86    (501) staff       (20)       69 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/base/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2198 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/base/patch.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8725 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/base/registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5684 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/base/repository.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    43339 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/base/scmclient.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18324 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/bazaar.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    85641 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/clearcase.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8472 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/cvs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5929 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    71722 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/git.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    48684 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/mercurial.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    87257 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/perforce.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13524 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/plastic.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    67835 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/sos.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    61018 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/svn.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.827797 RBTools-4.1/rbtools/clients/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)    15736 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7646 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_base_scmclient.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    36461 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_bzr.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    74494 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_clearcase.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11969 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_cvs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    97417 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_git.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    75237 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_mercurial.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    37076 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_p4.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1448 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_plastic.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2797 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_scanning.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8252 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_scmclient_registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)   127100 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_sos.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    71167 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_svn.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    73825 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tests/test_tfs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    49842 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/clients/tfs.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.832525 RBTools-4.1/rbtools/commands/
+-rw-r--r--   0 chipx86    (501) staff       (20)    65688 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3934 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/alias.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1963 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/api_get.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3243 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/attach.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      938 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/clearcache.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2662 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/close.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.832764 RBTools-4.1/rbtools/commands/conf/
+-rw-r--r--   0 chipx86    (501) staff       (20)      329 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/conf/_rbt-zsh-completion
+-rw-r--r--   0 chipx86    (501) staff       (20)      527 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/conf/rbt-bash-completion
+-rw-r--r--   0 chipx86    (501) staff       (20)     3409 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/diff.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3038 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/info.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7350 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/install.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17814 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/land.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1594 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/list_repo_types.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1733 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/login.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      901 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/logout.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     7733 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/main.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    26729 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/patch.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    67221 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/post.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3044 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/publish.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    14071 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/review.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3930 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/setup_completion.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10332 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/setup_repo.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6279 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/stamp.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8383 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/status.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    18275 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/status_update.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.833298 RBTools-4.1/rbtools/commands/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3977 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/tests/test_alias.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6457 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/tests/test_main.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    48811 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/tests/test_post.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5310 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/commands/tests/test_setup_repo.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9305 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/deprecation.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.833494 RBTools-4.1/rbtools/diffs/
+-rw-r--r--   0 chipx86    (501) staff       (20)       90 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.834164 RBTools-4.1/rbtools/diffs/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10469 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/test_apple_diff_tool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    35136 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/test_diff_file_result.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6322 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/test_diff_tools_registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17043 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/test_gnu_diff_tool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17425 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tests/test_unified_diff_writer.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.834489 RBTools-4.1/rbtools/diffs/tools/
+-rw-r--r--   0 chipx86    (501) staff       (20)       77 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.834787 RBTools-4.1/rbtools/diffs/tools/backends/
+-rw-r--r--   0 chipx86    (501) staff       (20)       79 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/backends/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8434 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/backends/apple.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10452 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/backends/gnu.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.835095 RBTools-4.1/rbtools/diffs/tools/base/
+-rw-r--r--   0 chipx86    (501) staff       (20)      597 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/base/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    13031 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/base/diff_file_result.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5553 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/base/diff_tool.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     2711 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     8535 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/tools/registry.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    12538 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/diffs/writers.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.835284 RBTools-4.1/rbtools/helpers/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/helpers/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      557 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/helpers/hgext.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.835570 RBTools-4.1/rbtools/hooks/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/hooks/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4648 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/hooks/common.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4250 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/hooks/git.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.835967 RBTools-4.1/rbtools/testing/
+-rw-r--r--   0 chipx86    (501) staff       (20)      297 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/__init__.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.836266 RBTools-4.1/rbtools/testing/api/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/api/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    38529 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/api/payloads.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    35191 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/api/transport.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9335 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/commands.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    11601 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/testcase.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4221 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/testing/transport.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      637 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/tests.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.838297 RBTools-4.1/rbtools/utils/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     5006 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/aliases.py
+-rwxr-xr-x   0 chipx86    (501) staff       (20)    22374 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/appdirs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3867 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/checks.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3222 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/commands.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     9067 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/console.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6022 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/diffs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1272 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/encoding.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      859 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/errors.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    10190 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/filesystem.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1817 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/graphs.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1801 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/match_score.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    21837 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/process.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4143 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/repository.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    29289 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/review_request.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    16398 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/source_tree.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3157 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/streams.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      985 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/testbase.py
+drwxr-xr-x   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.839342 RBTools-4.1/rbtools/utils/tests/
+-rw-r--r--   0 chipx86    (501) staff       (20)        0 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/__init__.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3857 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_aliases.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     4140 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_buffered_iterator.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     1676 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_checks.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    16400 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_console.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3057 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_filesystem.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17193 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_process.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     6065 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_repository.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    30319 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_review_request.py
+-rw-r--r--   0 chipx86    (501) staff       (20)    17128 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/tests/test_source_tree.py
+-rw-r--r--   0 chipx86    (501) staff       (20)     3354 2023-05-23 21:07:43.000000 RBTools-4.1/rbtools/utils/users.py
+-rw-r--r--   0 chipx86    (501) staff       (20)      408 2023-05-23 21:07:43.839770 RBTools-4.1/setup.cfg
+-rwxr-xr-x   0 chipx86    (501) staff       (20)     6798 2023-05-23 21:07:43.000000 RBTools-4.1/setup.py
```

### Comparing `RBTools-4.0/AUTHORS` & `RBTools-4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/COPYING` & `RBTools-4.1/COPYING`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/PKG-INFO` & `RBTools-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RBTools
-Version: 4.0
+Version: 4.1
 Summary: Command line tools and API for working with code and document reviews on Review Board
 Home-page: https://www.reviewboard.org/downloads/rbtools/
-Download-URL: https://downloads.reviewboard.org/releases/RBTools/4.0/
+Download-URL: https://downloads.reviewboard.org/releases/RBTools/4.1/
 Author: Beanbag, Inc.
 Author-email: reviewboard@googlegroups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `RBTools-4.0/RBTools.egg-info/PKG-INFO` & `RBTools-4.1/RBTools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RBTools
-Version: 4.0
+Version: 4.1
 Summary: Command line tools and API for working with code and document reviews on Review Board
 Home-page: https://www.reviewboard.org/downloads/rbtools/
-Download-URL: https://downloads.reviewboard.org/releases/RBTools/4.0/
+Download-URL: https://downloads.reviewboard.org/releases/RBTools/4.1/
 Author: Beanbag, Inc.
 Author-email: reviewboard@googlegroups.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Review Board
 Classifier: Intended Audience :: Developers
```

### Comparing `RBTools-4.0/RBTools.egg-info/SOURCES.txt` & `RBTools-4.1/RBTools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 setup.py
 RBTools.egg-info/PKG-INFO
 RBTools.egg-info/SOURCES.txt
 RBTools.egg-info/dependency_links.txt
 RBTools.egg-info/entry_points.txt
 RBTools.egg-info/requires.txt
 RBTools.egg-info/top_level.txt
-contrib/P4Tool.txt
-contrib/README.P4Tool
+contrib/P4V/README.md
 contrib/installers/windows/scripts/get-version.py
 rbtools/__init__.py
 rbtools/deprecation.py
 rbtools/tests.py
 rbtools/api/__init__.py
 rbtools/api/cache.py
 rbtools/api/capabilities.py
```

### Comparing `RBTools-4.0/RBTools.egg-info/entry_points.txt` & `RBTools-4.1/RBTools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/README.md` & `RBTools-4.1/README.md`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/__init__.py` & `RBTools-4.1/rbtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 #: The version of RBTools
 #:
 #: This is in the format of:
 #:
 #: (Major, Minor, Micro, Patch, alpha/beta/rc/final, Release Number, Released)
 #:
-VERSION = (4, 0, 0, 0, 'final', 0, True)
+VERSION = (4, 1, 0, 0, 'final', 0, True)
 
 
 def get_version_string():
     """Return the version as a human-readable string.
 
     Returns:
         str:
```

### Comparing `RBTools-4.0/rbtools/api/cache.py` & `RBTools-4.1/rbtools/api/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,27 @@
                     return False
 
         return True
 
     def up_to_date(self) -> bool:
         """Determine if the cache entry is up to date.
 
+        Version Changed:
+            4.1:
+            This now returns ``False`` if ``max_age`` is not available.
+
         Returns:
             bool:
             ``True`` if the cache entry is still valid. ``False``, otherwise.
         """
         if self.max_age is not None:
             max_age = datetime.timedelta(seconds=self.max_age)
             return self.local_date + max_age > datetime.datetime.now()
 
-        return True
+        return False
 
 
 class LiveHTTPResponse(object):
     """An uncached HTTP response that can be read() more than once.
 
     This is intended to be API-compatible with an
     :py:class:`http.client.HTTPResponse` object. This allows a response to be
```

### Comparing `RBTools-4.0/rbtools/api/capabilities.py` & `RBTools-4.1/rbtools/api/capabilities.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/client.py` & `RBTools-4.1/rbtools/api/client.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/decode.py` & `RBTools-4.1/rbtools/api/decode.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/decorators.py` & `RBTools-4.1/rbtools/api/decorators.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/factory.py` & `RBTools-4.1/rbtools/api/factory.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/request.py` & `RBTools-4.1/rbtools/api/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+from __future__ import annotations
+
 import base64
 import logging
 import mimetypes
 import os
 import random
 import shutil
 import ssl
 import sys
 from collections import OrderedDict
-from http.client import HTTPMessage, HTTPResponse, NOT_MODIFIED
+from http.client import (HTTPMessage, HTTPResponse, HTTPSConnection,
+                         NOT_MODIFIED)
 from http.cookiejar import Cookie, CookieJar, MozillaCookieJar
 from io import BytesIO
 from json import loads as json_loads
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from urllib.error import HTTPError, URLError
 from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 from urllib.request import (
     BaseHandler,
     HTTPBasicAuthHandler,
     HTTPCookieProcessor,
     HTTPDigestAuthHandler,
@@ -24,19 +27,23 @@
     HTTPSHandler,
     ProxyHandler,
     Request as URLRequest,
     build_opener,
     install_opener,
     urlopen)
 
+import certifi
 from typing_extensions import TypeAlias
 
 from rbtools import get_package_version
 from rbtools.api.cache import APICache, CachedHTTPResponse, LiveHTTPResponse
-from rbtools.api.errors import APIError, create_api_error, ServerInterfaceError
+from rbtools.api.errors import (APIError,
+                                ServerInterfaceError,
+                                ServerInterfaceSSLError,
+                                create_api_error)
 from rbtools.deprecation import RemovedInRBTools50Warning
 from rbtools.utils.encoding import force_bytes, force_unicode
 from rbtools.utils.filesystem import get_home_path
 
 
 RBTOOLS_COOKIE_FILE = '.rbtools-cookies'
 RB_COOKIE_NAME = 'rbsessionid'
@@ -321,14 +328,106 @@
             The generated boundary.
         """
         fmt = '%%0%dd' % len(repr(sys.maxsize - 1))
         token = random.randrange(sys.maxsize)
         return (b'=' * 15) + (fmt % token).encode('utf-8') + b'=='
 
 
+class RBToolsHTTPSConnection(HTTPSConnection):
+    """Connection class for HTTPS connections.
+
+    This is a specialization of the default HTTPS connection class that
+    provides custom error handling for SSL errors.
+
+    Version Added:
+        4.1
+    """
+
+    def connect(self, *args, **kwargs) -> Any:
+        """Connect to the server.
+
+        This will catch SSL errors and wrap them with our own error classes.
+
+        Args:
+            *args (tuple):
+                Positional arguments to pass to the parent method.
+
+            **kwargs (dict):
+                Keyword arguments to pass to the parent method.
+
+        Returns:
+            object:
+            The result from the parent method.
+
+        Raises:
+            rbtools.api.errors.ServerInterfaceSSLError:
+                An SSL error occurred during communication. Details will be
+                in the error message.
+        """
+        try:
+            return super().connect(*args, **kwargs)
+        except ssl.SSLError as e:
+            # This seems to be the only way to get access to the context
+            # here. Assert that it's reachable.
+            context = getattr(self, '_context', None)
+            assert context is not None
+
+            raise ServerInterfaceSSLError(
+                host=self.host,
+                port=self.port,
+                ssl_error=e,
+                ssl_context=context)
+
+
+class RBToolsHTTPSHandler(HTTPSHandler):
+    """Request/response handler for HTTPS connections.
+
+    This wraps the default HTTPS handler, passing in a specialized HTTPS
+    connection class used to generate more useful SSL-related errors.
+
+    Version Added:
+        4.1
+    """
+
+    def do_open(
+        self,
+        http_class,
+        *args,
+        **kwargs,
+    ) -> HTTPResponse:
+        """Open a connection to the server.
+
+        Args:
+            http_class (type, unused):
+                The original HTTPS connection class. This will be replaced
+                with our own.
+
+            *args (tuple):
+                Positional arguments to pass to the parent method.
+
+            **kwargs (dict):
+                Keyword arguments to pass to the parent method.
+
+        Returns:
+            http.client.HTTPResponse:
+            The resulting HTTP response.
+
+        Raises:
+            rbtools.api.errors.ServerInterfaceSSLError:
+                An SSL error occurred during communication. Details will be
+                in the error message.
+        """
+        # Note that we're ignoring the typing below, as the type hints for
+        # do_open() mistakenly lack the 'self' parameter and think that
+        # RBToolsHTTPSConnection is therefore a mismatch on a different
+        # parameter.
+        return super().do_open(RBToolsHTTPSConnection,  # type: ignore
+                               *args, **kwargs)
+
+
 class Request(URLRequest):
     """A request which contains a method attribute."""
 
     #: The HTTP method to use.
     #:
     #: Type: str
     method: str
@@ -1002,23 +1101,24 @@
                                                   auth_callback,
                                                   otp_token_callback)
         self.preset_auth_handler = PresetHTTPAuthHandler(self.url,
                                                          password_mgr)
 
         handlers: List[BaseHandler] = []
 
-        if not verify_ssl:
-            context = ssl._create_unverified_context()
+        if verify_ssl:
+            context = ssl.create_default_context(
+                cafile=ca_certs or certifi.where())
         else:
-            context = ssl.create_default_context(cafile=ca_certs)
+            context = ssl._create_unverified_context()
 
         if client_cert and client_key:
             context.load_cert_chain(client_cert, client_key)
 
-        handlers.append(HTTPSHandler(context=context))
+        handlers.append(RBToolsHTTPSHandler(context=context))
 
         if disable_proxy:
             handlers.append(ProxyHandler({}))
 
         handlers += [
             HTTPCookieProcessor(self.cookie_jar),
             ReviewBoardHTTPBasicAuthHandler(password_mgr),
```

### Comparing `RBTools-4.0/rbtools/api/resource.py` & `RBTools-4.1/rbtools/api/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,16 @@
-from __future__ import unicode_literals
-
 import copy
 import json
 import logging
 import re
 from collections import defaultdict, deque
+from collections.abc import MutableMapping
+from urllib.parse import urljoin
 
-try:
-    from collections.abc import MutableMapping
-except ImportError:
-    from collections import MutableMapping
-
-import six
 from pkg_resources import parse_version
-from six.moves import range
-from six.moves.urllib.parse import urljoin
 
 from rbtools.api.cache import MINIMUM_VERSION
 from rbtools.api.decorators import request_method_decorator
 from rbtools.api.request import HttpRequest
 from rbtools.api.utils import rem_mime_format
 from rbtools.deprecation import RemovedInRBTools50Warning
 from rbtools.utils.graphs import path_exists
@@ -68,15 +60,15 @@
     Yields:
         tuple:
         A 2-tuple of:
 
         1. The normalized field name to send in the request.
         2. The normalized value to send.
     """
-    field_names = set(six.iterkeys(fields))
+    field_names = set(fields.keys())
 
     # Serialize the JSON Merge Patch or JSON Patch payloads first.
     for norm_field_name, field_name in (('extra_data:json',
                                          'extra_data_json'),
                                         ('extra_data:json-patch',
                                          'extra_data_json_patch')):
         if field_name in field_names:
@@ -315,24 +307,24 @@
               EXPANDED_TOKEN in self._payload[token]):
             self._expanded_info = self._payload[token][EXPANDED_TOKEN]
         else:
             self._expanded_info = {}
 
         # Add a method for each supported REST operation, and
         # for retrieving 'self'.
-        for link, method in six.iteritems(SPECIAL_LINKS):
+        for link, method in SPECIAL_LINKS.items():
             if link in self._links and method[1]:
                 setattr(self,
                         method[0],
                         lambda resource=self, meth=method[1], **kwargs: (
                             meth(resource, **kwargs)))
 
         # Generate request methods for any additional links
         # the resource has.
-        for link, body in six.iteritems(self._links):
+        for link, body in self._links.items():
             if link not in SPECIAL_LINKS:
                 setattr(self,
                         'get_%s' % link,
                         lambda resource=self, url=body['href'], **kwargs: (
                             self._get_url(url, **kwargs)))
 
     def _wrap_field(self, field_payload, field_name=None, field_url=None,
@@ -570,15 +562,15 @@
     def __iter__(self):
         """Iterate through the dictionary.
 
         Yields:
             object:
             Each item in the dictionary.
         """
-        return six.iterkeys(self._fields)
+        yield from self._fields.keys()
 
     def __repr__(self):
         """Return a string representation of the dictionary field.
 
         Returns:
             unicode:
             The string representation.
@@ -821,15 +813,15 @@
 
         # Determine the body of the resource's data.
         if token is not None:
             data = self._payload[token]
         else:
             data = self._payload
 
-        for name, value in six.iteritems(data):
+        for name, value in data.items():
             if name not in self._excluded_attrs:
                 self._fields[name] = value
 
     def __getattr__(self, name):
         """Return the value for an attribute on the resource.
 
         If the attribute represents an expanded resource, and there's
@@ -1067,15 +1059,15 @@
     _excluded_attrs = ['uri_templates']
     _TEMPLATE_PARAM_RE = re.compile(r'\{(?P<key>[A-Za-z_0-9]*)\}')
 
     def __init__(self, transport, payload, url, **kwargs):
         super(RootResource, self).__init__(transport, payload, url, token=None)
         # Generate methods for accessing resources directly using
         # the uri-templates.
-        for name, url in six.iteritems(payload['uri_templates']):
+        for name, url in payload['uri_templates'].items():
             attr_name = 'get_%s' % name
 
             if not hasattr(self, attr_name):
                 setattr(self,
                         attr_name,
                         lambda resource=self, url=url, **kwargs: (
                             self._get_template_request(url, **kwargs)))
@@ -1477,15 +1469,15 @@
         return self.update(data=data, internal=True)
 
     @request_method_decorator
     def get_or_create_draft(self, **kwargs):
         request = self.get_draft(internal=True)
         request.method = 'POST'
 
-        for name, value in six.iteritems(kwargs):
+        for name, value in kwargs.items():
             request.add_field(name, value)
 
         return request
 
     def build_dependency_graph(self):
         """Build the dependency graph for the review request.
```

### Comparing `RBTools-4.0/rbtools/api/tests/base.py` & `RBTools-4.1/rbtools/api/tests/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Base support for API unit tests."""
 
-from __future__ import unicode_literals
-
 from rbtools.api.transport import Transport
 from rbtools.testing import TestCase
 
 
 class MockResponse(object):
     """A mock up for a response from urllib2."""
```

### Comparing `RBTools-4.0/rbtools/api/tests/test_capabilities.py` & `RBTools-4.1/rbtools/api/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/tests/test_factory.py` & `RBTools-4.1/rbtools/api/tests/test_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for rbtools.api.factory."""
 
-from __future__ import unicode_literals
-
 from rbtools.api.factory import create_resource
 from rbtools.api.resource import (CountResource,
                                   ItemResource,
                                   ListResource,
                                   RootResource)
 from rbtools.api.tests.base import TestWithPayloads
```

### Comparing `RBTools-4.0/rbtools/api/tests/test_http_request.py` & `RBTools-4.1/rbtools/api/tests/test_http_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Unit tests for rbtools.api.request.HttpRequest."""
 
-from __future__ import unicode_literals
-
-import six
-from six.moves.urllib.parse import parse_qsl, urlparse
+from urllib.parse import parse_qsl, urlparse
 
 from kgb import SpyAgency
 
 from rbtools.api.request import HttpRequest
 from rbtools.testing import TestCase
```

### Comparing `RBTools-4.0/rbtools/api/tests/test_resource.py` & `RBTools-4.1/rbtools/api/tests/test_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """Unit tests for rbtools.api.resource."""
 
-from __future__ import unicode_literals
-
 import re
 
-from six.moves import range
-
 from rbtools.api.factory import create_resource
 from rbtools.api.request import HttpRequest
 from rbtools.api.resource import (CountResource,
                                   ItemResource,
                                   ListResource,
                                   RESOURCE_MAP,
                                   ResourceDictField,
```

### Comparing `RBTools-4.0/rbtools/api/transport/__init__.py` & `RBTools-4.1/rbtools/api/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/transport/sync.py` & `RBTools-4.1/rbtools/api/transport/sync.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/api/utils.py` & `RBTools-4.1/rbtools/api/utils.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/__init__.py` & `RBTools-4.1/rbtools/clients/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
       :py:class:`rbtools.clients.base.scmclient.BaseSCMClient` and added a
       forwarding import and temporary legacy class.
 
     * Moved :py:class:`~rbtools.clients.base.repository.RepositoryInfo` and
       added a forwarding import.
 """
 
-from __future__ import unicode_literals
-
 import logging
 import os
 import sys
 
 from rbtools.clients.base.patch import PatchAuthor, PatchResult
 from rbtools.clients.base.registry import scmclient_registry
 from rbtools.clients.base.repository import RepositoryInfo
```

### Comparing `RBTools-4.0/rbtools/clients/base/patch.py` & `RBTools-4.1/rbtools/clients/base/patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Classes for representing patch results in SCM clients.
 
 Version Added:
     4.0
 """
 
-from __future__ import unicode_literals
-
 
 class PatchAuthor(object):
     """The author of a patch or commit.
 
     This wraps the full name and e-mail address of a commit or patch's
     author primarily for use in :py:meth:`BaseSCMClient.apply_patch
     <rbtools.clients.base.scmclient.BaseSCMClient.apply_patch>`.
```

### Comparing `RBTools-4.0/rbtools/clients/base/registry.py` & `RBTools-4.1/rbtools/clients/base/registry.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/base/repository.py` & `RBTools-4.1/rbtools/clients/base/repository.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/base/scmclient.py` & `RBTools-4.1/rbtools/clients/base/scmclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1247,14 +1247,18 @@
         Args:
             branch_name (str):
                 The name of the branch to delete.
 
             merged_only (bool, optional):
                 Whether to limit branch deletion to only those branches which
                 have been merged into the current HEAD.
+
+        Raises:
+            rbtools.clients.errors.SCMError:
+                An error occurred while deleting the branch.
         """
         raise NotImplementedError
 
     @deprecate_non_keyword_only_args(RemovedInRBTools50Warning)
     def merge(
         self,
         *,
```

### Comparing `RBTools-4.0/rbtools/clients/bazaar.py` & `RBTools-4.1/rbtools/clients/bazaar.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/clearcase.py` & `RBTools-4.1/rbtools/clients/clearcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 import io
 import itertools
 import logging
 import os
 import re
 import sys
 import threading
-from collections import defaultdict, deque
+from collections import OrderedDict, defaultdict, deque
 from typing import Dict, List, Optional
 
-import six
 from pydiffx.dom import DiffX
 from pydiffx.dom.objects import DiffXChangeSection
 
 from rbtools.api.errors import APIError
 from rbtools.clients.base.repository import RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
                                             SCMClientDiffResult,
@@ -189,18 +188,34 @@
         self._old_version = None
 
         self.new_path = new_path
         self._new_name = None
         self._new_oid = new_oid
         self._new_version = None
 
+        self._vob_oid = None
+
         self.op = op
         self.is_dir = is_dir
 
     @property
+    def vob_oid(self):
+        """The OID of the VOB that the element is in.
+
+        Type:
+            unicode
+        """
+        if self._vob_oid is None:
+            self._vob_oid = execute(
+                ['cleartool', 'describe', '-fmt', '%On',
+                 'vob:%s' % (self.new_path or self.old_path)])
+
+        return self._vob_oid
+
+    @property
     def old_oid(self):
         """The OID of the old version of the element.
 
         Type:
             unicode
         """
         if self._old_oid is None:
@@ -231,16 +246,17 @@
     def old_version(self):
         """The version of the old version of the element.
 
         Type:
             unicode
         """
         if self._old_version is None and self.old_path:
-            self._old_version = execute(['cleartool', 'describe', '-fmt',
-                                         '%Vn', 'oid:%s' % self.old_oid])
+            self._old_version = execute(
+                ['cleartool', 'describe', '-fmt', '%Vn',
+                 'oid:%s@vobuuid:%s' % (self.old_oid, self.vob_oid)])
 
         return self._old_version
 
     @property
     def new_oid(self):
         """The OID of the new version of the element.
 
@@ -270,18 +286,19 @@
                 self.root_path)
 
         return self._new_name
 
     @property
     def new_version(self):
         if self._new_version is None and self.new_path:
-            self._new_version = execute(['cleartool', 'describe', '-fmt',
-                                         '%Vn', 'oid:%s' % self.new_oid],
-                                        ignore_errors=True,
-                                        with_errors=True)
+            self._new_version = execute(
+                ['cleartool', 'describe', '-fmt', '%Vn',
+                 'oid:%s@vobuuid:%s' % (self.new_oid, self.vob_oid)],
+                ignore_errors=True,
+                with_errors=True)
 
             if 'Not a vob object' in self._new_version:
                 self._new_version = 'CHECKEDOUT'
 
         return self._new_version
 
     def __repr__(self):
@@ -1051,15 +1068,15 @@
             repository_info (ClearCaseRepositoryInfo):
                 The repository info structure.
 
         Returns:
             list:
             The list of file versions.
         """
-        changelist = {}
+        changelist = OrderedDict()
         ignored_changes = []
         changeset = list(changeset)
 
         for change in changeset:
             # Split from the right on /main/, just in case some directory
             # elements are reported with a different version.
             path, current = change.rsplit(_MAIN, 1)
@@ -1112,15 +1129,15 @@
                 print(change)
 
             print()
 
         # Convert to list
         changeranges = []
 
-        for path, version in six.iteritems(changelist):
+        for path, version in changelist.items():
             current_version = version['current']
             branch_path, current_version_number = cpath.split(current_version)
 
             lowest_version = version['lowest']
 
             if lowest_version == sys.maxsize:
                 # This is a new file.
@@ -1169,23 +1186,19 @@
             if version_number == 0:
                 # Previous version of 0 version on branch is base
                 changelist[path]['previous'] = previous
             elif version_number > changelist[path]['highest']:
                 changelist[path]['highest'] = version_number
                 changelist[path]['current'] = current
 
-        # Convert to list
-        changeranges = []
-        for path, version in six.iteritems(changelist):
-            changeranges.append(
-                (self._construct_extended_path(path, version['previous']),
-                 self._construct_extended_path(path, version['current']))
-            )
-
-        return changeranges
+        return [
+            (self._construct_extended_path(path, version['previous']),
+             self._construct_extended_path(path, version['current']))
+            for path, version in changelist.items()
+        ]
 
     def _sanitize_checkedout_changeset(self, changeset):
         """Return extended paths for all modifications in a changeset.
 
         Args:
             changeset (unicode):
                 The changeset to fetch.
@@ -1690,22 +1703,17 @@
                        entry.new_oid.encode('utf-8')))
 
             diff_writer.write_diff_file_result_hunks(diff_result)
 
         diff_contents = stream.getvalue()
 
         if not repository_info.is_legacy:
-            # We need oids of files to translate them to paths on reviewboard
-            # repository.
-            vob_oid = execute(['cleartool', 'describe', '-fmt', '%On',
-                               'vob:%s' % (entry.new_path or entry.old_path)])
-
             vv_metadata = {
                 'directory-diff': 'legacy-filenames',
-                'vob': vob_oid,
+                'vob': entry.vob_oid,
             }
 
             if entry.op == 'create':
                 assert entry.new_path
 
                 path = os.path.relpath(entry.new_path, self.root_path)
                 revision = {
@@ -2136,28 +2144,28 @@
                                                     op='delete'))
 
             for old_file, old_oid, new_file, new_oid in changes['renamed']:
                 # Just using the old filename that we get from the
                 # directory diff will break in odd ways depending on
                 # the view type. Explicitly appending the element
                 # version seems to work.
-                old_version = execute(
-                    ['cleartool', 'describe', '-fmt', '%Vn', file.old_path])
-                old_path = '%s@@%s' % (old_file, old_version)
 
                 for file in files:
                     if (file.old_oid == old_oid or
                         file.new_oid == new_oid):
-                        file.old_path = old_path
+                        old_version = execute(['cleartool', 'describe',
+                                               '-fmt', '%Vn', file.old_path])
+                        file.old_path = '%s@@%s' % (old_file, old_version)
                         file.op = 'move'
+
                         break
                 else:
                     if not self._is_dir(new_file):
                         files.append(ChangesetEntry(self.root_path,
-                                                    old_path=old_path,
+                                                    old_path=old_file,
                                                     new_path=new_file,
                                                     old_oid=old_oid,
                                                     new_oid=new_oid,
                                                     op='move'))
 
         return files
 
@@ -2442,15 +2450,15 @@
                 tags[uuid].add(tag.strip())
             except Exception:
                 pass
 
         self.vob_tags = set()
         self.uuid_to_tags = {}
 
-        for uuid, tags in six.iteritems(tags):
+        for uuid, tags in tags.items():
             self.vob_tags.update(tags)
             self.uuid_to_tags[uuid] = list(tags)
 
         if self.is_legacy:
             self.base_path = self.vobtag
 
     def find_server_repository_info(self, api_root):
```

### Comparing `RBTools-4.0/rbtools/clients/cvs.py` & `RBTools-4.1/rbtools/clients/cvs.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/errors.py` & `RBTools-4.1/rbtools/clients/errors.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/git.py` & `RBTools-4.1/rbtools/clients/git.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """A client for Git."""
 
-from __future__ import unicode_literals
-
 import logging
 import os
 import re
 import sys
-from typing import Dict, List, Optional, cast
-
-import six
+from typing import Dict, Iterator, List, Optional, cast
 
 from rbtools.clients import PatchResult, RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
                                             SCMClientDiffResult,
                                             SCMClientRevisionSpec)
 from rbtools.clients.errors import (AmendError,
                                     CreateCommitError,
@@ -28,15 +24,17 @@
                                  deprecate_non_keyword_only_args)
 from rbtools.utils.checks import check_install
 from rbtools.utils.console import edit_text
 from rbtools.utils.diffs import (normalize_patterns,
                                  remove_filenames_matching_patterns)
 from rbtools.utils.encoding import force_unicode
 from rbtools.utils.errors import EditorError
-from rbtools.utils.process import RunProcessError, execute
+from rbtools.utils.process import (RunProcessError,
+                                   RunProcessResult,
+                                   run_process)
 
 
 def get_git_candidates(
     target_platform: str = sys.platform,
 ) -> List[str]:
     """Return candidate names for the git command line tool.
 
@@ -173,26 +171,31 @@
         Returns:
             bool:
             ``True`` if the user's installed git supports ``-c``.
         """
         if not hasattr(self, '_git_version_at_least_180'):
             self._git_version_least_180 = False
 
-            version_str = execute([self.git, 'version'], ignore_errors=True,
-                                  none_on_ignored_error=True)
+            version_str = (
+                self._run_git(['version'],
+                              ignore_errors=True)
+                .stdout
+                .read()
+                .strip()
+            )
 
             if version_str:
                 m = re.search(r'(\d+)\.(\d+)\.(\d+)', version_str)
 
                 if m:
                     git_version = (int(m.group(1)),
                                    int(m.group(2)),
                                    int(m.group(3)))
 
-                    self._git_version_at_least_180 = git_version >= (1, 8, 0)
+                    self._git_version_at_least_180 = (git_version >= (1, 8, 0))
 
         return self._git_version_at_least_180
 
     def parse_revision_spec(
         self,
         revisions: List[str] = [],
     ) -> SCMClientRevisionSpec:
@@ -225,14 +228,17 @@
 
             ``parent_base`` may also be populated.
 
         Raises:
             rbtools.clients.errors.InvalidRevisionSpecError:
                 The given revisions could not be parsed.
 
+            rbtools.clients.errors.SCMError:
+                There was an error retrieving information from Git.
+
             rbtools.clients.errors.TooManyRevisionsError:
                 The specified revisions list contained too many revisions.
         """
         n_revs = len(revisions)
         result: SCMClientRevisionSpec
 
         if n_revs == 0:
@@ -296,30 +302,43 @@
                     result = {
                         'base': parsed[0],
                         'tip': parsed[1],
                     }
             elif n_parsed_revs == 3 and parsed[2].startswith('^'):
                 # Revision spec is diff-since-merge. Find the merge-base of the
                 # two revs to use as base.
-                merge_base = self._execute([self.git, 'merge-base', parsed[0],
-                                            parsed[1]]).strip()
+                try:
+                    merge_base = (
+                        self._run_git(['merge-base', parsed[0], parsed[1]])
+                        .stdout
+                        .read()
+                        .strip()
+                    )
+                except RunProcessError:
+                    raise SCMError('Error retrieving the merge base for '
+                                   'Git revisions %s and %s'
+                                   % (parsed[0], parsed[1]))
+
                 result = {
                     'base': merge_base,
                     'tip': parsed[0],
                 }
             else:
                 raise InvalidRevisionSpecError(
                     'Unexpected result while parsing revision spec')
 
             parent_branch = self._get_parent_branch()
             remote = self._find_remote(parent_branch)
-            parent_base = self._rev_list_youngest_remote_ancestor(
-                result['base'], remote)
 
-            if parent_base != result['base']:
+            base = result['base']
+            assert isinstance(base, str)
+
+            parent_base = self._rev_list_youngest_remote_ancestor(base, remote)
+
+            if parent_base != base:
                 result['parent_base'] = parent_base
         else:
             raise TooManyRevisionsError
 
         return result
 
     def get_local_path(self) -> Optional[str]:
@@ -343,29 +362,33 @@
         self._git_dir = self._get_git_dir()
 
         if self._git_dir is None:
             return None
 
         # Sometimes core.bare is not set, and generates an error, so ignore
         # errors. Valid values are 'true' or '1'.
-        bare = execute([self.git, 'config', 'core.bare'],
-                       ignore_errors=True).strip()
-        self.bare = bare in ('true', '1')
+        self.bare = self._get_git_config('core.bare') in ('true', '1')
 
         # Running in directories other than the top level of
         # of a work-tree would result in broken diffs on the server
         if not self.bare:
-            git_top = execute([self.git, 'rev-parse', '--show-toplevel'],
-                              ignore_errors=True).rstrip('\n')
+            git_top: str
+
+            process_result = self._run_git(['rev-parse', '--show-toplevel'],
+                                           ignore_errors=True)
+
+            stderr = process_result.stderr_bytes.read()
 
             # Top level might not work on old git version se we use git dir
             # to find it.
-            if (git_top.startswith(('fatal:', 'cygdrive')) or
+            if (stderr.startswith((b'fatal:', b'cygdrive')) or
                 not os.path.isdir(self._git_dir)):
                 git_top = self._git_dir
+            else:
+                git_top = process_result.stdout.read().strip()
 
             self._git_toplevel = os.path.abspath(git_top)
 
         return self._git_toplevel
 
     def get_repository_info(self) -> Optional[RepositoryInfo]:
         """Return repository information for the current working tree.
@@ -377,29 +400,38 @@
         local_path = self.get_local_path()
 
         if not local_path:
             return None
 
         assert self._git_dir
 
-        self._head_ref = self._execute(
-            [self.git, 'symbolic-ref', '-q', 'HEAD'],
-            ignore_errors=True).strip()
+        self._head_ref = (
+            self._run_git(['symbolic-ref', '-q', 'HEAD'],
+                          ignore_errors=True)
+            .stdout
+            .read()
+            .strip()
+        )
 
         # We know we have something we can work with. Let's find out
         # what it is. We'll try SVN first, but only if there's a .git/svn
         # directory. Otherwise, it may attempt to create one and scan
         # revisions, which can be slow. Also skip SVN detection if the git
         # repository was specified on command line.
         git_svn_dir = os.path.join(self._git_dir, 'svn')
 
         if (not getattr(self.options, 'repository_url', None) and
             os.path.isdir(git_svn_dir) and
             len(os.listdir(git_svn_dir)) > 0):
-            data = self._execute([self.git, 'svn', 'info'], ignore_errors=True)
+            data = (
+                self._run_git(['svn', 'info'],
+                              ignore_errors=True)
+                .stdout
+                .read()
+            )
 
             m = re.search(r'^Repository Root: (.+)$', data, re.M)
 
             if m:
                 path = m.group(1)
                 m = re.search(r'^URL: (.+)$', data, re.M)
 
@@ -424,43 +456,55 @@
                                                  local_path=local_path,
                                                  uuid=uuid)
             else:
                 # Versions of git-svn before 1.5.4 don't (appear to) support
                 # 'git svn info'.  If we fail because of an older git install,
                 # here, figure out what version of git is installed and give
                 # the user a hint about what to do next.
-                version = self._execute([self.git, 'svn', '--version'],
-                                        ignore_errors=True)
+                version_str = (
+                    self._run_git(['svn', '--version'],
+                                  ignore_errors=True)
+                    .stdout
+                    .read()
+                    .strip()
+                )
                 version_parts = re.search(r'version (\d+)\.(\d+)\.(\d+)',
-                                          version)
-                svn_remote = self._execute(
-                    [self.git, 'config', '--get', 'svn-remote.svn.url'],
-                    ignore_errors=True)
+                                          version_str)
+                svn_remote = self._get_git_config('svn-remote.svn.url')
 
                 if version_parts and svn_remote:
                     version = (
                         int(version_parts.group(1)),
                         int(version_parts.group(2)),
                         int(version_parts.group(3)),
                     )
 
                     if version < (1, 5, 4):
                         raise SCMError('Your installation of git-svn must be '
                                        'upgraded to version 1.5.4 or later.')
 
         # Okay, maybe Perforce (git-p4).
-        git_p4_ref = self._execute(
-            [self.git, 'show-ref', '--verify', 'refs/remotes/p4/master'],
-            none_on_ignored_error=True,
-            ignore_errors=True)
+        git_p4_ref: Optional[str]
+
+        try:
+            git_p4_ref = (
+                self._run_git([
+                    'show-ref', '--verify', 'refs/remotes/p4/master',
+                ])
+                .stdout
+                .read()
+                .strip()
+            )
+        except RunProcessError:
+            git_p4_ref = None
 
         if git_p4_ref:
-            data = self._execute([self.git, 'config', '--get', 'git-p4.port'],
-                                 ignore_errors=True)
+            data = self._get_git_config('git-p4.port') or ''
             m = re.search(r'(.+)', data)
+
             if m:
                 port = m.group(1)
             else:
                 port = os.getenv('P4PORT')
 
             if port:
                 self._type = self.TYPE_GIT_P4
@@ -475,20 +519,24 @@
 
         repository_url = getattr(self.options, 'repository_url', None)
 
         if repository_url:
             url = repository_url
         else:
             upstream_branch = self._get_parent_branch()
-            url = self._get_origin(upstream_branch).rstrip('/')
 
-            if url.startswith('fatal:'):
+            try:
+                url = self._get_origin(upstream_branch)
+            except SCMError:
                 raise SCMError('Could not determine remote URL for upstream '
                                'branch %s' % upstream_branch)
 
+            if url:
+                url = url.rstrip('/')
+
             # Central bare repositories don't have origin URLs.
             # We return git_dir instead and hope for the best.
             if not url:
                 url = os.path.abspath(self._git_dir)
 
         if url:
             return RepositoryInfo(path=url,
@@ -502,18 +550,27 @@
         This will return the :file:`.git` directory corresponding to the full
         checkout, traversing up in the case of worktrees.
 
         Returns:
             unicode:
             The path to the :file:`.git` directory for the repository.
         """
-        git_dir = self._execute([self.git, 'rev-parse', '--git-dir'],
-                                ignore_errors=True).rstrip('\n')
+        try:
+            git_dir = (
+                self._run_git(['rev-parse', '--git-dir'],
+                              redirect_stderr=True,
+                              ignore_errors=True)
+                .stdout
+                .read()
+                .rstrip('\n')
+            )
+        except RunProcessError:
+            return None
 
-        if git_dir.startswith('fatal:') or not os.path.isdir(git_dir):
+        if not os.path.isdir(git_dir):
             return None
 
         try:
             # In the case of a worktree, find the common gitdir.
             with open(os.path.join(git_dir, 'commondir')) as f:
                 common_dir = f.read().strip()
                 git_dir = os.path.abspath(os.path.join(git_dir, common_dir))
@@ -539,40 +596,35 @@
         """Return the remote URL for the given upstream branch.
 
         Args:
             upstream_branch (unicode):
                 The name of the upstream branch.
 
         Returns:
-            tuple of unicode:
-            A 2-tuple, containing the upstream branch name and the remote URL.
+            str:
+            The remote URL, or ``None`` if it could not be found.
         """
-        upstream_remote = upstream_branch.split('/')[0]
-        return self._execute(
-            [self.git, 'config', '--get', 'remote.%s.url' % upstream_remote],
-            ignore_errors=True).rstrip('\n')
+        return self._get_git_config(
+            'remote.%s.url' % upstream_branch.split('/')[0])
 
     def scan_for_server(self, repository_info):
         """Find the Review Board server matching this repository.
 
         Args:
             repository_info (rbtools.clients.base.repository.RepositoryInfo):
                 The repository information structure.
 
         Returns:
-            unicode:
-            The Review Board server URL, if available.
+            str:
+            The Review Board server URL, if available, or ``None`` if not
+            found.
         """
         if self._type == self.TYPE_GIT:
             # TODO: Maybe support a server per remote later? Is that useful?
-            server_url = self._execute(
-                [self.git, 'config', '--get', 'reviewboard.url'],
-                ignore_errors=True).strip()
-
-            return server_url or None
+            return self._get_git_config('reviewboard.url')
         elif self._type == self.TYPE_GIT_SVN:
             # Try using the reviewboard:url property on the SVN repo, if it
             # exists.
             return SVNClient().scan_for_server(repository_info)
         elif self._type == self.TYPE_GIT_P4:
             return PerforceClient().scan_for_server(repository_info)
         else:
@@ -582,29 +634,47 @@
         """Extract the commit message based on the provided revision range.
 
         Args:
             revisions (dict):
                 A dictionary containing ``base`` and ``tip`` keys.
 
         Returns:
-            unicode:
+            str:
             The commit messages of all commits between (base, tip].
         """
-        return self._execute(
-            [self.git, 'log', '--reverse', '--pretty=format:%s%n%n%b',
-             '^%s' % revisions['base'], revisions['tip']],
-            ignore_errors=True).strip()
+        base = revisions['base']
+        tip = revisions['tip']
+
+        assert isinstance(base, str)
+        assert isinstance(tip, str)
+
+        return (
+            self._run_git(
+                [
+                    'log',
+                    '--reverse',
+                    '--pretty=format:%s%n%n%b',
+                    '^%s' % base,
+                    tip,
+                ],
+                ignore_errors=True)
+            .stdout
+            .read()
+            .strip()
+        )
 
     def _get_parent_branch(self):
         """Return the parent branch.
 
         Returns:
-            unicode:
+            str:
             The name of the current parent branch.
         """
+        assert self._git_dir
+
         # If the user has manually specified the parent, return that.
         parent_branch = (getattr(self.options, 'parent_branch', None) or
                          getattr(self.options, 'tracking', None))
 
         if parent_branch:
             return parent_branch
 
@@ -618,37 +688,34 @@
                                 'Defaulting to "master"\n')
                 return 'master'
         elif self._type == self.TYPE_GIT_P4:
             return 'p4/master'
         elif self._type == self.TYPE_GIT:
             if self._head_ref:
                 short_head = self._strip_heads_prefix(self._head_ref)
-                merge = self._strip_heads_prefix(self._execute(
-                    [self.git, 'config', '--get',
-                     'branch.%s.merge' % short_head],
-                    ignore_errors=True).strip())
+                merge = self._strip_heads_prefix(
+                    self._get_git_config('branch.%s.merge' % short_head) or '')
                 remote = self._get_remote(short_head)
 
                 if remote and remote != '.' and merge:
                     return '%s/%s' % (remote, merge)
 
             # As of Git 2.28, users can configure a default main branch name.
             # In most cases, this will be handled by the _get_remote call
             # above. This here is a fallback to a fallback, and assumes that if
             # they're operating with a bare checkout with a non-standard main
             # branch name, they're configured correctly.
-            defaultBranch = self._execute([self.git, 'config', '--global',
-                                           '--get', 'init.defaultBranch'],
-                                          ignore_errors=True).strip()
+            default_branch = self._get_git_config('init.defaultBranch',
+                                                  global_config=True)
 
-            if (defaultBranch and
+            if (default_branch and
                 os.path.exists(os.path.join(self._git_dir, 'refs',
                                             'remotes', 'origin',
-                                            defaultBranch))):
-                return 'origin/%s' % defaultBranch
+                                            default_branch))):
+                return 'origin/%s' % default_branch
 
             # Finally, just fall back to the old standard.
             return 'origin/master'
         else:
             raise ValueError('Unknown git client type %s' % self._type)
 
     def get_head_ref(self):
@@ -660,33 +727,38 @@
         """
         return self._head_ref or 'HEAD'
 
     def _rev_parse(self, revisions):
         """Parse a git symbolic reference.
 
         Args:
-            revisions (unicode or list):
+            revisions (str or list):
                 A set of revisions passed in by the user. This can either be a
                 single revision name or a range.
 
         Returns:
-            list of unicode:
+            list of str:
             A list of the parsed revision data. This can be either 1, 2, or 3
             elements long, depending on the exact string provided.
         """
         if not isinstance(revisions, list):
             revisions = [revisions]
 
         try:
-            revisions = self._execute([self.git, 'rev-parse'] + revisions)
+            # Note that we're using splitlines() instead of readlines() in
+            # order to keep line endings off.
+            return (
+                self._run_git(['rev-parse'] + revisions)
+                .stdout
+                .read()
+                .splitlines()
+            )
         except RunProcessError:
             return []
 
-        return revisions.strip().split('\n')
-
     def _rev_list_youngest_remote_ancestor(
         self,
         local_branch: str,
         remote: str,
     ) -> str:
         """Return the youngest ancestor of ``local_branch`` on ``remote``.
 
@@ -713,20 +785,31 @@
 
             if svn_remote_info and remote == svn_remote_info['remote']:
                 # The git-svn "remote" is not really a remote, so we can't pass
                 # it to --remotes. However, it is a valid reference we can pass
                 # directly.
                 exclude_option = remote
 
-        cmdline: List[str] = [self.git, 'rev-list', local_branch, '--not',
-                              exclude_option]
+        local_commits: List[str]
 
-        local_commits = self._execute(cmdline).split()
+        try:
+            # Note that we're using splitlines() instead of readlines() in
+            # order to keep line endings off.
+            local_commits = (
+                self._run_git([
+                    'rev-list', local_branch, '--not', exclude_option,
+                ])
+                .stdout
+                .read()
+                .splitlines()
+            )
+        except RunProcessError:
+            local_commits = []
 
-        if local_commits == []:
+        if not local_commits:
             # We are currently at a commit also available to the remote.
             return local_branch
 
         local_commit = local_commits[-1]
 
         try:
             youngest_remote_commit = self._rev_parse('%s^' % local_commit)[0]
@@ -863,32 +946,38 @@
             find_renames_threshold (unicode, optional):
                 The threshhold to pass to ``--find-renames``, if any.
 
         Returns:
             bytes:
             The diff between (base, tip].
         """
+        git_toplevel = self._git_toplevel
+        assert git_toplevel
+
+        assert isinstance(base, str)
+        assert isinstance(tip, str)
+
         rev_range = '%s..%s' % (base, tip)
 
         if include_files:
             include_files = ['--'] + include_files
 
-        git_cmd = [self.git]
+        git_args: List[str] = []
 
         if self._supports_git_config_flag():
-            git_cmd.extend(['-c', 'core.quotepath=false'])
+            git_args += ['-c', 'core.quotepath=false']
 
         if self._type in (self.TYPE_GIT_SVN, self.TYPE_GIT_P4):
             diff_cmd_params = ['--no-color', '--no-prefix', '-r', '-u']
         elif self._type == self.TYPE_GIT:
             diff_cmd_params = ['--no-color', '--full-index',
                                '--ignore-submodules']
 
             if self._supports_git_config_flag():
-                git_cmd.extend(['-c', 'diff.noprefix=false'])
+                git_args += ['-c', 'diff.noprefix=false']
 
             if (not no_renames and
                 self.capabilities is not None and
                 self.capabilities.has_capability('diffs', 'moved_files')):
 
                 if find_renames_threshold is not None:
                     diff_cmd_params.append('--find-renames=%s'
@@ -903,82 +992,78 @@
         # By default, don't allow using external diff commands. This prevents
         # things from breaking horribly if someone configures a graphical diff
         # viewer like p4merge or kaleidoscope. This can be overridden by
         # setting GIT_USE_EXT_DIFF = True in ~/.reviewboardrc
         if not self.config.get('GIT_USE_EXT_DIFF', False):
             diff_cmd_params.append('--no-ext-diff')
 
-        diff_cmd = git_cmd + ['diff'] + diff_cmd_params
+        diff_cmd = git_args + ['diff'] + diff_cmd_params
 
         if exclude_patterns:
             # If we have specified files to exclude, we will get a list of all
             # changed files and run `git diff` on each un-excluded file
             # individually.
-            changed_files_cmd = git_cmd + ['diff-tree'] + diff_cmd_params
+            changed_files_cmd = git_args + ['diff-tree'] + diff_cmd_params
 
             if self._type in (self.TYPE_GIT_SVN, self.TYPE_GIT_P4):
                 # We don't want to send -u along to git diff-tree because it
                 # will generate diff information along with the list of
                 # changed files.
                 changed_files_cmd.remove('-u')
             elif self._type == self.TYPE_GIT:
                 changed_files_cmd.append('-r')
 
-            changed_files = self._execute(
-                changed_files_cmd + [rev_range] + include_files,
-                split_lines=True,
-                with_errors=False,
-                ignore_errors=True,
-                none_on_ignored_error=True,
-                log_output_on_error=False)
-
-            git_toplevel = self._git_toplevel
-            assert git_toplevel
+            changed_files: Iterator[str] = (
+                self._run_git(
+                    changed_files_cmd + [rev_range] + include_files,
+                    ignore_errors=True,
+                    log_debug_output_on_error=False)
+                .stdout
+            )
 
             # The output of git diff-tree will be a list of entries that have
             # changed between the two revisions that we give it. The last part
             # of the line is the name of the file that has changed.
             changed_files = remove_filenames_matching_patterns(
                 filenames=(
                     filename.split()[-1]
                     for filename in changed_files
                 ),
                 patterns=exclude_patterns,
                 base_dir=git_toplevel)
 
-            diff_lines = []
+            diff_lines: List[bytes] = []
 
             for filename in changed_files:
-                lines = self._execute(diff_cmd + [rev_range, '--', filename],
-                                      split_lines=True,
-                                      with_errors=False,
-                                      ignore_errors=True,
-                                      none_on_ignored_error=True,
-                                      log_output_on_error=False,
-                                      results_unicode=False)
+                lines = (
+                    self._run_git(diff_cmd + [rev_range, '--', filename],
+                                  ignore_errors=True,
+                                  log_debug_output_on_error=False)
+                    .stdout_bytes
+                    .readlines()
+                )
 
-                if lines is None:
+                if not lines:
                     logging.error(
                         'Could not get diff for all files (git-diff failed '
                         'for "%s"). Refusing to return a partial diff.',
                         filename)
 
-                    diff_lines = None
+                    diff_lines = []
                     break
 
                 diff_lines += lines
-
         else:
-            diff_lines = self._execute(diff_cmd + [rev_range] + include_files,
-                                       split_lines=True,
-                                       with_errors=False,
-                                       ignore_errors=True,
-                                       none_on_ignored_error=True,
-                                       log_output_on_error=False,
-                                       results_unicode=False)
+            diff_lines = (
+                self._run_git(diff_cmd + [rev_range] + include_files,
+                              ignore_errors=True,
+                              log_debug_output_on_error=False)
+                .stdout_bytes
+                .readlines()
+            )
 
         if self._type == self.TYPE_GIT_SVN:
             return self.make_svn_diff(merge_base, diff_lines)
         elif self._type == self.TYPE_GIT_P4:
             return self.make_perforce_diff(merge_base, diff_lines)
         else:
             return b''.join(diff_lines)
@@ -1002,17 +1087,21 @@
             diff_lines (list of bytes):
                 The lines of the diff.
 
         Returns:
             bytes:
             The reformatted diff contents.
         """
-        rev = self._execute(
-            [self.git, 'svn', 'find-rev', merge_base],
-            results_unicode=False).strip()
+        rev = (
+            self._run_git(['svn', 'find-rev', merge_base],
+                          ignore_errors=True)
+            .stdout_bytes
+            .read()
+            .strip()
+        )
 
         if not rev:
             return None
 
         diff_data = b''
         old_filename = b''
         new_filename = b''
@@ -1112,21 +1201,23 @@
         diff_data = b''
         old_filename = b''
         new_filename = b''
         p4rev = b''
         is_full_rename = False
 
         # Find which depot changelist we're based on
-        log = self._execute([self.git, 'log', merge_base],
-                            ignore_errors=True,
-                            results_unicode=False)
+        log = (
+            self._run_git(['log', merge_base],
+                          ignore_errors=True)
+            .stdout_bytes
+        )
 
         for line in log:
             m = re.search(br'[rd]epo.-paths = "(.+)": change = (\d+).*\]',
-                          log, re.M)
+                          line, re.M)
 
             if m:
                 base_path = m.group(1).strip()
                 p4rev = m.group(2).strip()
                 break
             else:
                 # We should really raise an error here, base_path is required
@@ -1171,17 +1262,20 @@
                 # Followed by an empty line. We then skip the following 2 lines
                 # which would otherwise print "Move from: ..." and
                 # "Move to: ...".
                 old_filename = diff_lines[i + 1].split(b' ', 2)[2].strip()
                 new_filename = diff_lines[i + 2].split(b' ', 2)[2].strip()
 
                 p4path = force_unicode(base_path + old_filename + b'@' + p4rev)
-                data = self._execute(['p4', 'files', p4path],
-                                     ignore_errors=True,
-                                     results_unicode=False)
+                data = (
+                    self._run_process(['p4', 'files', p4path],
+                                      ignore_errors=True)
+                    .stdout_bytes
+                    .read()
+                )
                 m = re.search(br'^%s%s#(\d+).*$' % (re.escape(base_path),
                                                     re.escape(old_filename)),
                               data, re.M)
 
                 if m:
                     file_version = m.group(1).strip()
                 else:
@@ -1240,17 +1334,20 @@
                     # out the +++ line.
                     new_filename = old_filename
                 elif old_filename == b'/dev/null':
                     # The file is new, use the new filename in the --- line.
                     old_filename = new_filename
 
                 p4path = force_unicode(base_path + old_filename + b'@' + p4rev)
-                data = self._execute(['p4', 'files', p4path],
-                                     ignore_errors=True,
-                                     results_unicode=False)
+                data = (
+                    self._run_process(['p4', 'files', p4path],
+                                      ignore_errors=True)
+                    .stdout_bytes
+                    .read()
+                )
                 m = re.search(br'^%s%s#(\d+).*$' % (re.escape(base_path),
                                                     re.escape(old_filename)),
                               data, re.M)
 
                 if m:
                     file_version = m.group(1).strip()
                 else:
@@ -1274,48 +1371,59 @@
         """Check if there are changes waiting to be committed.
 
         Returns:
             bool:
             ``True`` if the working directory has been modified or if changes
             have been staged in the index.
         """
-        status = self._execute(['git', 'status', '--porcelain',
-                                '--untracked-files=no',
-                                '--ignore-submodules=dirty'])
-        return status != ''
+        try:
+            return (
+                self._run_git([
+                    'status',
+                    '--porcelain',
+                    '--untracked-files=no',
+                    '--ignore-submodules=dirty',
+                ])
+                .stdout_bytes
+                .read(1)
+            ) != b''
+        except RunProcessError:
+            return False
 
     def amend_commit_description(self, message, revisions):
         """Update a commit message to the given string.
 
         Args:
             message (unicode):
                 The commit message to use when amending the commit.
 
             revisions (dict):
                 A dictionary of revisions, as returned by
                 :py:meth:`parse_revision_spec`.
 
         Raises:
             rbtools.clients.errors.AmendError:
-                The requested revision tip was not the most recent commit.
-                Unless rewriting the entire series of commits, git can only
-                amend the latest commit on the branch.
+                The commit could not be amended.
+
+                This may occur if the tip is not the most recent commit, or
+                if there's an error invoking git.
         """
         if revisions and revisions['tip']:
-            commit_ids = self._execute(
-                [self.git, 'rev-parse', 'HEAD', revisions['tip']],
-                split_lines=True)
+            commit_ids = self._rev_parse(['HEAD', revisions['tip']])
             head_id = commit_ids[0].strip()
             revision_id = commit_ids[1].strip()
 
             if head_id != revision_id:
                 raise AmendError('Commit "%s" is not the latest commit, '
                                  'and thus cannot be modified' % revision_id)
 
-        self._execute([self.git, 'commit', '--amend', '-m', message])
+        try:
+            self._run_git(['commit', '--amend', '-m', message])
+        except RunProcessError as e:
+            raise AmendError(str(e))
 
     def apply_patch(self, patch_file, base_path=None, base_dir=None, p=None,
                     revert=False):
         """Apply the given patch to index.
 
         This will take the given patch file and apply it to the index,
         scheduling all changes for commit.
@@ -1339,31 +1447,30 @@
             revert (bool, optional):
                 Whether the patch should be reverted rather than applied.
 
         Returns:
             rbtools.clients.base.patch.PatchResult:
             The result of the patch operation.
         """
-        cmd = ['git', 'apply', '-3']
+        cmd = ['apply', '-3']
 
         if revert:
             cmd.append('-R')
 
         if p:
             cmd += ['-p', p]
 
         cmd.append(patch_file)
 
-        rc, data = self._execute(cmd,
-                                 ignore_errors=True,
-                                 with_errors=True,
-                                 return_error_code=True,
-                                 results_unicode=False)
+        patch_output = self._run_git(cmd,
+                                     ignore_errors=True,
+                                     redirect_stderr=True)
+        data = patch_output.stdout_bytes.read()
 
-        if rc == 0:
+        if patch_output.exit_code == 0:
             return PatchResult(applied=True, patch_output=data)
         elif b'with conflicts' in data:
             return PatchResult(
                 applied=True,
                 has_conflicts=True,
                 conflicting_files=[
                     line.split(b' ', 1)[1]
@@ -1404,69 +1511,76 @@
         Raises:
             rbtools.clients.errors.CreateCommitError:
                 The commit message could not be created. It may have been
                 aborted by the user.
         """
         try:
             if all_files:
-                self._execute(['git', 'add', '--all', ':/'])
+                self._run_git(['add', '--all', ':/'])
             elif files:
-                self._execute(['git', 'add'] + files)
-        except Exception as e:
-            raise CreateCommitError(six.text_type(e))
+                self._run_git(['add'] + files)
+        except RunProcessError as e:
+            raise CreateCommitError(str(e))
 
         if run_editor:
             try:
                 modified_message = edit_text(message,
                                              filename='COMMIT_EDITMSG')
             except EditorError as e:
-                raise CreateCommitError(six.text_type(e))
+                raise CreateCommitError(str(e))
         else:
             modified_message = message
 
         if not modified_message.strip():
             raise CreateCommitError(
                 "A commit message wasn't provided. The patched files are in "
                 "your tree and are staged for commit, but haven't been "
                 "committed. Run `git commit` to commit them.")
 
-        cmd = ['git', 'commit', '-m', modified_message]
+        cmd = ['commit', '-m', modified_message]
 
         try:
             cmd += ['--author', '%s <%s>' % (author.fullname, author.email)]
         except AttributeError:
             # Users who have marked their profile as private won't include the
             # fullname or email fields in the API payload. Just commit as the
             # user running RBTools.
             logging.warning('The author has marked their Review Board profile '
                             'information as private. Committing without '
                             'author attribution.')
 
         try:
-            self._execute(cmd)
-        except Exception as e:
-            raise CreateCommitError(six.text_type(e))
+            self._run_git(cmd)
+        except RunProcessError as e:
+            raise CreateCommitError(str(e))
 
     def delete_branch(self, branch_name, merged_only=True):
         """Delete the specified branch.
 
         Args:
             branch_name (unicode):
                 The name of the branch to delete.
 
             merged_only (bool, optional):
                 Whether to limit branch deletion to only those branches which
                 have been merged into the current HEAD.
+
+        Raises:
+            rbtools.clients.errors.SCMError:
+                An error occurred while deleting the branch.
         """
         if merged_only:
             delete_flag = '-d'
         else:
             delete_flag = '-D'
 
-        self._execute(['git', 'branch', delete_flag, branch_name])
+        try:
+            self._run_git(['branch', delete_flag, branch_name])
+        except RunProcessError as e:
+            raise SCMError(str(e))
 
     def merge(self, target, destination, message, author, squash=False,
               run_editor=False, close_branch=False, **kwargs):
         """Merge the target branch with destination branch.
 
         Args:
             target (unicode):
@@ -1495,41 +1609,53 @@
             **kwargs (dict, unused):
                 Additional keyword arguments passed, for future expansion.
 
         Raises:
             rbtools.clients.errors.MergeError:
                 An error occurred while merging the branch.
         """
-        rc, output = self._execute(
-            ['git', 'checkout', destination],
-            ignore_errors=True,
-            return_error_code=True)
-
-        if rc:
-            raise MergeError('Could not checkout to branch "%s".\n\n%s' %
-                             (destination, output))
+        try:
+            self._run_git(['checkout', destination],
+                          redirect_stderr=True)
+        except RunProcessError as e:
+            raise MergeError(
+                'Could not checkout to branch "%(destination)s".\n'
+                '\n'
+                '%(output)s'
+                % {
+                    'destination': destination,
+                    'output': e.result.stdout.read(),
+                })
 
         if squash:
             method = '--squash'
         else:
             method = '--no-ff'
 
-        rc, output = self._execute(
-            ['git', 'merge', target, method, '--no-commit'],
-            ignore_errors=True,
-            return_error_code=True)
-
-        if rc:
-            raise MergeError('Could not merge branch "%s" into "%s".\n\n%s' %
-                             (target, destination, output))
+        try:
+            self._run_git(['merge', target, method, '--no-commit'],
+                          redirect_stderr=True)
+        except RunProcessError as e:
+            raise MergeError(
+                'Could not merge branch "%(target)s" into "%(destination)s".\n'
+                '\n'
+                '%(output)s'
+                % {
+                    'destination': destination,
+                    'output': e.result.stdout.read(),
+                    'target': target,
+                })
 
-        self.create_commit(message, author, run_editor)
+        try:
+            self.create_commit(message, author, run_editor)
 
-        if close_branch:
-            self.delete_branch(target, merged_only=False)
+            if close_branch:
+                self.delete_branch(target, merged_only=False)
+        except (CreateCommitError, SCMError) as e:
+            raise MergeError(str(e))
 
     def push_upstream(self, local_branch):
         """Push the current branch to upstream.
 
         Args:
             local_branch (unicode):
                 The name of the branch to push.
@@ -1540,63 +1666,134 @@
         """
         remote = self._get_remote(local_branch)
 
         if remote is None:
             raise PushError('Could not determine remote for branch "%s".'
                             % local_branch)
 
-        rc, output = self._execute(
-            ['git', 'pull', '--rebase', remote, local_branch],
-            ignore_errors=True,
-            return_error_code=True)
-
-        if rc:
+        try:
+            self._run_git(['pull', '--rebase', remote, local_branch])
+        except RunProcessError:
             raise PushError('Could not pull changes from upstream.')
 
-        rc, output = self._execute(
-            ['git', 'push', remote, local_branch],
-            ignore_errors=True,
-            return_error_code=True)
-
-        if rc:
-            raise PushError('Could not push branch "%s" to upstream.' %
-                            local_branch)
+        try:
+            self._run_git(['push', remote, local_branch])
+        except RunProcessError:
+            raise PushError('Could not push branch "%s" to upstream.'
+                            % local_branch)
 
     def get_current_branch(self):
         """Return the name of the current branch.
 
         Returns:
             unicode:
             The name of the directory corresponding to the root of the current
             working directory (whether a plain checkout or a git worktree). If
             no repository can be found, this will return None.
         """
-        return self._execute([self.git, 'rev-parse', '--abbrev-ref', 'HEAD'],
-                             ignore_errors=True).strip()
+        try:
+            return (
+                self._run_git(['rev-parse', '--abbrev-ref', 'HEAD'])
+                .stdout
+                .read()
+                .strip()
+            )
+        except RunProcessError:
+            return None
+
+    def _get_git_config(
+        self,
+        key: str,
+        global_config: bool = False,
+    ) -> Optional[str]:
+        """Return the value of a Git configuration key.
+
+        The value will be stripped, if found.
+
+        Args:
+            key (str):
+                The key to retrieve.
+
+            global_config (bool, optional):
+                Whether to retrieve this from the global Git config, rather
+                than the local clone's.
+
+        Returns:
+            str:
+            The value from the key, or ``None`` if not found.
+
+        Raises:
+            rbtools.clients.errors.SCMError:
+                There was a fatal error retrieving Git configuration.
+        """
+        cmdline: List[str] = ['config']
+
+        if global_config:
+            cmdline.append('--global')
+
+        cmdline += ['--get', key]
 
-    def _execute(self, cmdline, *args, **kwargs):
-        """Execute a git command within the correct cwd.
+        try:
+            return (
+                self._run_git(cmdline)
+                .stdout
+                .read()
+                .strip()
+            )
+        except RunProcessError as e:
+            errors = e.result.stderr.read()
+
+            if errors.startswith('fatal:'):
+                raise SCMError(errors)
+
+            return None
+
+    def _run_git(
+        self,
+        git_args: List[str],
+        **kwargs,
+    ) -> RunProcessResult:
+        """Execute a git command within the clone directory.
 
         Args:
-            cmdline (list of unicode):
-                A command-line to execute.
+            git_args (list of str):
+                A list of additional arguments to add to the Git command line.
 
-            *args (list):
-                Positional arguments to pass through to
-                :py:func:`rbtools.utils.process.execute`.
+            *kwargs (dict):
+                Keyword arguments to pass through to
+                :py:func:`rbtools.utils.process.run_process.`.
+
+        Returns:
+            rbtools.utils.process.RunProcessResult:
+            The value returned by :py:func:`rbtools.utils.process.run_process`.
+        """
+        return self._run_process([self.git] + git_args, **kwargs)
+
+    def _run_process(
+        self,
+        cmdline: List[str],
+        **kwargs,
+    ) -> RunProcessResult:
+        """Execute a command within the clone directory.
+
+        Args:
+            cmdline (list of str):
+                The full command line to run.
 
             *kwargs (dict):
                 Keyword arguments to pass through to
-                :py:func:`rbtools.utils.process.execute`.
+                :py:func:`rbtools.utils.process.run_process.`.
 
         Returns:
-            tuple:
-            The result from the execute call.
+            rbtools.utils.process.RunProcessResult:
+            The value returned by :py:func:`rbtools.utils.process.run_process`.
         """
-        return execute(cmdline, cwd=self._git_toplevel, *args, **kwargs)
+        return run_process(cmdline,
+                           cwd=self._git_toplevel,
+                           **kwargs)
 
     def get_commit_history(self, revisions):
         """Return the commit history specified by the revisions.
 
         Args:
             revisions (dict):
                 A dictionary of revisions to generate history for, as returned
@@ -1634,50 +1831,56 @@
             ``commit_message``:
                 The commit's message.
 
         Raises:
             rbtools.clients.errors.SCMError:
                 The history is non-linear or there is a commit with no parents.
         """
+        base = revisions['base']
+        tip = revisions['tip']
+
+        assert isinstance(base, str)
+        assert isinstance(tip, str)
+
         log_fields = {
-            'commit_id': b'%H',
-            'parent_id': b'%P',
-            'author_name': b'%an',
-            'author_email': b'%ae',
-            'author_date': b'%ad',
-            'committer_name': b'%cn',
-            'committer_email': b'%ce',
-            'committer_date': b'%cd',
-            'commit_message': b'%B',
+            'commit_id': '%H',
+            'parent_id': '%P',
+            'author_name': '%an',
+            'author_email': '%ae',
+            'author_date': '%ad',
+            'committer_name': '%cn',
+            'committer_email': '%ce',
+            'committer_date': '%cd',
+            'commit_message': '%B',
         }
 
         # 0x1f is the ASCII field separator. It is a non-printable character
         # that should not appear in any field in `git log`.
-        log_format = b'%x1f'.join(six.itervalues(log_fields))
+        log_format = '%x1f'.join(log_fields.values())
 
-        log_entries = execute(
-            [
-                self.git,
-                b'log',
-                b'-z',
-                b'--reverse',
-                b'--pretty=format:%s' % log_format,
-                b'--date=iso8601-strict',
-                b'%s..%s' % (revisions['base'].encode('utf-8'),
-                             revisions['tip'].encode('utf-8')),
-            ],
-            ignore_errors=True,
-            none_on_ignored_error=True,
-            results_unicode=True)
+        log_entries = (
+            self._run_git(
+                [
+                    'log',
+                    '-z',
+                    '--reverse',
+                    '--pretty=format:%s' % log_format,
+                    '--date=iso8601-strict',
+                    '%s..%s' % (base, tip),
+                ],
+                ignore_errors=True)
+            .stdout
+            .read()
+        )
 
         if not log_entries:
             return None
 
         history = []
-        field_names = six.viewkeys(log_fields)
+        field_names = log_fields.keys()
 
         for log_entry in log_entries.split(self._NUL):
             fields = log_entry.split(self._FIELD_SEP)
             entry = dict(zip(field_names, fields))
 
             parents = entry['parent_id'].split()
 
@@ -1702,23 +1905,20 @@
                 The name of the local branch.
 
         Returns:
             unicode:
             The name of the remote corresponding to the local branch. May
             return None if there is no remote.
         """
-        rc, output = self._execute(
-            ['git', 'config', '--get', 'branch.%s.remote' % local_branch],
-            ignore_errors=True,
-            return_error_code=True)
+        remote = self._get_git_config('branch.%s.remote' % local_branch)
 
-        if rc == 0:
-            return output.strip()
-        else:
-            return None
+        if remote:
+            return remote.strip()
+
+        return None
 
     def _get_svn_remote(self) -> Dict[str, str]:
         """Return information on the SVN remote.
 
         This will include the remote branch name corresponding to the SVN clone
         and the full reference.
 
@@ -1738,17 +1938,20 @@
                     The remote name.
         """
         assert self._type == self.TYPE_GIT_SVN
 
         svn_remote_info = self._git_svn_remote_info
 
         if svn_remote_info is None:
-            data = self._execute(
-                [self.git, 'svn', 'rebase', '-n'],
-                ignore_errors=True)
+            data = (
+                self._run_git(['svn', 'rebase', '-n'],
+                              ignore_errors=True)
+                .stdout
+                .read()
+            )
 
             m = re.search(
                 r'^Remote Branch:\s*'
                 r'(?P<ref>(refs\/remotes\/)?(?P<remote>.+))$',
                 data, re.M)
 
             if m:
@@ -1780,16 +1983,19 @@
 
         Raises:
             rbtools.clients.errors.SCMError:
                 The current repository did not have any remotes configured.
         """
         all_remote_branches = {
             branch.strip()
-            for branch in self._execute(['git', 'branch', '--remotes'],
-                                        split_lines=True)
+            for branch in (
+                self._run_git(['branch', '--remotes'],
+                              ignore_errors=True)
+                .stdout
+            )
         }
 
         if local_or_remote_branch in all_remote_branches:
             return local_or_remote_branch.split('/', 1)[0]
 
         remote = self._get_remote(local_or_remote_branch)
 
@@ -1802,16 +2008,19 @@
 
             if svn_remote_info:
                 return svn_remote_info['remote']
 
         # Try to find a reasonable remote to use.
         all_remotes = [
             _remote.strip()
-            for _remote in self._execute(['git', 'remote'],
-                                         split_lines=True)
+            for _remote in (
+                self._run_git(['remote'],
+                              ignore_errors=True)
+                .stdout
+            )
         ]
 
         if len(all_remotes) >= 1:
             # We prefer "origin" if it's present, otherwise just choose at
             # random.
             if 'origin' in all_remotes:
                 return 'origin'
```

### Comparing `RBTools-4.0/rbtools/clients/mercurial.py` & `RBTools-4.1/rbtools/clients/mercurial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 """A client for Mercurial."""
 
-from __future__ import unicode_literals
-
 import logging
 import os
 import re
 import uuid
 from typing import List, Optional
-
-import six
-from six.moves.urllib.parse import urlsplit, urlunparse
+from urllib.parse import urlsplit, urlunparse
 
 from rbtools.clients import PatchResult, RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
                                             SCMClientDiffResult,
                                             SCMClientRevisionSpec)
 from rbtools.clients.errors import (CreateCommitError,
                                     InvalidRevisionSpecError,
@@ -235,15 +231,15 @@
             'parent_id': '{p1node}',
             'author_name': '{author|person}',
             'author_email': '{author|email}',
             'author_date': '{date|rfc3339date}',
             'parent2': '{p2node}',
             'commit_message': '{desc}',
         }
-        log_format = self._FIELD_SEP_ESC.join(six.itervalues(log_fields))
+        log_format = self._FIELD_SEP_ESC.join(log_fields.values())
 
         log_entries = self._execute(
             [
                 self._exe,
                 'log',
                 '--template',
                 '%s%s' % (log_format, self._RECORD_SEP_ESC),
@@ -254,15 +250,15 @@
             none_on_ignored_error=True,
             results_unicode=True)
 
         if not log_entries:
             return None
 
         history = []
-        field_names = six.viewkeys(log_fields)
+        field_names = log_fields.keys()
 
         # The ASCII record separator will be appended to every record, so if we
         # attempt to split the entire output by the record separator, we will
         # end up with an empty ``log_entry`` at the end, which will cause
         # errors.
         for log_entry in log_entries[:-1].split(self._RECORD_SEP):
             fields = log_entry.split(self._FIELD_SEP)
@@ -929,15 +925,15 @@
             filename = make_tempfile(content=message.encode('utf-8'),
                                      prefix='hg-editor-',
                                      suffix='.txt')
 
             try:
                 modified_message = edit_file(filename)
             except EditorError as e:
-                raise CreateCommitError(six.text_type(e))
+                raise CreateCommitError(str(e))
             finally:
                 try:
                     os.unlink(filename)
                 except OSError:
                     pass
         else:
             modified_message = message
@@ -963,15 +959,15 @@
             hg_command.append('-A')
         else:
             hg_command += files
 
         try:
             self._execute(hg_command)
         except Exception as e:
-            raise CreateCommitError(six.text_type(e))
+            raise CreateCommitError(str(e))
 
     def merge(self, target, destination, message, author, squash=False,
               run_editor=False, close_branch=False, **kwargs):
         """Merge the target branch with destination branch.
 
         Args:
             target (unicode):
```

### Comparing `RBTools-4.0/rbtools/clients/perforce.py` & `RBTools-4.1/rbtools/clients/perforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 import stat
 import string
 import subprocess
 import sys
 from fnmatch import fnmatch
 from typing import List, Optional, Tuple, Union
 
-import six
-
 from rbtools.clients import RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
                                             SCMClientDiffResult,
                                             SCMClientRevisionSpec)
 from rbtools.clients.errors import (AmendError,
                                     EmptyChangeError,
                                     InvalidRevisionSpecError,
@@ -101,27 +99,36 @@
 
         Returns:
             object:
             The contents of the change description, either as a unicode
             object or a list depending on the value of ``marshalled``.
         """
         return self.run_p4(['change', '-o', str(changenum)],
-                           ignore_errors=True,
                            none_on_ignored_error=True,
                            marshalled=marshalled)
 
-    def modify_change(self, new_change_spec):
+    def modify_change(
+        self,
+        new_change_spec: str,
+        *,
+        changenum: Optional[str] = None,
+    ) -> None:
         """Modify a change description.
 
         Args:
             new_change_spec (unicode):
                 The new changeset description. This must contain the changelist
                 number.
         """
-        self.run_p4(['change', '-i'], input_string=new_change_spec)
+        args: List[str] = ['change', '-i']
+
+        if changenum is not None:
+            args.append(changenum)
+
+        self.run_p4(args, input_string=new_change_spec)
 
     def files(self, path):
         """Return the opened files within the given path.
 
         Args:
             path (unicode):
                 The Perforce path to check. This can be a mix of file paths
@@ -306,15 +313,18 @@
 
         if getattr(self.options, 'p4_passwd', None):
             cmd += ['-P', self.options.p4_passwd]
 
         cmd += p4_args
 
         if marshalled:
-            p = subprocess.Popen(cmd, stdout=subprocess.PIPE)
+            logging.debug('Running: %s', subprocess.list2cmdline(cmd))
+            p = subprocess.Popen(cmd,
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE)
             result = []
             has_error = False
 
             while 1:
                 try:
                     decoded_data = marshal.load(p.stdout)
                 except EOFError:
@@ -332,15 +342,15 @@
                                        'file a bug about this.'
                                        % type(decoded_data))
 
                     # The dictionary data should consist of byte strings.
                     # We need to convert these over to Unicode.
                     data = {}
 
-                    for key, value in six.iteritems(decoded_data):
+                    for key, value in decoded_data.items():
                         key = force_unicode(key)
 
                         # Values are typically strings, but error payloads
                         # contain integers as well.
                         if isinstance(value, bytes):
                             value = force_unicode(value)
 
@@ -349,31 +359,50 @@
                     result.append(data)
 
                     if data.get('code') == 'error':
                         has_error = True
 
             rc = p.wait()
 
+            try:
+                stderr = p.stderr.read()
+            except Exception as e:
+                stderr = '<stderr exception: %r>' % e
+
+            logging.debug('Command results = %r; stderr=%r',
+                          result, stderr)
+
             if not ignore_errors and (rc or has_error):
                 for record in result:
                     if 'data' in record:
                         print(record['data'])
 
-                raise SCMError('Failed to execute command: %s' % cmd)
+                raise SCMError(
+                    'Failed to execute command `%s`; payload=%r, stderr=%r'
+                    % (subprocess.list2cmdline(cmd), result, stderr))
 
             return result
         elif input_string is not None:
             if not isinstance(input_string, bytes):
                 input_string = input_string.encode('utf8')
 
-            p = subprocess.Popen(cmd, stdin=subprocess.PIPE)
-            p.communicate(input_string)  # Send input, wait, set returncode
+            p = subprocess.Popen(cmd, stdin=subprocess.PIPE,
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.PIPE)
 
-            if not ignore_errors and p.returncode:
-                raise SCMError('Failed to execute command: %s' % cmd)
+            try:
+                stdout, stderr = p.communicate(input_string, timeout=30)
+            except subprocess.TimeoutExpired:
+                p.kill()
+                stdout, stderr = p.communicate()
+
+            if not ignore_errors and p.returncode != 0:
+                raise SCMError('Failed to execute command: %s; stdout=%r; '
+                               'stderr=%r'
+                               % (cmd, stdout, stderr))
 
             return None
         else:
             result = execute(cmd, ignore_errors=ignore_errors, *args, **kwargs)
 
         return result
 
@@ -800,15 +829,15 @@
         url = counters.get('reviewboard.url', None)
 
         if url:
             return url
 
         # Next try for a counter of the form:
         # reviewboard_url.http:||reviewboard.example.com
-        for key, value in six.iteritems(counters):
+        for key, value in counters.items():
             m = self.ENCODED_COUNTER_URL_RE.match(key)
 
             if m:
                 return m.group(1).replace('|', '/')
 
         return None
 
@@ -1220,17 +1249,19 @@
                 cid += 1
 
                 changesets.setdefault(cln, {})[depot_file] = change
 
         # Now run through the changesets in order and compute a change journal
         # for each file.
         files = []
+
         for cln in sorted(changesets.keys()):
             changeset = changesets[cln]
-            for depot_file, change in six.iteritems(changeset):
+
+            for depot_file, change in changeset.items():
                 action = change['action']
 
                 # Moves will be handled in the 'move/delete' entry
                 if action == 'move/add':
                     continue
 
                 file_entry = None
@@ -1807,16 +1838,15 @@
                             m[1] = record
                         except KeyError:
                             files[record['depotFile']] = [None, record]
 
             old_file = new_file = empty_filename
             changetype_short = None
 
-            for depot_path, (first_record, second_record) in \
-                    six.iteritems(files):
+            for depot_path, (first_record, second_record) in files.items():
                 old_file = new_file = empty_filename
                 if first_record is None:
                     new_path = '%s#%s' % (depot_path, second_record['rev'])
                     self._write_file(new_path, tmp_diff_to_filename)
                     new_file = tmp_diff_to_filename
                     changetype_short = 'A'
                     base_revision = 0
@@ -2245,60 +2275,62 @@
                 # current working directory.
                 p = os.path.join(cwd, p)
 
             return os.path.normpath(p)
 
         return [normalize(pattern) for pattern in patterns]
 
-    def _replace_description_in_changelist_spec(self, old_spec,
-                                                new_description):
+    def _replace_changeset_description(
+        self,
+        old_spec: str,
+        new_description: str,
+    ) -> str:
         """Replace the description in the given changelist spec.
 
         Args:
-            old_spec (unicode):
+            old_spec (str):
                 The p4 changelist spec string (the raw output from p4 change).
 
-            new_description (unicode):
+            new_description (str):
                 The new description text to use.
 
         Returns:
-            unicode:
+            str:
             The new changelist spec.
         """
-        new_spec = ''
-        whitespace = tuple(string.whitespace)
-        description_key = 'Description:'
-        skipping_old_description = False
+        new_lines: List[str] = []
+        key = 'Description:'
+        skipping_to_next_field: bool = False
 
         for line in old_spec.splitlines(True):
-            if not skipping_old_description:
-                if not line.startswith(description_key):
-                    new_spec += line
-
-                else:
-                    # Insert the new description. Don't include the first line
-                    # of the old one if it happens to be on the same line as
-                    # the key.
-                    skipping_old_description = True
-                    new_spec += description_key
-
-                    for desc_line in new_description.splitlines():
-                        new_spec += '\t%s\n' % desc_line
-
+            if skipping_to_next_field:
+                # Ignore the content in the current field until we find another
+                # key. We'll skip anything that starts with whitespace, which
+                # would indicate content within the current field.
+                if not line[0].isspace():
+                    # There's content here, so we're in a field again.
+                    # Mark it, and make sure to add a leading newline to
+                    # separate this field from the previously-injected
+                    # content.
+                    skipping_to_next_field = False
+                    new_lines.append(f'\n{line}')
+            elif line.startswith(key):
+                # Insert the new description. Don't include the first line
+                # of the old one if it happens to be on the same line as
+                # the key.
+                new_lines.append(f'{key}\n')
+                new_lines += [
+                    f'\t{_line}\n'
+                    for _line in new_description.splitlines()
+                ]
+                skipping_to_next_field = True
             else:
-                # Ignore the description from the original file (all lines
-                # that start with whitespace until the next key is
-                # encountered).
-                if line.startswith(whitespace):
-                    continue
-                else:
-                    skipping_old_description = False
-                    new_spec += '\n%s' % line
+                new_lines.append(line)
 
-        return new_spec
+        return ''.join(new_lines)
 
     def amend_commit_description(self, message, revisions):
         """Update a commit message to the given string.
 
         Since local changelists on Perforce have no ordering with respect to
         each other, the revisions argument is mandatory.
 
@@ -2330,10 +2362,10 @@
         elif not changelist_num.isdigit():
             raise AmendError('%s is an invalid changelist ID' % changelist_num)
 
         # Get the current changelist description and insert the new message.
         # Since p4 change -i doesn't take in marshalled objects, we get the
         # description as raw text and manually edit it.
         change = self.p4.change(changelist_num, marshalled=False)
-        new_change = self._replace_description_in_changelist_spec(
-            change, message)
+        new_change = self._replace_changeset_description(change, message)
+
         self.p4.modify_change(new_change)
```

### Comparing `RBTools-4.0/rbtools/clients/plastic.py` & `RBTools-4.1/rbtools/clients/plastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """A client for Plastic SCM."""
 
-from __future__ import unicode_literals
-
 import logging
 import os
 import re
 from typing import List, Optional
 
 from rbtools.clients import RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
```

### Comparing `RBTools-4.0/rbtools/clients/sos.py` & `RBTools-4.1/rbtools/clients/sos.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,25 @@
 `Cliosoft SOS <https://www.cliosoft.com/products/sos/>`_ is an Enterprise
 SCM focused on hardware design and configuration management.
 
 Version Added:
     3.1
 """
 
-from __future__ import unicode_literals
-
 import io
 import logging
 import os
 import re
 import sqlite3
 from collections import OrderedDict
 from contextlib import contextmanager
 from typing import List, Optional, Union, cast
 
-import six
 from pydiffx import DiffType, DiffX
 from pydiffx.utils.text import guess_line_endings
-from six.moves import range
 from typing_extensions import NotRequired, TypedDict
 
 from rbtools.api.resource import ReviewRequestResource
 from rbtools.clients import RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
                                             SCMClientDiffResult,
                                             SCMClientRevisionSpec)
@@ -722,15 +718,15 @@
                 diffx_file.meta['op'] = op
 
                 # Note that currently, a revision range of older files
                 # cannot be diffed, so we don't have a "new" key to include.
                 # This might change in the future.
                 if revision != SOSObjectRevision.UNMANAGED:
                     diffx_file.meta['revision'] = {
-                        'old': six.text_type(revision),
+                        'old': str(revision),
                     }
 
                 if rev_id not in (None, SOSObjectRevision.UNMANAGED):
                     diffx_file.meta['sos'] = {
                         'rev_id': {
                             'old': rev_id,
                         },
@@ -1096,15 +1092,15 @@
         # We start with this in order to convert any renamed directories
         # into lists of renamed files, which may themselves be converted
         # into individual adds/deletes in the next phase.
         #
         # Generally, if any directories were renamed, we'll want to include
         # each file in that directory or any subdirectories in the diff as a
         # moved file.
-        for new_dirname, old_dirname in six.iteritems(renamed_dirs):
+        for new_dirname, old_dirname in renamed_dirs.items():
             full_walk_path = os.path.normpath(
                 os.path.join(wa_root, new_dirname))
 
             for walk_root, walk_dirs, walk_files in os.walk(full_walk_path):
                 # We need to ensure all file paths use "./" syntax.
                 walk_root = self._make_sos_path(walk_root, wa_root)
 
@@ -1118,15 +1114,15 @@
         # Handle any files marked as renamed.
         #
         # This may include files from the step above.
         #
         # If we're working with a changelist, then the changelist must include
         # both the add and the delete in order to treat it as a rename.
         # Otherwise, we'll process this in the adds or deletes blocks below.
-        for new_filename, old_filename in six.iteritems(renamed_files):
+        for new_filename, old_filename in renamed_files.items():
             if changelist:
                 is_deleted = old_filename in changelist.deletes
                 is_added = new_filename in changelist.adds
 
                 if not is_deleted and not is_added:
                     # This isn't in the changelist at all. Skip it.
                     continue
@@ -1220,26 +1216,26 @@
                     'orig_content': orig_content,
                 }
 
         # Batch-fetch revision information and populate the payloads.
         # We'll fetch 25 at a time so we won't have any real risk of
         # hitting max command line lengths, even with very long path names.
         revisions_iter = self._iter_obj_revisions(
-            list(six.iterkeys(pending_revision_payloads)))
+            list(pending_revision_payloads.keys()))
 
         for info in revisions_iter:
             pending_revision_payloads[info['path']].update({
                 'rev_id': info['rev_id'],
                 'revision': info['revision'],
             })
 
         logger.debug('File information for diff: %r', files)
 
         return sorted(
-            six.itervalues(files),
+            files.values(),
             key=lambda info: os.path.split(info['new_filename'] or
                                            info['old_filename']))
 
     @contextmanager
     def _access_deleted_file(self, path):
         """Provide temporary access to a deleted file.
 
@@ -1418,15 +1414,15 @@
                      file_changes)
 
         deletes = []
         adds = []
         renamed_dirs = {}
         renamed_files = {}
 
-        for file_change in six.itervalues(file_changes):
+        for file_change in file_changes.values():
             obj_type = FILE_CHANGE_TYPE_MAP.get(file_change['type'])
             old_filename = file_change.get('old_filename')
             new_filename = file_change.get('new_filename')
 
             if old_filename:
                 old_filename = os.path.join(path, old_filename)
 
@@ -1487,15 +1483,15 @@
             unicode:
             The original name/path of a file, if found.
         """
         if path in renamed_files:
             return renamed_files[path]
 
         if renamed_dirs:
-            for new_dir_name, old_dir_name in six.iteritems(renamed_dirs):
+            for new_dir_name, old_dir_name in renamed_dirs.items():
                 if path.startswith(new_dir_name):
                     return os.path.join(old_dir_name,
                                         path[len(new_dir_name):])
 
         return path
 
     def _iter_nobjstatus(self, attributes, selection=None):
```

### Comparing `RBTools-4.0/rbtools/clients/svn.py` & `RBTools-4.1/rbtools/clients/svn.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import logging
 import os
 import posixpath
 import re
 import sys
 from xml.etree import ElementTree
 from typing import Dict, Iterator, List, Optional, Tuple, Union, cast
-
-from six.moves.urllib.parse import unquote
+from urllib.parse import unquote
 
 from rbtools.api.errors import APIError
 from rbtools.api.resource import (ItemResource,
                                   ListResource,
                                   RootResource)
 from rbtools.clients import PatchResult, RepositoryInfo
 from rbtools.clients.base.scmclient import (BaseSCMClient,
```

### Comparing `RBTools-4.0/rbtools/clients/tests/__init__.py` & `RBTools-4.1/rbtools/clients/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/tests/test_base_scmclient.py` & `RBTools-4.1/rbtools/clients/tests/test_base_scmclient.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/tests/test_bzr.py` & `RBTools-4.1/rbtools/clients/tests/test_bzr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for BazaarClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 from typing import List
 
 import kgb
 
 from rbtools.clients import RepositoryInfo
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_clearcase.py` & `RBTools-4.1/rbtools/clients/tests/test_clearcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for ClearCaseClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 
 import kgb
 
 from rbtools.clients.clearcase import ClearCaseClient, ClearCaseRepositoryInfo
 from rbtools.clients.errors import SCMClientDependencyError, SCMError
@@ -1539,16 +1537,25 @@
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test2.py-fake-old-oid',
                     b'',
                 )),
             },
             {
+                'args': (['cleartool', 'describe', '-fmt', '%On',
+                          'vob:test2.py'],),
+                'op': kgb.SpyOpReturn((
+                    0,
+                    b'test2.py-fake-vob-oid',
+                    b'',
+                )),
+            },
+            {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test2.py-fake-old-oid'],),
+                          'oid:test2.py-fake-old-oid@vobuuid:test2.py-fake-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test2.py-fake-version-old',
                     b'',
                 )),
             },
             {
@@ -1558,15 +1565,15 @@
                     0,
                     b'test2.py-fake-oid',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test2.py-fake-oid'],),
+                          'oid:test2.py-fake-oid@vobuuid:test2.py-fake-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test2.py-fake-version',
                     b'',
                 )),
             },
             {
@@ -1614,16 +1621,25 @@
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test.pdf-fake-old-oid',
                     b'',
                 )),
             },
             {
+                'args': (['cleartool', 'describe', '-fmt', '%On',
+                          'vob:test.pdf'],),
+                'op': kgb.SpyOpReturn((
+                    0,
+                    b'test.pdf-vob-oid',
+                    b'',
+                )),
+            },
+            {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test.pdf-fake-old-oid'],),
+                          'oid:test.pdf-fake-old-oid@vobuuid:test.pdf-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test.pdf-fake-version-old',
                     b'',
                 )),
             },
             {
@@ -1633,15 +1649,15 @@
                     0,
                     b'test.pdf-fake-oid',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test.pdf-fake-oid'],),
+                          'oid:test.pdf-fake-oid@vobuuid:test.pdf-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test.pdf-fake-version',
                     b'',
                 )),
             },
             {
@@ -2061,24 +2077,24 @@
                     0,
                     b'test-dir-old-oid',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test-dir-old-oid'],),
+                          'oid:test-dir-old-oid@vobuuid:test-dir-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test-dir-old-version',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:test-dir-new-oid'],),
+                          'oid:test-dir-new-oid@vobuuid:test-dir-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'test-dir-new-version',
                     b'',
                 )),
             },
             {
@@ -2136,15 +2152,15 @@
                     0,
                     b'empty-dir-vob-oid',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:empty-dir-new-oid'],),
+                          'oid:empty-dir-new-oid@vobuuid:empty-dir-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'empty-dir-new-version',
                     b'',
                 )),
             },
             {
@@ -2163,15 +2179,15 @@
                     0,
                     b'empty-dir-old-oid',
                     b'',
                 )),
             },
             {
                 'args': (['cleartool', 'describe', '-fmt', '%Vn',
-                          'oid:empty-dir-old-oid'],),
+                          'oid:empty-dir-old-oid@vobuuid:empty-dir-vob-oid'],),
                 'op': kgb.SpyOpReturn((
                     0,
                     b'empty-dir-old-version',
                     b'',
                 )),
             },
             {
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_cvs.py` & `RBTools-4.1/rbtools/clients/tests/test_cvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for CVSClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 from typing import Optional
 
 import kgb
 
 from rbtools.clients import RepositoryInfo
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_git.py` & `RBTools-4.1/rbtools/clients/tests/test_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for GitClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 import unittest
 from typing import List, Optional
 
 import kgb
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_mercurial.py` & `RBTools-4.1/rbtools/clients/tests/test_mercurial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for MercurialClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 import shutil
 import tempfile
 import time
 import unittest
 from random import randint
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_p4.py` & `RBTools-4.1/rbtools/clients/tests/test_p4.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for PerforceClient."""
 
-from __future__ import unicode_literals
-
 import os
 import re
 import time
 from typing import Type
 
 import kgb
 
@@ -16,14 +14,35 @@
 from rbtools.clients.tests import SCMClientTestCase
 from rbtools.deprecation import RemovedInRBTools50Warning
 from rbtools.testing import TestCase
 from rbtools.utils.checks import check_install
 from rbtools.utils.filesystem import make_tempfile
 
 
+SAMPLE_CHANGEDESC_TEMPLATE_BASIC = (
+    'Change:\t123\n'
+    '\n'
+    'Date:\t2023/05/06 01:02:03\n'
+    '\n'
+    'Client:\tTestClient\n'
+    '\n'
+    'User:\ttest-user\n'
+    '\n'
+    'Status:\tpending\n'
+    '\n'
+    'Type:\tpublic\n'
+    '\n'
+    '%s'
+    '\n'
+    'Files:\n'
+    '\t//depot/main/test1\t# edit\n'
+    '\t//depot/main/test2\t# edit\n'
+)
+
+
 class P4WrapperTests(TestCase):
     """Unit tests for P4Wrapper."""
 
     def is_supported(self):
         return True
 
     def test_counters(self):
@@ -908,7 +927,171 @@
             # directory.
             os.path.join(cwd, patterns[2]),
         ]
 
         result = client.normalize_exclude_patterns(patterns)
 
         self.assertEqual(result, normalized_patterns)
+
+    def test_replace_changeset_description(self) -> None:
+        """Testing PerforceClient._replace_changeset_description"""
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\tWith multiple...\n'
+            '\t...lines.\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            'Here is the original description.\n'
+            '\n'
+            'With multiple...\n'
+            '...lines.\n'
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\tWith multiple...\n'
+            '\t...lines.\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
+
+    def test_replace_changeset_description_with_summary(self) -> None:
+        """Testing PerforceClient._replace_changeset_description with existing
+        summary only
+        """
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            'Here is the original description.\n'
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
+
+    def test_replace_changeset_description_with_single(self) -> None:
+        """Testing PerforceClient._replace_changeset_description with single
+        line
+        """
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\tHere is the original description.\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            'Here is the original description.\n'
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
+
+    def test_replace_changeset_description_with_spaces(self) -> None:
+        """Testing PerforceClient._replace_changeset_description with spaces
+        """
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '    Here is the original description.\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            'Here is the original description.\n'
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
+
+    def test_replace_changeset_description_with_indents(self) -> None:
+        """Testing PerforceClient._replace_changeset_description with indents
+        within body
+        """
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\n'
+            '\t    And we indent here.\n'
+            '\n'
+            '\tAnd back to normal.\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            'Here is the original description.\n'
+            '\n'
+            '    And we indent here.\n'
+            '\n'
+            'And back to normal.\n'
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\tHere is the original description.\n'
+            '\t\n'
+            '\t    And we indent here.\n'
+            '\t\n'
+            '\tAnd back to normal.\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
+
+    def test_replace_changeset_description_with_empty(self) -> None:
+        """Testing PerforceClient._replace_changeset_description with empty
+        description
+        """
+        client = self.build_client()
+
+        old_changedesc = SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+        )
+
+        new_changedesc = client._replace_changeset_description(
+            old_changedesc,
+            '\n'
+            'Reviewed at https://reviews.example.com/r/123/\n'
+        )
+
+        self.assertEqual(new_changedesc, SAMPLE_CHANGEDESC_TEMPLATE_BASIC % (
+            'Description:\n'
+            '\t\n'
+            '\tReviewed at https://reviews.example.com/r/123/\n'
+        ))
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_plastic.py` & `RBTools-4.1/rbtools/clients/tests/test_plastic.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/tests/test_scanning.py` & `RBTools-4.1/rbtools/clients/tests/test_scanning.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for client scanning."""
 
-from __future__ import unicode_literals
-
 import os
 
 from rbtools.clients import scan_usable_client
 from rbtools.clients.git import GitClient
 from rbtools.clients.svn import SVNClient
 from rbtools.clients.tests import SCMClientTestCase
 from rbtools.utils.process import execute
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_scmclient_registry.py` & `RBTools-4.1/rbtools/clients/tests/test_scmclient_registry.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/tests/test_sos.py` & `RBTools-4.1/rbtools/clients/tests/test_sos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Unit tests for rbtools.clients.sos.
 
 Version Added:
     3.1
 """
 
-from __future__ import unicode_literals
-
 import os
 import re
 from typing import Any, Dict, List
 
 import kgb
 
 from rbtools.api.resource import ReviewRequestResource
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_svn.py` & `RBTools-4.1/rbtools/clients/tests/test_svn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+# coding: utf-8
 """Unit tests for SubversionClient."""
 
 import json
 import os
 import re
 import sys
 import unittest
 from typing import List
+from urllib.request import urlopen
 
 import kgb
-from six.moves.urllib.request import urlopen
 
 from rbtools.api.client import RBClient
 from rbtools.api.tests.base import MockResponse
 from rbtools.clients.base.scmclient import SCMClientDiffResult
 from rbtools.clients.errors import (InvalidRevisionSpecError,
                                     SCMClientDependencyError,
                                     TooManyRevisionsError)
```

### Comparing `RBTools-4.0/rbtools/clients/tests/test_tfs.py` & `RBTools-4.1/rbtools/clients/tests/test_tfs.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/clients/tfs.py` & `RBTools-4.1/rbtools/clients/tfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import logging
 import os
 import re
 import sys
 import tempfile
 import xml.etree.ElementTree as ET
 from typing import Any, Dict, List, Optional, cast
-
-from six.moves.urllib.parse import unquote
+from urllib.parse import unquote
 
 from rbtools.clients import BaseSCMClient, RepositoryInfo
 from rbtools.clients.base.scmclient import (SCMClientDiffResult,
                                             SCMClientRevisionSpec)
 from rbtools.clients.errors import (InvalidRevisionSpecError,
                                     SCMClientDependencyError,
                                     SCMError,
```

### Comparing `RBTools-4.0/rbtools/commands/__init__.py` & `RBTools-4.1/rbtools/commands/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from __future__ import unicode_literals
+"""Base support for creating commands."""
 
 import argparse
 import inspect
 import io
 import json
 import logging
 import platform
 import os
 import subprocess
 import sys
+from urllib.parse import urlparse
 
 import colorama
 import pkg_resources
-import six
-from six.moves.urllib.parse import urlparse
 
 from rbtools import get_version_string
 from rbtools.api.capabilities import Capabilities
 from rbtools.api.client import RBClient
 from rbtools.api.errors import APIError, ServerInterfaceError
 from rbtools.api.resource import RootResource
 from rbtools.api.transport.sync import SyncTransport
@@ -182,24 +181,23 @@
 
             end (unicode, optional):
                 String to append to end of msg. This defaults to ``\\n```.
         """
         if self.output_stream:
             if end:
                 if (isinstance(msg, bytes) and
-                    isinstance(end, six.string_types)):
+                    isinstance(end, str)):
                     msg += end.encode('utf-8')
                 else:
                     msg += end
 
             self.output_stream.write(msg)
 
     def new_line(self):
-        """Pass a new line character to output stream object.
-        """
+        """Pass a new line character to output stream object."""
         if self.output_stream:
             self.output_stream.write('\n')
 
 
 class Option(object):
     """Represents an option for a command.
 
@@ -1107,19 +1105,20 @@
             maxargs = None
 
         if len(args) < minargs or (maxargs is not None and
                                    len(args) > maxargs):
             parser.error('Invalid number of arguments provided')
             sys.exit(1)
 
-        self._init_logging()
-        self.initialize()
-        logging.debug('Command line: %s', subprocess.list2cmdline(argv))
-
         try:
+            self._init_logging()
+            logging.debug('Command line: %s', subprocess.list2cmdline(argv))
+
+            self.initialize()
+
             exit_code = self.main(*args) or 0
         except CommandError as e:
             if isinstance(e, ParseError):
                 parser.error(e)
             elif self.options.debug:
                 raise
```

### Comparing `RBTools-4.0/rbtools/commands/alias.py` & `RBTools-4.1/rbtools/commands/alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import unicode_literals
+"""Implementation of rbt alias."""
 
 from collections import defaultdict
 from subprocess import list2cmdline
 
-import six
-
 from rbtools.commands import command_exists, Command, CommandError, Option
 from rbtools.utils.aliases import expand_alias
 from rbtools.utils.filesystem import get_config_paths, parse_config_file
 
 
 class Alias(Command):
     """A command for managing aliases defined in .reviewboardrc files."""
@@ -46,15 +44,15 @@
 
         config_paths = get_config_paths()
 
         for config_path in config_paths:
             config = parse_config_file(config_path)
 
             if 'ALIASES' in config:
-                for alias_name, alias_cmd in six.iteritems(config['ALIASES']):
+                for alias_name, alias_cmd in config['ALIASES'].items():
                     predefined = alias_name in predefined_aliases
 
                     aliases[config_path][alias_name] = {
                         'command': alias_cmd,
                         'overridden': predefined,
                         'invalid': command_exists(alias_name),
                     }
@@ -62,15 +60,15 @@
                     if not predefined:
                         predefined_aliases[alias_name] = config_path
 
         for config_path in config_paths:
             if aliases[config_path]:
                 self.stdout.write('[%s]' % config_path)
 
-                for alias_name, entry in six.iteritems(aliases[config_path]):
+                for alias_name, entry in aliases[config_path].items():
                     self.stdout.write('    %s = %s'
                                       % (alias_name, entry['command']))
 
                     if entry['invalid']:
                         self.stdout.write('      !! This alias is overridden '
                                           'by an rbt command !!')
                     elif entry['overridden']:
```

### Comparing `RBTools-4.0/rbtools/commands/api_get.py` & `RBTools-4.1/rbtools/commands/api_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt api-get."""
 
 import json
 import re
 
 from rbtools.api.errors import APIError
 from rbtools.commands import (Command,
                               CommandError,
```

### Comparing `RBTools-4.0/rbtools/commands/attach.py` & `RBTools-4.1/rbtools/commands/attach.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from __future__ import unicode_literals
+"""Implementation of rbt attach."""
 
 import os
-
-from six.moves.urllib.parse import urljoin
+from urllib.parse import urljoin
 
 from rbtools.api.errors import APIError
 from rbtools.commands import Command, CommandError, Option
 
 
 class Attach(Command):
     """Attach a file to a review request."""
```

### Comparing `RBTools-4.0/rbtools/commands/clearcache.py` & `RBTools-4.1/rbtools/commands/clearcache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt clear-cache."""
 
 from rbtools.api.cache import APICache, clear_cache
 from rbtools.commands import Command, Option
 
 
 class ClearCache(Command):
     """Delete the HTTP cache used for the API."""
```

### Comparing `RBTools-4.0/rbtools/commands/close.py` & `RBTools-4.1/rbtools/commands/close.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt close."""
 
 from rbtools.api.errors import APIError
 from rbtools.commands import Command, CommandError, Option
 
 
 SUBMITTED = 'submitted'
 DISCARDED = 'discarded'
```

### Comparing `RBTools-4.0/rbtools/commands/conf/rbt-bash-completion` & `RBTools-4.1/rbtools/commands/conf/rbt-bash-completion`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/commands/diff.py` & `RBTools-4.1/rbtools/commands/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import unicode_literals
+"""Implementation of rbt diff."""
 
 from rbtools.clients.errors import InvalidRevisionSpecError
 from rbtools.commands import Command, CommandError
 
-import six
-
 
 class Diff(Command):
     """Prints a diff to the terminal."""
 
     name = 'diff'
     author = 'The Review Board Project'
 
@@ -90,13 +88,10 @@
             repository_info=self.repository_info,
             extra_args=extra_args,
             **diff_kwargs)
 
         diff = diff_info['diff']
 
         if diff:
-            if six.PY2:
-                self.stdout.write(diff)
-            else:
-                # Write the non-decoded binary diff to standard out
-                self.stdout_bytes.write(diff)
-                self.stdout.new_line()
+            # Write the non-decoded binary diff to standard out.
+            self.stdout_bytes.write(diff)
+            self.stdout.new_line()
```

### Comparing `RBTools-4.0/rbtools/commands/info.py` & `RBTools-4.1/rbtools/commands/info.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/commands/install.py` & `RBTools-4.1/rbtools/commands/install.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import division, unicode_literals
+"""Implementation of rbt install."""
 
 import hashlib
 import logging
 import os
 import shutil
 import tempfile
 import zipfile
+from urllib.error import HTTPError, URLError
+from urllib.request import urlopen
 
 import tqdm
-from six.moves.urllib.error import HTTPError, URLError
-from six.moves.urllib.request import urlopen
 
 from rbtools.commands import Command, CommandError
 from rbtools.utils.appdirs import user_data_dir
 from rbtools.utils.checks import check_install
 from rbtools.utils.process import execute
```

### Comparing `RBTools-4.0/rbtools/commands/land.py` & `RBTools-4.1/rbtools/commands/land.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import unicode_literals
+"""Implementation of rbt land."""
 
 import logging
 
-import six
-
 from rbtools.api.errors import APIError
 from rbtools.clients.errors import MergeError, PushError
 from rbtools.commands import Command, CommandError, Option, RB_MAIN
 from rbtools.utils.commands import (build_rbtools_cmd_argv,
                                     extract_commit_message)
 from rbtools.utils.console import confirm
 from rbtools.utils.errors import MatchReviewRequestsError
@@ -146,15 +144,15 @@
             patch_command.append('-c')
         else:
             patch_command.append('-C')
 
         if squash:
             patch_command.append('--squash')
 
-        patch_command.append(six.text_type(review_request_id))
+        patch_command.append(str(review_request_id))
 
         rc, output = execute(patch_command, ignore_errors=True,
                              return_error_code=True)
 
         if rc:
             raise CommandError('Failed to execute "rbt patch":\n%s'
                                % output)
@@ -253,15 +251,15 @@
                                     destination=destination_branch,
                                     message=review_commit_message,
                                     author=author,
                                     squash=squash,
                                     run_editor=edit,
                                     close_branch=delete_branch)
                 except MergeError as e:
-                    raise CommandError(six.text_type(e))
+                    raise CommandError(str(e))
         else:
             self.stdout.write('Applying patch from review request %s.'
                               % review_request.id)
 
             json_data['type'] = 'patch'
 
             if not dry_run:
@@ -341,15 +339,15 @@
                     api_client=self.api_client,
                     tool=self.tool,
                     revisions=revisions,
                     commit_id=revisions.get('commit_id'),
                     is_fuzzy_match_func=self._ask_review_request_match,
                     repository_id=self.repository.id)
             except MatchReviewRequestsError as e:
-                raise CommandError(six.text_type(e))
+                raise CommandError(str(e))
 
             if not review_request or not review_request.id:
                 raise CommandError('Could not determine the existing review '
                                    'request URL to land.')
 
             review_request_id = review_request.id
             is_local = True
@@ -442,14 +440,14 @@
             self.stdout.write('Pushing branch "%s" upstream'
                               % self.options.destination_branch)
 
             if not self.options.dry_run:
                 try:
                     self.tool.push_upstream(self.options.destination_branch)
                 except PushError as e:
-                    raise CommandError(six.text_type(e))
+                    raise CommandError(str(e))
 
     def _ask_review_request_match(self, review_request):
         return confirm(
             'Land Review Request #%s: "%s"? '
             % (review_request.id,
                get_draft_or_current_value('summary', review_request)))
```

### Comparing `RBTools-4.0/rbtools/commands/list_repo_types.py` & `RBTools-4.1/rbtools/commands/list_repo_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import unicode_literals
+"""Implementation of rbt list-repo-types."""
 
 import textwrap
 
-import six
-
 from rbtools.clients import load_scmclients
 from rbtools.commands import Command
 
 
 class ListRepoTypes(Command):
     """List available repository types."""
 
@@ -32,15 +30,15 @@
         self.stdout.new_line()
 
         load_scmclients(self.config, self.options)
         from rbtools.clients import SCMCLIENTS
 
         self.json.add('repository_types', [])
 
-        for name, tool in six.iteritems(SCMCLIENTS):
+        for name, tool in SCMCLIENTS.items():
             has_repository_info = tool.get_repository_info() is not None
 
             self.json.append('repository_types', {
                 'name': name,
                 'tool': tool.name,
                 'detected': has_repository_info
             })
```

### Comparing `RBTools-4.0/rbtools/commands/login.py` & `RBTools-4.1/rbtools/commands/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt login."""
 
 import logging
 
 from rbtools.api.errors import AuthorizationError
 from rbtools.commands import Command, CommandError
 from rbtools.utils.users import get_authenticated_session
```

### Comparing `RBTools-4.0/rbtools/commands/logout.py` & `RBTools-4.1/rbtools/commands/logout.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt logout."""
 
 import logging
 
 from rbtools.commands import Command
 
 
 class Logout(Command):
```

### Comparing `RBTools-4.0/rbtools/commands/main.py` & `RBTools-4.1/rbtools/commands/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import print_function, unicode_literals
+"""Main handler for the rbt command."""
 
 import argparse
 import glob
 import os
 import pkg_resources
 import signal
 import subprocess
```

### Comparing `RBTools-4.0/rbtools/commands/patch.py` & `RBTools-4.1/rbtools/commands/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-"""The rbt patch command."""
-
-from __future__ import unicode_literals
+"""Implementation of rbt patch."""
 
 import logging
 import os
 import re
 from gettext import gettext as _, ngettext
 
-import six
 from rbtools.api.errors import APIError
 from rbtools.clients import PatchAuthor
 from rbtools.clients.errors import CreateCommitError
 from rbtools.commands import Command, CommandError, Option
 from rbtools.utils.commands import extract_commit_message
 from rbtools.utils.filesystem import make_tempfile
 from rbtools.utils.review_request import parse_review_request_url
@@ -352,21 +349,16 @@
             p=self.options.px,
             revert=revert)
 
         if result.patch_output:
             self.stdout.new_line()
 
             patch_output = result.patch_output.strip()
-
-            if six.PY2:
-                self.stdout.write(patch_output)
-            else:
-                self.stdout_bytes.write(patch_output)
-                self.stdout.new_line()
-
+            self.stdout_bytes.write(patch_output)
+            self.stdout.new_line()
             self.stdout.new_line()
 
         if not result.applied:
             if revert:
                 raise CommandError(
                     'Unable to revert the patch. The patch may be invalid, or '
                     'there may be conflicts that could not be resolved.')
@@ -691,11 +683,11 @@
 
                 try:
                     self.tool.create_commit(
                         message=message,
                         author=author,
                         run_editor=not commit_no_edit)
                 except CreateCommitError as e:
-                    raise CommandError(six.text_type(e))
+                    raise CommandError(str(e))
                 except NotImplementedError:
                     raise CommandError('--commit is not supported with %s'
                                        % self.tool.name)
```

### Comparing `RBTools-4.0/rbtools/commands/post.py` & `RBTools-4.1/rbtools/commands/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from __future__ import unicode_literals
+"""Implementation of rbt post."""
 
 import logging
 import os
 import platform
 import re
 import sys
 from collections import namedtuple
 
-import six
-from six.moves import zip
 from tqdm import tqdm
 
 from rbtools.api.errors import APIError
 from rbtools.commands import Command, CommandError, Option, OptionGroup
 from rbtools.utils.commands import (AlreadyStampedError,
                                     stamp_commit_with_review_url)
 from rbtools.utils.console import confirm
@@ -1074,15 +1072,15 @@
                     revisions=self.revisions,
                     commit_id=self.revisions.get('commit_id'),
                     is_fuzzy_match_func=self._ask_review_request_match,
                     submit_as=self.options.submit_as,
                     additional_fields=additional_fields,
                     repository_id=self.repository.id)
             except MatchReviewRequestsError as e:
-                raise CommandError(six.text_type(e))
+                raise CommandError(str(e))
 
             if not review_request or not review_request.id:
                 raise CommandError('Could not determine existing review '
                                    'request to update.')
 
             # We found a match, but the review request object we got back only
             # has partial information. We now need to re-fetch the review
@@ -1346,15 +1344,15 @@
             # on older releases, so we'll continue to do so).
             #
             # It's better than shoe-horning in complex types and then
             # having to deal with that later.
             if extra_data_patch:
                 request_data.update({
                     'extra_data__%s' % _key: _value
-                    for _key, _value in six.iteritems(extra_data_patch)
+                    for _key, _value in extra_data_patch.items()
                 })
 
     def _get_diff_history(self, extra_args):
         """Compute and return the diff history of the selected revisions.
 
         Args:
             extra_args (list):
```

### Comparing `RBTools-4.0/rbtools/commands/publish.py` & `RBTools-4.1/rbtools/commands/publish.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt publish."""
 
 import logging
 
 from rbtools.api.errors import APIError
 from rbtools.commands import Command, CommandError, Option
```

### Comparing `RBTools-4.0/rbtools/commands/review.py` & `RBTools-4.1/rbtools/commands/review.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""RBTools command to create and publish reviews.
+"""Implementation of rbt review.
 
-Version Added: 3.0
+Version Added:
+    3.0
 """
 
-from __future__ import unicode_literals
-
 import logging
 
 from rbtools.api.errors import APIError
 from rbtools.commands import (BaseSubCommand,
                               BaseMultiCommand,
                               Command,
                               CommandError,
```

### Comparing `RBTools-4.0/rbtools/commands/setup_completion.py` & `RBTools-4.1/rbtools/commands/setup_completion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt setup-completion."""
 
 import logging
 import os
 import platform
 import sys
 
 from pkg_resources import resource_string
```

### Comparing `RBTools-4.0/rbtools/commands/setup_repo.py` & `RBTools-4.1/rbtools/commands/setup_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from __future__ import unicode_literals
+"""Implementation of rbt setup-repo."""
 
 import difflib
 import os
 import textwrap
 
-import six
-from six.moves import input
-
 from rbtools.commands import Command, CommandError
 from rbtools.utils.console import confirm, confirm_select
 from rbtools.utils.filesystem import CONFIG_FILE
 from rbtools.utils.repository import get_repository_resource
 
 
 class SetupRepo(Command):
@@ -75,16 +72,17 @@
         for repository in repositories.all_items:
             repo_paths[repository['path']] = repository
 
             if 'mirror_path' in repository:
                 repo_paths[repository['mirror_path']] = repository
 
         closest_paths = difflib.get_close_matches(repository_paths,
-                                                  six.iterkeys(repo_paths),
-                                                  n=4, cutoff=0.4)
+                                                  repo_paths.keys(),
+                                                  n=4,
+                                                  cutoff=0.4)
 
         if closest_paths:
             self.stdout.new_line()
             self.stdout.write(
                 '%(num)s matching %(repo_type)s repositories found:'
                 % {
                     'num': len(closest_paths),
```

### Comparing `RBTools-4.0/rbtools/commands/stamp.py` & `RBTools-4.1/rbtools/commands/stamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import unicode_literals
+"""Implementation of rbt stamp."""
 
 import logging
 
-import six
-
 from rbtools.api.errors import APIError
 from rbtools.commands import Command, CommandError, Option, OptionGroup
 from rbtools.utils.commands import stamp_commit_with_review_url
 from rbtools.utils.console import confirm
 from rbtools.utils.errors import MatchReviewRequestsError
 from rbtools.utils.review_request import (find_review_request_by_change_id,
                                           get_draft_or_current_value,
@@ -111,15 +109,15 @@
                 tool=self.tool,
                 revisions=revisions,
                 commit_id=revisions.get('commit_id'),
                 is_fuzzy_match_func=self._ask_review_request_match,
                 no_commit_error=self.no_commit_error,
                 repository_id=self.repository.id)
         except MatchReviewRequestsError as e:
-            raise CommandError(six.text_type(e))
+            raise CommandError(str(e))
 
         if review_request:
             logging.debug('Found review request ID %d', review_request.id)
             return review_request.id, review_request.absolute_url
         else:
             logging.debug('Could not find a matching review request')
             return None, None
```

### Comparing `RBTools-4.0/rbtools/commands/status.py` & `RBTools-4.1/rbtools/commands/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Implementation of rbt status."""
 
 import logging
 import re
 from shutil import get_terminal_size
 
 import texttable as tt
```

### Comparing `RBTools-4.0/rbtools/commands/status_update.py` & `RBTools-4.1/rbtools/commands/status_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-"""Interact with review request status-updates on Review Board.
-
-For getting or setting status-updates on review requests. Also for including a
-review when creating a status-update.
-"""
-
-from __future__ import print_function, unicode_literals
+"""Implementation of rbt status-update."""
 
 import json
 import logging
 
 from rbtools.api.errors import APIError
 from rbtools.commands import (BaseMultiCommand,
                               BaseSubCommand,
```

### Comparing `RBTools-4.0/rbtools/commands/tests/test_alias.py` & `RBTools-4.1/rbtools/commands/tests/test_alias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Tests for RBTools alias command."""
 
-from __future__ import unicode_literals
-
 from rbtools.commands.alias import Alias
 from rbtools.testing import CommandTestsMixin, TestCase
 
 
 class AliasCommandTests(CommandTestsMixin, TestCase):
     """Tests for rbt alias commmand."""
```

### Comparing `RBTools-4.0/rbtools/commands/tests/test_main.py` & `RBTools-4.1/rbtools/commands/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Tests for RBTools help command and rbt command help options."""
 
-from __future__ import unicode_literals
-
 import sys
 
 import kgb
 
 from rbtools import get_version_string
 from rbtools.commands import JSONOutput, main as rbt_main
 from rbtools.testing import TestCase
```

### Comparing `RBTools-4.0/rbtools/commands/tests/test_post.py` & `RBTools-4.1/rbtools/commands/tests/test_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Test for RBTools post command."""
 
-from __future__ import unicode_literals
-
 from rbtools.clients import RepositoryInfo
 from rbtools.clients.git import GitClient
 from rbtools.commands import CommandError
 from rbtools.commands.post import DiffHistory, Post, SquashedDiff
 from rbtools.testing import CommandTestsMixin, TestCase
```

### Comparing `RBTools-4.0/rbtools/commands/tests/test_setup_repo.py` & `RBTools-4.1/rbtools/commands/tests/test_setup_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Tests for RBTools setup-repo command."""
 
-from __future__ import unicode_literals
-
 import os
 
 from kgb import SpyAgency
 
 from rbtools.api.resource import ItemResource
 from rbtools.commands.setup_repo import SetupRepo
 from rbtools.testing import CommandTestsMixin, TestCase
```

### Comparing `RBTools-4.0/rbtools/deprecation.py` & `RBTools-4.1/rbtools/deprecation.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,22 +163,26 @@
         if args_cache:
             param_names = args_cache['param_names']
             first_kwonly_arg_index = args_cache['first_kwonly_i']
         else:
             sig = inspect.signature(func)
             first_kwonly_arg_index = -1
             param_names = []
+            i = 0
 
             # This is guaranteed to be in the correct order.
-            for i, param in enumerate(sig.parameters.values()):
-                param_names.append(param.name)
+            for param in sig.parameters.values():
+                if param.kind not in (param.VAR_POSITIONAL, param.VAR_KEYWORD):
+                    param_names.append(param.name)
+
+                    if (param.kind == param.KEYWORD_ONLY and
+                        first_kwonly_arg_index == -1):
+                        first_kwonly_arg_index = i
 
-                if (param.kind == param.KEYWORD_ONLY and
-                    first_kwonly_arg_index == -1):
-                    first_kwonly_arg_index = i
+                    i += 1
 
             assert first_kwonly_arg_index != -1, (
                 '@deprecate_non_keyword_only_args cannot be used on '
                 'functions that do not contain keyword-only arguments.')
 
             args_cache.update({
                 'first_kwonly_i': first_kwonly_arg_index,
@@ -227,26 +231,31 @@
             return args, kwargs
 
         # Figure out which we need to move over to keyword-only
         # arguments.
         new_args: List = []
         new_kwargs: Dict[str, Any] = kwargs.copy()
         moved_args: List[str] = []
+        i = 0
 
-        for i, param_name in enumerate(param_names):
-            if i < first_kwonly_arg_index:
-                # This is a valid positional argument.
-                new_args.append(args[i])
-            elif i < num_args:
-                # This must be converted to a keyword argument.
-                new_kwargs[param_name] = args[i]
-                moved_args.append(param_name)
-            else:
-                # We've handled all positional arguments. We're done.
-                break
+        for param_name in param_names:
+            if param_name not in kwargs:
+                if i < first_kwonly_arg_index:
+                    new_args.append(args[i])
+                elif i < num_args:
+                    # This must be converted to a keyword argument.
+                    new_kwargs[param_name] = args[i]
+                    moved_args.append(param_name)
+                else:
+                    # We've handled all positional arguments. We're done.
+                    break
+
+                i += 1
+
+        new_args += args[i:]
 
         warning_cls.warn(
             message or (
                 'Positional argument(s) %s must be passed as keyword '
                 'arguments when calling %s(). This will be required in '
                 'RBTools %s.'
                 % (
```

### Comparing `RBTools-4.0/rbtools/diffs/tests/test_apple_diff_tool.py` & `RBTools-4.1/rbtools/diffs/tests/test_apple_diff_tool.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tests/test_diff_file_result.py` & `RBTools-4.1/rbtools/diffs/tests/test_diff_file_result.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tests/test_diff_tools_registry.py` & `RBTools-4.1/rbtools/diffs/tests/test_diff_tools_registry.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tests/test_gnu_diff_tool.py` & `RBTools-4.1/rbtools/diffs/tests/test_gnu_diff_tool.py`

 * *Files 15% similar despite different names*

```diff
@@ -44,16 +44,21 @@
     def test_get_install_instructions_on_windows(self):
         """Testing GNUDiffTool.get_install_instructions on Windows"""
         self.spy_on(platform.system,
                     op=kgb.SpyOpReturn('Windows'))
 
         self.assertEqual(
             GNUDiffTool.get_install_instructions(),
-            'On Windows, you can install GNU Diff from: '
-            'http://gnuwin32.sourceforge.net/packages/diffutils.htm')
+            "On Windows, if you're not using our RBTools for Windows "
+            "installer, you can manually download our version of diff.exe "
+            "(http://downloads.reviewboard.org/ports/gnu-diffutils/) and "
+            "place the bin/ directory in your system path. Alternatively, "
+            "install Git for Windows (https://git-scm.com/download/win) and "
+            "place it in your system path, as this version will also be "
+            "compatible.")
 
     def test_check_available_with_found(self):
         """Testing GNUDiffTool.check_available with diff found"""
         self.spy_on(
             run_process_exec,
             op=kgb.SpyOpMatchInOrder([
                 {
@@ -140,14 +145,129 @@
             ]))
 
         diff_tool = GNUDiffTool()
         available = diff_tool.check_available()
 
         self.assertFalse(available)
         self.assertIsNone(diff_tool.exe_path)
+        self.assertIsNone(diff_tool.version_info)
+
+    def test_check_available_with_not_found_on_windows(self):
+        """Testing GNUDiffTool.check_available with diff not found on
+        Windows
+        """
+        self.spy_on(platform.system,
+                    op=kgb.SpyOpReturn('Windows'))
+
+        self.spy_on(
+            run_process_exec,
+            op=kgb.SpyOpMatchInOrder([
+                {
+                    'args': ([
+                        r'C:\Program Files\RBTools\bin\diff.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        0,
+                        b'Some Other Diff v1.2.3\n',
+                        b'',
+                    )),
+                },
+                {
+                    'args': ([
+                        r'C:\Program Files\Git\bin\git.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        1,
+                        b'',
+                        b'Some error.',
+                    )),
+                },
+                {
+                    'args': ([
+                        r'C:\Program Files\Unity\Editor\Data\Tools\diff.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        1,
+                        b'',
+                        b'Some error.',
+                    )),
+                },
+                {
+                    'args': ([
+                        r'C:\Program Files\FooApp\gdiff.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        1,
+                        b'',
+                        b'Some error.',
+                    )),
+                },
+                {
+                    'args': ([
+                        r'C:\Program Files\BarApp\gdiff.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        1,
+                        b'',
+                        b'Some error.',
+                    )),
+                },
+                {
+                    'args': ([
+                        r'C:\Program Files\OtherApp\diff.exe',
+                        '--version',
+                    ],),
+                    'op': kgb.SpyOpReturn((
+                        1,
+                        b'',
+                        b'Some error.',
+                    )),
+                },
+            ]))
+
+        self.spy_on(
+            iter_exes_in_path,
+            op=kgb.SpyOpMatchInOrder([
+                {
+                    'args': ('rbt',),
+                    'op': kgb.SpyOpReturn([
+                        r'C:\Program Files\RBTools\bin\rbt.cmd',
+                    ]),
+                },
+                {
+                    'args': ('git',),
+                    'op': kgb.SpyOpReturn([
+                        r'C:\Program Files\Git\bin\git.exe',
+                    ]),
+                },
+                {
+                    'args': ('gdiff',),
+                    'op': kgb.SpyOpReturn([
+                        r'C:\Program Files\FooApp\gdiff.exe',
+                        r'C:\Program Files\BarApp\gdiff.exe',
+                    ]),
+                },
+                {
+                    'args': ('diff',),
+                    'op': kgb.SpyOpReturn([
+                        r'C:\Program Files\OtherApp\diff.exe',
+                    ]),
+                },
+            ]))
+
+        diff_tool = GNUDiffTool()
+        available = diff_tool.check_available()
+
+        self.assertFalse(available)
+        self.assertIsNone(diff_tool.exe_path)
         self.assertIsNone(diff_tool.version_info)
 
     def test_run_diff_file_with_no_differences(self):
         """Testing GNUDiffTool.run_diff_file with no differences"""
         self.spy_on(
             run_process_exec,
             op=kgb.SpyOpMatchInOrder([
```

### Comparing `RBTools-4.0/rbtools/diffs/tests/test_unified_diff_writer.py` & `RBTools-4.1/rbtools/diffs/tests/test_unified_diff_writer.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/backends/apple.py` & `RBTools-4.1/rbtools/diffs/tools/backends/apple.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/base/__init__.py` & `RBTools-4.1/rbtools/diffs/tools/base/__init__.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/base/diff_file_result.py` & `RBTools-4.1/rbtools/diffs/tools/base/diff_file_result.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/base/diff_tool.py` & `RBTools-4.1/rbtools/diffs/tools/base/diff_tool.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/errors.py` & `RBTools-4.1/rbtools/diffs/tools/errors.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/tools/registry.py` & `RBTools-4.1/rbtools/diffs/tools/registry.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/diffs/writers.py` & `RBTools-4.1/rbtools/diffs/writers.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/helpers/hgext.py` & `RBTools-4.1/rbtools/helpers/hgext.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from __future__ import unicode_literals
-
-
 # This file provides a Mercurial extension that resets certain
 # config options to provide consistent output.
 
 # We use reposetup because the config is re-read for each repo, after
 # uisetup() is called.
 ALLOWED_PARAMS = ['git', 'svn']
```

### Comparing `RBTools-4.0/rbtools/hooks/common.py` & `RBTools-4.1/rbtools/hooks/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import print_function, unicode_literals
+"""Common functionality for working with repository hooks."""
 
 import logging
 import subprocess
 
 from rbtools.api.client import RBClient
 from rbtools.api.errors import APIError, ServerInterfaceError
 
@@ -57,27 +57,46 @@
     if process.returncode:
         logging.warning('Failed to execute command: %s', command)
         return None
 
     return output
 
 
-def initialize_logging():
+def initialize_logging(
+    debug: bool = False,
+) -> None:
     """Sets up a log handler to format log messages.
 
     Warning, error, and critical messages will show the level name as a prefix,
-    followed by the message.
+    followed by the message. Debug logs can optionally be enabled as well.
+
+    Version Changed:
+        4.1:
+        Added the ``debug`` argument.
+
+    Args:
+        debug (bool, optional):
+            Whether to enable debug logging.
+
+            Version Added:
+                4.1
     """
     root = logging.getLogger()
 
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter('%(levelname)s: %(message)s'))
-    handler.setLevel(logging.WARNING)
     root.addHandler(handler)
 
+    if debug:
+        handler.setLevel(logging.DEBUG)
+        root.setLevel(logging.DEBUG)
+    else:
+        handler.setLevel(logging.WARNING)
+        root.setLevel(logging.WARNING)
+
 
 def get_review_request_id(regex, commit_message):
     """Returns the review request ID referenced in the commit message.
 
     We assume there is at most one review request associated with each commit.
     If a matching review request cannot be found, we return 0.
     """
```

### Comparing `RBTools-4.0/rbtools/hooks/git.py` & `RBTools-4.1/rbtools/hooks/git.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import unicode_literals
+"""Git repository hook utilities."""
 
 from collections import defaultdict
 from copy import deepcopy
 
-import six
-
 from rbtools.hooks.common import execute, get_review_request_id
 
 
 def get_branch_name(ref_name):
     """Returns the branch name corresponding to the specified ref name."""
     branch_ref_prefix = 'refs/heads/'
 
@@ -91,16 +89,15 @@
 
     # If there are new branches, check every commit in the dictionary
     # (corresponding to only old branches) to see if the new branches also
     # contain that commit.
     if new_branches:
         review_id_to_commits_map_copy = deepcopy(review_id_to_commits_map)
 
-        for review_id, commit_list in six.iteritems(
-                review_id_to_commits_map_copy):
+        for review_id, commit_list in review_id_to_commits_map_copy.items():
             for commit in commit_list:
                 commit_branch = commit[:commit.find('(') - 1]
 
                 if commit_branch in new_branches:
                     continue
 
                 commit_hash = commit[commit.find('(') + 1:-1]
```

### Comparing `RBTools-4.0/rbtools/testing/api/payloads.py` & `RBTools-4.1/rbtools/testing/api/payloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """API payload generation factory for unit tests.
 
 Version Added:
     3.1
 """
 
-from __future__ import unicode_literals
-
 from copy import deepcopy
 
 
 class LinkExpansionType(object):
     """A type of link expansion.
 
     This helps to indicate if a link should expand as an item or a list.
```

### Comparing `RBTools-4.0/rbtools/testing/api/transport.py` & `RBTools-4.1/rbtools/testing/api/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """API transports for unit tests.
 
 Version Added:
     3.1
 """
 
-from __future__ import unicode_literals
-
 import json
 import logging
 from collections import defaultdict
-
-from six.moves.urllib.parse import parse_qs, urljoin, urlparse
+from urllib.parse import parse_qs, urljoin, urlparse
 
 from rbtools.api.errors import create_api_error
 from rbtools.api.factory import create_resource
 from rbtools.api.request import HttpRequest
 from rbtools.api.transport import Transport
 from rbtools.testing.api.payloads import (LinkExpansionType,
                                           ResourcePayloadFactory)
```

### Comparing `RBTools-4.0/rbtools/testing/commands.py` & `RBTools-4.1/rbtools/testing/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Command unit testing support.
 
 Version Added:
     3.1
 """
 
-from __future__ import unicode_literals
-
 import io
 
 import kgb
 
 from rbtools.clients import scan_usable_client
 from rbtools.testing.api.transport import URLMapTransport
 from rbtools.utils.filesystem import cleanup_tempfiles
```

### Comparing `RBTools-4.0/rbtools/testing/testcase.py` & `RBTools-4.1/rbtools/testing/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import sys
 import tempfile
 import unittest
 from contextlib import contextmanager
 from typing import List
 
 import kgb
-import six
 
 from rbtools.api.client import RBClient
 from rbtools.testing.api.transport import URLMapTransport
 from rbtools.utils.filesystem import (cleanup_tempfiles,
                                       make_tempdir,
                                       make_tempfile)
 
@@ -370,15 +369,15 @@
         """
         if use_temp_dir:
             temp_dir = tempfile.mkdtemp()
             cwd = os.getcwd()
             os.chdir(temp_dir)
 
         with open('.reviewboardrc', 'w') as fp:
-            for key, value in six.iteritems(config):
+            for key, value in config.items():
                 fp.write('%s = %r\n' % (key, value))
 
         try:
             yield
         finally:
             if use_temp_dir:
                 os.chdir(cwd)
```

### Comparing `RBTools-4.0/rbtools/testing/transport.py` & `RBTools-4.1/rbtools/testing/transport.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 Deprecated::
     3.1:
     Replaced with
     :py:class:`rbtools.testing.api.transport.URLMapTransport.`
 """
 
-from __future__ import unicode_literals
-
 from rbtools.api.factory import create_resource
 from rbtools.api.request import HttpRequest
 from rbtools.api.tests.base import TestWithPayloads
 from rbtools.api.transport import Transport
 
 
 class TestTransport(Transport):
```

### Comparing `RBTools-4.0/rbtools/tests.py` & `RBTools-4.1/rbtools/tests.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/aliases.py` & `RBTools-4.1/rbtools/utils/aliases.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from __future__ import unicode_literals
+"""Utilities for working with command aliases."""
 
 import logging
 import re
 import shlex
 import sys
 import subprocess
 
-import six
-
 from rbtools.commands import RB_MAIN
 
 
 # Regular expression for matching argument replacement
 _arg_re = re.compile(r'\$(\d+)')
 
 # Prior to Python 2.7.3, the shlex module could not accept unicode input.
@@ -57,15 +55,15 @@
             return args[index]
         except IndexError:
             return ''
 
     did_replacement = False
 
     shlex_convert_text_type = (not _SHLEX_SUPPORTS_UNICODE and
-                               isinstance(cmd, six.text_type))
+                               isinstance(cmd, str))
 
     if shlex_convert_text_type:
         # This version of Python does not have a shlex module that supports
         # unicode arguments. We will encode it to a bytestring and then decode
         # it as we are processing the results.
         cmd = cmd.encode('utf-8')
```

### Comparing `RBTools-4.0/rbtools/utils/appdirs.py` & `RBTools-4.1/rbtools/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/checks.py` & `RBTools-4.1/rbtools/utils/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Utilities for checking for dependencies."""
 
 import os
 import subprocess
 
 from rbtools.deprecation import RemovedInRBTools50Warning
 from rbtools.utils.process import execute
```

### Comparing `RBTools-4.0/rbtools/utils/commands.py` & `RBTools-4.1/rbtools/utils/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from __future__ import unicode_literals
-
-import six
-
+"""Utilities for commands."""
 
 DEFAULT_OPTIONS_MAP = {
     'debug': '--debug',
     'server': '--server',
     'enable_proxy': '--disable-proxy',
     'disable_ssl_verification': '--disable-ssl-verification',
     'username': '--username',
@@ -64,15 +61,15 @@
 
     Used for building command line arguments from existing options, when
     calling another RBTools command. ``options_map`` specifies the options
     and their corresponding argument names that need to be included.
     """
     argv = []
 
-    for option_key, arg_name in six.iteritems(options_map):
+    for option_key, arg_name in options_map.items():
         option_value = getattr(options, option_key, None)
 
         if option_value is True and option_key != 'enable_proxy':
             argv.append(arg_name)
         elif option_value not in (True, False, None):
             argv.extend([arg_name, option_value])
```

### Comparing `RBTools-4.0/rbtools/utils/console.py` & `RBTools-4.1/rbtools/utils/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from __future__ import print_function, unicode_literals
+"""Utilities for working with console interactions."""
 
 import getpass
 import logging
 import os
 import subprocess
 import sys
 
-import six
-from six.moves import input
-
 from rbtools.utils.encoding import force_unicode
 from rbtools.utils.errors import EditorError
 from rbtools.utils.filesystem import make_tempfile
 
 
 logger = logging.getLogger(__name__)
 
@@ -63,15 +60,15 @@
         if hasattr(stdin, 'isatty') and stdin.isatty():
             result = input()
         else:
             result = stdin.readline().rstrip()
 
         return result
 
-    prompt = six.text_type(prompt)
+    prompt = str(prompt)
 
     if require:
         value = None
 
         while not value:
             value = _get_input()
     else:
@@ -120,15 +117,15 @@
             result = getpass.getpass(prompt)
         else:
             stderr.write(prompt)
             result = stdin.readline()
 
         return result.strip()
 
-    prompt = six.text_type(prompt)
+    prompt = str(prompt)
 
     if require:
         password = None
 
         while not password:
             password = _get_pass(prompt)
     else:
```

### Comparing `RBTools-4.0/rbtools/utils/diffs.py` & `RBTools-4.1/rbtools/utils/diffs.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/encoding.py` & `RBTools-4.1/rbtools/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/errors.py` & `RBTools-4.1/rbtools/utils/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Error classes for utility functions."""
 
-from __future__ import unicode_literals
-
 
 class EditorError(Exception):
     """An error invoking an external text editor."""
 
 
 # For backwards-compatibility, this inherits from ValueError.
 class MatchReviewRequestsError(ValueError):
```

### Comparing `RBTools-4.0/rbtools/utils/filesystem.py` & `RBTools-4.1/rbtools/utils/filesystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,43 +48,56 @@
 def iter_exes_in_path(
     name: str,
 ) -> Iterable[str]:
     """Iterate through all executables with a name in the user's search path.
 
     This expects a name without any system-specific executable extension. It
     will append the proper extension as necessary. For example, use "myapp"
-    and not "myapp.exe".
+    and not "myapp.exe" or "myapp.cmd". This will look for both variations.
+
+    Version Changed:
+        4.0.1:
+        On Windows, if not searching for a deliberate ``.exe`` or ``.cmd``
+        extension, this will now look for variations with both extensions.
 
     Version Added:
         4.0
 
     Args:
         name (str):
             The name of the executable.
 
     Yields:
         str:
         The location of an executable in the path.
     """
-    if sys.platform == 'win32' and not name.endswith('.exe'):
-        name += '.exe'
+    names: List[str] = []
+
+    if (sys.platform == 'win32' and not name.endswith(('.exe', '.cmd'))):
+        names += [
+            '%s.exe' % name,
+            '%s.cmd' % name,
+        ]
+    else:
+        names.append(name)
 
     cache = _iter_exes_in_path_cache
 
     for dirname in os.environ['PATH'].split(os.pathsep):
-        path = os.path.join(dirname, name)
+        for name in names:
+            path = os.path.join(dirname, name)
 
-        try:
-            found = cache[path]
-        except KeyError:
-            found = os.path.exists(path)
-            cache[path] = found
+            try:
+                found = cache[path]
+            except KeyError:
+                found = os.path.exists(path)
+                cache[path] = found
 
-        if found:
-            yield path
+            if found:
+                yield path
 
 
 def cleanup_tempfiles():
     for tmpfile in tempfiles:
         try:
             os.unlink(tmpfile)
         except OSError:
```

### Comparing `RBTools-4.0/rbtools/utils/graphs.py` & `RBTools-4.1/rbtools/utils/graphs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from __future__ import unicode_literals
+"""Topological graphing and sorting utilities."""
 
 from collections import defaultdict, deque
 
-import six
-
 
 def visit_depth_first(graph, start):
     """Yield vertices in the graph starting at the start vertex.
 
     The vertices are yielded in a depth first order and only those vertices
     that can be reached from the start vertex will be yielded.
     """
@@ -45,35 +43,35 @@
 
     If the graph contains cycles, ValueError is raised.
     """
     result = []
 
     indegrees = defaultdict(int)  # The in-degree of each vertex in the graph.
 
-    for head in six.iterkeys(graph):
+    for head in graph.keys():
         indegrees[head] = 0
 
-    for tails in six.itervalues(graph):
+    for tails in graph.values():
         for tail in tails:
             indegrees[tail] += 1
 
     heads = set(
         vertex
-        for vertex, indegree in six.iteritems(indegrees)
+        for vertex, indegree in indegrees.items()
         if indegree == 0
     )
 
     while len(heads):
         head = heads.pop()
         result.append(head)
 
         if head in graph:
             for tail in graph[head]:
                 indegrees[tail] -= 1
 
                 if indegrees[tail] == 0:
                     heads.add(tail)
 
-    if any(six.itervalues(indegrees)):
+    if any(indegrees.values()):
         raise ValueError('Graph contains cycles.')
 
     return result
```

### Comparing `RBTools-4.0/rbtools/utils/match_score.py` & `RBTools-4.1/rbtools/utils/match_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Utilities for applying matching scores for summaries and descriptions.
 
 Deprecated:
     3.1:
     This will be removed in RBTools 4.0.
 """
 
-from __future__ import unicode_literals
-
 from difflib import SequenceMatcher
 
 from rbtools.deprecation import RemovedInRBTools40Warning
 
 
 class Score(object):
     """Encapsulates ranking information for matching existing requests.
```

### Comparing `RBTools-4.0/rbtools/utils/process.py` & `RBTools-4.1/rbtools/utils/process.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/repository.py` & `RBTools-4.1/rbtools/utils/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Utility functions for working with repositories."""
 
-from __future__ import unicode_literals
-
 from rbtools.api.errors import APIError
 
 
 def get_repository_resource(api_root,
                             tool=None,
                             repository_name=None,
                             repository_paths=None):
```

### Comparing `RBTools-4.0/rbtools/utils/review_request.py` & `RBTools-4.1/rbtools/utils/review_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import unicode_literals
+"""Utilities for matching review requests."""
 
 import logging
 import re
 from collections import OrderedDict
 from difflib import SequenceMatcher
 from itertools import islice
```

### Comparing `RBTools-4.0/rbtools/utils/source_tree.py` & `RBTools-4.1/rbtools/utils/source_tree.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/streams.py` & `RBTools-4.1/rbtools/utils/streams.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/testbase.py` & `RBTools-4.1/rbtools/utils/testbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Legacy testing support for RBTools.
 
 Deprecated:
     3.0:
     This will be removed in RBTools 4.0.
 """
 
-from __future__ import unicode_literals
-
 from rbtools.deprecation import RemovedInRBTools40Warning
 from rbtools.testing import TestCase
 
 
 class RBTestBase(TestCase):
     """Legacy base class for RBTools unit tests.
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_aliases.py` & `RBTools-4.1/rbtools/utils/tests/test_aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for rbtools.utils.aliases."""
 
-from __future__ import unicode_literals
-
 from rbtools.testing import TestCase
 from rbtools.utils.aliases import replace_arguments
 
 
 class AliasTests(TestCase):
     """Tests for rbtools.utils.aliases."""
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_buffered_iterator.py` & `RBTools-4.1/rbtools/utils/tests/test_buffered_iterator.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/tests/test_checks.py` & `RBTools-4.1/rbtools/utils/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/tests/test_console.py` & `RBTools-4.1/rbtools/utils/tests/test_console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for rbtools.utils.console."""
 
-from __future__ import unicode_literals
-
 import io
 import os
 import subprocess
 
 import kgb
 
 from rbtools.testing import TestCase
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_filesystem.py` & `RBTools-4.1/rbtools/utils/tests/test_filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for rbtools.utils.filesystem."""
 
-from __future__ import unicode_literals
-
 import os
 import shutil
 
 from rbtools.testing import TestCase
 from rbtools.utils import filesystem
 from rbtools.utils.filesystem import (cleanup_tempfiles, make_empty_files,
                                       make_tempdir, make_tempfile)
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_process.py` & `RBTools-4.1/rbtools/utils/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/tests/test_repository.py` & `RBTools-4.1/rbtools/utils/tests/test_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Unit tests for rbtools.utils.repository."""
 
-from __future__ import unicode_literals
-
 import json
+from urllib.request import urlopen
 
 import kgb
-from six.moves.urllib.request import urlopen
 
 from rbtools.api.client import RBClient
 from rbtools.api.tests.base import MockResponse
 from rbtools.testing import TestCase
 from rbtools.utils.repository import get_repository_resource
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_review_request.py` & `RBTools-4.1/rbtools/utils/tests/test_review_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Unit tests for rbtools.utils.review_request."""
 
-from __future__ import unicode_literals
-
 import kgb
 
 from rbtools.api.errors import APIError
 from rbtools.clients import BaseSCMClient
 from rbtools.testing import TestCase
 from rbtools.utils.errors import MatchReviewRequestsError
 from rbtools.utils.review_request import (find_review_request_matches,
```

### Comparing `RBTools-4.0/rbtools/utils/tests/test_source_tree.py` & `RBTools-4.1/rbtools/utils/tests/test_source_tree.py`

 * *Files identical despite different names*

### Comparing `RBTools-4.0/rbtools/utils/users.py` & `RBTools-4.1/rbtools/utils/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from __future__ import unicode_literals
+"""Utilities for working with user sessions."""
 
 import logging
 import sys
 
-from six.moves import range
-
 from rbtools.api.errors import AuthorizationError
 from rbtools.utils.console import get_input, get_pass
 
 
 def get_authenticated_session(api_client, api_root, auth_required=False,
                               session=None, num_retries=3):
     """Return an authenticated session.
```

### Comparing `RBTools-4.0/setup.py` & `RBTools-4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,18 @@
         'console_scripts': [
             'rbt = rbtools.commands.main:main',
         ],
         'rbtools_commands': rb_commands,
     },
     install_requires=[
         'importlib-metadata~=4.12; python_version < "3.10"',
+        'certifi>=2023.5.7',
         'colorama',
         'pydiffx~=1.1.0',
         'setuptools',
-        'six>=1.8.0',
         'texttable',
         'typing_extensions>=4.3.0',
         'tqdm',
     ],
     packages=find_packages(exclude=['tests']),
     include_package_data=True,
     url='https://www.reviewboard.org/downloads/rbtools/',
```

