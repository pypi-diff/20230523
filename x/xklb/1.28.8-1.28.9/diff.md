# Comparing `tmp/xklb-1.28.8.tar.gz` & `tmp/xklb-1.28.9.tar.gz`

## Comparing `xklb-1.28.8.tar` & `xklb-1.28.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.8/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.8/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.8/Windows.md
--rw-r--r--   0        0        0   416122 2020-02-02 00:00:00.000000 xklb-1.28.8/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.8/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.8/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.8/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.8/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/__init__.py
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/books.py
--rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/consts.py
--rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/dl_extract.py
--rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/fs_extract.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/lb.py
--rw-r--r--   0        0        0    37927 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/playback.py
--rw-r--r--   0        0        0    30605 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/stats.py
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/tube_extract.py
--rw-r--r--   0        0        0    28913 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.8/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.8/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.8/LICENSE
--rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.8/README.md
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-1.28.8/pyproject.toml
--rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.8/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.28.9/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.28.9/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.28.9/Windows.md
+-rw-r--r--   0        0        0   416121 2020-02-02 00:00:00.000000 xklb-1.28.9/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.28.9/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.28.9/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.28.9/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/__init__.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/books.py
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/consts.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/data.py
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/lb.py
+-rw-r--r--   0        0        0    37322 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/playback.py
+-rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/stats.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21954 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/tube_extract.py
+-rw-r--r--   0        0        0    29149 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.28.9/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.28.9/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.28.9/LICENSE
+-rw-r--r--   0        0        0    40704 2020-02-02 00:00:00.000000 xklb-1.28.9/README.md
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-1.28.9/pyproject.toml
+-rw-r--r--   0        0        0    44218 2020-02-02 00:00:00.000000 xklb-1.28.9/PKG-INFO
```

### Comparing `xklb-1.28.8/Windows.md` & `xklb-1.28.9/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/pdm.lock` & `xklb-1.28.9/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -811,15 +811,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.267"
+version = "0.0.269"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -943,15 +943,15 @@
 summary = "extract text from any document. no muss. no fuss."
 dependencies = [
     "SpeechRecognition~=3.8.1",
     "argcomplete~=1.10.0",
     "beautifulsoup4~=4.8.0",
     "chardet==3.*",
     "docx2txt~=0.8",
-    "extract-msg<=0.29.*",
+    "extract-msg<0.29.0",
     "pdfminer-six==20191110",
     "python-pptx~=0.6.18",
     "six~=1.12.0",
     "xlrd~=1.2.0",
 ]
 
 [[package]]
@@ -2542,32 +2542,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.3.5" = [
     {url = "https://files.pythonhosted.org/packages/39/03/6de23bdd88f5ee7f8b03f94f6e88108f5d7ffe6d207e95cdb06d9aa4cd57/rich-13.3.5-py3-none-any.whl", hash = "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"},
     {url = "https://files.pythonhosted.org/packages/3d/0b/8dd34d20929c4b5e474db2e64426175469c2b7fea5ba71c6d4b3397a9729/rich-13.3.5.tar.gz", hash = "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c"},
 ]
-"ruff 0.0.267" = [
-    {url = "https://files.pythonhosted.org/packages/1e/6c/a5a28b7c4df1316ff0ede0ce51af3a9af76b23c6f19a2d9edcd28036aa8d/ruff-0.0.267-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:5a898953949e37c109dd242cfcf9841e065319995ebb7cdfd213b446094a942f"},
-    {url = "https://files.pythonhosted.org/packages/21/80/c68a5d5117f84b6d4892cf8a5e1b164bd5b14bc0894ce0cba5343e40f132/ruff-0.0.267-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:9adf1307fa9d840d1acaa477eb04f9702032a483214c409fca9dc46f5f157fe3"},
-    {url = "https://files.pythonhosted.org/packages/3e/52/d1015fa5a13e9bd11b7a4e1147f541e52fe666b550f14e9ca1249bdc447b/ruff-0.0.267-py3-none-musllinux_1_2_i686.whl", hash = "sha256:786de30723c71fc46b80a173c3313fc0dbe73c96bd9da8dd1212cbc2f84cdfb2"},
-    {url = "https://files.pythonhosted.org/packages/45/1e/f423a80da2217137ef3d287aec70d978ae71038cce92cdc61659ebb4a063/ruff-0.0.267-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:2107cec3699ca4d7bd41543dc1d475c97ae3a21ea9212238b5c2088fa8ee7722"},
-    {url = "https://files.pythonhosted.org/packages/53/0c/8897fc309498b48fc60552c714264e91fda10c44defa9401a5c6288cb198/ruff-0.0.267-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:bbe104f21a429b77eb5ac276bd5352fd8c0e1fbb580b4c772f77ee8c76825654"},
-    {url = "https://files.pythonhosted.org/packages/53/49/fe3e44b5ebd9456e4e0acf79d9c0a777da59f170b7b95e2438f7e10deb15/ruff-0.0.267-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:45d61a2b01bdf61581a2ee039503a08aa603dc74a6bbe6fb5d1ce3052f5370e5"},
-    {url = "https://files.pythonhosted.org/packages/54/e3/eaa63e3a5c03613088ca00857ba4cf6e6e0e7463a183633a2083b167d02f/ruff-0.0.267-py3-none-win_amd64.whl", hash = "sha256:d09aecc9f5845586ba90911d815f9772c5a6dcf2e34be58c6017ecb124534ac4"},
-    {url = "https://files.pythonhosted.org/packages/56/8f/0ea8e8023f2005e86d9177a250ac0bda008143e5d38f3c21301d81fc09ac/ruff-0.0.267-py3-none-win32.whl", hash = "sha256:d12ab329474c46b96d962e2bdb92e3ad2144981fe41b89c7770f370646c0101f"},
-    {url = "https://files.pythonhosted.org/packages/5d/ba/5dfcde964c63c37e825889dc706afd8641c5460a01eeb6764b2440d1ba25/ruff-0.0.267-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f731d81cb939e757b0335b0090f18ca2e9ff8bcc8e6a1cf909245958949b6e11"},
-    {url = "https://files.pythonhosted.org/packages/67/85/249e6d52ed6272cdb9785e00bd8f1f7b7ac9ed3285c42300137faabb50ae/ruff-0.0.267-py3-none-win_arm64.whl", hash = "sha256:7df7eb5f8d791566ba97cc0b144981b9c080a5b861abaf4bb35a26c8a77b83e9"},
-    {url = "https://files.pythonhosted.org/packages/6d/7d/1c3a89baa73a7880db0706092b668061c172cda6a7ac510646af54bd746a/ruff-0.0.267-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:67254ae34c38cba109fdc52e4a70887de1f850fb3971e5eeef343db67305d1c1"},
-    {url = "https://files.pythonhosted.org/packages/96/e4/c9a745407e204e755fa39a1819dc602662fef90fd9b00f44aac3b4d67176/ruff-0.0.267-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:0afca3633c8e2b6c0a48ad0061180b641b3b404d68d7e6736aab301c8024c424"},
-    {url = "https://files.pythonhosted.org/packages/b8/3e/ef28832b87a177b3815c6e1fbe314498359122d671e8d80eca22a933784f/ruff-0.0.267-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:20c594eb56c19063ef5a57f89340e64c6550e169d6a29408a45130a8c3068adc"},
-    {url = "https://files.pythonhosted.org/packages/d9/da/ee9b62a02de95d716522095e62e7b2fb94dba13d9943e27400c59813bfb5/ruff-0.0.267.tar.gz", hash = "sha256:632cec7bbaf3c06fcf0a72a1dd029b7d8b7f424ba95a574aaa135f5d20a00af7"},
-    {url = "https://files.pythonhosted.org/packages/f1/7a/08f4803d440ee8fac3f007ca41e1a061fa529833c90b3b8dd37662393bbf/ruff-0.0.267-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:db33deef2a5e1cf528ca51cc59dd764122a48a19a6c776283b223d147041153f"},
-    {url = "https://files.pythonhosted.org/packages/fa/25/cd00b70d749cff37dc567e7267926211ddfaeb8b4eb05aed43d0decfceea/ruff-0.0.267-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:2972241065b1c911bce3db808837ed10f4f6f8a8e15520a4242d291083605ab6"},
-    {url = "https://files.pythonhosted.org/packages/fb/09/6db9f4e8f5dbbe82a72abf2b89cc2bd5033ebee9767187428061e93b4e17/ruff-0.0.267-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:4adbbbe314d8fcc539a245065bad89446a3cef2e0c9cf70bf7bb9ed6fe31856d"},
+"ruff 0.0.269" = [
+    {url = "https://files.pythonhosted.org/packages/02/65/c49103428b27ef3831f6f8023a062de07d7a88d4d9d9f22cbf4941331b4b/ruff-0.0.269-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:f062059b8289a4fab7f6064601b811d447c2f9d3d432a17f689efe4d68988450"},
+    {url = "https://files.pythonhosted.org/packages/18/f1/28f24e47a8dfb72762056713fd66c2f6fd543d0f6d3858291cb3d4993c2a/ruff-0.0.269-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1f19f59ca3c28742955241fb452f3346241ddbd34e72ac5cb3d84fadebcf6bc8"},
+    {url = "https://files.pythonhosted.org/packages/1d/97/60d69db70fa1e7e29a553fc6719ef6b750da0d570285f4c890ba686655f8/ruff-0.0.269-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6da8ee25ef2f0cc6cc8e6e20942c1d44d25a36dce35070d7184655bc14f63f63"},
+    {url = "https://files.pythonhosted.org/packages/26/64/3e1fc0ccf7d59d7c45ec643541642cd3bcc95c36b5c2e01f9f9f908650c4/ruff-0.0.269-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:cec2f4b84a14b87f1b121488649eb5b4eaa06467a2387373f750da74bdcb5679"},
+    {url = "https://files.pythonhosted.org/packages/2a/22/514380df775cac977caaa1394e2955c600e6f3895c0713e5f5aa99735d02/ruff-0.0.269-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3f5dc7aac52c58e82510217e3c7efd80765c134c097c2815d59e40face0d1fe6"},
+    {url = "https://files.pythonhosted.org/packages/30/ff/e1e0ec0e4e31b3f163ef3e80456150a41a3b910cac04472a13248b812ce6/ruff-0.0.269-py3-none-win_arm64.whl", hash = "sha256:bbeb857b1e508a4487bdb02ca1e6d41dd8d5ac5335a5246e25de8a3dff38c1ff"},
+    {url = "https://files.pythonhosted.org/packages/3c/42/88f5242e41988bb83a37a04f16f3523c4b65b2133fa5e9d05ef276dd0b70/ruff-0.0.269-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:5a20658f0b97d207c7841c13d528f36d666bf445b00b01139f28a8ccb80093bb"},
+    {url = "https://files.pythonhosted.org/packages/4a/04/77ad67155861ccf0deead144e4ba766b54c669c37aafc25d092a1a4f0af7/ruff-0.0.269.tar.gz", hash = "sha256:11ddcfbab32cf5c420ea9dd5531170ace5a3e59c16d9251c7bd2581f7b16f602"},
+    {url = "https://files.pythonhosted.org/packages/5b/93/67a13d30ae7d709774ab14b12ba6e90d3d8116a19afae1f0a5a818513ea1/ruff-0.0.269-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:a374434e588e06550df0f8dcb74777290f285678de991fda4e1063c367ab2eb2"},
+    {url = "https://files.pythonhosted.org/packages/95/19/0c3372acb612100e7417e394b85d98e3a73d80c6cc5a86d0253a40bc68ca/ruff-0.0.269-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:374b161753a247904aec7a32d45e165302b76b6e83d22d099bf3ff7c232c888f"},
+    {url = "https://files.pythonhosted.org/packages/9c/38/1ce6bc423e9e86ed21e4cae62a0f67f08ddc8bfdadcd2c340e427fd3e9a1/ruff-0.0.269-py3-none-win_amd64.whl", hash = "sha256:f3b59ccff57b21ef0967ea8021fd187ec14c528ec65507d8bcbe035912050776"},
+    {url = "https://files.pythonhosted.org/packages/a9/a4/b555c6fb6880c64cd88e42e44c235770abf6263457ab493dac4ad123c427/ruff-0.0.269-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:bd81b8e681b9eaa6cf15484f3985bd8bd97c3d114e95bff3e8ea283bf8865062"},
+    {url = "https://files.pythonhosted.org/packages/b9/9f/692b03ed8f2065e4fd628d5f55ba68fe941cd23bd6f9afa4eddcba27316b/ruff-0.0.269-py3-none-win32.whl", hash = "sha256:03ff42bc91ceca58e0f0f072cb3f9286a9208f609812753474e799a997cdad1a"},
+    {url = "https://files.pythonhosted.org/packages/bf/0b/6415002df30de68a541f0fce1adb77d8160b5afb36edeea2e0c3fbf28192/ruff-0.0.269-py3-none-musllinux_1_2_i686.whl", hash = "sha256:9ca0a1ddb1d835b5f742db9711c6cf59f213a1ad0088cb1e924a005fd399e7d8"},
+    {url = "https://files.pythonhosted.org/packages/d4/7c/1b8378f80962ff7d129a39785964710f92ebd9fa91e2444f00635ba3f510/ruff-0.0.269-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:3569bcdee679045c09c0161fabc057599759c49219a08d9a4aad2cc3982ccba3"},
+    {url = "https://files.pythonhosted.org/packages/f6/0c/eced078f3e0a4461b10dbf163160bd7a860378303a07253cbe8d1541fff4/ruff-0.0.269-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:56347da63757a56cbce7d4b3d6044ca4f1941cd1bbff3714f7554360c3361f83"},
+    {url = "https://files.pythonhosted.org/packages/f8/17/90e1cb087a20e136da10b0187cf1bf25ac80da1c5fcb0256b683e6eee047/ruff-0.0.269-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e131b4dbe798c391090c6407641d6ab12c0fa1bb952379dde45e5000e208dabb"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
```

### Comparing `xklb-1.28.8/readme.py` & `xklb-1.28.9/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.28.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.28.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/.github/workflows/push.yaml` & `xklb-1.28.9/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/sql/transfer.sql` & `xklb-1.28.9/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/av.py` & `xklb-1.28.9/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/books.py` & `xklb-1.28.9/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/consts.py` & `xklb-1.28.9/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/db.py` & `xklb-1.28.9/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/dl_config.py` & `xklb-1.28.9/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/dl_extract.py` & `xklb-1.28.9/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/fs_extract.py` & `xklb-1.28.9/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/gui.py` & `xklb-1.28.9/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/hn_extract.py` & `xklb-1.28.9/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/lb.py` & `xklb-1.28.9/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/play_actions.py` & `xklb-1.28.9/xklb/play_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -604,27 +604,20 @@
         args.select += "cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"
     args.select_sql = "\n        , ".join(args.select)
     args.limit_sql = "LIMIT " + str(args.limit) if args.limit else ""
     args.offset_sql = f"OFFSET {args.skip}" if args.skip and args.limit else ""
     query = f"""WITH m as (
     SELECT rowid, * FROM {args.table}
     WHERE 1=1
-        {'and path like "http%"' if args.safe else ''}
-        {f'and path not like "{args.keep_dir}%"' if Path(args.keep_dir).exists() else ''}
-        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and 'time_deleted' not in ' '.join(sys.argv) else ''}
-        {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
-        {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
-        {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only else ''}
-        {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only else ''}
+        {" ".join(args.filter_sql)}
+        {player.filter_args_sql(args, m_columns)}
     )
     SELECT
         {args.select_sql}
     FROM m
-    WHERE 1=1
-        {" ".join(args.filter_sql)}
     ORDER BY 1=1
         , {args.sort}
     {args.limit_sql} {args.offset_sql}
     """
 
     args.filter_sql = [
         s for s in args.filter_sql if "rowid" not in s
```

### Comparing `xklb-1.28.8/xklb/playback.py` & `xklb-1.28.9/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/player.py` & `xklb-1.28.9/xklb/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import csv, operator, os, platform, re, shutil, socket, subprocess
+import csv, operator, os, platform, re, shutil, socket, subprocess, sys
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 from platform import system
 from random import randrange
 from shlex import join, quote, split
@@ -381,20 +381,32 @@
     while len(remove_chars) < 1:
         remove_chars += remove_groups[-number_of_groups]
         number_of_groups += 1
 
     return remove_chars
 
 
+def filter_args_sql(args, m_columns):
+    return f"""
+        {'and path like "http%"' if args.safe else ''}
+        {f'and path not like "{args.keep_dir}%"' if Path(args.keep_dir).exists() else ''}
+        {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns and 'time_deleted' not in ' '.join(sys.argv) else ''}
+        {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
+        {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
+        {'AND COALESCE(time_downloaded,0) = 0' if args.online_media_only else ''}
+        {'AND COALESCE(time_downloaded,1)!= 0 AND path not like "http%"' if args.local_media_only else ''}
+    """
+
+
 def get_ordinal_media(args, m: Dict, ignore_paths=None) -> Dict:
     # TODO: maybe try https://dba.stackexchange.com/questions/43415/algorithm-for-finding-the-longest-prefix
     if ignore_paths is None:
         ignore_paths = []
 
-    columns = args.db["media"].columns_dict
+    m_columns = args.db["media"].columns_dict
 
     total_media = args.db.execute("select count(*) val from media").fetchone()[0]
     candidate = deepcopy(m["path"])
     similar_videos = []
     while len(similar_videos) <= 1:
         if candidate == "":
             return m
@@ -410,15 +422,15 @@
         candidate = new_candidate
         query = f"""
             SELECT
                 {args.select_sql}
             FROM {'media' if args.play_in_order >= consts.SIMILAR_NO_FILTER_NO_FTS else args.table}
             WHERE 1=1
                 and path like :candidate
-                {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in columns else ''}
+                {filter_args_sql(args, m_columns)}
                 {'' if args.play_in_order >= consts.SIMILAR_NO_FILTER else (" ".join(args.filter_sql) or '')}
                 {"and path not in ({})".format(",".join([":ignore_path{}".format(i) for i in range(len(ignore_paths))])) if len(ignore_paths) > 0 else ''}
             ORDER BY play_count, path
             LIMIT 1000
             """
         ignore_path_params = {"ignore_path{}".format(i): value for i, value in enumerate(ignore_paths)}
         bindings = {"candidate": candidate + "%", **ignore_path_params}
@@ -449,41 +461,44 @@
     m_columns = args.db["media"].columns_dict
     m_columns.update(rank=int)
 
     m = args.db["media"].get(m["path"])
     words = set(
         utils.conform(utils.extract_words(m.get(k)) for k in m.keys() if k in db.config["media"]["search_columns"])
     )
-
-    args.include = words
+    args.include = sorted(words, key=len, reverse=True)[:100]
     args.table = db.fts_flexible_search(args)
 
     cols = args.cols or ["path", "title", "duration", "size", "subtitle_count", "is_dir", "rank"]
     args.select = [c for c in cols if c in m_columns or c in ["*"]]
     args.select_sql = "\n        , ".join(args.select)
     query = f"""
         SELECT
             {args.select_sql}, rank
-        FROM {args.table}
+        FROM {args.table} m
         WHERE 1=1
-            {'and COALESCE(time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
+            and path != :path
+            {filter_args_sql(args, m_columns)}
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.filter_sql) or '')}
-        ORDER BY play_count, rank, path
-        {args.limit_sql} {args.offset_sql}
+        ORDER BY play_count
+            , m.path like "http%"
+            , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank), {args.sort}'}
+            , path
+        {"LIMIT " + str(args.limit - 1) if args.limit else ""} {args.offset_sql}
         """
-    bindings = {}
+    bindings = {"path": m["path"]}
     if args.related >= consts.RELATED_NO_FILTER:
         bindings = {**bindings, "query": args.filter_bindings["query"]}
     else:
         bindings = {**bindings, **args.filter_bindings}
 
     related_videos = list(args.db.query(query, bindings))
     log.debug(related_videos)
 
-    return related_videos
+    return [m] + related_videos
 
 
 def watch_chromecast(args, m: dict, subtitles_file=None) -> Optional[subprocess.CompletedProcess]:
     if "vlc" in args.player:
         catt_log = cmd(
             "vlc",
             "--sout",
```

### Comparing `xklb-1.28.8/xklb/praw_extract.py` & `xklb-1.28.9/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/stats.py` & `xklb-1.28.9/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/subtitle.py` & `xklb-1.28.9/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/tabs_actions.py` & `xklb-1.28.9/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/tabs_extract.py` & `xklb-1.28.9/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/tube_backend.py` & `xklb-1.28.9/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/tube_extract.py` & `xklb-1.28.9/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/utils.py` & `xklb-1.28.9/xklb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import humanize
 from IPython.core import ultratb
 from IPython.terminal.debugger import TerminalPdb
 from rich import prompt
 from rich.logging import RichHandler
 
-from xklb import consts
+from xklb import consts, data
 
 try:
     import ipdb
 except ModuleNotFoundError:
     pass
 else:
     sys.breakpointhook = ipdb.set_trace
@@ -345,20 +345,36 @@
         .replace(" _", "_")
         .replace("_ ", "_")
     )
     p = remove_consecutive_whitespace(p)
     return p
 
 
+def safe_int(s) -> Optional[int]:
+    try:
+        return int(float(s))
+    except Exception:
+        return None
+
+
 def extract_words(string):
     if not string:
         return None
 
     cleaned_string = re.sub(r"[^\w\s]", " ", string)
     words = [remove_consecutive_whitespace(s) for s in cleaned_string.split()]
+    words = [
+        s
+        for s in words
+        if not (
+            s.lower() in data.stop_words
+            or s.lower() in data.prepositions
+            or (safe_int(s) is not None and safe_int(s) < 100)
+        )
+    ]
     return words
 
 
 def clean_path(b, dot_space=False) -> str:
     import ftfy
 
     p = b.decode("utf-8", "backslashreplace")
@@ -465,21 +481,14 @@
             continue
         else:
             filtered_media.append(m)
 
     return filtered_media
 
 
-def safe_int(s) -> Optional[int]:
-    try:
-        return int(float(s))
-    except Exception:
-        return None
-
-
 def mpv_enrich2(args, media) -> List[Dict]:
     md5s = {path_to_mpv_watchlater_md5(m["path"]): m for m in media}
     paths = set(Path(args.watch_later_directory).glob("*"))
 
     previously_watched = [
         {
             **(md5s.get(p.stem) or {}),
```

### Comparing `xklb-1.28.8/xklb/scripts/__init__.py` & `xklb-1.28.9/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/bigdirs.py` & `xklb-1.28.9/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/christen.py` & `xklb-1.28.9/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/copy_play_counts.py` & `xklb-1.28.9/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/dedupe.py` & `xklb-1.28.9/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/merge_dbs.py` & `xklb-1.28.9/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/merge_online_local.py` & `xklb-1.28.9/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/move_list.py` & `xklb-1.28.9/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/optimize_db.py` & `xklb-1.28.9/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/redownload.py` & `xklb-1.28.9/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/relmv.py` & `xklb-1.28.9/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/scatter.py` & `xklb-1.28.9/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/streaming_tab_loader.py` & `xklb-1.28.9/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/mining/data.py` & `xklb-1.28.9/xklb/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/mining/extract_links.py` & `xklb-1.28.9/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/mining/nouns.py` & `xklb-1.28.9/xklb/scripts/mining/nouns.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import sys
 from html.parser import HTMLParser
 from io import StringIO
 
+from xklb import data
 from xklb.utils import pipe_print
 
-from . import data
-
 """
 extract compound nouns and phrases from unstructured mixed HTML plain text
 
 xsv select text hn_comment_202210242109.csv | library nouns | sort | uniq -c | sort --numeric-sort
 """
```

### Comparing `xklb-1.28.8/xklb/scripts/mining/pushshift.py` & `xklb-1.28.9/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.28.9/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/.gitignore` & `xklb-1.28.9/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/LICENSE` & `xklb-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/README.md` & `xklb-1.28.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.008)
+    xk media library subcommands (v1.28.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.28.8/pyproject.toml` & `xklb-1.28.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.28.8/PKG-INFO` & `xklb-1.28.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.28.8
+Version: 1.28.9
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.28.008)
+    xk media library subcommands (v1.28.009)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

