# Comparing `tmp/jupyterlab-katex-3.3.0.tar.gz` & `tmp/jupyterlab_katex-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab-katex-3.3.0.tar", last modified: Mon Jan 17 16:36:48 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `jupyterlab-katex-3.3.0.tar` & `jupyterlab_katex-3.4.0.tar`

### file list

```diff
@@ -1,89 +1,105 @@
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.090692 jupyterlab-katex-3.3.0/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     1533 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/LICENSE
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      447 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/MANIFEST.in
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     3121 2022-01-17 16:36:48.090692 jupyterlab-katex-3.3.0/PKG-INFO
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     2316 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/README.md
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      193 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/install.json
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.070691 jupyterlab-katex-3.3.0/jupyterlab-katex/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      319 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/__init__.py
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      441 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/_version.py
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.070691 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     2590 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/package.json
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.066691 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.066691 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.070691 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/katex-extension/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     2448 2022-01-17 16:36:37.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/katex-extension/package.json.orig
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      597 2022-01-17 16:36:37.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/katex-extension/plugin.json
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.086691 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    46028 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/06af0fba8798a625f89e5c605569a3a44828e2677fa9481fe06205d2062c7ba9.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    28708 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/081f08cf7e0a8a68cdbb29977fb0bb10a1dc71f7ae9b53648f79e98532ee26fe.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    17988 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/08f69ff860ef323f559c5a640b7ec5f3dc469a01b7159cddfa4286acb629c360.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    37856 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/0b9f6662c0c07fbd4c68949975aa6cb8d3881a86f9e6375af5b3bc3742f25273.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    15880 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/10914c41ecc86f46941584f301555614fe8c59463e0452bef84dfd999a56adcc.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    10008 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/114d46ba510a4d816884afcd2b98a4d6cebd5ea7afdeb6f849fe5abf9b727ee9.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    17044 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/1182f7b49fead9d22f3f14541e71e3331977a0441643c56664806949b96bed5a.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    24500 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/120253ea1310e3b80891610430105b0226766a4fa3d2c80f22c2cf887d84fd79.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    19700 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/15978c32403fa18a1843e66b0f0f5a9ca3c6a33aa128c6dfb4aa07251ab6990b.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    31136 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/15df487e2d49d960851524efb8c1fcca6b1197890cf4309f05c29d5010adcf32.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    11792 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2227c4c4953e65cbf7f67e83c12a27243478265619aae313353fda3b1458ed2c.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    42300 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/23d872b2185ce3c530e32c25bbad141de622dcc3171e939f33b2b1b55086396e.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    24668 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/252ec45ca7d1b70a8ee070ed0b8863f5554e2c5190cf409a6b3179a0ebe0cf26.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    13300 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2673b817a2a74139b1d9bd2f9d70148426346cbae579a5141abd839436126e2e.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    21244 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/27fccaf740860a615575c6af8549677fdb33401266cab7caa1765f16e0d57a42.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    29932 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2eb5660215fd2009a794b550df1b19df65acda11f4dff65d91a684f061214b55.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    21192 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/3467e032f722c3b5e0254862103bd24182049cd8781b86ffe2a9c8d77511e43f.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    70936 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/479c8788e05d188c708214c72d2b1d03a0834b035cf621fd26ecc2a048e97d9b.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    11080 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/48c988b76e6f36614ca627c3c1ff550fa02da781a97364475374b5c02912f2a2.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    44484 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/517b4b11866ae3d18e74168ebb179f88cb56668de40ea1e23fff0a61f78ef04a.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    11932 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/5293e7e9ac564ccd10deceec3a4cf3fa0754d3ce53ba3a4af21ae215686af001.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)   147397 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/533.d6b9fd7a31727b57ec5a.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    29860 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/60b247213ad93691bcdb19438cb0b67c7ea2fb4b3a72e82078beb791dd2b941a.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    12992 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/611edea9609d5b7728e2df2cb6034ea0aea459c7c06e6d8b8f83ca21a9f440d2.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      982 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/643.bb10b0cf3cac77c8d13d.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)   247527 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/654.37cda6b64b789e43ffac.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    14484 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/66034ad79f0f68739b7be69771748a1c61d524d4dbba570905318595151377ad.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    15416 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/697b1c9f6e11e42800664b58d06173e96548f87ad8b96a37cb01fa4b897dff9b.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     3716 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/704.654ced8aac282e7771a2.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    32312 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/7b7be7af132561e043a429328fcde231634bfeace1c9e3024887fc4a6f09b6bf.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    23980 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/82880d882256c6098e5c4a8bdb8f67fbbccb42bf33a5b68e3662bd9bf1f34448.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    21668 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/9339484861f622622c4d4fecffcb05da810407cc23305e8799bc1100329223b9.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    25352 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/a4f24d9b4244d4341ba0214cac621ec5727218df842af6de8e228aae985b5512.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    42872 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/a70a4daf27a074dbc86ca6b186306b852792929da734394fbc62ad3b788aefe5.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    23904 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/ae44802f0b88aca9a5b0150990c7dbd2c51bcf725da05cfb71f878c476017711.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    16868 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/af1d60bcfc57febf32ab10cc5467219f76117ef82fa663f92db22194f376b424.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    14908 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/b40a2796e46b2f558dcb5158bc76ffd7d5a7cbe35c0662a7599c9e1a88ae4e3c.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    34560 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/c3d1c2c8c0455af0db352e704e4fd4c5ae692cb3b895b6be752f5a89bf3b93f5.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    16208 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/cb6b7776d09864b2dc99c1ae5ee3659a7115db75b6ed660def2161968a2437c2.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    23520 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/cc796f5fea153a7134e5050fad1bcccadee89d52ace60d498f6fc1f1e069032e.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    15712 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/dc8093175e397ea58bed6a7bcc810e05e2125742763f1599babaa926461a32cb.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    59972 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/deba64bdc3911c01e7bee8c1c9c736d3f5859eaea0d91d5a793a140b21d6b1c6.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    13668 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/df5e2dff7ff874a1c50566b93ea32bdf9b219fb1646240ad61ad332c950cfa9d.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    22076 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/e5d73a831c38e3782f1698d94716025e26a59d34272bcf9ac7ab188d2cc9af16.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    32588 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/e818e3cd8065e949ca547607045e1cca24912d02f1b44d3efcac67ba6320f619.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    68880 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/eab76eab40c7dd342bc38c05d008b96a3a603f6c0bf635701ed1c6b2f0c12fcd.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    35056 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/eebf6eacab4b4238f927271da3bc942970ba7dcdeb6226a0b893dba3f73801ef.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    13912 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f1527a373f9e2f3b9b9a44d5a9f4fcc225fe15b9c64735b434de8a5d93fcdf12.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    36912 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f5b0e1ff158f892d45bbd24799d83b3f046ea492b248674a7d2e26787ff9f5bd.woff
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    15296 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f6f61cab7740ef34b23a8e941760bf54a5c3e8975d70d5cea3c244bbf699fad9.woff2
--rw-rw-r--   0 jtp       (1000) jtp       (1000)    24400 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f7184e0f0eb9ebd69d81acbd01bbd2519b82f4a4701530d40e47154680d07a02.ttf
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     7027 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/remoteEntry.ed329d57579564c8b6bc.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      170 2022-01-17 16:36:37.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/style.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     3703 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/third-party-licenses.json
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.086691 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     3121 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/PKG-INFO
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     6098 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/SOURCES.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)        1 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/dependency_links.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)        1 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/not-zip-safe
--rw-rw-r--   0 jtp       (1000) jtp       (1000)       17 2022-01-17 16:36:47.000000 jupyterlab-katex-3.3.0/jupyterlab_katex.egg-info/top_level.txt
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     2448 2022-01-17 16:34:54.000000 jupyterlab-katex-3.3.0/package.json
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      145 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/pyproject.toml
--rw-rw-r--   0 jtp       (1000) jtp       (1000)       38 2022-01-17 16:36:48.090692 jupyterlab-katex-3.3.0/setup.cfg
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     2393 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/setup.py
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.086691 jupyterlab-katex-3.3.0/src/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     5800 2022-01-17 16:32:53.000000 jupyterlab-katex-3.3.0/src/autorender.ts
--rw-rw-r--   0 jtp       (1000) jtp       (1000)     1685 2022-01-17 16:32:53.000000 jupyterlab-katex-3.3.0/src/index.ts
-drwxrwxr-x   0 jtp       (1000) jtp       (1000)        0 2022-01-17 16:36:48.090692 jupyterlab-katex-3.3.0/style/
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      632 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/style/base.css
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      287 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/style/index.css
--rw-rw-r--   0 jtp       (1000) jtp       (1000)       21 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/style/index.js
--rw-rw-r--   0 jtp       (1000) jtp       (1000)      555 2022-01-17 16:29:50.000000 jupyterlab-katex-3.3.0/tsconfig.json
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/.copier-answers.yml
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/.eslintignore
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/.yarnrc.yml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/install.json
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/tsconfig.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/_version.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/package.json
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/schemas/@jupyterlab/katex-extension/package.json.orig
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/schemas/@jupyterlab/katex-extension/plugin.json
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/01e074cc3dcd71407103.woff2
+-rw-r--r--   0        0        0    46028 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/06af0fba8798a625f89e.ttf
+-rw-r--r--   0        0        0    28708 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/081f08cf7e0a8a68cdbb.ttf
+-rw-r--r--   0        0        0    17988 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/08f69ff860ef323f559c.woff
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/0b27467a453fa09303e0.woff2
+-rw-r--r--   0        0        0    37856 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/0b9f6662c0c07fbd4c68.woff
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/10914c41ecc86f469415.woff
+-rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/114d46ba510a4d816884.ttf
+-rw-r--r--   0        0        0    17044 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/1182f7b49fead9d22f3f.woff
+-rw-r--r--   0        0        0    24500 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/120253ea1310e3b80891.woff
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/14c6e060c8735876e3cd.woff
+-rw-r--r--   0        0        0    19700 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/15978c32403fa18a1843.woff
+-rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/15df487e2d49d9608515.woff2
+-rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2227c4c4953e65cbf7f6.woff2
+-rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/230588b650d4d4d4e471.ttf
+-rw-r--r--   0        0        0    42300 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/23d872b2185ce3c530e3.ttf
+-rw-r--r--   0        0        0    24668 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/252ec45ca7d1b70a8ee0.woff
+-rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2673b817a2a74139b1d9.woff2
+-rw-r--r--   0        0        0    21244 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/27fccaf740860a615575.woff2
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/283580ac91c54b6fa655.woff
+-rw-r--r--   0        0        0    29932 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2eb5660215fd2009a794.woff2
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/325df4744e9e1c1e978c.woff2
+-rw-r--r--   0        0        0    21192 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/3467e032f722c3b5e025.woff2
+-rw-r--r--   0        0        0     6012 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/38e966e4ea4cc3f91f70.woff
+-rw-r--r--   0        0        0     9376 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/3cc9328f43e5092aaaeb.woff
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/41e4c13808366d1e102f.woff
+-rw-r--r--   0        0        0    70936 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/479c8788e05d188c7082.ttf
+-rw-r--r--   0        0        0    11080 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/48c988b76e6f36614ca6.ttf
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/4b4d0fa429e52f14c25e.woff2
+-rw-r--r--   0        0        0    44484 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/517b4b11866ae3d18e74.ttf
+-rw-r--r--   0        0        0    11932 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/5293e7e9ac564ccd10de.ttf
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/537.320d67943944ccaf87fc.js
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/579306c793600772ef71.woff2
+-rw-r--r--   0        0        0    29860 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/60b247213ad93691bcdb.ttf
+-rw-r--r--   0        0        0    12992 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/611edea9609d5b7728e2.woff
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/643.a63dec0bcc09cf695f3a.js
+-rw-r--r--   0        0        0   246229 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/654.e293e14ee956f393cfa0.js
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/66034ad79f0f68739b7b.woff2
+-rw-r--r--   0        0        0    34640 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/689.a2a55bd7baeb48f90f2c.js
+-rw-r--r--   0        0        0    15416 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/697b1c9f6e11e4280066.ttf
+-rw-r--r--   0        0        0    32312 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/7b7be7af132561e043a4.woff2
+-rw-r--r--   0        0        0    23980 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/82880d882256c6098e5c.woff
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/86f923f6b2ba9aa499e7.woff2
+-rw-r--r--   0        0        0    21668 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/9339484861f622622c4d.woff2
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/9d4aa93853e15f82ea86.woff
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/a4f24d9b4244d4341ba0.woff
+-rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/a70a4daf27a074dbc86c.ttf
+-rw-r--r--   0        0        0    23904 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/ae44802f0b88aca9a5b0.ttf
+-rw-r--r--   0        0        0    16868 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/af1d60bcfc57febf32ab.woff2
+-rw-r--r--   0        0        0    14908 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/b40a2796e46b2f558dcb.ttf
+-rw-r--r--   0        0        0    34560 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/c3d1c2c8c0455af0db35.ttf
+-rw-r--r--   0        0        0    16208 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/cb6b7776d09864b2dc99.woff
+-rw-r--r--   0        0        0    23520 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/cc796f5fea153a7134e5.ttf
+-rw-r--r--   0        0        0    15712 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/dc8093175e397ea58bed.woff
+-rw-r--r--   0        0        0    59972 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/deba64bdc3911c01e7be.ttf
+-rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/df5e2dff7ff874a1c505.woff2
+-rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/e5d73a831c38e3782f16.woff2
+-rw-r--r--   0        0        0    32588 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/e818e3cd8065e949ca54.ttf
+-rw-r--r--   0        0        0    68880 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/eab76eab40c7dd342bc3.ttf
+-rw-r--r--   0        0        0    35056 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/eebf6eacab4b4238f927.woff
+-rw-r--r--   0        0        0    13912 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f1527a373f9e2f3b9b9a.woff2
+-rw-r--r--   0        0        0    36912 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f5b0e1ff158f892d45bb.woff
+-rw-r--r--   0        0        0    15296 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f6f61cab7740ef34b23a.woff2
+-rw-r--r--   0        0        0    24400 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f7184e0f0eb9ebd69d81.ttf
+-rw-r--r--   0        0        0     7008 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/remoteEntry.704fe5b2eb7ee9890e7f.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/style.js
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/schema/plugin.json
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/src/autorender.ts
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/src/index.ts
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/style/base.css
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-1-linux.html
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-1-linux.png
+-rw-r--r--   0        0        0    13250 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-2-linux.html
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-2-linux.png
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-3-linux.html
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-3-linux.png
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-4-linux.html
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/ui-tests/tests/jupyterlab_katex.spec.ts-snapshots/katex-notebook-4-linux.png
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/.gitignore
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/LICENSE
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/README.md
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 jupyterlab_katex-3.4.0/PKG-INFO
```

### Comparing `jupyterlab-katex-3.3.0/LICENSE` & `jupyterlab_katex-3.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2015-2017, Project Jupyter Contributors
+Copyright (c) 2015-2023, Project Jupyter Contributors
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `jupyterlab-katex-3.3.0/PKG-INFO` & `jupyterlab_katex-3.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: jupyterlab-katex
-Version: 3.3.0
-Summary: KaTeX math renderer for JupyterLab
-Home-page: https://github.com/jupyterlab/jupyter-renderers
-Author: Project Jupyter
-Author-email: jupyter@googlegroups.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # jupyterlab-katex
 
 A JupyterLab extension for rendering [KaTeX](https://khan.github.io/KaTeX/) math.
 
 The default LaTeX renderer in JupyterLab uses [MathJax](https://www.mathjax.org/),
 which, while powerful, can be slow to render complex equations.
 This extension substitutes the MathJax renderer with the KaTeX renderer.
@@ -85,9 +61,7 @@
 ```
 
 ### Uninstall
 
 ```bash
 pip uninstall jupyterlab-katex
 ```
-
-
```

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/katex-extension/package.json.orig` & `jupyterlab_katex-3.4.0/package.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9152649176954734%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.0.0 || ^4.0.0', '@jupyterlab/rendermime': "*

 * *                   "'^3.0.0 || ^4.0.0', '@jupyterlab/rendermime-interfaces': '^3.0.0 || ^3.8.0', "*

 * *                   "'@jupyterlab/settingregistry': '^3.0.0 || ^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', 'rimraf': '^4.4.1', 'typescript': "*

 * *                      "'~5.0.2', '@types/json-schema': '^7.0.11', "*

 * *                      "'@typescript-eslint/eslint-plugin': '^5.55.0', '@typescript- […]*

```diff
@@ -3,45 +3,62 @@
         "email": "jupyter@googlegroups.com",
         "name": "Project Jupyter"
     },
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-renderers/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.2.8",
-        "@jupyterlab/rendermime": "^3.2.8",
-        "@jupyterlab/rendermime-interfaces": "^3.2.8",
-        "@jupyterlab/settingregistry": "^3.2.8",
+        "@jupyterlab/application": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime-interfaces": "^3.0.0 || ^3.8.0",
+        "@jupyterlab/settingregistry": "^3.0.0 || ^4.0.0",
         "katex": "^0.12.0"
     },
     "description": "KaTeX math renderer for JupyterLab",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.2.8",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
         "@types/katex": "^0.11.0",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "npm-run-all": "^4.1.5",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js",
         "schema/*.json",
         "style/*.*",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-renderers",
     "jupyterlab": {
         "disabledExtensions": [
+            "@jupyterlab/mathjax-extension:plugin",
             "@jupyterlab/mathjax2-extension:plugin"
         ],
         "extension": true,
-        "outputDir": "jupyterlab-katex/labextension",
+        "outputDir": "jupyterlab_katex/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "katex"
@@ -50,30 +67,36 @@
     "main": "lib/index.js",
     "name": "@jupyterlab/katex-extension",
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-renderers.git"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:dist",
-        "clean:dist": "rimraf dist",
-        "clean:labextension": "rimraf ./jupyterlab-katex/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_katex/labextension jupyterlab_katex/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jupyter labextension develop --overwrite .",
-        "prepack": "npm run clean && npm run build",
-        "prepare": "jlpm run clean && jlpm run build:prod",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.3.0"
+    "version": "3.4.0"
 }
```

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/schemas/@jupyterlab/katex-extension/plugin.json` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/schemas/@jupyterlab/katex-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/06af0fba8798a625f89e5c605569a3a44828e2677fa9481fe06205d2062c7ba9.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/06af0fba8798a625f89e.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/081f08cf7e0a8a68cdbb29977fb0bb10a1dc71f7ae9b53648f79e98532ee26fe.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/081f08cf7e0a8a68cdbb.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/08f69ff860ef323f559c5a640b7ec5f3dc469a01b7159cddfa4286acb629c360.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/08f69ff860ef323f559c.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/0b9f6662c0c07fbd4c68949975aa6cb8d3881a86f9e6375af5b3bc3742f25273.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/0b9f6662c0c07fbd4c68.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/10914c41ecc86f46941584f301555614fe8c59463e0452bef84dfd999a56adcc.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/10914c41ecc86f469415.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/114d46ba510a4d816884afcd2b98a4d6cebd5ea7afdeb6f849fe5abf9b727ee9.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/114d46ba510a4d816884.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/1182f7b49fead9d22f3f14541e71e3331977a0441643c56664806949b96bed5a.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/1182f7b49fead9d22f3f.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/120253ea1310e3b80891610430105b0226766a4fa3d2c80f22c2cf887d84fd79.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/120253ea1310e3b80891.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/15978c32403fa18a1843e66b0f0f5a9ca3c6a33aa128c6dfb4aa07251ab6990b.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/15978c32403fa18a1843.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/15df487e2d49d960851524efb8c1fcca6b1197890cf4309f05c29d5010adcf32.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/15df487e2d49d9608515.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2227c4c4953e65cbf7f67e83c12a27243478265619aae313353fda3b1458ed2c.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2227c4c4953e65cbf7f6.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/23d872b2185ce3c530e32c25bbad141de622dcc3171e939f33b2b1b55086396e.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/23d872b2185ce3c530e3.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/252ec45ca7d1b70a8ee070ed0b8863f5554e2c5190cf409a6b3179a0ebe0cf26.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/252ec45ca7d1b70a8ee0.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2673b817a2a74139b1d9bd2f9d70148426346cbae579a5141abd839436126e2e.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2673b817a2a74139b1d9.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/27fccaf740860a615575c6af8549677fdb33401266cab7caa1765f16e0d57a42.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/27fccaf740860a615575.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/2eb5660215fd2009a794b550df1b19df65acda11f4dff65d91a684f061214b55.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/2eb5660215fd2009a794.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/3467e032f722c3b5e0254862103bd24182049cd8781b86ffe2a9c8d77511e43f.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/3467e032f722c3b5e025.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/479c8788e05d188c708214c72d2b1d03a0834b035cf621fd26ecc2a048e97d9b.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/479c8788e05d188c7082.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/48c988b76e6f36614ca627c3c1ff550fa02da781a97364475374b5c02912f2a2.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/48c988b76e6f36614ca6.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/517b4b11866ae3d18e74168ebb179f88cb56668de40ea1e23fff0a61f78ef04a.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/517b4b11866ae3d18e74.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/5293e7e9ac564ccd10deceec3a4cf3fa0754d3ce53ba3a4af21ae215686af001.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/5293e7e9ac564ccd10de.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/60b247213ad93691bcdb19438cb0b67c7ea2fb4b3a72e82078beb791dd2b941a.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/60b247213ad93691bcdb.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/611edea9609d5b7728e2df2cb6034ea0aea459c7c06e6d8b8f83ca21a9f440d2.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/611edea9609d5b7728e2.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/643.bb10b0cf3cac77c8d13d.js` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/643.a63dec0bcc09cf695f3a.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,28 +1,36 @@
 "use strict";
 (self.webpackChunk_jupyterlab_katex_extension = self.webpackChunk_jupyterlab_katex_extension || []).push([
     [643], {
         1246: (e, n, t) => {
             t.d(n, {
-                Z: () => o
+                Z: () => p
             });
-            var i = t(2609),
+            var s = t(9601),
+                a = t.n(s),
+                i = t(2609),
                 r = t.n(i),
-                a = t(4605),
-                s = r()((function(e) {
-                    return e[1]
-                }));
-            s.i(a.Z), s.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/**\n * Note: the KaTeX CSS doesn't apply a height property\n * to its SVG objects, so it can be overridden by low-\n * specificity rules elsewhere on the page. This\n * is a workaround for that behavior.\n */\n.katex svg {\n  height: inherit;\n}\n\n.jp-OutputArea-output.jp-RenderedLatex .katex-display {\n  text-align: left;\n  margin: 0;\n}\n", ""]);
-            const o = s
+                l = t(4605),
+                o = r()(a());
+            o.i(l.Z), o.push([e.id, "/* -----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|---------------------------------------------------------------------------- */\n\n/* stylelint-disable selector-class-pattern */\n\n/**\n * Note: the KaTeX CSS doesn't apply a height property\n * to its SVG objects, so it can be overridden by low-\n * specificity rules elsewhere on the page. This\n * is a workaround for that behavior.\n */\n.katex svg {\n  height: inherit;\n}\n\n.jp-OutputArea-output.jp-RenderedLatex .katex-display {\n  text-align: left;\n  margin: 0;\n}\n", ""]);
+            const p = o
         },
         6643: (e, n, t) => {
             t.r(n);
-            var i = t(6062),
+            var s = t(6062),
+                a = t.n(s),
+                i = t(4036),
                 r = t.n(i),
-                a = t(1246);
-            r()(a.Z, {
-                insert: "head",
-                singleton: !1
-            }), a.Z.locals
+                l = t(6793),
+                o = t.n(l),
+                p = t(7892),
+                h = t.n(p),
+                u = t(1173),
+                d = t.n(u),
+                c = t(2464),
+                b = t.n(c),
+                y = t(1246),
+                k = {};
+            k.styleTagTransform = b(), k.setAttributes = h(), k.insert = o().bind(null, "head"), k.domAPI = r(), k.insertStyleElement = d(), a()(y.Z, k), y.Z && y.Z.locals && y.Z.locals
         }
     }
 ]);
```

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/654.37cda6b64b789e43ffac.js` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/654.e293e14ee956f393cfa0.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -92,40 +92,42 @@
                             '"': "&quot;",
                             "'": "&#x27;"
                         },
                         h = /[&><"']/g,
                         m = function e(t) {
                             return "ordgroup" === t.type || "color" === t.type ? 1 === t.body.length ? e(t.body[0]) : t : "font" === t.type ? e(t.body) : t
                         },
-                        c = function(e, t) {
-                            return -1 !== e.indexOf(t)
-                        },
-                        u = function(e, t) {
-                            return void 0 === e ? t : e
-                        },
-                        p = function(e) {
-                            return String(e).replace(h, (function(e) {
-                                return l[e]
-                            }))
-                        },
-                        d = function(e) {
-                            return e.replace(s, "-$1").toLowerCase()
-                        },
-                        f = m,
-                        g = function(e) {
-                            var t = m(e);
-                            return "mathord" === t.type || "textord" === t.type || "atom" === t.type
-                        },
-                        v = function(e) {
-                            var t = /^\s*([^\\/#]*?)(?::|&#0*58|&#x0*3a)/i.exec(e);
-                            return null != t ? t[1] : "_relative"
+                        c = {
+                            contains: function(e, t) {
+                                return -1 !== e.indexOf(t)
+                            },
+                            deflt: function(e, t) {
+                                return void 0 === e ? t : e
+                            },
+                            escape: function(e) {
+                                return String(e).replace(h, (function(e) {
+                                    return l[e]
+                                }))
+                            },
+                            hyphenate: function(e) {
+                                return e.replace(s, "-$1").toLowerCase()
+                            },
+                            getBaseElem: m,
+                            isCharacterBox: function(e) {
+                                var t = m(e);
+                                return "mathord" === t.type || "textord" === t.type || "atom" === t.type
+                            },
+                            protocolFromUrl: function(e) {
+                                var t = /^\s*([^\\/#]*?)(?::|&#0*58|&#x0*3a)/i.exec(e);
+                                return null != t ? t[1] : "_relative"
+                            }
                         },
-                        b = function() {
+                        u = function() {
                             function e(e) {
-                                this.displayMode = void 0, this.output = void 0, this.leqno = void 0, this.fleqn = void 0, this.throwOnError = void 0, this.errorColor = void 0, this.macros = void 0, this.minRuleThickness = void 0, this.colorIsTextColor = void 0, this.strict = void 0, this.trust = void 0, this.maxSize = void 0, this.maxExpand = void 0, this.globalGroup = void 0, e = e || {}, this.displayMode = u(e.displayMode, !1), this.output = u(e.output, "htmlAndMathml"), this.leqno = u(e.leqno, !1), this.fleqn = u(e.fleqn, !1), this.throwOnError = u(e.throwOnError, !0), this.errorColor = u(e.errorColor, "#cc0000"), this.macros = e.macros || {}, this.minRuleThickness = Math.max(0, u(e.minRuleThickness, 0)), this.colorIsTextColor = u(e.colorIsTextColor, !1), this.strict = u(e.strict, "warn"), this.trust = u(e.trust, !1), this.maxSize = Math.max(0, u(e.maxSize, 1 / 0)), this.maxExpand = Math.max(0, u(e.maxExpand, 1e3)), this.globalGroup = u(e.globalGroup, !1)
+                                this.displayMode = void 0, this.output = void 0, this.leqno = void 0, this.fleqn = void 0, this.throwOnError = void 0, this.errorColor = void 0, this.macros = void 0, this.minRuleThickness = void 0, this.colorIsTextColor = void 0, this.strict = void 0, this.trust = void 0, this.maxSize = void 0, this.maxExpand = void 0, this.globalGroup = void 0, e = e || {}, this.displayMode = c.deflt(e.displayMode, !1), this.output = c.deflt(e.output, "htmlAndMathml"), this.leqno = c.deflt(e.leqno, !1), this.fleqn = c.deflt(e.fleqn, !1), this.throwOnError = c.deflt(e.throwOnError, !0), this.errorColor = c.deflt(e.errorColor, "#cc0000"), this.macros = e.macros || {}, this.minRuleThickness = Math.max(0, c.deflt(e.minRuleThickness, 0)), this.colorIsTextColor = c.deflt(e.colorIsTextColor, !1), this.strict = c.deflt(e.strict, "warn"), this.trust = c.deflt(e.trust, !1), this.maxSize = Math.max(0, c.deflt(e.maxSize, 1 / 0)), this.maxExpand = Math.max(0, c.deflt(e.maxExpand, 1e3)), this.globalGroup = c.deflt(e.globalGroup, !1)
                             }
                             var t = e.prototype;
                             return t.reportNonstrict = function(e, t, r) {
                                 var n = this.strict;
                                 if ("function" == typeof n && (n = n(e, t, r)), n && "ignore" !== n) {
                                     if (!0 === n || "error" === n) throw new o("LaTeX-incompatible input and strict mode is set to 'error': " + t + " [" + e + "]", r);
                                     "warn" === n ? "undefined" != typeof console && console.warn("LaTeX-incompatible input and strict mode is set to 'warn': " + t + " [" + e + "]") : "undefined" != typeof console && console.warn("LaTeX-incompatible input and strict mode is set to unrecognized '" + n + "': " + t + " [" + e + "]")
@@ -135,54 +137,54 @@
                                 if ("function" == typeof n) try {
                                     n = n(e, t, r)
                                 } catch (e) {
                                     n = "error"
                                 }
                                 return !(!n || "ignore" === n || !0 !== n && "error" !== n && ("warn" === n ? ("undefined" != typeof console && console.warn("LaTeX-incompatible input and strict mode is set to 'warn': " + t + " [" + e + "]"), 1) : ("undefined" != typeof console && console.warn("LaTeX-incompatible input and strict mode is set to unrecognized '" + n + "': " + t + " [" + e + "]"), 1)))
                             }, t.isTrusted = function(e) {
-                                e.url && !e.protocol && (e.protocol = v(e.url));
+                                e.url && !e.protocol && (e.protocol = c.protocolFromUrl(e.url));
                                 var t = "function" == typeof this.trust ? this.trust(e) : this.trust;
                                 return Boolean(t)
                             }, e
                         }(),
-                        y = function() {
+                        p = function() {
                             function e(e, t, r) {
                                 this.id = void 0, this.size = void 0, this.cramped = void 0, this.id = e, this.size = t, this.cramped = r
                             }
                             var t = e.prototype;
                             return t.sup = function() {
-                                return x[w[this.id]]
+                                return d[f[this.id]]
                             }, t.sub = function() {
-                                return x[k[this.id]]
+                                return d[g[this.id]]
                             }, t.fracNum = function() {
-                                return x[S[this.id]]
+                                return d[v[this.id]]
                             }, t.fracDen = function() {
-                                return x[M[this.id]]
+                                return d[b[this.id]]
                             }, t.cramp = function() {
-                                return x[z[this.id]]
+                                return d[y[this.id]]
                             }, t.text = function() {
-                                return x[A[this.id]]
+                                return d[x[this.id]]
                             }, t.isTight = function() {
                                 return this.size >= 2
                             }, e
                         }(),
-                        x = [new y(0, 0, !1), new y(1, 0, !0), new y(2, 1, !1), new y(3, 1, !0), new y(4, 2, !1), new y(5, 2, !0), new y(6, 3, !1), new y(7, 3, !0)],
-                        w = [4, 5, 4, 5, 6, 7, 6, 7],
-                        k = [5, 5, 5, 5, 7, 7, 7, 7],
-                        S = [2, 3, 4, 5, 6, 7, 6, 7],
-                        M = [3, 3, 5, 5, 7, 7, 7, 7],
-                        z = [1, 1, 3, 3, 5, 5, 7, 7],
-                        A = [0, 1, 2, 3, 2, 3, 2, 3],
-                        T = {
-                            DISPLAY: x[0],
-                            TEXT: x[2],
-                            SCRIPT: x[4],
-                            SCRIPTSCRIPT: x[6]
+                        d = [new p(0, 0, !1), new p(1, 0, !0), new p(2, 1, !1), new p(3, 1, !0), new p(4, 2, !1), new p(5, 2, !0), new p(6, 3, !1), new p(7, 3, !0)],
+                        f = [4, 5, 4, 5, 6, 7, 6, 7],
+                        g = [5, 5, 5, 5, 7, 7, 7, 7],
+                        v = [2, 3, 4, 5, 6, 7, 6, 7],
+                        b = [3, 3, 5, 5, 7, 7, 7, 7],
+                        y = [1, 1, 3, 3, 5, 5, 7, 7],
+                        x = [0, 1, 2, 3, 2, 3, 2, 3],
+                        w = {
+                            DISPLAY: d[0],
+                            TEXT: d[2],
+                            SCRIPT: d[4],
+                            SCRIPTSCRIPT: d[6]
                         },
-                        B = [{
+                        k = [{
                             name: "latin",
                             blocks: [
                                 [256, 591],
                                 [768, 879]
                             ]
                         }, {
                             name: "cyrillic",
@@ -208,27 +210,27 @@
                             ]
                         }, {
                             name: "hangul",
                             blocks: [
                                 [44032, 55215]
                             ]
                         }],
-                        C = [];
+                        S = [];
 
-                    function q(e) {
-                        for (var t = 0; t < C.length; t += 2)
-                            if (e >= C[t] && e <= C[t + 1]) return !0;
+                    function M(e) {
+                        for (var t = 0; t < S.length; t += 2)
+                            if (e >= S[t] && e <= S[t + 1]) return !0;
                         return !1
                     }
-                    B.forEach((function(e) {
+                    k.forEach((function(e) {
                         return e.blocks.forEach((function(e) {
-                            return C.push.apply(C, e)
+                            return S.push.apply(S, e)
                         }))
                     }));
-                    var N = {
+                    var z = {
                             leftParenInner: "M291 0 H417 V300 H291 z",
                             rightParenInner: "M457 0 H583 V300 H457 z",
                             doubleleftarrow: "M262 157\nl10-10c34-36 62.7-77 86-123 3.3-8 5-13.3 5-16 0-5.3-6.7-8-20-8-7.3\n 0-12.2.5-14.5 1.5-2.3 1-4.8 4.5-7.5 10.5-49.3 97.3-121.7 169.3-217 216-28\n 14-57.3 25-88 33-6.7 2-11 3.8-13 5.5-2 1.7-3 4.2-3 7.5s1 5.8 3 7.5\nc2 1.7 6.3 3.5 13 5.5 68 17.3 128.2 47.8 180.5 91.5 52.3 43.7 93.8 96.2 124.5\n 157.5 9.3 8 15.3 12.3 18 13h6c12-.7 18-4 18-10 0-2-1.7-7-5-15-23.3-46-52-87\n-86-123l-10-10h399738v-40H218c328 0 0 0 0 0l-10-8c-26.7-20-65.7-43-117-69 2.7\n-2 6-3.7 10-5 36.7-16 72.3-37.3 107-64l10-8h399782v-40z\nm8 0v40h399730v-40zm0 194v40h399730v-40z",
                             doublerightarrow: "M399738 392l\n-10 10c-34 36-62.7 77-86 123-3.3 8-5 13.3-5 16 0 5.3 6.7 8 20 8 7.3 0 12.2-.5\n 14.5-1.5 2.3-1 4.8-4.5 7.5-10.5 49.3-97.3 121.7-169.3 217-216 28-14 57.3-25 88\n-33 6.7-2 11-3.8 13-5.5 2-1.7 3-4.2 3-7.5s-1-5.8-3-7.5c-2-1.7-6.3-3.5-13-5.5-68\n-17.3-128.2-47.8-180.5-91.5-52.3-43.7-93.8-96.2-124.5-157.5-9.3-8-15.3-12.3-18\n-13h-6c-12 .7-18 4-18 10 0 2 1.7 7 5 15 23.3 46 52 87 86 123l10 10H0v40h399782\nc-328 0 0 0 0 0l10 8c26.7 20 65.7 43 117 69-2.7 2-6 3.7-10 5-36.7 16-72.3 37.3\n-107 64l-10 8H0v40zM0 157v40h399730v-40zm0 194v40h399730v-40z",
                             leftarrow: "M400000 241H110l3-3c68.7-52.7 113.7-120\n 135-202 4-14.7 6-23 6-25 0-7.3-7-11-21-11-8 0-13.2.8-15.5 2.5-2.3 1.7-4.2 5.8\n-5.5 12.5-1.3 4.7-2.7 10.3-4 17-12 48.7-34.8 92-68.5 130S65.3 228.3 18 247\nc-10 4-16 7.7-18 11 0 8.7 6 14.3 18 17 47.3 18.7 87.8 47 121.5 85S196 441.3 208\n 490c.7 2 1.3 5 2 9s1.2 6.7 1.5 8c.3 1.3 1 3.3 2 6s2.2 4.5 3.5 5.5c1.3 1 3.3\n 1.8 6 2.5s6 1 10 1c14 0 21-3.7 21-11 0-2-2-10.3-6-25-20-79.3-65-146.7-135-202\n l-3-3h399890zM100 241v40h399900v-40z",
                             leftbrace: "M6 548l-6-6v-35l6-11c56-104 135.3-181.3 238-232 57.3-28.7 117\n-45 179-50h399577v120H403c-43.3 7-81 15-113 26-100.7 33-179.7 91-237 174-2.7\n 5-6 9-10 13-.7 1-7.3 1-20 1H6z",
                             leftbraceunder: "M0 6l6-6h17c12.688 0 19.313.3 20 1 4 4 7.313 8.3 10 13\n 35.313 51.3 80.813 93.8 136.5 127.5 55.688 33.7 117.188 55.8 184.5 66.5.688\n 0 2 .3 4 1 18.688 2.7 76 4.3 172 5h399450v120H429l-6-1c-124.688-8-235-61.7\n-331-161C60.687 138.7 32.312 99.3 7 54L0 41V6z",
@@ -279,149 +281,149 @@
                             baraboveleftarrow: "M400000 620h-399890l3 -3c68.7 -52.7 113.7 -120 135 -202\nc4 -14.7 6 -23 6 -25c0 -7.3 -7 -11 -21 -11c-8 0 -13.2 0.8 -15.5 2.5\nc-2.3 1.7 -4.2 5.8 -5.5 12.5c-1.3 4.7 -2.7 10.3 -4 17c-12 48.7 -34.8 92 -68.5 130\ns-74.2 66.3 -121.5 85c-10 4 -16 7.7 -18 11c0 8.7 6 14.3 18 17c47.3 18.7 87.8 47\n121.5 85s56.5 81.3 68.5 130c0.7 2 1.3 5 2 9s1.2 6.7 1.5 8c0.3 1.3 1 3.3 2 6\ns2.2 4.5 3.5 5.5c1.3 1 3.3 1.8 6 2.5s6 1 10 1c14 0 21 -3.7 21 -11\nc0 -2 -2 -10.3 -6 -25c-20 -79.3 -65 -146.7 -135 -202l-3 -3h399890z\nM100 620v40h399900v-40z M0 241v40h399900v-40zM0 241v40h399900v-40z",
                             rightarrowabovebar: "M0 241v40h399891c-47.3 35.3-84 78-110 128-16.7 32\n-27.7 63.7-33 95 0 1.3-.2 2.7-.5 4-.3 1.3-.5 2.3-.5 3 0 7.3 6.7 11 20 11 8 0\n13.2-.8 15.5-2.5 2.3-1.7 4.2-5.5 5.5-11.5 2-13.3 5.7-27 11-41 14.7-44.7 39\n-84.5 73-119.5s73.7-60.2 119-75.5c6-2 9-5.7 9-11s-3-9-9-11c-45.3-15.3-85-40.5\n-119-75.5s-58.3-74.8-73-119.5c-4.7-14-8.3-27.3-11-40-1.3-6.7-3.2-10.8-5.5\n-12.5-2.3-1.7-7.5-2.5-15.5-2.5-14 0-21 3.7-21 11 0 2 2 10.3 6 25 20.7 83.3 67\n151.7 139 205zm96 379h399894v40H0zm0 0h399904v40H0z",
                             baraboveshortleftharpoon: "M507,435c-4,4,-6.3,8.7,-7,14c0,5.3,0.7,9,2,11\nc1.3,2,5.3,5.3,12,10c90.7,54,156,130,196,228c3.3,10.7,6.3,16.3,9,17\nc2,0.7,5,1,9,1c0,0,5,0,5,0c10.7,0,16.7,-2,18,-6c2,-2.7,1,-9.7,-3,-21\nc-32,-87.3,-82.7,-157.7,-152,-211c0,0,-3,-3,-3,-3l399351,0l0,-40\nc-398570,0,-399437,0,-399437,0z M593 435 v40 H399500 v-40z\nM0 281 v-40 H399908 v40z M0 281 v-40 H399908 v40z",
                             rightharpoonaboveshortbar: "M0,241 l0,40c399126,0,399993,0,399993,0\nc4.7,-4.7,7,-9.3,7,-14c0,-9.3,-3.7,-15.3,-11,-18c-92.7,-56.7,-159,-133.7,-199,\n-231c-3.3,-9.3,-6,-14.7,-8,-16c-2,-1.3,-7,-2,-15,-2c-10.7,0,-16.7,2,-18,6\nc-2,2.7,-1,9.7,3,21c15.3,42,36.7,81.8,64,119.5c27.3,37.7,58,69.2,92,94.5z\nM0 241 v40 H399908 v-40z M0 475 v-40 H399500 v40z M0 475 v-40 H399500 v40z",
                             shortbaraboveleftharpoon: "M7,435c-4,4,-6.3,8.7,-7,14c0,5.3,0.7,9,2,11\nc1.3,2,5.3,5.3,12,10c90.7,54,156,130,196,228c3.3,10.7,6.3,16.3,9,17c2,0.7,5,1,9,\n1c0,0,5,0,5,0c10.7,0,16.7,-2,18,-6c2,-2.7,1,-9.7,-3,-21c-32,-87.3,-82.7,-157.7,\n-152,-211c0,0,-3,-3,-3,-3l399907,0l0,-40c-399126,0,-399993,0,-399993,0z\nM93 435 v40 H400000 v-40z M500 241 v40 H400000 v-40z M500 241 v40 H400000 v-40z",
                             shortrightharpoonabovebar: "M53,241l0,40c398570,0,399437,0,399437,0\nc4.7,-4.7,7,-9.3,7,-14c0,-9.3,-3.7,-15.3,-11,-18c-92.7,-56.7,-159,-133.7,-199,\n-231c-3.3,-9.3,-6,-14.7,-8,-16c-2,-1.3,-7,-2,-15,-2c-10.7,0,-16.7,2,-18,6\nc-2,2.7,-1,9.7,3,21c15.3,42,36.7,81.8,64,119.5c27.3,37.7,58,69.2,92,94.5z\nM500 241 v40 H399408 v-40z M500 435 v40 H400000 v-40z"
                         },
-                        I = function() {
+                        A = function() {
                             function e(e) {
                                 this.children = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, this.children = e, this.classes = [], this.height = 0, this.depth = 0, this.maxFontSize = 0, this.style = {}
                             }
                             var t = e.prototype;
                             return t.hasClass = function(e) {
-                                return c(this.classes, e)
+                                return c.contains(this.classes, e)
                             }, t.toNode = function() {
                                 for (var e = document.createDocumentFragment(), t = 0; t < this.children.length; t++) e.appendChild(this.children[t].toNode());
                                 return e
                             }, t.toMarkup = function() {
                                 for (var e = "", t = 0; t < this.children.length; t++) e += this.children[t].toMarkup();
                                 return e
                             }, t.toText = function() {
                                 return this.children.map((function(e) {
                                     return e.toText()
                                 })).join("")
                             }, e
                         }(),
-                        O = function(e) {
+                        T = function(e) {
                             return e.filter((function(e) {
                                 return e
                             })).join(" ")
                         },
-                        R = function(e, t, r) {
+                        B = function(e, t, r) {
                             if (this.classes = e || [], this.attributes = {}, this.height = 0, this.depth = 0, this.maxFontSize = 0, this.style = r || {}, t) {
                                 t.style.isTight() && this.classes.push("mtight");
                                 var n = t.getColor();
                                 n && (this.style.color = n)
                             }
                         },
-                        E = function(e) {
+                        C = function(e) {
                             var t = document.createElement(e);
-                            for (var r in t.className = O(this.classes), this.style) this.style.hasOwnProperty(r) && (t.style[r] = this.style[r]);
+                            for (var r in t.className = T(this.classes), this.style) this.style.hasOwnProperty(r) && (t.style[r] = this.style[r]);
                             for (var n in this.attributes) this.attributes.hasOwnProperty(n) && t.setAttribute(n, this.attributes[n]);
                             for (var a = 0; a < this.children.length; a++) t.appendChild(this.children[a].toNode());
                             return t
                         },
-                        L = function(e) {
+                        q = function(e) {
                             var t = "<" + e;
-                            this.classes.length && (t += ' class="' + p(O(this.classes)) + '"');
+                            this.classes.length && (t += ' class="' + c.escape(T(this.classes)) + '"');
                             var r = "";
-                            for (var n in this.style) this.style.hasOwnProperty(n) && (r += d(n) + ":" + this.style[n] + ";");
-                            for (var a in r && (t += ' style="' + p(r) + '"'), this.attributes) this.attributes.hasOwnProperty(a) && (t += " " + a + '="' + p(this.attributes[a]) + '"');
+                            for (var n in this.style) this.style.hasOwnProperty(n) && (r += c.hyphenate(n) + ":" + this.style[n] + ";");
+                            for (var a in r && (t += ' style="' + c.escape(r) + '"'), this.attributes) this.attributes.hasOwnProperty(a) && (t += " " + a + '="' + c.escape(this.attributes[a]) + '"');
                             t += ">";
                             for (var i = 0; i < this.children.length; i++) t += this.children[i].toMarkup();
                             return t + "</" + e + ">"
                         },
-                        P = function() {
+                        N = function() {
                             function e(e, t, r, n) {
-                                this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, R.call(this, e, r, n), this.children = t || []
+                                this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.width = void 0, this.maxFontSize = void 0, this.style = void 0, B.call(this, e, r, n), this.children = t || []
                             }
                             var t = e.prototype;
                             return t.setAttribute = function(e, t) {
                                 this.attributes[e] = t
                             }, t.hasClass = function(e) {
-                                return c(this.classes, e)
+                                return c.contains(this.classes, e)
                             }, t.toNode = function() {
-                                return E.call(this, "span")
+                                return C.call(this, "span")
                             }, t.toMarkup = function() {
-                                return L.call(this, "span")
+                                return q.call(this, "span")
                             }, e
                         }(),
-                        D = function() {
+                        I = function() {
                             function e(e, t, r, n) {
-                                this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, R.call(this, t, n), this.children = r || [], this.setAttribute("href", e)
+                                this.children = void 0, this.attributes = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, B.call(this, t, n), this.children = r || [], this.setAttribute("href", e)
                             }
                             var t = e.prototype;
                             return t.setAttribute = function(e, t) {
                                 this.attributes[e] = t
                             }, t.hasClass = function(e) {
-                                return c(this.classes, e)
+                                return c.contains(this.classes, e)
                             }, t.toNode = function() {
-                                return E.call(this, "a")
+                                return C.call(this, "a")
                             }, t.toMarkup = function() {
-                                return L.call(this, "a")
+                                return q.call(this, "a")
                             }, e
                         }(),
-                        H = function() {
+                        O = function() {
                             function e(e, t, r) {
                                 this.src = void 0, this.alt = void 0, this.classes = void 0, this.height = void 0, this.depth = void 0, this.maxFontSize = void 0, this.style = void 0, this.alt = t, this.src = e, this.classes = ["mord"], this.style = r
                             }
                             var t = e.prototype;
                             return t.hasClass = function(e) {
-                                return c(this.classes, e)
+                                return c.contains(this.classes, e)
                             }, t.toNode = function() {
                                 var e = document.createElement("img");
                                 for (var t in e.src = this.src, e.alt = this.alt, e.className = "mord", this.style) this.style.hasOwnProperty(t) && (e.style[t] = this.style[t]);
                                 return e
                             }, t.toMarkup = function() {
                                 var e = "<img  src='" + this.src + " 'alt='" + this.alt + "' ",
                                     t = "";
-                                for (var r in this.style) this.style.hasOwnProperty(r) && (t += d(r) + ":" + this.style[r] + ";");
-                                return t && (e += ' style="' + p(t) + '"'), e + "'/>"
+                                for (var r in this.style) this.style.hasOwnProperty(r) && (t += c.hyphenate(r) + ":" + this.style[r] + ";");
+                                return t && (e += ' style="' + c.escape(t) + '"'), e + "'/>"
                             }, e
                         }(),
-                        F = {
+                        R = {
                             î: "ı̂",
                             ï: "ı̈",
                             í: "ı́",
                             ì: "ı̀"
                         },
-                        V = function() {
+                        E = function() {
                             function e(e, t, r, n, a, i, o, s) {
                                 this.text = void 0, this.height = void 0, this.depth = void 0, this.italic = void 0, this.skew = void 0, this.width = void 0, this.maxFontSize = void 0, this.classes = void 0, this.style = void 0, this.text = e, this.height = t || 0, this.depth = r || 0, this.italic = n || 0, this.skew = a || 0, this.width = i || 0, this.classes = o || [], this.style = s || {}, this.maxFontSize = 0;
                                 var l = function(e) {
-                                    for (var t = 0; t < B.length; t++)
-                                        for (var r = B[t], n = 0; n < r.blocks.length; n++) {
+                                    for (var t = 0; t < k.length; t++)
+                                        for (var r = k[t], n = 0; n < r.blocks.length; n++) {
                                             var a = r.blocks[n];
                                             if (e >= a[0] && e <= a[1]) return r.name
                                         }
                                     return null
                                 }(this.text.charCodeAt(0));
-                                l && this.classes.push(l + "_fallback"), /[îïíì]/.test(this.text) && (this.text = F[this.text])
+                                l && this.classes.push(l + "_fallback"), /[îïíì]/.test(this.text) && (this.text = R[this.text])
                             }
                             var t = e.prototype;
                             return t.hasClass = function(e) {
-                                return c(this.classes, e)
+                                return c.contains(this.classes, e)
                             }, t.toNode = function() {
                                 var e = document.createTextNode(this.text),
                                     t = null;
-                                for (var r in this.italic > 0 && ((t = document.createElement("span")).style.marginRight = this.italic + "em"), this.classes.length > 0 && ((t = t || document.createElement("span")).className = O(this.classes)), this.style) this.style.hasOwnProperty(r) && ((t = t || document.createElement("span")).style[r] = this.style[r]);
+                                for (var r in this.italic > 0 && ((t = document.createElement("span")).style.marginRight = this.italic + "em"), this.classes.length > 0 && ((t = t || document.createElement("span")).className = T(this.classes)), this.style) this.style.hasOwnProperty(r) && ((t = t || document.createElement("span")).style[r] = this.style[r]);
                                 return t ? (t.appendChild(e), t) : e
                             }, t.toMarkup = function() {
                                 var e = !1,
                                     t = "<span";
-                                this.classes.length && (e = !0, t += ' class="', t += p(O(this.classes)), t += '"');
+                                this.classes.length && (e = !0, t += ' class="', t += c.escape(T(this.classes)), t += '"');
                                 var r = "";
-                                for (var n in this.italic > 0 && (r += "margin-right:" + this.italic + "em;"), this.style) this.style.hasOwnProperty(n) && (r += d(n) + ":" + this.style[n] + ";");
-                                r && (e = !0, t += ' style="' + p(r) + '"');
-                                var a = p(this.text);
+                                for (var n in this.italic > 0 && (r += "margin-right:" + this.italic + "em;"), this.style) this.style.hasOwnProperty(n) && (r += c.hyphenate(n) + ":" + this.style[n] + ";");
+                                r && (e = !0, t += ' style="' + c.escape(r) + '"');
+                                var a = c.escape(this.text);
                                 return e ? (t += ">", t += a, t += "</span>") : a
                             }, e
                         }(),
-                        U = function() {
+                        L = function() {
                             function e(e, t) {
                                 this.children = void 0, this.attributes = void 0, this.children = e || [], this.attributes = t || {}
                             }
                             var t = e.prototype;
                             return t.toNode = function() {
                                 var e = document.createElementNS("http://www.w3.org/2000/svg", "svg");
                                 for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && e.setAttribute(t, this.attributes[t]);
@@ -431,27 +433,27 @@
                                 var e = "<svg";
                                 for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && (e += " " + t + "='" + this.attributes[t] + "'");
                                 e += ">";
                                 for (var r = 0; r < this.children.length; r++) e += this.children[r].toMarkup();
                                 return e + "</svg>"
                             }, e
                         }(),
-                        G = function() {
+                        P = function() {
                             function e(e, t) {
                                 this.pathName = void 0, this.alternate = void 0, this.pathName = e, this.alternate = t
                             }
                             var t = e.prototype;
                             return t.toNode = function() {
                                 var e = document.createElementNS("http://www.w3.org/2000/svg", "path");
-                                return this.alternate ? e.setAttribute("d", this.alternate) : e.setAttribute("d", N[this.pathName]), e
+                                return this.alternate ? e.setAttribute("d", this.alternate) : e.setAttribute("d", z[this.pathName]), e
                             }, t.toMarkup = function() {
-                                return this.alternate ? "<path d='" + this.alternate + "'/>" : "<path d='" + N[this.pathName] + "'/>"
+                                return this.alternate ? "<path d='" + this.alternate + "'/>" : "<path d='" + z[this.pathName] + "'/>"
                             }, e
                         }(),
-                        Y = function() {
+                        D = function() {
                             function e(e) {
                                 this.attributes = void 0, this.attributes = e || {}
                             }
                             var t = e.prototype;
                             return t.toNode = function() {
                                 var e = document.createElementNS("http://www.w3.org/2000/svg", "line");
                                 for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && e.setAttribute(t, this.attributes[t]);
@@ -459,19 +461,19 @@
                             }, t.toMarkup = function() {
                                 var e = "<line";
                                 for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && (e += " " + t + "='" + this.attributes[t] + "'");
                                 return e + "/>"
                             }, e
                         }();
 
-                    function _(e) {
-                        if (e instanceof V) return e;
+                    function H(e) {
+                        if (e instanceof E) return e;
                         throw new Error("Expected symbolNode but got " + String(e) + ".")
                     }
-                    var W = {
+                    var F = {
                             "AMS-Regular": {
                                 32: [0, 0, 0, 0, .25],
                                 65: [0, .68889, 0, 0, .72222],
                                 66: [0, .68889, 0, 0, .66667],
                                 67: [0, .68889, 0, 0, .72222],
                                 68: [0, .68889, 0, 0, .72222],
                                 69: [0, .68889, 0, 0, .66667],
@@ -2538,15 +2540,15 @@
                                 937: [0, .61111, 0, 0, .525],
                                 8216: [0, .61111, 0, 0, .525],
                                 8217: [0, .61111, 0, 0, .525],
                                 8242: [0, .61111, 0, 0, .525],
                                 9251: [.11111, .21944, 0, 0, .525]
                             }
                         },
-                        X = {
+                        V = {
                             slant: [.25, .25, .25],
                             space: [0, 0, 0],
                             stretch: [0, 0, 0],
                             shrink: [0, 0, 0],
                             xHeight: [.431, .431, .431],
                             quad: [1, 1.171, 1.472],
                             extraSpace: [0, 0, 0],
@@ -2574,15 +2576,15 @@
                             sqrtRuleThickness: [.04, .04, .04],
                             ptPerEm: [10, 10, 10],
                             doubleRuleSep: [.2, .2, .2],
                             arrayRuleWidth: [.04, .04, .04],
                             fboxsep: [.3, .3, .3],
                             fboxrule: [.04, .04, .04]
                         },
-                        j = {
+                        U = {
                             Å: "A",
                             Ç: "C",
                             Ð: "D",
                             Þ: "o",
                             å: "a",
                             ç: "c",
                             ð: "d",
@@ -2649,105 +2651,105 @@
                             ы: "m",
                             ь: "a",
                             э: "e",
                             ю: "m",
                             я: "r"
                         };
 
-                    function $(e, t, r) {
-                        if (!W[t]) throw new Error("Font metrics not found for font: " + t + ".");
+                    function G(e, t, r) {
+                        if (!F[t]) throw new Error("Font metrics not found for font: " + t + ".");
                         var n = e.charCodeAt(0),
-                            a = W[t][n];
-                        if (!a && e[0] in j && (n = j[e[0]].charCodeAt(0), a = W[t][n]), a || "text" !== r || q(n) && (a = W[t][77]), a) return {
+                            a = F[t][n];
+                        if (!a && e[0] in U && (n = U[e[0]].charCodeAt(0), a = F[t][n]), a || "text" !== r || M(n) && (a = F[t][77]), a) return {
                             depth: a[0],
                             height: a[1],
                             italic: a[2],
                             skew: a[3],
                             width: a[4]
                         }
                     }
-                    var Z = {},
-                        K = {
+                    var Y = {},
+                        _ = {
                             bin: 1,
                             close: 1,
                             inner: 1,
                             open: 1,
                             punct: 1,
                             rel: 1
                         },
-                        J = {
+                        W = {
                             "accent-token": 1,
                             mathord: 1,
                             "op-token": 1,
                             spacing: 1,
                             textord: 1
                         },
-                        Q = {
+                        X = {
                             math: {},
                             text: {}
                         },
-                        ee = Q;
+                        j = X;
 
-                    function te(e, t, r, n, a, i) {
-                        Q[e][a] = {
+                    function $(e, t, r, n, a, i) {
+                        X[e][a] = {
                             font: t,
                             group: r,
                             replace: n
-                        }, i && n && (Q[e][n] = Q[e][a])
+                        }, i && n && (X[e][n] = X[e][a])
                     }
-                    var re = "math",
-                        ne = "text",
-                        ae = "main",
-                        ie = "ams",
-                        oe = "accent-token",
-                        se = "bin",
-                        le = "close",
-                        he = "inner",
-                        me = "mathord",
-                        ce = "op-token",
-                        ue = "open",
-                        pe = "punct",
-                        de = "rel",
-                        fe = "spacing",
-                        ge = "textord";
-                    te(re, ae, de, "≡", "\\equiv", !0), te(re, ae, de, "≺", "\\prec", !0), te(re, ae, de, "≻", "\\succ", !0), te(re, ae, de, "∼", "\\sim", !0), te(re, ae, de, "⊥", "\\perp"), te(re, ae, de, "⪯", "\\preceq", !0), te(re, ae, de, "⪰", "\\succeq", !0), te(re, ae, de, "≃", "\\simeq", !0), te(re, ae, de, "∣", "\\mid", !0), te(re, ae, de, "≪", "\\ll", !0), te(re, ae, de, "≫", "\\gg", !0), te(re, ae, de, "≍", "\\asymp", !0), te(re, ae, de, "∥", "\\parallel"), te(re, ae, de, "⋈", "\\bowtie", !0), te(re, ae, de, "⌣", "\\smile", !0), te(re, ae, de, "⊑", "\\sqsubseteq", !0), te(re, ae, de, "⊒", "\\sqsupseteq", !0), te(re, ae, de, "≐", "\\doteq", !0), te(re, ae, de, "⌢", "\\frown", !0), te(re, ae, de, "∋", "\\ni", !0), te(re, ae, de, "∝", "\\propto", !0), te(re, ae, de, "⊢", "\\vdash", !0), te(re, ae, de, "⊣", "\\dashv", !0), te(re, ae, de, "∋", "\\owns"), te(re, ae, pe, ".", "\\ldotp"), te(re, ae, pe, "⋅", "\\cdotp"), te(re, ae, ge, "#", "\\#"), te(ne, ae, ge, "#", "\\#"), te(re, ae, ge, "&", "\\&"), te(ne, ae, ge, "&", "\\&"), te(re, ae, ge, "ℵ", "\\aleph", !0), te(re, ae, ge, "∀", "\\forall", !0), te(re, ae, ge, "ℏ", "\\hbar", !0), te(re, ae, ge, "∃", "\\exists", !0), te(re, ae, ge, "∇", "\\nabla", !0), te(re, ae, ge, "♭", "\\flat", !0), te(re, ae, ge, "ℓ", "\\ell", !0), te(re, ae, ge, "♮", "\\natural", !0), te(re, ae, ge, "♣", "\\clubsuit", !0), te(re, ae, ge, "℘", "\\wp", !0), te(re, ae, ge, "♯", "\\sharp", !0), te(re, ae, ge, "♢", "\\diamondsuit", !0), te(re, ae, ge, "ℜ", "\\Re", !0), te(re, ae, ge, "♡", "\\heartsuit", !0), te(re, ae, ge, "ℑ", "\\Im", !0), te(re, ae, ge, "♠", "\\spadesuit", !0), te(ne, ae, ge, "§", "\\S", !0), te(ne, ae, ge, "¶", "\\P", !0), te(re, ae, ge, "†", "\\dag"), te(ne, ae, ge, "†", "\\dag"), te(ne, ae, ge, "†", "\\textdagger"), te(re, ae, ge, "‡", "\\ddag"), te(ne, ae, ge, "‡", "\\ddag"), te(ne, ae, ge, "‡", "\\textdaggerdbl"), te(re, ae, le, "⎱", "\\rmoustache", !0), te(re, ae, ue, "⎰", "\\lmoustache", !0), te(re, ae, le, "⟯", "\\rgroup", !0), te(re, ae, ue, "⟮", "\\lgroup", !0), te(re, ae, se, "∓", "\\mp", !0), te(re, ae, se, "⊖", "\\ominus", !0), te(re, ae, se, "⊎", "\\uplus", !0), te(re, ae, se, "⊓", "\\sqcap", !0), te(re, ae, se, "∗", "\\ast"), te(re, ae, se, "⊔", "\\sqcup", !0), te(re, ae, se, "◯", "\\bigcirc"), te(re, ae, se, "∙", "\\bullet"), te(re, ae, se, "‡", "\\ddagger"), te(re, ae, se, "≀", "\\wr", !0), te(re, ae, se, "⨿", "\\amalg"), te(re, ae, se, "&", "\\And"), te(re, ae, de, "⟵", "\\longleftarrow", !0), te(re, ae, de, "⇐", "\\Leftarrow", !0), te(re, ae, de, "⟸", "\\Longleftarrow", !0), te(re, ae, de, "⟶", "\\longrightarrow", !0), te(re, ae, de, "⇒", "\\Rightarrow", !0), te(re, ae, de, "⟹", "\\Longrightarrow", !0), te(re, ae, de, "↔", "\\leftrightarrow", !0), te(re, ae, de, "⟷", "\\longleftrightarrow", !0), te(re, ae, de, "⇔", "\\Leftrightarrow", !0), te(re, ae, de, "⟺", "\\Longleftrightarrow", !0), te(re, ae, de, "↦", "\\mapsto", !0), te(re, ae, de, "⟼", "\\longmapsto", !0), te(re, ae, de, "↗", "\\nearrow", !0), te(re, ae, de, "↩", "\\hookleftarrow", !0), te(re, ae, de, "↪", "\\hookrightarrow", !0), te(re, ae, de, "↘", "\\searrow", !0), te(re, ae, de, "↼", "\\leftharpoonup", !0), te(re, ae, de, "⇀", "\\rightharpoonup", !0), te(re, ae, de, "↙", "\\swarrow", !0), te(re, ae, de, "↽", "\\leftharpoondown", !0), te(re, ae, de, "⇁", "\\rightharpoondown", !0), te(re, ae, de, "↖", "\\nwarrow", !0), te(re, ae, de, "⇌", "\\rightleftharpoons", !0), te(re, ie, de, "≮", "\\nless", !0), te(re, ie, de, "", "\\@nleqslant"), te(re, ie, de, "", "\\@nleqq"), te(re, ie, de, "⪇", "\\lneq", !0), te(re, ie, de, "≨", "\\lneqq", !0), te(re, ie, de, "", "\\@lvertneqq"), te(re, ie, de, "⋦", "\\lnsim", !0), te(re, ie, de, "⪉", "\\lnapprox", !0), te(re, ie, de, "⊀", "\\nprec", !0), te(re, ie, de, "⋠", "\\npreceq", !0), te(re, ie, de, "⋨", "\\precnsim", !0), te(re, ie, de, "⪹", "\\precnapprox", !0), te(re, ie, de, "≁", "\\nsim", !0), te(re, ie, de, "", "\\@nshortmid"), te(re, ie, de, "∤", "\\nmid", !0), te(re, ie, de, "⊬", "\\nvdash", !0), te(re, ie, de, "⊭", "\\nvDash", !0), te(re, ie, de, "⋪", "\\ntriangleleft"), te(re, ie, de, "⋬", "\\ntrianglelefteq", !0), te(re, ie, de, "⊊", "\\subsetneq", !0), te(re, ie, de, "", "\\@varsubsetneq"), te(re, ie, de, "⫋", "\\subsetneqq", !0), te(re, ie, de, "", "\\@varsubsetneqq"), te(re, ie, de, "≯", "\\ngtr", !0), te(re, ie, de, "", "\\@ngeqslant"), te(re, ie, de, "", "\\@ngeqq"), te(re, ie, de, "⪈", "\\gneq", !0), te(re, ie, de, "≩", "\\gneqq", !0), te(re, ie, de, "", "\\@gvertneqq"), te(re, ie, de, "⋧", "\\gnsim", !0), te(re, ie, de, "⪊", "\\gnapprox", !0), te(re, ie, de, "⊁", "\\nsucc", !0), te(re, ie, de, "⋡", "\\nsucceq", !0), te(re, ie, de, "⋩", "\\succnsim", !0), te(re, ie, de, "⪺", "\\succnapprox", !0), te(re, ie, de, "≆", "\\ncong", !0), te(re, ie, de, "", "\\@nshortparallel"), te(re, ie, de, "∦", "\\nparallel", !0), te(re, ie, de, "⊯", "\\nVDash", !0), te(re, ie, de, "⋫", "\\ntriangleright"), te(re, ie, de, "⋭", "\\ntrianglerighteq", !0), te(re, ie, de, "", "\\@nsupseteqq"), te(re, ie, de, "⊋", "\\supsetneq", !0), te(re, ie, de, "", "\\@varsupsetneq"), te(re, ie, de, "⫌", "\\supsetneqq", !0), te(re, ie, de, "", "\\@varsupsetneqq"), te(re, ie, de, "⊮", "\\nVdash", !0), te(re, ie, de, "⪵", "\\precneqq", !0), te(re, ie, de, "⪶", "\\succneqq", !0), te(re, ie, de, "", "\\@nsubseteqq"), te(re, ie, se, "⊴", "\\unlhd"), te(re, ie, se, "⊵", "\\unrhd"), te(re, ie, de, "↚", "\\nleftarrow", !0), te(re, ie, de, "↛", "\\nrightarrow", !0), te(re, ie, de, "⇍", "\\nLeftarrow", !0), te(re, ie, de, "⇏", "\\nRightarrow", !0), te(re, ie, de, "↮", "\\nleftrightarrow", !0), te(re, ie, de, "⇎", "\\nLeftrightarrow", !0), te(re, ie, de, "△", "\\vartriangle"), te(re, ie, ge, "ℏ", "\\hslash"), te(re, ie, ge, "▽", "\\triangledown"), te(re, ie, ge, "◊", "\\lozenge"), te(re, ie, ge, "Ⓢ", "\\circledS"), te(re, ie, ge, "®", "\\circledR"), te(ne, ie, ge, "®", "\\circledR"), te(re, ie, ge, "∡", "\\measuredangle", !0), te(re, ie, ge, "∄", "\\nexists"), te(re, ie, ge, "℧", "\\mho"), te(re, ie, ge, "Ⅎ", "\\Finv", !0), te(re, ie, ge, "⅁", "\\Game", !0), te(re, ie, ge, "‵", "\\backprime"), te(re, ie, ge, "▲", "\\blacktriangle"), te(re, ie, ge, "▼", "\\blacktriangledown"), te(re, ie, ge, "■", "\\blacksquare"), te(re, ie, ge, "⧫", "\\blacklozenge"), te(re, ie, ge, "★", "\\bigstar"), te(re, ie, ge, "∢", "\\sphericalangle", !0), te(re, ie, ge, "∁", "\\complement", !0), te(re, ie, ge, "ð", "\\eth", !0), te(ne, ae, ge, "ð", "ð"), te(re, ie, ge, "╱", "\\diagup"), te(re, ie, ge, "╲", "\\diagdown"), te(re, ie, ge, "□", "\\square"), te(re, ie, ge, "□", "\\Box"), te(re, ie, ge, "◊", "\\Diamond"), te(re, ie, ge, "¥", "\\yen", !0), te(ne, ie, ge, "¥", "\\yen", !0), te(re, ie, ge, "✓", "\\checkmark", !0), te(ne, ie, ge, "✓", "\\checkmark"), te(re, ie, ge, "ℶ", "\\beth", !0), te(re, ie, ge, "ℸ", "\\daleth", !0), te(re, ie, ge, "ℷ", "\\gimel", !0), te(re, ie, ge, "ϝ", "\\digamma", !0), te(re, ie, ge, "ϰ", "\\varkappa"), te(re, ie, ue, "┌", "\\@ulcorner", !0), te(re, ie, le, "┐", "\\@urcorner", !0), te(re, ie, ue, "└", "\\@llcorner", !0), te(re, ie, le, "┘", "\\@lrcorner", !0), te(re, ie, de, "≦", "\\leqq", !0), te(re, ie, de, "⩽", "\\leqslant", !0), te(re, ie, de, "⪕", "\\eqslantless", !0), te(re, ie, de, "≲", "\\lesssim", !0), te(re, ie, de, "⪅", "\\lessapprox", !0), te(re, ie, de, "≊", "\\approxeq", !0), te(re, ie, se, "⋖", "\\lessdot"), te(re, ie, de, "⋘", "\\lll", !0), te(re, ie, de, "≶", "\\lessgtr", !0), te(re, ie, de, "⋚", "\\lesseqgtr", !0), te(re, ie, de, "⪋", "\\lesseqqgtr", !0), te(re, ie, de, "≑", "\\doteqdot"), te(re, ie, de, "≓", "\\risingdotseq", !0), te(re, ie, de, "≒", "\\fallingdotseq", !0), te(re, ie, de, "∽", "\\backsim", !0), te(re, ie, de, "⋍", "\\backsimeq", !0), te(re, ie, de, "⫅", "\\subseteqq", !0), te(re, ie, de, "⋐", "\\Subset", !0), te(re, ie, de, "⊏", "\\sqsubset", !0), te(re, ie, de, "≼", "\\preccurlyeq", !0), te(re, ie, de, "⋞", "\\curlyeqprec", !0), te(re, ie, de, "≾", "\\precsim", !0), te(re, ie, de, "⪷", "\\precapprox", !0), te(re, ie, de, "⊲", "\\vartriangleleft"), te(re, ie, de, "⊴", "\\trianglelefteq"), te(re, ie, de, "⊨", "\\vDash", !0), te(re, ie, de, "⊪", "\\Vvdash", !0), te(re, ie, de, "⌣", "\\smallsmile"), te(re, ie, de, "⌢", "\\smallfrown"), te(re, ie, de, "≏", "\\bumpeq", !0), te(re, ie, de, "≎", "\\Bumpeq", !0), te(re, ie, de, "≧", "\\geqq", !0), te(re, ie, de, "⩾", "\\geqslant", !0), te(re, ie, de, "⪖", "\\eqslantgtr", !0), te(re, ie, de, "≳", "\\gtrsim", !0), te(re, ie, de, "⪆", "\\gtrapprox", !0), te(re, ie, se, "⋗", "\\gtrdot"), te(re, ie, de, "⋙", "\\ggg", !0), te(re, ie, de, "≷", "\\gtrless", !0), te(re, ie, de, "⋛", "\\gtreqless", !0), te(re, ie, de, "⪌", "\\gtreqqless", !0), te(re, ie, de, "≖", "\\eqcirc", !0), te(re, ie, de, "≗", "\\circeq", !0), te(re, ie, de, "≜", "\\triangleq", !0), te(re, ie, de, "∼", "\\thicksim"), te(re, ie, de, "≈", "\\thickapprox"), te(re, ie, de, "⫆", "\\supseteqq", !0), te(re, ie, de, "⋑", "\\Supset", !0), te(re, ie, de, "⊐", "\\sqsupset", !0), te(re, ie, de, "≽", "\\succcurlyeq", !0), te(re, ie, de, "⋟", "\\curlyeqsucc", !0), te(re, ie, de, "≿", "\\succsim", !0), te(re, ie, de, "⪸", "\\succapprox", !0), te(re, ie, de, "⊳", "\\vartriangleright"), te(re, ie, de, "⊵", "\\trianglerighteq"), te(re, ie, de, "⊩", "\\Vdash", !0), te(re, ie, de, "∣", "\\shortmid"), te(re, ie, de, "∥", "\\shortparallel"), te(re, ie, de, "≬", "\\between", !0), te(re, ie, de, "⋔", "\\pitchfork", !0), te(re, ie, de, "∝", "\\varpropto"), te(re, ie, de, "◀", "\\blacktriangleleft"), te(re, ie, de, "∴", "\\therefore", !0), te(re, ie, de, "∍", "\\backepsilon"), te(re, ie, de, "▶", "\\blacktriangleright"), te(re, ie, de, "∵", "\\because", !0), te(re, ie, de, "⋘", "\\llless"), te(re, ie, de, "⋙", "\\gggtr"), te(re, ie, se, "⊲", "\\lhd"), te(re, ie, se, "⊳", "\\rhd"), te(re, ie, de, "≂", "\\eqsim", !0), te(re, ae, de, "⋈", "\\Join"), te(re, ie, de, "≑", "\\Doteq", !0), te(re, ie, se, "∔", "\\dotplus", !0), te(re, ie, se, "∖", "\\smallsetminus"), te(re, ie, se, "⋒", "\\Cap", !0), te(re, ie, se, "⋓", "\\Cup", !0), te(re, ie, se, "⩞", "\\doublebarwedge", !0), te(re, ie, se, "⊟", "\\boxminus", !0), te(re, ie, se, "⊞", "\\boxplus", !0), te(re, ie, se, "⋇", "\\divideontimes", !0), te(re, ie, se, "⋉", "\\ltimes", !0), te(re, ie, se, "⋊", "\\rtimes", !0), te(re, ie, se, "⋋", "\\leftthreetimes", !0), te(re, ie, se, "⋌", "\\rightthreetimes", !0), te(re, ie, se, "⋏", "\\curlywedge", !0), te(re, ie, se, "⋎", "\\curlyvee", !0), te(re, ie, se, "⊝", "\\circleddash", !0), te(re, ie, se, "⊛", "\\circledast", !0), te(re, ie, se, "⋅", "\\centerdot"), te(re, ie, se, "⊺", "\\intercal", !0), te(re, ie, se, "⋒", "\\doublecap"), te(re, ie, se, "⋓", "\\doublecup"), te(re, ie, se, "⊠", "\\boxtimes", !0), te(re, ie, de, "⇢", "\\dashrightarrow", !0), te(re, ie, de, "⇠", "\\dashleftarrow", !0), te(re, ie, de, "⇇", "\\leftleftarrows", !0), te(re, ie, de, "⇆", "\\leftrightarrows", !0), te(re, ie, de, "⇚", "\\Lleftarrow", !0), te(re, ie, de, "↞", "\\twoheadleftarrow", !0), te(re, ie, de, "↢", "\\leftarrowtail", !0), te(re, ie, de, "↫", "\\looparrowleft", !0), te(re, ie, de, "⇋", "\\leftrightharpoons", !0), te(re, ie, de, "↶", "\\curvearrowleft", !0), te(re, ie, de, "↺", "\\circlearrowleft", !0), te(re, ie, de, "↰", "\\Lsh", !0), te(re, ie, de, "⇈", "\\upuparrows", !0), te(re, ie, de, "↿", "\\upharpoonleft", !0), te(re, ie, de, "⇃", "\\downharpoonleft", !0), te(re, ie, de, "⊸", "\\multimap", !0), te(re, ie, de, "↭", "\\leftrightsquigarrow", !0), te(re, ie, de, "⇉", "\\rightrightarrows", !0), te(re, ie, de, "⇄", "\\rightleftarrows", !0), te(re, ie, de, "↠", "\\twoheadrightarrow", !0), te(re, ie, de, "↣", "\\rightarrowtail", !0), te(re, ie, de, "↬", "\\looparrowright", !0), te(re, ie, de, "↷", "\\curvearrowright", !0), te(re, ie, de, "↻", "\\circlearrowright", !0), te(re, ie, de, "↱", "\\Rsh", !0), te(re, ie, de, "⇊", "\\downdownarrows", !0), te(re, ie, de, "↾", "\\upharpoonright", !0), te(re, ie, de, "⇂", "\\downharpoonright", !0), te(re, ie, de, "⇝", "\\rightsquigarrow", !0), te(re, ie, de, "⇝", "\\leadsto"), te(re, ie, de, "⇛", "\\Rrightarrow", !0), te(re, ie, de, "↾", "\\restriction"), te(re, ae, ge, "‘", "`"), te(re, ae, ge, "$", "\\$"), te(ne, ae, ge, "$", "\\$"), te(ne, ae, ge, "$", "\\textdollar"), te(re, ae, ge, "%", "\\%"), te(ne, ae, ge, "%", "\\%"), te(re, ae, ge, "_", "\\_"), te(ne, ae, ge, "_", "\\_"), te(ne, ae, ge, "_", "\\textunderscore"), te(re, ae, ge, "∠", "\\angle", !0), te(re, ae, ge, "∞", "\\infty", !0), te(re, ae, ge, "′", "\\prime"), te(re, ae, ge, "△", "\\triangle"), te(re, ae, ge, "Γ", "\\Gamma", !0), te(re, ae, ge, "Δ", "\\Delta", !0), te(re, ae, ge, "Θ", "\\Theta", !0), te(re, ae, ge, "Λ", "\\Lambda", !0), te(re, ae, ge, "Ξ", "\\Xi", !0), te(re, ae, ge, "Π", "\\Pi", !0), te(re, ae, ge, "Σ", "\\Sigma", !0), te(re, ae, ge, "Υ", "\\Upsilon", !0), te(re, ae, ge, "Φ", "\\Phi", !0), te(re, ae, ge, "Ψ", "\\Psi", !0), te(re, ae, ge, "Ω", "\\Omega", !0), te(re, ae, ge, "A", "Α"), te(re, ae, ge, "B", "Β"), te(re, ae, ge, "E", "Ε"), te(re, ae, ge, "Z", "Ζ"), te(re, ae, ge, "H", "Η"), te(re, ae, ge, "I", "Ι"), te(re, ae, ge, "K", "Κ"), te(re, ae, ge, "M", "Μ"), te(re, ae, ge, "N", "Ν"), te(re, ae, ge, "O", "Ο"), te(re, ae, ge, "P", "Ρ"), te(re, ae, ge, "T", "Τ"), te(re, ae, ge, "X", "Χ"), te(re, ae, ge, "¬", "\\neg", !0), te(re, ae, ge, "¬", "\\lnot"), te(re, ae, ge, "⊤", "\\top"), te(re, ae, ge, "⊥", "\\bot"), te(re, ae, ge, "∅", "\\emptyset"), te(re, ie, ge, "∅", "\\varnothing"), te(re, ae, me, "α", "\\alpha", !0), te(re, ae, me, "β", "\\beta", !0), te(re, ae, me, "γ", "\\gamma", !0), te(re, ae, me, "δ", "\\delta", !0), te(re, ae, me, "ϵ", "\\epsilon", !0), te(re, ae, me, "ζ", "\\zeta", !0), te(re, ae, me, "η", "\\eta", !0), te(re, ae, me, "θ", "\\theta", !0), te(re, ae, me, "ι", "\\iota", !0), te(re, ae, me, "κ", "\\kappa", !0), te(re, ae, me, "λ", "\\lambda", !0), te(re, ae, me, "μ", "\\mu", !0), te(re, ae, me, "ν", "\\nu", !0), te(re, ae, me, "ξ", "\\xi", !0), te(re, ae, me, "ο", "\\omicron", !0), te(re, ae, me, "π", "\\pi", !0), te(re, ae, me, "ρ", "\\rho", !0), te(re, ae, me, "σ", "\\sigma", !0), te(re, ae, me, "τ", "\\tau", !0), te(re, ae, me, "υ", "\\upsilon", !0), te(re, ae, me, "ϕ", "\\phi", !0), te(re, ae, me, "χ", "\\chi", !0), te(re, ae, me, "ψ", "\\psi", !0), te(re, ae, me, "ω", "\\omega", !0), te(re, ae, me, "ε", "\\varepsilon", !0), te(re, ae, me, "ϑ", "\\vartheta", !0), te(re, ae, me, "ϖ", "\\varpi", !0), te(re, ae, me, "ϱ", "\\varrho", !0), te(re, ae, me, "ς", "\\varsigma", !0), te(re, ae, me, "φ", "\\varphi", !0), te(re, ae, se, "∗", "*"), te(re, ae, se, "+", "+"), te(re, ae, se, "−", "-"), te(re, ae, se, "⋅", "\\cdot", !0), te(re, ae, se, "∘", "\\circ"), te(re, ae, se, "÷", "\\div", !0), te(re, ae, se, "±", "\\pm", !0), te(re, ae, se, "×", "\\times", !0), te(re, ae, se, "∩", "\\cap", !0), te(re, ae, se, "∪", "\\cup", !0), te(re, ae, se, "∖", "\\setminus"), te(re, ae, se, "∧", "\\land"), te(re, ae, se, "∨", "\\lor"), te(re, ae, se, "∧", "\\wedge", !0), te(re, ae, se, "∨", "\\vee", !0), te(re, ae, ge, "√", "\\surd"), te(re, ae, ue, "⟨", "\\langle", !0), te(re, ae, ue, "∣", "\\lvert"), te(re, ae, ue, "∥", "\\lVert"), te(re, ae, le, "?", "?"), te(re, ae, le, "!", "!"), te(re, ae, le, "⟩", "\\rangle", !0), te(re, ae, le, "∣", "\\rvert"), te(re, ae, le, "∥", "\\rVert"), te(re, ae, de, "=", "="), te(re, ae, de, ":", ":"), te(re, ae, de, "≈", "\\approx", !0), te(re, ae, de, "≅", "\\cong", !0), te(re, ae, de, "≥", "\\ge"), te(re, ae, de, "≥", "\\geq", !0), te(re, ae, de, "←", "\\gets"), te(re, ae, de, ">", "\\gt", !0), te(re, ae, de, "∈", "\\in", !0), te(re, ae, de, "", "\\@not"), te(re, ae, de, "⊂", "\\subset", !0), te(re, ae, de, "⊃", "\\supset", !0), te(re, ae, de, "⊆", "\\subseteq", !0), te(re, ae, de, "⊇", "\\supseteq", !0), te(re, ie, de, "⊈", "\\nsubseteq", !0), te(re, ie, de, "⊉", "\\nsupseteq", !0), te(re, ae, de, "⊨", "\\models"), te(re, ae, de, "←", "\\leftarrow", !0), te(re, ae, de, "≤", "\\le"), te(re, ae, de, "≤", "\\leq", !0), te(re, ae, de, "<", "\\lt", !0), te(re, ae, de, "→", "\\rightarrow", !0), te(re, ae, de, "→", "\\to"), te(re, ie, de, "≱", "\\ngeq", !0), te(re, ie, de, "≰", "\\nleq", !0), te(re, ae, fe, " ", "\\ "), te(re, ae, fe, " ", "~"), te(re, ae, fe, " ", "\\space"), te(re, ae, fe, " ", "\\nobreakspace"), te(ne, ae, fe, " ", "\\ "), te(ne, ae, fe, " ", " "), te(ne, ae, fe, " ", "~"), te(ne, ae, fe, " ", "\\space"), te(ne, ae, fe, " ", "\\nobreakspace"), te(re, ae, fe, null, "\\nobreak"), te(re, ae, fe, null, "\\allowbreak"), te(re, ae, pe, ",", ","), te(re, ae, pe, ";", ";"), te(re, ie, se, "⊼", "\\barwedge", !0), te(re, ie, se, "⊻", "\\veebar", !0), te(re, ae, se, "⊙", "\\odot", !0), te(re, ae, se, "⊕", "\\oplus", !0), te(re, ae, se, "⊗", "\\otimes", !0), te(re, ae, ge, "∂", "\\partial", !0), te(re, ae, se, "⊘", "\\oslash", !0), te(re, ie, se, "⊚", "\\circledcirc", !0), te(re, ie, se, "⊡", "\\boxdot", !0), te(re, ae, se, "△", "\\bigtriangleup"), te(re, ae, se, "▽", "\\bigtriangledown"), te(re, ae, se, "†", "\\dagger"), te(re, ae, se, "⋄", "\\diamond"), te(re, ae, se, "⋆", "\\star"), te(re, ae, se, "◃", "\\triangleleft"), te(re, ae, se, "▹", "\\triangleright"), te(re, ae, ue, "{", "\\{"), te(ne, ae, ge, "{", "\\{"), te(ne, ae, ge, "{", "\\textbraceleft"), te(re, ae, le, "}", "\\}"), te(ne, ae, ge, "}", "\\}"), te(ne, ae, ge, "}", "\\textbraceright"), te(re, ae, ue, "{", "\\lbrace"), te(re, ae, le, "}", "\\rbrace"), te(re, ae, ue, "[", "\\lbrack", !0), te(ne, ae, ge, "[", "\\lbrack", !0), te(re, ae, le, "]", "\\rbrack", !0), te(ne, ae, ge, "]", "\\rbrack", !0), te(re, ae, ue, "(", "\\lparen", !0), te(re, ae, le, ")", "\\rparen", !0), te(ne, ae, ge, "<", "\\textless", !0), te(ne, ae, ge, ">", "\\textgreater", !0), te(re, ae, ue, "⌊", "\\lfloor", !0), te(re, ae, le, "⌋", "\\rfloor", !0), te(re, ae, ue, "⌈", "\\lceil", !0), te(re, ae, le, "⌉", "\\rceil", !0), te(re, ae, ge, "\\", "\\backslash"), te(re, ae, ge, "∣", "|"), te(re, ae, ge, "∣", "\\vert"), te(ne, ae, ge, "|", "\\textbar", !0), te(re, ae, ge, "∥", "\\|"), te(re, ae, ge, "∥", "\\Vert"), te(ne, ae, ge, "∥", "\\textbardbl"), te(ne, ae, ge, "~", "\\textasciitilde"), te(ne, ae, ge, "\\", "\\textbackslash"), te(ne, ae, ge, "^", "\\textasciicircum"), te(re, ae, de, "↑", "\\uparrow", !0), te(re, ae, de, "⇑", "\\Uparrow", !0), te(re, ae, de, "↓", "\\downarrow", !0), te(re, ae, de, "⇓", "\\Downarrow", !0), te(re, ae, de, "↕", "\\updownarrow", !0), te(re, ae, de, "⇕", "\\Updownarrow", !0), te(re, ae, ce, "∐", "\\coprod"), te(re, ae, ce, "⋁", "\\bigvee"), te(re, ae, ce, "⋀", "\\bigwedge"), te(re, ae, ce, "⨄", "\\biguplus"), te(re, ae, ce, "⋂", "\\bigcap"), te(re, ae, ce, "⋃", "\\bigcup"), te(re, ae, ce, "∫", "\\int"), te(re, ae, ce, "∫", "\\intop"), te(re, ae, ce, "∬", "\\iint"), te(re, ae, ce, "∭", "\\iiint"), te(re, ae, ce, "∏", "\\prod"), te(re, ae, ce, "∑", "\\sum"), te(re, ae, ce, "⨂", "\\bigotimes"), te(re, ae, ce, "⨁", "\\bigoplus"), te(re, ae, ce, "⨀", "\\bigodot"), te(re, ae, ce, "∮", "\\oint"), te(re, ae, ce, "⨆", "\\bigsqcup"), te(re, ae, ce, "∫", "\\smallint"), te(ne, ae, he, "…", "\\textellipsis"), te(re, ae, he, "…", "\\mathellipsis"), te(ne, ae, he, "…", "\\ldots", !0), te(re, ae, he, "…", "\\ldots", !0), te(re, ae, he, "⋯", "\\@cdots", !0), te(re, ae, he, "⋱", "\\ddots", !0), te(re, ae, ge, "⋮", "\\varvdots"), te(re, ae, oe, "ˊ", "\\acute"), te(re, ae, oe, "ˋ", "\\grave"), te(re, ae, oe, "¨", "\\ddot"), te(re, ae, oe, "~", "\\tilde"), te(re, ae, oe, "ˉ", "\\bar"), te(re, ae, oe, "˘", "\\breve"), te(re, ae, oe, "ˇ", "\\check"), te(re, ae, oe, "^", "\\hat"), te(re, ae, oe, "⃗", "\\vec"), te(re, ae, oe, "˙", "\\dot"), te(re, ae, oe, "˚", "\\mathring"), te(re, ae, me, "", "\\@imath"), te(re, ae, me, "", "\\@jmath"), te(re, ae, ge, "ı", "ı"), te(re, ae, ge, "ȷ", "ȷ"), te(ne, ae, ge, "ı", "\\i", !0), te(ne, ae, ge, "ȷ", "\\j", !0), te(ne, ae, ge, "ß", "\\ss", !0), te(ne, ae, ge, "æ", "\\ae", !0), te(ne, ae, ge, "œ", "\\oe", !0), te(ne, ae, ge, "ø", "\\o", !0), te(ne, ae, ge, "Æ", "\\AE", !0), te(ne, ae, ge, "Œ", "\\OE", !0), te(ne, ae, ge, "Ø", "\\O", !0), te(ne, ae, oe, "ˊ", "\\'"), te(ne, ae, oe, "ˋ", "\\`"), te(ne, ae, oe, "ˆ", "\\^"), te(ne, ae, oe, "˜", "\\~"), te(ne, ae, oe, "ˉ", "\\="), te(ne, ae, oe, "˘", "\\u"), te(ne, ae, oe, "˙", "\\."), te(ne, ae, oe, "˚", "\\r"), te(ne, ae, oe, "ˇ", "\\v"), te(ne, ae, oe, "¨", '\\"'), te(ne, ae, oe, "˝", "\\H"), te(ne, ae, oe, "◯", "\\textcircled");
-                    var ve = {
+                    var Z = "math",
+                        K = "text",
+                        J = "main",
+                        Q = "ams",
+                        ee = "accent-token",
+                        te = "bin",
+                        re = "close",
+                        ne = "inner",
+                        ae = "mathord",
+                        ie = "op-token",
+                        oe = "open",
+                        se = "punct",
+                        le = "rel",
+                        he = "spacing",
+                        me = "textord";
+                    $(Z, J, le, "≡", "\\equiv", !0), $(Z, J, le, "≺", "\\prec", !0), $(Z, J, le, "≻", "\\succ", !0), $(Z, J, le, "∼", "\\sim", !0), $(Z, J, le, "⊥", "\\perp"), $(Z, J, le, "⪯", "\\preceq", !0), $(Z, J, le, "⪰", "\\succeq", !0), $(Z, J, le, "≃", "\\simeq", !0), $(Z, J, le, "∣", "\\mid", !0), $(Z, J, le, "≪", "\\ll", !0), $(Z, J, le, "≫", "\\gg", !0), $(Z, J, le, "≍", "\\asymp", !0), $(Z, J, le, "∥", "\\parallel"), $(Z, J, le, "⋈", "\\bowtie", !0), $(Z, J, le, "⌣", "\\smile", !0), $(Z, J, le, "⊑", "\\sqsubseteq", !0), $(Z, J, le, "⊒", "\\sqsupseteq", !0), $(Z, J, le, "≐", "\\doteq", !0), $(Z, J, le, "⌢", "\\frown", !0), $(Z, J, le, "∋", "\\ni", !0), $(Z, J, le, "∝", "\\propto", !0), $(Z, J, le, "⊢", "\\vdash", !0), $(Z, J, le, "⊣", "\\dashv", !0), $(Z, J, le, "∋", "\\owns"), $(Z, J, se, ".", "\\ldotp"), $(Z, J, se, "⋅", "\\cdotp"), $(Z, J, me, "#", "\\#"), $(K, J, me, "#", "\\#"), $(Z, J, me, "&", "\\&"), $(K, J, me, "&", "\\&"), $(Z, J, me, "ℵ", "\\aleph", !0), $(Z, J, me, "∀", "\\forall", !0), $(Z, J, me, "ℏ", "\\hbar", !0), $(Z, J, me, "∃", "\\exists", !0), $(Z, J, me, "∇", "\\nabla", !0), $(Z, J, me, "♭", "\\flat", !0), $(Z, J, me, "ℓ", "\\ell", !0), $(Z, J, me, "♮", "\\natural", !0), $(Z, J, me, "♣", "\\clubsuit", !0), $(Z, J, me, "℘", "\\wp", !0), $(Z, J, me, "♯", "\\sharp", !0), $(Z, J, me, "♢", "\\diamondsuit", !0), $(Z, J, me, "ℜ", "\\Re", !0), $(Z, J, me, "♡", "\\heartsuit", !0), $(Z, J, me, "ℑ", "\\Im", !0), $(Z, J, me, "♠", "\\spadesuit", !0), $(K, J, me, "§", "\\S", !0), $(K, J, me, "¶", "\\P", !0), $(Z, J, me, "†", "\\dag"), $(K, J, me, "†", "\\dag"), $(K, J, me, "†", "\\textdagger"), $(Z, J, me, "‡", "\\ddag"), $(K, J, me, "‡", "\\ddag"), $(K, J, me, "‡", "\\textdaggerdbl"), $(Z, J, re, "⎱", "\\rmoustache", !0), $(Z, J, oe, "⎰", "\\lmoustache", !0), $(Z, J, re, "⟯", "\\rgroup", !0), $(Z, J, oe, "⟮", "\\lgroup", !0), $(Z, J, te, "∓", "\\mp", !0), $(Z, J, te, "⊖", "\\ominus", !0), $(Z, J, te, "⊎", "\\uplus", !0), $(Z, J, te, "⊓", "\\sqcap", !0), $(Z, J, te, "∗", "\\ast"), $(Z, J, te, "⊔", "\\sqcup", !0), $(Z, J, te, "◯", "\\bigcirc"), $(Z, J, te, "∙", "\\bullet"), $(Z, J, te, "‡", "\\ddagger"), $(Z, J, te, "≀", "\\wr", !0), $(Z, J, te, "⨿", "\\amalg"), $(Z, J, te, "&", "\\And"), $(Z, J, le, "⟵", "\\longleftarrow", !0), $(Z, J, le, "⇐", "\\Leftarrow", !0), $(Z, J, le, "⟸", "\\Longleftarrow", !0), $(Z, J, le, "⟶", "\\longrightarrow", !0), $(Z, J, le, "⇒", "\\Rightarrow", !0), $(Z, J, le, "⟹", "\\Longrightarrow", !0), $(Z, J, le, "↔", "\\leftrightarrow", !0), $(Z, J, le, "⟷", "\\longleftrightarrow", !0), $(Z, J, le, "⇔", "\\Leftrightarrow", !0), $(Z, J, le, "⟺", "\\Longleftrightarrow", !0), $(Z, J, le, "↦", "\\mapsto", !0), $(Z, J, le, "⟼", "\\longmapsto", !0), $(Z, J, le, "↗", "\\nearrow", !0), $(Z, J, le, "↩", "\\hookleftarrow", !0), $(Z, J, le, "↪", "\\hookrightarrow", !0), $(Z, J, le, "↘", "\\searrow", !0), $(Z, J, le, "↼", "\\leftharpoonup", !0), $(Z, J, le, "⇀", "\\rightharpoonup", !0), $(Z, J, le, "↙", "\\swarrow", !0), $(Z, J, le, "↽", "\\leftharpoondown", !0), $(Z, J, le, "⇁", "\\rightharpoondown", !0), $(Z, J, le, "↖", "\\nwarrow", !0), $(Z, J, le, "⇌", "\\rightleftharpoons", !0), $(Z, Q, le, "≮", "\\nless", !0), $(Z, Q, le, "", "\\@nleqslant"), $(Z, Q, le, "", "\\@nleqq"), $(Z, Q, le, "⪇", "\\lneq", !0), $(Z, Q, le, "≨", "\\lneqq", !0), $(Z, Q, le, "", "\\@lvertneqq"), $(Z, Q, le, "⋦", "\\lnsim", !0), $(Z, Q, le, "⪉", "\\lnapprox", !0), $(Z, Q, le, "⊀", "\\nprec", !0), $(Z, Q, le, "⋠", "\\npreceq", !0), $(Z, Q, le, "⋨", "\\precnsim", !0), $(Z, Q, le, "⪹", "\\precnapprox", !0), $(Z, Q, le, "≁", "\\nsim", !0), $(Z, Q, le, "", "\\@nshortmid"), $(Z, Q, le, "∤", "\\nmid", !0), $(Z, Q, le, "⊬", "\\nvdash", !0), $(Z, Q, le, "⊭", "\\nvDash", !0), $(Z, Q, le, "⋪", "\\ntriangleleft"), $(Z, Q, le, "⋬", "\\ntrianglelefteq", !0), $(Z, Q, le, "⊊", "\\subsetneq", !0), $(Z, Q, le, "", "\\@varsubsetneq"), $(Z, Q, le, "⫋", "\\subsetneqq", !0), $(Z, Q, le, "", "\\@varsubsetneqq"), $(Z, Q, le, "≯", "\\ngtr", !0), $(Z, Q, le, "", "\\@ngeqslant"), $(Z, Q, le, "", "\\@ngeqq"), $(Z, Q, le, "⪈", "\\gneq", !0), $(Z, Q, le, "≩", "\\gneqq", !0), $(Z, Q, le, "", "\\@gvertneqq"), $(Z, Q, le, "⋧", "\\gnsim", !0), $(Z, Q, le, "⪊", "\\gnapprox", !0), $(Z, Q, le, "⊁", "\\nsucc", !0), $(Z, Q, le, "⋡", "\\nsucceq", !0), $(Z, Q, le, "⋩", "\\succnsim", !0), $(Z, Q, le, "⪺", "\\succnapprox", !0), $(Z, Q, le, "≆", "\\ncong", !0), $(Z, Q, le, "", "\\@nshortparallel"), $(Z, Q, le, "∦", "\\nparallel", !0), $(Z, Q, le, "⊯", "\\nVDash", !0), $(Z, Q, le, "⋫", "\\ntriangleright"), $(Z, Q, le, "⋭", "\\ntrianglerighteq", !0), $(Z, Q, le, "", "\\@nsupseteqq"), $(Z, Q, le, "⊋", "\\supsetneq", !0), $(Z, Q, le, "", "\\@varsupsetneq"), $(Z, Q, le, "⫌", "\\supsetneqq", !0), $(Z, Q, le, "", "\\@varsupsetneqq"), $(Z, Q, le, "⊮", "\\nVdash", !0), $(Z, Q, le, "⪵", "\\precneqq", !0), $(Z, Q, le, "⪶", "\\succneqq", !0), $(Z, Q, le, "", "\\@nsubseteqq"), $(Z, Q, te, "⊴", "\\unlhd"), $(Z, Q, te, "⊵", "\\unrhd"), $(Z, Q, le, "↚", "\\nleftarrow", !0), $(Z, Q, le, "↛", "\\nrightarrow", !0), $(Z, Q, le, "⇍", "\\nLeftarrow", !0), $(Z, Q, le, "⇏", "\\nRightarrow", !0), $(Z, Q, le, "↮", "\\nleftrightarrow", !0), $(Z, Q, le, "⇎", "\\nLeftrightarrow", !0), $(Z, Q, le, "△", "\\vartriangle"), $(Z, Q, me, "ℏ", "\\hslash"), $(Z, Q, me, "▽", "\\triangledown"), $(Z, Q, me, "◊", "\\lozenge"), $(Z, Q, me, "Ⓢ", "\\circledS"), $(Z, Q, me, "®", "\\circledR"), $(K, Q, me, "®", "\\circledR"), $(Z, Q, me, "∡", "\\measuredangle", !0), $(Z, Q, me, "∄", "\\nexists"), $(Z, Q, me, "℧", "\\mho"), $(Z, Q, me, "Ⅎ", "\\Finv", !0), $(Z, Q, me, "⅁", "\\Game", !0), $(Z, Q, me, "‵", "\\backprime"), $(Z, Q, me, "▲", "\\blacktriangle"), $(Z, Q, me, "▼", "\\blacktriangledown"), $(Z, Q, me, "■", "\\blacksquare"), $(Z, Q, me, "⧫", "\\blacklozenge"), $(Z, Q, me, "★", "\\bigstar"), $(Z, Q, me, "∢", "\\sphericalangle", !0), $(Z, Q, me, "∁", "\\complement", !0), $(Z, Q, me, "ð", "\\eth", !0), $(K, J, me, "ð", "ð"), $(Z, Q, me, "╱", "\\diagup"), $(Z, Q, me, "╲", "\\diagdown"), $(Z, Q, me, "□", "\\square"), $(Z, Q, me, "□", "\\Box"), $(Z, Q, me, "◊", "\\Diamond"), $(Z, Q, me, "¥", "\\yen", !0), $(K, Q, me, "¥", "\\yen", !0), $(Z, Q, me, "✓", "\\checkmark", !0), $(K, Q, me, "✓", "\\checkmark"), $(Z, Q, me, "ℶ", "\\beth", !0), $(Z, Q, me, "ℸ", "\\daleth", !0), $(Z, Q, me, "ℷ", "\\gimel", !0), $(Z, Q, me, "ϝ", "\\digamma", !0), $(Z, Q, me, "ϰ", "\\varkappa"), $(Z, Q, oe, "┌", "\\@ulcorner", !0), $(Z, Q, re, "┐", "\\@urcorner", !0), $(Z, Q, oe, "└", "\\@llcorner", !0), $(Z, Q, re, "┘", "\\@lrcorner", !0), $(Z, Q, le, "≦", "\\leqq", !0), $(Z, Q, le, "⩽", "\\leqslant", !0), $(Z, Q, le, "⪕", "\\eqslantless", !0), $(Z, Q, le, "≲", "\\lesssim", !0), $(Z, Q, le, "⪅", "\\lessapprox", !0), $(Z, Q, le, "≊", "\\approxeq", !0), $(Z, Q, te, "⋖", "\\lessdot"), $(Z, Q, le, "⋘", "\\lll", !0), $(Z, Q, le, "≶", "\\lessgtr", !0), $(Z, Q, le, "⋚", "\\lesseqgtr", !0), $(Z, Q, le, "⪋", "\\lesseqqgtr", !0), $(Z, Q, le, "≑", "\\doteqdot"), $(Z, Q, le, "≓", "\\risingdotseq", !0), $(Z, Q, le, "≒", "\\fallingdotseq", !0), $(Z, Q, le, "∽", "\\backsim", !0), $(Z, Q, le, "⋍", "\\backsimeq", !0), $(Z, Q, le, "⫅", "\\subseteqq", !0), $(Z, Q, le, "⋐", "\\Subset", !0), $(Z, Q, le, "⊏", "\\sqsubset", !0), $(Z, Q, le, "≼", "\\preccurlyeq", !0), $(Z, Q, le, "⋞", "\\curlyeqprec", !0), $(Z, Q, le, "≾", "\\precsim", !0), $(Z, Q, le, "⪷", "\\precapprox", !0), $(Z, Q, le, "⊲", "\\vartriangleleft"), $(Z, Q, le, "⊴", "\\trianglelefteq"), $(Z, Q, le, "⊨", "\\vDash", !0), $(Z, Q, le, "⊪", "\\Vvdash", !0), $(Z, Q, le, "⌣", "\\smallsmile"), $(Z, Q, le, "⌢", "\\smallfrown"), $(Z, Q, le, "≏", "\\bumpeq", !0), $(Z, Q, le, "≎", "\\Bumpeq", !0), $(Z, Q, le, "≧", "\\geqq", !0), $(Z, Q, le, "⩾", "\\geqslant", !0), $(Z, Q, le, "⪖", "\\eqslantgtr", !0), $(Z, Q, le, "≳", "\\gtrsim", !0), $(Z, Q, le, "⪆", "\\gtrapprox", !0), $(Z, Q, te, "⋗", "\\gtrdot"), $(Z, Q, le, "⋙", "\\ggg", !0), $(Z, Q, le, "≷", "\\gtrless", !0), $(Z, Q, le, "⋛", "\\gtreqless", !0), $(Z, Q, le, "⪌", "\\gtreqqless", !0), $(Z, Q, le, "≖", "\\eqcirc", !0), $(Z, Q, le, "≗", "\\circeq", !0), $(Z, Q, le, "≜", "\\triangleq", !0), $(Z, Q, le, "∼", "\\thicksim"), $(Z, Q, le, "≈", "\\thickapprox"), $(Z, Q, le, "⫆", "\\supseteqq", !0), $(Z, Q, le, "⋑", "\\Supset", !0), $(Z, Q, le, "⊐", "\\sqsupset", !0), $(Z, Q, le, "≽", "\\succcurlyeq", !0), $(Z, Q, le, "⋟", "\\curlyeqsucc", !0), $(Z, Q, le, "≿", "\\succsim", !0), $(Z, Q, le, "⪸", "\\succapprox", !0), $(Z, Q, le, "⊳", "\\vartriangleright"), $(Z, Q, le, "⊵", "\\trianglerighteq"), $(Z, Q, le, "⊩", "\\Vdash", !0), $(Z, Q, le, "∣", "\\shortmid"), $(Z, Q, le, "∥", "\\shortparallel"), $(Z, Q, le, "≬", "\\between", !0), $(Z, Q, le, "⋔", "\\pitchfork", !0), $(Z, Q, le, "∝", "\\varpropto"), $(Z, Q, le, "◀", "\\blacktriangleleft"), $(Z, Q, le, "∴", "\\therefore", !0), $(Z, Q, le, "∍", "\\backepsilon"), $(Z, Q, le, "▶", "\\blacktriangleright"), $(Z, Q, le, "∵", "\\because", !0), $(Z, Q, le, "⋘", "\\llless"), $(Z, Q, le, "⋙", "\\gggtr"), $(Z, Q, te, "⊲", "\\lhd"), $(Z, Q, te, "⊳", "\\rhd"), $(Z, Q, le, "≂", "\\eqsim", !0), $(Z, J, le, "⋈", "\\Join"), $(Z, Q, le, "≑", "\\Doteq", !0), $(Z, Q, te, "∔", "\\dotplus", !0), $(Z, Q, te, "∖", "\\smallsetminus"), $(Z, Q, te, "⋒", "\\Cap", !0), $(Z, Q, te, "⋓", "\\Cup", !0), $(Z, Q, te, "⩞", "\\doublebarwedge", !0), $(Z, Q, te, "⊟", "\\boxminus", !0), $(Z, Q, te, "⊞", "\\boxplus", !0), $(Z, Q, te, "⋇", "\\divideontimes", !0), $(Z, Q, te, "⋉", "\\ltimes", !0), $(Z, Q, te, "⋊", "\\rtimes", !0), $(Z, Q, te, "⋋", "\\leftthreetimes", !0), $(Z, Q, te, "⋌", "\\rightthreetimes", !0), $(Z, Q, te, "⋏", "\\curlywedge", !0), $(Z, Q, te, "⋎", "\\curlyvee", !0), $(Z, Q, te, "⊝", "\\circleddash", !0), $(Z, Q, te, "⊛", "\\circledast", !0), $(Z, Q, te, "⋅", "\\centerdot"), $(Z, Q, te, "⊺", "\\intercal", !0), $(Z, Q, te, "⋒", "\\doublecap"), $(Z, Q, te, "⋓", "\\doublecup"), $(Z, Q, te, "⊠", "\\boxtimes", !0), $(Z, Q, le, "⇢", "\\dashrightarrow", !0), $(Z, Q, le, "⇠", "\\dashleftarrow", !0), $(Z, Q, le, "⇇", "\\leftleftarrows", !0), $(Z, Q, le, "⇆", "\\leftrightarrows", !0), $(Z, Q, le, "⇚", "\\Lleftarrow", !0), $(Z, Q, le, "↞", "\\twoheadleftarrow", !0), $(Z, Q, le, "↢", "\\leftarrowtail", !0), $(Z, Q, le, "↫", "\\looparrowleft", !0), $(Z, Q, le, "⇋", "\\leftrightharpoons", !0), $(Z, Q, le, "↶", "\\curvearrowleft", !0), $(Z, Q, le, "↺", "\\circlearrowleft", !0), $(Z, Q, le, "↰", "\\Lsh", !0), $(Z, Q, le, "⇈", "\\upuparrows", !0), $(Z, Q, le, "↿", "\\upharpoonleft", !0), $(Z, Q, le, "⇃", "\\downharpoonleft", !0), $(Z, Q, le, "⊸", "\\multimap", !0), $(Z, Q, le, "↭", "\\leftrightsquigarrow", !0), $(Z, Q, le, "⇉", "\\rightrightarrows", !0), $(Z, Q, le, "⇄", "\\rightleftarrows", !0), $(Z, Q, le, "↠", "\\twoheadrightarrow", !0), $(Z, Q, le, "↣", "\\rightarrowtail", !0), $(Z, Q, le, "↬", "\\looparrowright", !0), $(Z, Q, le, "↷", "\\curvearrowright", !0), $(Z, Q, le, "↻", "\\circlearrowright", !0), $(Z, Q, le, "↱", "\\Rsh", !0), $(Z, Q, le, "⇊", "\\downdownarrows", !0), $(Z, Q, le, "↾", "\\upharpoonright", !0), $(Z, Q, le, "⇂", "\\downharpoonright", !0), $(Z, Q, le, "⇝", "\\rightsquigarrow", !0), $(Z, Q, le, "⇝", "\\leadsto"), $(Z, Q, le, "⇛", "\\Rrightarrow", !0), $(Z, Q, le, "↾", "\\restriction"), $(Z, J, me, "‘", "`"), $(Z, J, me, "$", "\\$"), $(K, J, me, "$", "\\$"), $(K, J, me, "$", "\\textdollar"), $(Z, J, me, "%", "\\%"), $(K, J, me, "%", "\\%"), $(Z, J, me, "_", "\\_"), $(K, J, me, "_", "\\_"), $(K, J, me, "_", "\\textunderscore"), $(Z, J, me, "∠", "\\angle", !0), $(Z, J, me, "∞", "\\infty", !0), $(Z, J, me, "′", "\\prime"), $(Z, J, me, "△", "\\triangle"), $(Z, J, me, "Γ", "\\Gamma", !0), $(Z, J, me, "Δ", "\\Delta", !0), $(Z, J, me, "Θ", "\\Theta", !0), $(Z, J, me, "Λ", "\\Lambda", !0), $(Z, J, me, "Ξ", "\\Xi", !0), $(Z, J, me, "Π", "\\Pi", !0), $(Z, J, me, "Σ", "\\Sigma", !0), $(Z, J, me, "Υ", "\\Upsilon", !0), $(Z, J, me, "Φ", "\\Phi", !0), $(Z, J, me, "Ψ", "\\Psi", !0), $(Z, J, me, "Ω", "\\Omega", !0), $(Z, J, me, "A", "Α"), $(Z, J, me, "B", "Β"), $(Z, J, me, "E", "Ε"), $(Z, J, me, "Z", "Ζ"), $(Z, J, me, "H", "Η"), $(Z, J, me, "I", "Ι"), $(Z, J, me, "K", "Κ"), $(Z, J, me, "M", "Μ"), $(Z, J, me, "N", "Ν"), $(Z, J, me, "O", "Ο"), $(Z, J, me, "P", "Ρ"), $(Z, J, me, "T", "Τ"), $(Z, J, me, "X", "Χ"), $(Z, J, me, "¬", "\\neg", !0), $(Z, J, me, "¬", "\\lnot"), $(Z, J, me, "⊤", "\\top"), $(Z, J, me, "⊥", "\\bot"), $(Z, J, me, "∅", "\\emptyset"), $(Z, Q, me, "∅", "\\varnothing"), $(Z, J, ae, "α", "\\alpha", !0), $(Z, J, ae, "β", "\\beta", !0), $(Z, J, ae, "γ", "\\gamma", !0), $(Z, J, ae, "δ", "\\delta", !0), $(Z, J, ae, "ϵ", "\\epsilon", !0), $(Z, J, ae, "ζ", "\\zeta", !0), $(Z, J, ae, "η", "\\eta", !0), $(Z, J, ae, "θ", "\\theta", !0), $(Z, J, ae, "ι", "\\iota", !0), $(Z, J, ae, "κ", "\\kappa", !0), $(Z, J, ae, "λ", "\\lambda", !0), $(Z, J, ae, "μ", "\\mu", !0), $(Z, J, ae, "ν", "\\nu", !0), $(Z, J, ae, "ξ", "\\xi", !0), $(Z, J, ae, "ο", "\\omicron", !0), $(Z, J, ae, "π", "\\pi", !0), $(Z, J, ae, "ρ", "\\rho", !0), $(Z, J, ae, "σ", "\\sigma", !0), $(Z, J, ae, "τ", "\\tau", !0), $(Z, J, ae, "υ", "\\upsilon", !0), $(Z, J, ae, "ϕ", "\\phi", !0), $(Z, J, ae, "χ", "\\chi", !0), $(Z, J, ae, "ψ", "\\psi", !0), $(Z, J, ae, "ω", "\\omega", !0), $(Z, J, ae, "ε", "\\varepsilon", !0), $(Z, J, ae, "ϑ", "\\vartheta", !0), $(Z, J, ae, "ϖ", "\\varpi", !0), $(Z, J, ae, "ϱ", "\\varrho", !0), $(Z, J, ae, "ς", "\\varsigma", !0), $(Z, J, ae, "φ", "\\varphi", !0), $(Z, J, te, "∗", "*"), $(Z, J, te, "+", "+"), $(Z, J, te, "−", "-"), $(Z, J, te, "⋅", "\\cdot", !0), $(Z, J, te, "∘", "\\circ"), $(Z, J, te, "÷", "\\div", !0), $(Z, J, te, "±", "\\pm", !0), $(Z, J, te, "×", "\\times", !0), $(Z, J, te, "∩", "\\cap", !0), $(Z, J, te, "∪", "\\cup", !0), $(Z, J, te, "∖", "\\setminus"), $(Z, J, te, "∧", "\\land"), $(Z, J, te, "∨", "\\lor"), $(Z, J, te, "∧", "\\wedge", !0), $(Z, J, te, "∨", "\\vee", !0), $(Z, J, me, "√", "\\surd"), $(Z, J, oe, "⟨", "\\langle", !0), $(Z, J, oe, "∣", "\\lvert"), $(Z, J, oe, "∥", "\\lVert"), $(Z, J, re, "?", "?"), $(Z, J, re, "!", "!"), $(Z, J, re, "⟩", "\\rangle", !0), $(Z, J, re, "∣", "\\rvert"), $(Z, J, re, "∥", "\\rVert"), $(Z, J, le, "=", "="), $(Z, J, le, ":", ":"), $(Z, J, le, "≈", "\\approx", !0), $(Z, J, le, "≅", "\\cong", !0), $(Z, J, le, "≥", "\\ge"), $(Z, J, le, "≥", "\\geq", !0), $(Z, J, le, "←", "\\gets"), $(Z, J, le, ">", "\\gt", !0), $(Z, J, le, "∈", "\\in", !0), $(Z, J, le, "", "\\@not"), $(Z, J, le, "⊂", "\\subset", !0), $(Z, J, le, "⊃", "\\supset", !0), $(Z, J, le, "⊆", "\\subseteq", !0), $(Z, J, le, "⊇", "\\supseteq", !0), $(Z, Q, le, "⊈", "\\nsubseteq", !0), $(Z, Q, le, "⊉", "\\nsupseteq", !0), $(Z, J, le, "⊨", "\\models"), $(Z, J, le, "←", "\\leftarrow", !0), $(Z, J, le, "≤", "\\le"), $(Z, J, le, "≤", "\\leq", !0), $(Z, J, le, "<", "\\lt", !0), $(Z, J, le, "→", "\\rightarrow", !0), $(Z, J, le, "→", "\\to"), $(Z, Q, le, "≱", "\\ngeq", !0), $(Z, Q, le, "≰", "\\nleq", !0), $(Z, J, he, " ", "\\ "), $(Z, J, he, " ", "~"), $(Z, J, he, " ", "\\space"), $(Z, J, he, " ", "\\nobreakspace"), $(K, J, he, " ", "\\ "), $(K, J, he, " ", " "), $(K, J, he, " ", "~"), $(K, J, he, " ", "\\space"), $(K, J, he, " ", "\\nobreakspace"), $(Z, J, he, null, "\\nobreak"), $(Z, J, he, null, "\\allowbreak"), $(Z, J, se, ",", ","), $(Z, J, se, ";", ";"), $(Z, Q, te, "⊼", "\\barwedge", !0), $(Z, Q, te, "⊻", "\\veebar", !0), $(Z, J, te, "⊙", "\\odot", !0), $(Z, J, te, "⊕", "\\oplus", !0), $(Z, J, te, "⊗", "\\otimes", !0), $(Z, J, me, "∂", "\\partial", !0), $(Z, J, te, "⊘", "\\oslash", !0), $(Z, Q, te, "⊚", "\\circledcirc", !0), $(Z, Q, te, "⊡", "\\boxdot", !0), $(Z, J, te, "△", "\\bigtriangleup"), $(Z, J, te, "▽", "\\bigtriangledown"), $(Z, J, te, "†", "\\dagger"), $(Z, J, te, "⋄", "\\diamond"), $(Z, J, te, "⋆", "\\star"), $(Z, J, te, "◃", "\\triangleleft"), $(Z, J, te, "▹", "\\triangleright"), $(Z, J, oe, "{", "\\{"), $(K, J, me, "{", "\\{"), $(K, J, me, "{", "\\textbraceleft"), $(Z, J, re, "}", "\\}"), $(K, J, me, "}", "\\}"), $(K, J, me, "}", "\\textbraceright"), $(Z, J, oe, "{", "\\lbrace"), $(Z, J, re, "}", "\\rbrace"), $(Z, J, oe, "[", "\\lbrack", !0), $(K, J, me, "[", "\\lbrack", !0), $(Z, J, re, "]", "\\rbrack", !0), $(K, J, me, "]", "\\rbrack", !0), $(Z, J, oe, "(", "\\lparen", !0), $(Z, J, re, ")", "\\rparen", !0), $(K, J, me, "<", "\\textless", !0), $(K, J, me, ">", "\\textgreater", !0), $(Z, J, oe, "⌊", "\\lfloor", !0), $(Z, J, re, "⌋", "\\rfloor", !0), $(Z, J, oe, "⌈", "\\lceil", !0), $(Z, J, re, "⌉", "\\rceil", !0), $(Z, J, me, "\\", "\\backslash"), $(Z, J, me, "∣", "|"), $(Z, J, me, "∣", "\\vert"), $(K, J, me, "|", "\\textbar", !0), $(Z, J, me, "∥", "\\|"), $(Z, J, me, "∥", "\\Vert"), $(K, J, me, "∥", "\\textbardbl"), $(K, J, me, "~", "\\textasciitilde"), $(K, J, me, "\\", "\\textbackslash"), $(K, J, me, "^", "\\textasciicircum"), $(Z, J, le, "↑", "\\uparrow", !0), $(Z, J, le, "⇑", "\\Uparrow", !0), $(Z, J, le, "↓", "\\downarrow", !0), $(Z, J, le, "⇓", "\\Downarrow", !0), $(Z, J, le, "↕", "\\updownarrow", !0), $(Z, J, le, "⇕", "\\Updownarrow", !0), $(Z, J, ie, "∐", "\\coprod"), $(Z, J, ie, "⋁", "\\bigvee"), $(Z, J, ie, "⋀", "\\bigwedge"), $(Z, J, ie, "⨄", "\\biguplus"), $(Z, J, ie, "⋂", "\\bigcap"), $(Z, J, ie, "⋃", "\\bigcup"), $(Z, J, ie, "∫", "\\int"), $(Z, J, ie, "∫", "\\intop"), $(Z, J, ie, "∬", "\\iint"), $(Z, J, ie, "∭", "\\iiint"), $(Z, J, ie, "∏", "\\prod"), $(Z, J, ie, "∑", "\\sum"), $(Z, J, ie, "⨂", "\\bigotimes"), $(Z, J, ie, "⨁", "\\bigoplus"), $(Z, J, ie, "⨀", "\\bigodot"), $(Z, J, ie, "∮", "\\oint"), $(Z, J, ie, "⨆", "\\bigsqcup"), $(Z, J, ie, "∫", "\\smallint"), $(K, J, ne, "…", "\\textellipsis"), $(Z, J, ne, "…", "\\mathellipsis"), $(K, J, ne, "…", "\\ldots", !0), $(Z, J, ne, "…", "\\ldots", !0), $(Z, J, ne, "⋯", "\\@cdots", !0), $(Z, J, ne, "⋱", "\\ddots", !0), $(Z, J, me, "⋮", "\\varvdots"), $(Z, J, ee, "ˊ", "\\acute"), $(Z, J, ee, "ˋ", "\\grave"), $(Z, J, ee, "¨", "\\ddot"), $(Z, J, ee, "~", "\\tilde"), $(Z, J, ee, "ˉ", "\\bar"), $(Z, J, ee, "˘", "\\breve"), $(Z, J, ee, "ˇ", "\\check"), $(Z, J, ee, "^", "\\hat"), $(Z, J, ee, "⃗", "\\vec"), $(Z, J, ee, "˙", "\\dot"), $(Z, J, ee, "˚", "\\mathring"), $(Z, J, ae, "", "\\@imath"), $(Z, J, ae, "", "\\@jmath"), $(Z, J, me, "ı", "ı"), $(Z, J, me, "ȷ", "ȷ"), $(K, J, me, "ı", "\\i", !0), $(K, J, me, "ȷ", "\\j", !0), $(K, J, me, "ß", "\\ss", !0), $(K, J, me, "æ", "\\ae", !0), $(K, J, me, "œ", "\\oe", !0), $(K, J, me, "ø", "\\o", !0), $(K, J, me, "Æ", "\\AE", !0), $(K, J, me, "Œ", "\\OE", !0), $(K, J, me, "Ø", "\\O", !0), $(K, J, ee, "ˊ", "\\'"), $(K, J, ee, "ˋ", "\\`"), $(K, J, ee, "ˆ", "\\^"), $(K, J, ee, "˜", "\\~"), $(K, J, ee, "ˉ", "\\="), $(K, J, ee, "˘", "\\u"), $(K, J, ee, "˙", "\\."), $(K, J, ee, "˚", "\\r"), $(K, J, ee, "ˇ", "\\v"), $(K, J, ee, "¨", '\\"'), $(K, J, ee, "˝", "\\H"), $(K, J, ee, "◯", "\\textcircled");
+                    var ce = {
                         "--": !0,
                         "---": !0,
                         "``": !0,
                         "''": !0
                     };
-                    te(ne, ae, ge, "–", "--", !0), te(ne, ae, ge, "–", "\\textendash"), te(ne, ae, ge, "—", "---", !0), te(ne, ae, ge, "—", "\\textemdash"), te(ne, ae, ge, "‘", "`", !0), te(ne, ae, ge, "‘", "\\textquoteleft"), te(ne, ae, ge, "’", "'", !0), te(ne, ae, ge, "’", "\\textquoteright"), te(ne, ae, ge, "“", "``", !0), te(ne, ae, ge, "“", "\\textquotedblleft"), te(ne, ae, ge, "”", "''", !0), te(ne, ae, ge, "”", "\\textquotedblright"), te(re, ae, ge, "°", "\\degree", !0), te(ne, ae, ge, "°", "\\degree"), te(ne, ae, ge, "°", "\\textdegree", !0), te(re, ae, ge, "£", "\\pounds"), te(re, ae, ge, "£", "\\mathsterling", !0), te(ne, ae, ge, "£", "\\pounds"), te(ne, ae, ge, "£", "\\textsterling", !0), te(re, ie, ge, "✠", "\\maltese"), te(ne, ie, ge, "✠", "\\maltese");
-                    for (var be = '0123456789/@."', ye = 0; ye < be.length; ye++) {
-                        var xe = be.charAt(ye);
-                        te(re, ae, ge, xe, xe)
+                    $(K, J, me, "–", "--", !0), $(K, J, me, "–", "\\textendash"), $(K, J, me, "—", "---", !0), $(K, J, me, "—", "\\textemdash"), $(K, J, me, "‘", "`", !0), $(K, J, me, "‘", "\\textquoteleft"), $(K, J, me, "’", "'", !0), $(K, J, me, "’", "\\textquoteright"), $(K, J, me, "“", "``", !0), $(K, J, me, "“", "\\textquotedblleft"), $(K, J, me, "”", "''", !0), $(K, J, me, "”", "\\textquotedblright"), $(Z, J, me, "°", "\\degree", !0), $(K, J, me, "°", "\\degree"), $(K, J, me, "°", "\\textdegree", !0), $(Z, J, me, "£", "\\pounds"), $(Z, J, me, "£", "\\mathsterling", !0), $(K, J, me, "£", "\\pounds"), $(K, J, me, "£", "\\textsterling", !0), $(Z, Q, me, "✠", "\\maltese"), $(K, Q, me, "✠", "\\maltese");
+                    for (var ue = '0123456789/@."', pe = 0; pe < ue.length; pe++) {
+                        var de = ue.charAt(pe);
+                        $(Z, J, me, de, de)
                     }
-                    for (var we = '0123456789!@*()-=+";:?/.,', ke = 0; ke < we.length; ke++) {
-                        var Se = we.charAt(ke);
-                        te(ne, ae, ge, Se, Se)
+                    for (var fe = '0123456789!@*()-=+";:?/.,', ge = 0; ge < fe.length; ge++) {
+                        var ve = fe.charAt(ge);
+                        $(K, J, me, ve, ve)
                     }
-                    for (var Me = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz", ze = 0; ze < Me.length; ze++) {
-                        var Ae = Me.charAt(ze);
-                        te(re, ae, me, Ae, Ae), te(ne, ae, ge, Ae, Ae)
+                    for (var be = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz", ye = 0; ye < be.length; ye++) {
+                        var xe = be.charAt(ye);
+                        $(Z, J, ae, xe, xe), $(K, J, me, xe, xe)
                     }
-                    te(re, ie, ge, "C", "ℂ"), te(ne, ie, ge, "C", "ℂ"), te(re, ie, ge, "H", "ℍ"), te(ne, ie, ge, "H", "ℍ"), te(re, ie, ge, "N", "ℕ"), te(ne, ie, ge, "N", "ℕ"), te(re, ie, ge, "P", "ℙ"), te(ne, ie, ge, "P", "ℙ"), te(re, ie, ge, "Q", "ℚ"), te(ne, ie, ge, "Q", "ℚ"), te(re, ie, ge, "R", "ℝ"), te(ne, ie, ge, "R", "ℝ"), te(re, ie, ge, "Z", "ℤ"), te(ne, ie, ge, "Z", "ℤ"), te(re, ae, me, "h", "ℎ"), te(ne, ae, me, "h", "ℎ");
-                    for (var Te = "", Be = 0; Be < Me.length; Be++) {
-                        var Ce = Me.charAt(Be);
-                        te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56320 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56372 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56424 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56580 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56736 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56788 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56840 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56944 + Be)), te(ne, ae, ge, Ce, Te), Be < 26 && (te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56632 + Be)), te(ne, ae, ge, Ce, Te), te(re, ae, me, Ce, Te = String.fromCharCode(55349, 56476 + Be)), te(ne, ae, ge, Ce, Te))
+                    $(Z, Q, me, "C", "ℂ"), $(K, Q, me, "C", "ℂ"), $(Z, Q, me, "H", "ℍ"), $(K, Q, me, "H", "ℍ"), $(Z, Q, me, "N", "ℕ"), $(K, Q, me, "N", "ℕ"), $(Z, Q, me, "P", "ℙ"), $(K, Q, me, "P", "ℙ"), $(Z, Q, me, "Q", "ℚ"), $(K, Q, me, "Q", "ℚ"), $(Z, Q, me, "R", "ℝ"), $(K, Q, me, "R", "ℝ"), $(Z, Q, me, "Z", "ℤ"), $(K, Q, me, "Z", "ℤ"), $(Z, J, ae, "h", "ℎ"), $(K, J, ae, "h", "ℎ");
+                    for (var we = "", ke = 0; ke < be.length; ke++) {
+                        var Se = be.charAt(ke);
+                        $(Z, J, ae, Se, we = String.fromCharCode(55349, 56320 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56372 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56424 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56580 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56736 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56788 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56840 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56944 + ke)), $(K, J, me, Se, we), ke < 26 && ($(Z, J, ae, Se, we = String.fromCharCode(55349, 56632 + ke)), $(K, J, me, Se, we), $(Z, J, ae, Se, we = String.fromCharCode(55349, 56476 + ke)), $(K, J, me, Se, we))
                     }
-                    te(re, ae, me, "k", Te = String.fromCharCode(55349, 56668)), te(ne, ae, ge, "k", Te);
-                    for (var qe = 0; qe < 10; qe++) {
-                        var Ne = qe.toString();
-                        te(re, ae, me, Ne, Te = String.fromCharCode(55349, 57294 + qe)), te(ne, ae, ge, Ne, Te), te(re, ae, me, Ne, Te = String.fromCharCode(55349, 57314 + qe)), te(ne, ae, ge, Ne, Te), te(re, ae, me, Ne, Te = String.fromCharCode(55349, 57324 + qe)), te(ne, ae, ge, Ne, Te), te(re, ae, me, Ne, Te = String.fromCharCode(55349, 57334 + qe)), te(ne, ae, ge, Ne, Te)
+                    $(Z, J, ae, "k", we = String.fromCharCode(55349, 56668)), $(K, J, me, "k", we);
+                    for (var Me = 0; Me < 10; Me++) {
+                        var ze = Me.toString();
+                        $(Z, J, ae, ze, we = String.fromCharCode(55349, 57294 + Me)), $(K, J, me, ze, we), $(Z, J, ae, ze, we = String.fromCharCode(55349, 57314 + Me)), $(K, J, me, ze, we), $(Z, J, ae, ze, we = String.fromCharCode(55349, 57324 + Me)), $(K, J, me, ze, we), $(Z, J, ae, ze, we = String.fromCharCode(55349, 57334 + Me)), $(K, J, me, ze, we)
                     }
-                    for (var Ie = "ÇÐÞçþ", Oe = 0; Oe < Ie.length; Oe++) {
-                        var Re = Ie.charAt(Oe);
-                        te(re, ae, me, Re, Re), te(ne, ae, ge, Re, Re)
+                    for (var Ae = "ÇÐÞçþ", Te = 0; Te < Ae.length; Te++) {
+                        var Be = Ae.charAt(Te);
+                        $(Z, J, ae, Be, Be), $(K, J, me, Be, Be)
                     }
-                    var Ee = [
+                    var Ce = [
                             ["mathbf", "textbf", "Main-Bold"],
                             ["mathbf", "textbf", "Main-Bold"],
                             ["mathnormal", "textit", "Math-Italic"],
                             ["mathnormal", "textit", "Math-Italic"],
                             ["boldsymbol", "boldsymbol", "Main-BoldItalic"],
                             ["boldsymbol", "boldsymbol", "Main-BoldItalic"],
                             ["mathscr", "textscr", "Script-Regular"],
@@ -2767,41 +2769,41 @@
                             ["mathitsf", "textitsf", "SansSerif-Italic"],
                             ["mathitsf", "textitsf", "SansSerif-Italic"],
                             ["", "", ""],
                             ["", "", ""],
                             ["mathtt", "texttt", "Typewriter-Regular"],
                             ["mathtt", "texttt", "Typewriter-Regular"]
                         ],
-                        Le = [
+                        qe = [
                             ["mathbf", "textbf", "Main-Bold"],
                             ["", "", ""],
                             ["mathsf", "textsf", "SansSerif-Regular"],
                             ["mathboldsf", "textboldsf", "SansSerif-Bold"],
                             ["mathtt", "texttt", "Typewriter-Regular"]
                         ],
-                        Pe = [
+                        Ne = [
                             [1, 1, 1],
                             [2, 1, 1],
                             [3, 1, 1],
                             [4, 2, 1],
                             [5, 2, 1],
                             [6, 3, 1],
                             [7, 4, 2],
                             [8, 6, 3],
                             [9, 7, 6],
                             [10, 8, 7],
                             [11, 10, 9]
                         ],
-                        De = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
-                        He = function(e, t) {
-                            return t.size < 2 ? e : Pe[e - 1][t.size - 1]
+                        Ie = [.5, .6, .7, .8, .9, 1, 1.2, 1.44, 1.728, 2.074, 2.488],
+                        Oe = function(e, t) {
+                            return t.size < 2 ? e : Ne[e - 1][t.size - 1]
                         },
-                        Fe = function() {
+                        Re = function() {
                             function e(t) {
-                                this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || e.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = De[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
+                                this.style = void 0, this.color = void 0, this.size = void 0, this.textSize = void 0, this.phantom = void 0, this.font = void 0, this.fontFamily = void 0, this.fontWeight = void 0, this.fontShape = void 0, this.sizeMultiplier = void 0, this.maxSize = void 0, this.minRuleThickness = void 0, this._fontMetrics = void 0, this.style = t.style, this.color = t.color, this.size = t.size || e.BASESIZE, this.textSize = t.textSize || this.size, this.phantom = !!t.phantom, this.font = t.font || "", this.fontFamily = t.fontFamily || "", this.fontWeight = t.fontWeight || "", this.fontShape = t.fontShape || "", this.sizeMultiplier = Ie[this.size - 1], this.maxSize = t.maxSize, this.minRuleThickness = t.minRuleThickness, this._fontMetrics = void 0
                             }
                             var t = e.prototype;
                             return t.extend = function(t) {
                                 var r = {
                                     style: this.style,
                                     size: this.size,
                                     textSize: this.textSize,
@@ -2815,28 +2817,28 @@
                                     minRuleThickness: this.minRuleThickness
                                 };
                                 for (var n in t) t.hasOwnProperty(n) && (r[n] = t[n]);
                                 return new e(r)
                             }, t.havingStyle = function(e) {
                                 return this.style === e ? this : this.extend({
                                     style: e,
-                                    size: He(this.textSize, e)
+                                    size: Oe(this.textSize, e)
                                 })
                             }, t.havingCrampedStyle = function() {
                                 return this.havingStyle(this.style.cramp())
                             }, t.havingSize = function(e) {
                                 return this.size === e && this.textSize === e ? this : this.extend({
                                     style: this.style.text(),
                                     size: e,
                                     textSize: e,
-                                    sizeMultiplier: De[e - 1]
+                                    sizeMultiplier: Ie[e - 1]
                                 })
                             }, t.havingBaseStyle = function(t) {
                                 t = t || this.style.text();
-                                var r = He(e.BASESIZE, t);
+                                var r = Oe(e.BASESIZE, t);
                                 return this.size === r && this.textSize === e.BASESIZE && this.style === t ? this : this.extend({
                                     style: t,
                                     size: r
                                 })
                             }, t.havingBaseSizing = function() {
                                 var e;
                                 switch (this.style.id) {
@@ -2885,112 +2887,112 @@
                             }, t.sizingClasses = function(e) {
                                 return e.size !== this.size ? ["sizing", "reset-size" + e.size, "size" + this.size] : []
                             }, t.baseSizingClasses = function() {
                                 return this.size !== e.BASESIZE ? ["sizing", "reset-size" + this.size, "size" + e.BASESIZE] : []
                             }, t.fontMetrics = function() {
                                 return this._fontMetrics || (this._fontMetrics = function(e) {
                                     var t;
-                                    if (!Z[t = e >= 5 ? 0 : e >= 3 ? 1 : 2]) {
-                                        var r = Z[t] = {
-                                            cssEmPerMu: X.quad[t] / 18
+                                    if (!Y[t = e >= 5 ? 0 : e >= 3 ? 1 : 2]) {
+                                        var r = Y[t] = {
+                                            cssEmPerMu: V.quad[t] / 18
                                         };
-                                        for (var n in X) X.hasOwnProperty(n) && (r[n] = X[n][t])
+                                        for (var n in V) V.hasOwnProperty(n) && (r[n] = V[n][t])
                                     }
-                                    return Z[t]
+                                    return Y[t]
                                 }(this.size)), this._fontMetrics
                             }, t.getColor = function() {
                                 return this.phantom ? "transparent" : this.color
                             }, e
                         }();
-                    Fe.BASESIZE = 6;
-                    var Ve = Fe,
-                        Ue = {
+                    Re.BASESIZE = 6;
+                    var Ee = Re,
+                        Le = {
                             pt: 1,
                             mm: 7227 / 2540,
                             cm: 7227 / 254,
                             in: 72.27,
                             bp: 1.00375,
                             pc: 12,
                             dd: 1238 / 1157,
                             cc: 14856 / 1157,
                             nd: 685 / 642,
                             nc: 1370 / 107,
                             sp: 1 / 65536,
                             px: 1.00375
                         },
-                        Ge = {
+                        Pe = {
                             ex: !0,
                             em: !0,
                             mu: !0
                         },
-                        Ye = function(e) {
-                            return "string" != typeof e && (e = e.unit), e in Ue || e in Ge || "ex" === e
+                        De = function(e) {
+                            return "string" != typeof e && (e = e.unit), e in Le || e in Pe || "ex" === e
                         },
-                        _e = function(e, t) {
+                        He = function(e, t) {
                             var r;
-                            if (e.unit in Ue) r = Ue[e.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
+                            if (e.unit in Le) r = Le[e.unit] / t.fontMetrics().ptPerEm / t.sizeMultiplier;
                             else if ("mu" === e.unit) r = t.fontMetrics().cssEmPerMu;
                             else {
                                 var n;
                                 if (n = t.style.isTight() ? t.havingStyle(t.style.text()) : t, "ex" === e.unit) r = n.fontMetrics().xHeight;
                                 else {
                                     if ("em" !== e.unit) throw new o("Invalid unit: '" + e.unit + "'");
                                     r = n.fontMetrics().quad
                                 }
                                 n !== t && (r *= n.sizeMultiplier / t.sizeMultiplier)
                             }
                             return Math.min(e.number * r, t.maxSize)
                         },
-                        We = function(e, t, r) {
-                            return ee[r][e] && ee[r][e].replace && (e = ee[r][e].replace), {
+                        Fe = function(e, t, r) {
+                            return j[r][e] && j[r][e].replace && (e = j[r][e].replace), {
                                 value: e,
-                                metrics: $(e, t, r)
+                                metrics: G(e, t, r)
                             }
                         },
-                        Xe = function(e, t, r, n, a) {
-                            var i, o = We(e, t, r),
+                        Ve = function(e, t, r, n, a) {
+                            var i, o = Fe(e, t, r),
                                 s = o.metrics;
                             if (e = o.value, s) {
                                 var l = s.italic;
-                                ("text" === r || n && "mathit" === n.font) && (l = 0), i = new V(e, s.height, s.depth, l, s.skew, s.width, a)
-                            } else "undefined" != typeof console && console.warn("No character metrics for '" + e + "' in style '" + t + "' and mode '" + r + "'"), i = new V(e, 0, 0, 0, 0, 0, a);
+                                ("text" === r || n && "mathit" === n.font) && (l = 0), i = new E(e, s.height, s.depth, l, s.skew, s.width, a)
+                            } else "undefined" != typeof console && console.warn("No character metrics for '" + e + "' in style '" + t + "' and mode '" + r + "'"), i = new E(e, 0, 0, 0, 0, 0, a);
                             if (n) {
                                 i.maxFontSize = n.sizeMultiplier, n.style.isTight() && i.classes.push("mtight");
                                 var h = n.getColor();
                                 h && (i.style.color = h)
                             }
                             return i
                         },
-                        je = function(e, t) {
-                            if (O(e.classes) !== O(t.classes) || e.skew !== t.skew || e.maxFontSize !== t.maxFontSize) return !1;
+                        Ue = function(e, t) {
+                            if (T(e.classes) !== T(t.classes) || e.skew !== t.skew || e.maxFontSize !== t.maxFontSize) return !1;
                             for (var r in e.style)
                                 if (e.style.hasOwnProperty(r) && e.style[r] !== t.style[r]) return !1;
                             for (var n in t.style)
                                 if (t.style.hasOwnProperty(n) && e.style[n] !== t.style[n]) return !1;
                             return !0
                         },
-                        $e = function(e) {
+                        Ge = function(e) {
                             for (var t = 0, r = 0, n = 0, a = 0; a < e.children.length; a++) {
                                 var i = e.children[a];
                                 i.height > t && (t = i.height), i.depth > r && (r = i.depth), i.maxFontSize > n && (n = i.maxFontSize)
                             }
                             e.height = t, e.depth = r, e.maxFontSize = n
                         },
-                        Ze = function(e, t, r, n) {
-                            var a = new P(e, t, r, n);
-                            return $e(a), a
-                        },
-                        Ke = function(e, t, r, n) {
-                            return new P(e, t, r, n)
-                        },
-                        Je = function(e) {
-                            var t = new I(e);
-                            return $e(t), t
+                        Ye = function(e, t, r, n) {
+                            var a = new N(e, t, r, n);
+                            return Ge(a), a
+                        },
+                        _e = function(e, t, r, n) {
+                            return new N(e, t, r, n)
+                        },
+                        We = function(e) {
+                            var t = new A(e);
+                            return Ge(t), t
                         },
-                        Qe = function(e, t, r) {
+                        Xe = function(e, t, r) {
                             var n = "";
                             switch (e) {
                                 case "amsrm":
                                     n = "AMS";
                                     break;
                                 case "textrm":
                                     n = "Main";
@@ -3002,15 +3004,15 @@
                                     n = "Typewriter";
                                     break;
                                 default:
                                     n = e
                             }
                             return n + "-" + ("textbf" === t && "textit" === r ? "BoldItalic" : "textbf" === t ? "Bold" : "textit" === t ? "Italic" : "Regular")
                         },
-                        et = {
+                        je = {
                             mathbf: {
                                 variant: "bold",
                                 fontName: "Main-Bold"
                             },
                             mathrm: {
                                 variant: "normal",
                                 fontName: "Main-Regular"
@@ -3048,42 +3050,42 @@
                                 fontName: "SansSerif-Regular"
                             },
                             mathtt: {
                                 variant: "monospace",
                                 fontName: "Typewriter-Regular"
                             }
                         },
-                        tt = {
+                        $e = {
                             vec: ["vec", .471, .714],
                             oiintSize1: ["oiintSize1", .957, .499],
                             oiintSize2: ["oiintSize2", 1.472, .659],
                             oiiintSize1: ["oiiintSize1", 1.304, .499],
                             oiiintSize2: ["oiiintSize2", 1.98, .659],
                             leftParenInner: ["leftParenInner", .875, .3],
                             rightParenInner: ["rightParenInner", .875, .3]
                         },
-                        rt = {
-                            fontMap: et,
-                            makeSymbol: Xe,
+                        Ze = {
+                            fontMap: je,
+                            makeSymbol: Ve,
                             mathsym: function(e, t, r, n) {
-                                return void 0 === n && (n = []), "boldsymbol" === r.font && We(e, "Main-Bold", t).metrics ? Xe(e, "Main-Bold", t, r, n.concat(["mathbf"])) : "\\" === e || "main" === ee[t][e].font ? Xe(e, "Main-Regular", t, r, n) : Xe(e, "AMS-Regular", t, r, n.concat(["amsrm"]))
+                                return void 0 === n && (n = []), "boldsymbol" === r.font && Fe(e, "Main-Bold", t).metrics ? Ve(e, "Main-Bold", t, r, n.concat(["mathbf"])) : "\\" === e || "main" === j[t][e].font ? Ve(e, "Main-Regular", t, r, n) : Ve(e, "AMS-Regular", t, r, n.concat(["amsrm"]))
                             },
-                            makeSpan: Ze,
-                            makeSvgSpan: Ke,
+                            makeSpan: Ye,
+                            makeSvgSpan: _e,
                             makeLineSpan: function(e, t, r) {
-                                var n = Ze([e], [], t);
+                                var n = Ye([e], [], t);
                                 return n.height = Math.max(r || t.fontMetrics().defaultRuleThickness, t.minRuleThickness), n.style.borderBottomWidth = n.height + "em", n.maxFontSize = 1, n
                             },
                             makeAnchor: function(e, t, r, n) {
-                                var a = new D(e, t, r, n);
-                                return $e(a), a
+                                var a = new I(e, t, r, n);
+                                return Ge(a), a
                             },
-                            makeFragment: Je,
+                            makeFragment: We,
                             wrapFragment: function(e, t) {
-                                return e instanceof I ? Ze([], [e], t) : e
+                                return e instanceof A ? Ye([], [e], t) : e
                             },
                             makeVList: function(e, t) {
                                 for (var r = function(e) {
                                         if ("individualShift" === e.positionType) {
                                             for (var t = e.children, r = [t[0]], n = -t[0].shift - t[0].elem.depth, a = n, i = 1; i < t.length; i++) {
                                                 var o = -t[i].shift - a - t[i].elem.depth,
                                                     s = o - (t[i - 1].elem.height + t[i - 1].elem.depth);
@@ -3122,385 +3124,385 @@
                                     var s = n[o];
                                     if ("elem" === s.type) {
                                         var l = s.elem;
                                         i = Math.max(i, l.maxFontSize, l.height)
                                     }
                                 }
                                 i += 2;
-                                var h = Ze(["pstrut"], []);
+                                var h = Ye(["pstrut"], []);
                                 h.style.height = i + "em";
                                 for (var m = [], c = a, u = a, p = a, d = 0; d < n.length; d++) {
                                     var f = n[d];
                                     if ("kern" === f.type) p += f.size;
                                     else {
                                         var g = f.elem,
                                             v = f.wrapperClasses || [],
                                             b = f.wrapperStyle || {},
-                                            y = Ze(v, [h, g], void 0, b);
+                                            y = Ye(v, [h, g], void 0, b);
                                         y.style.top = -i - p - g.depth + "em", f.marginLeft && (y.style.marginLeft = f.marginLeft), f.marginRight && (y.style.marginRight = f.marginRight), m.push(y), p += g.height + g.depth
                                     }
                                     c = Math.min(c, p), u = Math.max(u, p)
                                 }
-                                var x, w = Ze(["vlist"], m);
+                                var x, w = Ye(["vlist"], m);
                                 if (w.style.height = u + "em", c < 0) {
-                                    var k = Ze([], []),
-                                        S = Ze(["vlist"], [k]);
+                                    var k = Ye([], []),
+                                        S = Ye(["vlist"], [k]);
                                     S.style.height = -c + "em";
-                                    var M = Ze(["vlist-s"], [new V("​")]);
-                                    x = [Ze(["vlist-r"], [w, M]), Ze(["vlist-r"], [S])]
-                                } else x = [Ze(["vlist-r"], [w])];
-                                var z = Ze(["vlist-t"], x);
+                                    var M = Ye(["vlist-s"], [new E("​")]);
+                                    x = [Ye(["vlist-r"], [w, M]), Ye(["vlist-r"], [S])]
+                                } else x = [Ye(["vlist-r"], [w])];
+                                var z = Ye(["vlist-t"], x);
                                 return 2 === x.length && z.classes.push("vlist-t2"), z.height = u, z.depth = -c, z
                             },
                             makeOrd: function(e, t, r) {
                                 var n = e.mode,
                                     a = e.text,
                                     i = ["mord"],
                                     s = "math" === n || "text" === n && t.font,
                                     l = s ? t.font : t.fontFamily;
                                 if (55349 === a.charCodeAt(0)) {
                                     var h = function(e, t) {
                                             var r = 1024 * (e.charCodeAt(0) - 55296) + (e.charCodeAt(1) - 56320) + 65536,
                                                 n = "math" === t ? 0 : 1;
                                             if (119808 <= r && r < 120484) {
                                                 var a = Math.floor((r - 119808) / 26);
-                                                return [Ee[a][2], Ee[a][n]]
+                                                return [Ce[a][2], Ce[a][n]]
                                             }
                                             if (120782 <= r && r <= 120831) {
                                                 var i = Math.floor((r - 120782) / 10);
-                                                return [Le[i][2], Le[i][n]]
+                                                return [qe[i][2], qe[i][n]]
                                             }
-                                            if (120485 === r || 120486 === r) return [Ee[0][2], Ee[0][n]];
+                                            if (120485 === r || 120486 === r) return [Ce[0][2], Ce[0][n]];
                                             if (120486 < r && r < 120782) return ["", ""];
                                             throw new o("Unsupported character: " + e)
                                         }(a, n),
                                         m = h[0],
                                         c = h[1];
-                                    return Xe(a, m, n, t, i.concat(c))
+                                    return Ve(a, m, n, t, i.concat(c))
                                 }
                                 if (l) {
                                     var u, p;
                                     if ("boldsymbol" === l) {
                                         var d = function(e, t, r, n, a) {
-                                            return "textord" !== a && We(e, "Math-BoldItalic", t).metrics ? {
+                                            return "textord" !== a && Fe(e, "Math-BoldItalic", t).metrics ? {
                                                 fontName: "Math-BoldItalic",
                                                 fontClass: "boldsymbol"
                                             } : {
                                                 fontName: "Main-Bold",
                                                 fontClass: "mathbf"
                                             }
                                         }(a, n, 0, 0, r);
                                         u = d.fontName, p = [d.fontClass]
-                                    } else s ? (u = et[l].fontName, p = [l]) : (u = Qe(l, t.fontWeight, t.fontShape), p = [l, t.fontWeight, t.fontShape]);
-                                    if (We(a, u, n).metrics) return Xe(a, u, n, t, i.concat(p));
-                                    if (ve.hasOwnProperty(a) && "Typewriter" === u.substr(0, 10)) {
-                                        for (var f = [], g = 0; g < a.length; g++) f.push(Xe(a[g], u, n, t, i.concat(p)));
-                                        return Je(f)
+                                    } else s ? (u = je[l].fontName, p = [l]) : (u = Xe(l, t.fontWeight, t.fontShape), p = [l, t.fontWeight, t.fontShape]);
+                                    if (Fe(a, u, n).metrics) return Ve(a, u, n, t, i.concat(p));
+                                    if (ce.hasOwnProperty(a) && "Typewriter" === u.substr(0, 10)) {
+                                        for (var f = [], g = 0; g < a.length; g++) f.push(Ve(a[g], u, n, t, i.concat(p)));
+                                        return We(f)
                                     }
                                 }
-                                if ("mathord" === r) return Xe(a, "Math-Italic", n, t, i.concat(["mathnormal"]));
+                                if ("mathord" === r) return Ve(a, "Math-Italic", n, t, i.concat(["mathnormal"]));
                                 if ("textord" === r) {
-                                    var v = ee[n][a] && ee[n][a].font;
+                                    var v = j[n][a] && j[n][a].font;
                                     if ("ams" === v) {
-                                        var b = Qe("amsrm", t.fontWeight, t.fontShape);
-                                        return Xe(a, b, n, t, i.concat("amsrm", t.fontWeight, t.fontShape))
+                                        var b = Xe("amsrm", t.fontWeight, t.fontShape);
+                                        return Ve(a, b, n, t, i.concat("amsrm", t.fontWeight, t.fontShape))
                                     }
                                     if ("main" !== v && v) {
-                                        var y = Qe(v, t.fontWeight, t.fontShape);
-                                        return Xe(a, y, n, t, i.concat(y, t.fontWeight, t.fontShape))
+                                        var y = Xe(v, t.fontWeight, t.fontShape);
+                                        return Ve(a, y, n, t, i.concat(y, t.fontWeight, t.fontShape))
                                     }
-                                    var x = Qe("textrm", t.fontWeight, t.fontShape);
-                                    return Xe(a, x, n, t, i.concat(t.fontWeight, t.fontShape))
+                                    var x = Xe("textrm", t.fontWeight, t.fontShape);
+                                    return Ve(a, x, n, t, i.concat(t.fontWeight, t.fontShape))
                                 }
                                 throw new Error("unexpected type: " + r + " in makeOrd")
                             },
                             makeGlue: function(e, t) {
-                                var r = Ze(["mspace"], [], t),
-                                    n = _e(e, t);
+                                var r = Ye(["mspace"], [], t),
+                                    n = He(e, t);
                                 return r.style.marginRight = n + "em", r
                             },
                             staticSvg: function(e, t) {
-                                var r = tt[e],
+                                var r = $e[e],
                                     n = r[0],
                                     a = r[1],
                                     i = r[2],
-                                    o = new G(n),
-                                    s = new U([o], {
+                                    o = new P(n),
+                                    s = new L([o], {
                                         width: a + "em",
                                         height: i + "em",
                                         style: "width:" + a + "em",
                                         viewBox: "0 0 " + 1e3 * a + " " + 1e3 * i,
                                         preserveAspectRatio: "xMinYMin"
                                     }),
-                                    l = Ke(["overlay"], [s], t);
+                                    l = _e(["overlay"], [s], t);
                                 return l.height = i, l.style.height = i + "em", l.style.width = a + "em", l
                             },
-                            svgData: tt,
+                            svgData: $e,
                             tryCombineChars: function(e) {
                                 for (var t = 0; t < e.length - 1; t++) {
                                     var r = e[t],
                                         n = e[t + 1];
-                                    r instanceof V && n instanceof V && je(r, n) && (r.text += n.text, r.height = Math.max(r.height, n.height), r.depth = Math.max(r.depth, n.depth), r.italic = n.italic, e.splice(t + 1, 1), t--)
+                                    r instanceof E && n instanceof E && Ue(r, n) && (r.text += n.text, r.height = Math.max(r.height, n.height), r.depth = Math.max(r.depth, n.depth), r.italic = n.italic, e.splice(t + 1, 1), t--)
                                 }
                                 return e
                             }
                         },
-                        nt = {
+                        Ke = {
                             number: 3,
                             unit: "mu"
                         },
-                        at = {
+                        Je = {
                             number: 4,
                             unit: "mu"
                         },
-                        it = {
+                        Qe = {
                             number: 5,
                             unit: "mu"
                         },
-                        ot = {
+                        et = {
                             mord: {
-                                mop: nt,
-                                mbin: at,
-                                mrel: it,
-                                minner: nt
+                                mop: Ke,
+                                mbin: Je,
+                                mrel: Qe,
+                                minner: Ke
                             },
                             mop: {
-                                mord: nt,
-                                mop: nt,
-                                mrel: it,
-                                minner: nt
+                                mord: Ke,
+                                mop: Ke,
+                                mrel: Qe,
+                                minner: Ke
                             },
                             mbin: {
-                                mord: at,
-                                mop: at,
-                                mopen: at,
-                                minner: at
+                                mord: Je,
+                                mop: Je,
+                                mopen: Je,
+                                minner: Je
                             },
                             mrel: {
-                                mord: it,
-                                mop: it,
-                                mopen: it,
-                                minner: it
+                                mord: Qe,
+                                mop: Qe,
+                                mopen: Qe,
+                                minner: Qe
                             },
                             mopen: {},
                             mclose: {
-                                mop: nt,
-                                mbin: at,
-                                mrel: it,
-                                minner: nt
+                                mop: Ke,
+                                mbin: Je,
+                                mrel: Qe,
+                                minner: Ke
                             },
                             mpunct: {
-                                mord: nt,
-                                mop: nt,
-                                mrel: it,
-                                mopen: nt,
-                                mclose: nt,
-                                mpunct: nt,
-                                minner: nt
+                                mord: Ke,
+                                mop: Ke,
+                                mrel: Qe,
+                                mopen: Ke,
+                                mclose: Ke,
+                                mpunct: Ke,
+                                minner: Ke
                             },
                             minner: {
-                                mord: nt,
-                                mop: nt,
-                                mbin: at,
-                                mrel: it,
-                                mopen: nt,
-                                mpunct: nt,
-                                minner: nt
+                                mord: Ke,
+                                mop: Ke,
+                                mbin: Je,
+                                mrel: Qe,
+                                mopen: Ke,
+                                mpunct: Ke,
+                                minner: Ke
                             }
                         },
-                        st = {
+                        tt = {
                             mord: {
-                                mop: nt
+                                mop: Ke
                             },
                             mop: {
-                                mord: nt,
-                                mop: nt
+                                mord: Ke,
+                                mop: Ke
                             },
                             mbin: {},
                             mrel: {},
                             mopen: {},
                             mclose: {
-                                mop: nt
+                                mop: Ke
                             },
                             mpunct: {},
                             minner: {
-                                mop: nt
+                                mop: Ke
                             }
                         },
-                        lt = {},
-                        ht = {},
-                        mt = {};
+                        rt = {},
+                        nt = {},
+                        at = {};
 
-                    function ct(e) {
+                    function it(e) {
                         for (var t = e.type, r = e.names, n = e.props, a = e.handler, i = e.htmlBuilder, o = e.mathmlBuilder, s = {
                                 type: t,
                                 numArgs: n.numArgs,
                                 argTypes: n.argTypes,
                                 greediness: void 0 === n.greediness ? 1 : n.greediness,
                                 allowedInText: !!n.allowedInText,
                                 allowedInMath: void 0 === n.allowedInMath || n.allowedInMath,
                                 numOptionalArgs: n.numOptionalArgs || 0,
                                 infix: !!n.infix,
                                 handler: a
-                            }, l = 0; l < r.length; ++l) lt[r[l]] = s;
-                        t && (i && (ht[t] = i), o && (mt[t] = o))
+                            }, l = 0; l < r.length; ++l) rt[r[l]] = s;
+                        t && (i && (nt[t] = i), o && (at[t] = o))
                     }
 
-                    function ut(e) {
-                        ct({
+                    function ot(e) {
+                        it({
                             type: e.type,
                             names: [],
                             props: {
                                 numArgs: 0
                             },
                             handler: function() {
                                 throw new Error("Should never be called.")
                             },
                             htmlBuilder: e.htmlBuilder,
                             mathmlBuilder: e.mathmlBuilder
                         })
                     }
-                    var pt = function(e) {
+                    var st = function(e) {
                             return "ordgroup" === e.type ? e.body : [e]
                         },
-                        dt = rt.makeSpan,
-                        ft = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
-                        gt = ["rightmost", "mrel", "mclose", "mpunct"],
-                        vt = {
-                            display: T.DISPLAY,
-                            text: T.TEXT,
-                            script: T.SCRIPT,
-                            scriptscript: T.SCRIPTSCRIPT
+                        lt = Ze.makeSpan,
+                        ht = ["leftmost", "mbin", "mopen", "mrel", "mop", "mpunct"],
+                        mt = ["rightmost", "mrel", "mclose", "mpunct"],
+                        ct = {
+                            display: w.DISPLAY,
+                            text: w.TEXT,
+                            script: w.SCRIPT,
+                            scriptscript: w.SCRIPTSCRIPT
                         },
-                        bt = {
+                        ut = {
                             mord: "mord",
                             mop: "mop",
                             mbin: "mbin",
                             mrel: "mrel",
                             mopen: "mopen",
                             mclose: "mclose",
                             mpunct: "mpunct",
                             minner: "minner"
                         },
-                        yt = function(e, t, r, n) {
+                        pt = function(e, t, r, n) {
                             void 0 === n && (n = [null, null]);
                             for (var a = [], i = 0; i < e.length; i++) {
-                                var o = zt(e[i], t);
-                                if (o instanceof I) {
+                                var o = yt(e[i], t);
+                                if (o instanceof A) {
                                     var s = o.children;
                                     a.push.apply(a, s)
                                 } else a.push(o)
                             }
                             if (!r) return a;
                             var l = t;
                             if (1 === e.length) {
                                 var h = e[0];
-                                "sizing" === h.type ? l = t.havingSize(h.size) : "styling" === h.type && (l = t.havingStyle(vt[h.style]))
+                                "sizing" === h.type ? l = t.havingSize(h.size) : "styling" === h.type && (l = t.havingStyle(ct[h.style]))
                             }
-                            var m = dt([n[0] || "leftmost"], [], t),
-                                u = dt([n[1] || "rightmost"], [], t),
+                            var m = lt([n[0] || "leftmost"], [], t),
+                                u = lt([n[1] || "rightmost"], [], t),
                                 p = "root" === r;
-                            return xt(a, (function(e, t) {
+                            return dt(a, (function(e, t) {
                                 var r = t.classes[0],
                                     n = e.classes[0];
-                                "mbin" === r && c(gt, n) ? t.classes[0] = "mord" : "mbin" === n && c(ft, r) && (e.classes[0] = "mord")
+                                "mbin" === r && c.contains(mt, n) ? t.classes[0] = "mord" : "mbin" === n && c.contains(ht, r) && (e.classes[0] = "mord")
                             }), {
                                 node: m
-                            }, u, p), xt(a, (function(e, t) {
-                                var r = St(t),
-                                    n = St(e),
-                                    a = r && n ? e.hasClass("mtight") ? st[r][n] : ot[r][n] : null;
-                                if (a) return rt.makeGlue(a, l)
+                            }, u, p), dt(a, (function(e, t) {
+                                var r = vt(t),
+                                    n = vt(e),
+                                    a = r && n ? e.hasClass("mtight") ? tt[r][n] : et[r][n] : null;
+                                if (a) return Ze.makeGlue(a, l)
                             }), {
                                 node: m
                             }, u, p), a
                         },
-                        xt = function e(t, r, n, a, i) {
+                        dt = function e(t, r, n, a, i) {
                             a && t.push(a);
                             for (var o = 0; o < t.length; o++) {
                                 var s = t[o],
-                                    l = wt(s);
+                                    l = ft(s);
                                 if (l) e(l.children, r, n, null, i);
                                 else {
                                     var h = !s.hasClass("mspace");
                                     if (h) {
                                         var m = r(s, n.node);
                                         m && (n.insertAfter ? n.insertAfter(m) : (t.unshift(m), o++))
                                     }
-                                    h ? n.node = s : i && s.hasClass("newline") && (n.node = dt(["leftmost"])), n.insertAfter = function(e) {
+                                    h ? n.node = s : i && s.hasClass("newline") && (n.node = lt(["leftmost"])), n.insertAfter = function(e) {
                                         return function(r) {
                                             t.splice(e + 1, 0, r), o++
                                         }
                                     }(o)
                                 }
                             }
                             a && t.pop()
                         },
-                        wt = function(e) {
-                            return e instanceof I || e instanceof D || e instanceof P && e.hasClass("enclosing") ? e : null
+                        ft = function(e) {
+                            return e instanceof A || e instanceof I || e instanceof N && e.hasClass("enclosing") ? e : null
                         },
-                        kt = function e(t, r) {
-                            var n = wt(t);
+                        gt = function e(t, r) {
+                            var n = ft(t);
                             if (n) {
                                 var a = n.children;
                                 if (a.length) {
                                     if ("right" === r) return e(a[a.length - 1], "right");
                                     if ("left" === r) return e(a[0], "left")
                                 }
                             }
                             return t
                         },
-                        St = function(e, t) {
-                            return e ? (t && (e = kt(e, t)), bt[e.classes[0]] || null) : null
+                        vt = function(e, t) {
+                            return e ? (t && (e = gt(e, t)), ut[e.classes[0]] || null) : null
                         },
-                        Mt = function(e, t) {
+                        bt = function(e, t) {
                             var r = ["nulldelimiter"].concat(e.baseSizingClasses());
-                            return dt(t.concat(r))
+                            return lt(t.concat(r))
                         },
-                        zt = function(e, t, r) {
-                            if (!e) return dt();
-                            if (ht[e.type]) {
-                                var n = ht[e.type](e, t);
+                        yt = function(e, t, r) {
+                            if (!e) return lt();
+                            if (nt[e.type]) {
+                                var n = nt[e.type](e, t);
                                 if (r && t.size !== r.size) {
-                                    n = dt(t.sizingClasses(r), [n], t);
+                                    n = lt(t.sizingClasses(r), [n], t);
                                     var a = t.sizeMultiplier / r.sizeMultiplier;
                                     n.height *= a, n.depth *= a
                                 }
                                 return n
                             }
                             throw new o("Got group of unknown type: '" + e.type + "'")
                         };
 
-                    function At(e, t) {
-                        var r = dt(["base"], e, t),
-                            n = dt(["strut"]);
+                    function xt(e, t) {
+                        var r = lt(["base"], e, t),
+                            n = lt(["strut"]);
                         return n.style.height = r.height + r.depth + "em", n.style.verticalAlign = -r.depth + "em", r.children.unshift(n), r
                     }
 
-                    function Tt(e, t) {
+                    function wt(e, t) {
                         var r = null;
                         1 === e.length && "tag" === e[0].type && (r = e[0].tag, e = e[0].body);
-                        for (var n, a = yt(e, t, "root"), i = [], o = [], s = 0; s < a.length; s++)
+                        for (var n, a = pt(e, t, "root"), i = [], o = [], s = 0; s < a.length; s++)
                             if (o.push(a[s]), a[s].hasClass("mbin") || a[s].hasClass("mrel") || a[s].hasClass("allowbreak")) {
                                 for (var l = !1; s < a.length - 1 && a[s + 1].hasClass("mspace") && !a[s + 1].hasClass("newline");) s++, o.push(a[s]), a[s].hasClass("nobreak") && (l = !0);
-                                l || (i.push(At(o, t)), o = [])
-                            } else a[s].hasClass("newline") && (o.pop(), o.length > 0 && (i.push(At(o, t)), o = []), i.push(a[s]));
-                        o.length > 0 && i.push(At(o, t)), r && ((n = At(yt(r, t, !0))).classes = ["tag"], i.push(n));
-                        var h = dt(["katex-html"], i);
+                                l || (i.push(xt(o, t)), o = [])
+                            } else a[s].hasClass("newline") && (o.pop(), o.length > 0 && (i.push(xt(o, t)), o = []), i.push(a[s]));
+                        o.length > 0 && i.push(xt(o, t)), r && ((n = xt(pt(r, t, !0))).classes = ["tag"], i.push(n));
+                        var h = lt(["katex-html"], i);
                         if (h.setAttribute("aria-hidden", "true"), n) {
                             var m = n.children[0];
                             m.style.height = h.height + h.depth + "em", m.style.verticalAlign = -h.depth + "em"
                         }
                         return h
                     }
 
-                    function Bt(e) {
-                        return new I(e)
+                    function kt(e) {
+                        return new A(e)
                     }
-                    var Ct = function() {
+                    var St = function() {
                             function e(e, t) {
                                 this.type = void 0, this.attributes = void 0, this.children = void 0, this.type = e, this.attributes = {}, this.children = t || []
                             }
                             var t = e.prototype;
                             return t.setAttribute = function(e, t) {
                                 this.attributes[e] = t
                             }, t.getAttribute = function(e) {
@@ -3508,40 +3510,40 @@
                             }, t.toNode = function() {
                                 var e = document.createElementNS("http://www.w3.org/1998/Math/MathML", this.type);
                                 for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && e.setAttribute(t, this.attributes[t]);
                                 for (var r = 0; r < this.children.length; r++) e.appendChild(this.children[r].toNode());
                                 return e
                             }, t.toMarkup = function() {
                                 var e = "<" + this.type;
-                                for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && (e += " " + t + '="', e += p(this.attributes[t]), e += '"');
+                                for (var t in this.attributes) Object.prototype.hasOwnProperty.call(this.attributes, t) && (e += " " + t + '="', e += c.escape(this.attributes[t]), e += '"');
                                 e += ">";
                                 for (var r = 0; r < this.children.length; r++) e += this.children[r].toMarkup();
                                 return e + "</" + this.type + ">"
                             }, t.toText = function() {
                                 return this.children.map((function(e) {
                                     return e.toText()
                                 })).join("")
                             }, e
                         }(),
-                        qt = function() {
+                        Mt = function() {
                             function e(e) {
                                 this.text = void 0, this.text = e
                             }
                             var t = e.prototype;
                             return t.toNode = function() {
                                 return document.createTextNode(this.text)
                             }, t.toMarkup = function() {
-                                return p(this.toText())
+                                return c.escape(this.toText())
                             }, t.toText = function() {
                                 return this.text
                             }, e
                         }(),
-                        Nt = {
-                            MathNode: Ct,
-                            TextNode: qt,
+                        zt = {
+                            MathNode: St,
+                            TextNode: Mt,
                             SpaceNode: function() {
                                 function e(e) {
                                     this.width = void 0, this.character = void 0, this.width = e, this.character = e >= .05555 && e <= .05556 ? " " : e >= .1666 && e <= .1667 ? " " : e >= .2222 && e <= .2223 ? " " : e >= .2777 && e <= .2778 ? "  " : e >= -.05556 && e <= -.05555 ? " ⁣" : e >= -.1667 && e <= -.1666 ? " ⁣" : e >= -.2223 && e <= -.2222 ? " ⁣" : e >= -.2778 && e <= -.2777 ? " ⁣" : null
                                 }
                                 var t = e.prototype;
                                 return t.toNode = function() {
                                     if (this.character) return document.createTextNode(this.character);
@@ -3549,23 +3551,23 @@
                                     return e.setAttribute("width", this.width + "em"), e
                                 }, t.toMarkup = function() {
                                     return this.character ? "<mtext>" + this.character + "</mtext>" : '<mspace width="' + this.width + 'em"/>'
                                 }, t.toText = function() {
                                     return this.character ? this.character : " "
                                 }, e
                             }(),
-                            newDocumentFragment: Bt
+                            newDocumentFragment: kt
                         },
-                        It = function(e, t, r) {
-                            return !ee[t][e] || !ee[t][e].replace || 55349 === e.charCodeAt(0) || ve.hasOwnProperty(e) && r && (r.fontFamily && "tt" === r.fontFamily.substr(4, 2) || r.font && "tt" === r.font.substr(4, 2)) || (e = ee[t][e].replace), new Nt.TextNode(e)
+                        At = function(e, t, r) {
+                            return !j[t][e] || !j[t][e].replace || 55349 === e.charCodeAt(0) || ce.hasOwnProperty(e) && r && (r.fontFamily && "tt" === r.fontFamily.substr(4, 2) || r.font && "tt" === r.font.substr(4, 2)) || (e = j[t][e].replace), new zt.TextNode(e)
                         },
-                        Ot = function(e) {
-                            return 1 === e.length ? e[0] : new Nt.MathNode("mrow", e)
+                        Tt = function(e) {
+                            return 1 === e.length ? e[0] : new zt.MathNode("mrow", e)
                         },
-                        Rt = function(e, t) {
+                        Bt = function(e, t) {
                             if ("texttt" === t.fontFamily) return "monospace";
                             if ("textsf" === t.fontFamily) return "textit" === t.fontShape && "textbf" === t.fontWeight ? "sans-serif-bold-italic" : "textit" === t.fontShape ? "sans-serif-italic" : "textbf" === t.fontWeight ? "bold-sans-serif" : "sans-serif";
                             if ("textit" === t.fontShape && "textbf" === t.fontWeight) return "bold-italic";
                             if ("textit" === t.fontShape) return "italic";
                             if ("textbf" === t.fontWeight) return "bold";
                             var r = t.font;
                             if (!r || "mathnormal" === r) return null;
@@ -3575,86 +3577,88 @@
                             if ("mathbf" === r) return "bold";
                             if ("mathbb" === r) return "double-struck";
                             if ("mathfrak" === r) return "fraktur";
                             if ("mathscr" === r || "mathcal" === r) return "script";
                             if ("mathsf" === r) return "sans-serif";
                             if ("mathtt" === r) return "monospace";
                             var a = e.text;
-                            return c(["\\imath", "\\jmath"], a) ? null : (ee[n][a] && ee[n][a].replace && (a = ee[n][a].replace), $(a, rt.fontMap[r].fontName, n) ? rt.fontMap[r].variant : null)
+                            return c.contains(["\\imath", "\\jmath"], a) ? null : (j[n][a] && j[n][a].replace && (a = j[n][a].replace), G(a, Ze.fontMap[r].fontName, n) ? Ze.fontMap[r].variant : null)
                         },
-                        Et = function(e, t, r) {
+                        Ct = function(e, t, r) {
                             if (1 === e.length) {
-                                var n = Pt(e[0], t);
-                                return r && n instanceof Ct && "mo" === n.type && (n.setAttribute("lspace", "0em"), n.setAttribute("rspace", "0em")), [n]
+                                var n = Nt(e[0], t);
+                                return r && n instanceof St && "mo" === n.type && (n.setAttribute("lspace", "0em"), n.setAttribute("rspace", "0em")), [n]
                             }
                             for (var a, i = [], o = 0; o < e.length; o++) {
-                                var s = Pt(e[o], t);
-                                if (s instanceof Ct && a instanceof Ct) {
+                                var s = Nt(e[o], t);
+                                if (s instanceof St && a instanceof St) {
                                     if ("mtext" === s.type && "mtext" === a.type && s.getAttribute("mathvariant") === a.getAttribute("mathvariant")) {
                                         var l;
                                         (l = a.children).push.apply(l, s.children);
                                         continue
                                     }
                                     if ("mn" === s.type && "mn" === a.type) {
                                         var h;
                                         (h = a.children).push.apply(h, s.children);
                                         continue
                                     }
                                     if ("mi" === s.type && 1 === s.children.length && "mn" === a.type) {
                                         var m = s.children[0];
-                                        if (m instanceof qt && "." === m.text) {
+                                        if (m instanceof Mt && "." === m.text) {
                                             var c;
                                             (c = a.children).push.apply(c, s.children);
                                             continue
                                         }
                                     } else if ("mi" === a.type && 1 === a.children.length) {
                                         var u = a.children[0];
-                                        if (u instanceof qt && "̸" === u.text && ("mo" === s.type || "mi" === s.type || "mn" === s.type)) {
+                                        if (u instanceof Mt && "̸" === u.text && ("mo" === s.type || "mi" === s.type || "mn" === s.type)) {
                                             var p = s.children[0];
-                                            p instanceof qt && p.text.length > 0 && (p.text = p.text.slice(0, 1) + "̸" + p.text.slice(1), i.pop())
+                                            p instanceof Mt && p.text.length > 0 && (p.text = p.text.slice(0, 1) + "̸" + p.text.slice(1), i.pop())
                                         }
                                     }
                                 }
                                 i.push(s), a = s
                             }
                             return i
                         },
-                        Lt = function(e, t, r) {
-                            return Ot(Et(e, t, r))
+                        qt = function(e, t, r) {
+                            return Tt(Ct(e, t, r))
                         },
-                        Pt = function(e, t) {
-                            if (!e) return new Nt.MathNode("mrow");
-                            if (mt[e.type]) return mt[e.type](e, t);
+                        Nt = function(e, t) {
+                            if (!e) return new zt.MathNode("mrow");
+                            if (at[e.type]) return at[e.type](e, t);
                             throw new o("Got group of unknown type: '" + e.type + "'")
                         };
 
-                    function Dt(e, t, r, n, a) {
-                        var i, o = Et(e, r);
-                        i = 1 === o.length && o[0] instanceof Ct && c(["mrow", "mtable"], o[0].type) ? o[0] : new Nt.MathNode("mrow", o);
-                        var s = new Nt.MathNode("annotation", [new Nt.TextNode(t)]);
+                    function It(e, t, r, n, a) {
+                        var i, o = Ct(e, r);
+                        i = 1 === o.length && o[0] instanceof St && c.contains(["mrow", "mtable"], o[0].type) ? o[0] : new zt.MathNode("mrow", o);
+                        var s = new zt.MathNode("annotation", [new zt.TextNode(t)]);
                         s.setAttribute("encoding", "application/x-tex");
-                        var l = new Nt.MathNode("semantics", [i, s]),
-                            h = new Nt.MathNode("math", [l]);
-                        return h.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), n && h.setAttribute("display", "block"), rt.makeSpan([a ? "katex" : "katex-mathml"], [h])
+                        var l = new zt.MathNode("semantics", [i, s]),
+                            h = new zt.MathNode("math", [l]);
+                        h.setAttribute("xmlns", "http://www.w3.org/1998/Math/MathML"), n && h.setAttribute("display", "block");
+                        var m = a ? "katex" : "katex-mathml";
+                        return Ze.makeSpan([m], [h])
                     }
-                    var Ht = function(e) {
-                            return new Ve({
-                                style: e.displayMode ? T.DISPLAY : T.TEXT,
+                    var Ot = function(e) {
+                            return new Ee({
+                                style: e.displayMode ? w.DISPLAY : w.TEXT,
                                 maxSize: e.maxSize,
                                 minRuleThickness: e.minRuleThickness
                             })
                         },
-                        Ft = function(e, t) {
+                        Rt = function(e, t) {
                             if (t.displayMode) {
                                 var r = ["katex-display"];
-                                t.leqno && r.push("leqno"), t.fleqn && r.push("fleqn"), e = rt.makeSpan(r, [e])
+                                t.leqno && r.push("leqno"), t.fleqn && r.push("fleqn"), e = Ze.makeSpan(r, [e])
                             }
                             return e
                         },
-                        Vt = {
+                        Et = {
                             widehat: "^",
                             widecheck: "ˇ",
                             widetilde: "~",
                             utilde: "~",
                             overleftarrow: "←",
                             underleftarrow: "←",
                             xleftarrow: "←",
@@ -3687,15 +3691,15 @@
                             xtwoheadrightarrow: "↠",
                             xlongequal: "=",
                             xtofrom: "⇄",
                             xrightleftarrows: "⇄",
                             xrightequilibrium: "⇌",
                             xleftequilibrium: "⇋"
                         },
-                        Ut = {
+                        Lt = {
                             overrightarrow: [
                                 ["rightarrow"], .888, 522, "xMaxYMin"
                             ],
                             overleftarrow: [
                                 ["leftarrow"], .888, 522, "xMinYMin"
                             ],
                             underrightarrow: [
@@ -3800,111 +3804,111 @@
                             xrightequilibrium: [
                                 ["baraboveshortleftharpoon", "rightharpoonaboveshortbar"], 1.75, 716
                             ],
                             xleftequilibrium: [
                                 ["shortbaraboveleftharpoon", "shortrightharpoonabovebar"], 1.75, 716
                             ]
                         },
-                        Gt = function(e) {
-                            var t = new Nt.MathNode("mo", [new Nt.TextNode(Vt[e.substr(1)])]);
+                        Pt = function(e) {
+                            var t = new zt.MathNode("mo", [new zt.TextNode(Et[e.substr(1)])]);
                             return t.setAttribute("stretchy", "true"), t
                         },
-                        Yt = function(e, t) {
+                        Dt = function(e, t) {
                             var r = function() {
                                     var r = 4e5,
                                         n = e.label.substr(1);
-                                    if (c(["widehat", "widecheck", "widetilde", "utilde"], n)) {
+                                    if (c.contains(["widehat", "widecheck", "widetilde", "utilde"], n)) {
                                         var a, i, o, s = "ordgroup" === (d = e.base).type ? d.body.length : 1;
                                         if (s > 5) "widehat" === n || "widecheck" === n ? (a = 420, r = 2364, o = .42, i = n + "4") : (a = 312, r = 2340, o = .34, i = "tilde4");
                                         else {
                                             var l = [1, 1, 2, 2, 3, 3][s];
                                             "widehat" === n || "widecheck" === n ? (r = [0, 1062, 2364, 2364, 2364][l], a = [0, 239, 300, 360, 420][l], o = [0, .24, .3, .3, .36, .42][l], i = n + l) : (r = [0, 600, 1033, 2339, 2340][l], a = [0, 260, 286, 306, 312][l], o = [0, .26, .286, .3, .306, .34][l], i = "tilde" + l)
                                         }
-                                        var h = new G(i),
-                                            m = new U([h], {
+                                        var h = new P(i),
+                                            m = new L([h], {
                                                 width: "100%",
                                                 height: o + "em",
                                                 viewBox: "0 0 " + r + " " + a,
                                                 preserveAspectRatio: "none"
                                             });
                                         return {
-                                            span: rt.makeSvgSpan([], [m], t),
+                                            span: Ze.makeSvgSpan([], [m], t),
                                             minWidth: 0,
                                             height: o
                                         }
                                     }
                                     var u, p, d, f = [],
-                                        g = Ut[n],
+                                        g = Lt[n],
                                         v = g[0],
                                         b = g[1],
                                         y = g[2],
                                         x = y / 1e3,
                                         w = v.length;
                                     if (1 === w) u = ["hide-tail"], p = [g[3]];
                                     else if (2 === w) u = ["halfarrow-left", "halfarrow-right"], p = ["xMinYMin", "xMaxYMin"];
                                     else {
                                         if (3 !== w) throw new Error("Correct katexImagesData or update code here to support\n                    " + w + " children.");
                                         u = ["brace-left", "brace-center", "brace-right"], p = ["xMinYMin", "xMidYMin", "xMaxYMin"]
                                     }
                                     for (var k = 0; k < w; k++) {
-                                        var S = new G(v[k]),
-                                            M = new U([S], {
+                                        var S = new P(v[k]),
+                                            M = new L([S], {
                                                 width: "400em",
                                                 height: x + "em",
                                                 viewBox: "0 0 " + r + " " + y,
                                                 preserveAspectRatio: p[k] + " slice"
                                             }),
-                                            z = rt.makeSvgSpan([u[k]], [M], t);
+                                            z = Ze.makeSvgSpan([u[k]], [M], t);
                                         if (1 === w) return {
                                             span: z,
                                             minWidth: b,
                                             height: x
                                         };
                                         z.style.height = x + "em", f.push(z)
                                     }
                                     return {
-                                        span: rt.makeSpan(["stretchy"], f, t),
+                                        span: Ze.makeSpan(["stretchy"], f, t),
                                         minWidth: b,
                                         height: x
                                     }
                                 }(),
                                 n = r.span,
                                 a = r.minWidth,
                                 i = r.height;
                             return n.height = i, n.style.height = i + "em", a > 0 && (n.style.minWidth = a + "em"), n
                         };
 
-                    function _t(e, t) {
+                    function Ht(e, t) {
                         if (!e || e.type !== t) throw new Error("Expected node of type " + t + ", but got " + (e ? "node of type " + e.type : String(e)));
                         return e
                     }
 
-                    function Wt(e) {
-                        var t = Xt(e);
+                    function Ft(e) {
+                        var t = Vt(e);
                         if (!t) throw new Error("Expected node of symbol group type, but got " + (e ? "node of type " + e.type : String(e)));
                         return t
                     }
 
-                    function Xt(e) {
-                        return e && ("atom" === e.type || J.hasOwnProperty(e.type)) ? e : null
+                    function Vt(e) {
+                        return e && ("atom" === e.type || W.hasOwnProperty(e.type)) ? e : null
                     }
-                    var jt = function(e, t) {
+                    var Ut = function(e, t) {
                             var r, n, a;
-                            e && "supsub" === e.type ? (r = (n = _t(e.base, "accent")).base, e.base = r, a = function(e) {
-                                if (e instanceof P) return e;
+                            e && "supsub" === e.type ? (r = (n = Ht(e.base, "accent")).base, e.base = r, a = function(e) {
+                                if (e instanceof N) return e;
                                 throw new Error("Expected span<HtmlDomNode> but got " + String(e) + ".")
-                            }(zt(e, t)), e.base = n) : r = (n = _t(e, "accent")).base;
-                            var i = zt(r, t.havingCrampedStyle()),
+                            }(yt(e, t)), e.base = n) : r = (n = Ht(e, "accent")).base;
+                            var i = yt(r, t.havingCrampedStyle()),
                                 o = 0;
-                            if (n.isShifty && g(r)) {
-                                var s = f(r);
-                                o = _(zt(s, t.havingCrampedStyle())).skew
+                            if (n.isShifty && c.isCharacterBox(r)) {
+                                var s = c.getBaseElem(r);
+                                o = H(yt(s, t.havingCrampedStyle())).skew
                             }
                             var l, h = Math.min(i.height, t.fontMetrics().xHeight);
-                            if (n.isStretchy) l = Yt(n, t), l = rt.makeVList({
+                            if (n.isStretchy) l = Dt(n, t), l = Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: i
                                 }, {
                                     type: "elem",
                                     elem: l,
@@ -3912,69 +3916,69 @@
                                     wrapperStyle: o > 0 ? {
                                         width: "calc(100% - " + 2 * o + "em)",
                                         marginLeft: 2 * o + "em"
                                     } : void 0
                                 }]
                             }, t);
                             else {
-                                var m, c;
-                                "\\vec" === n.label ? (m = rt.staticSvg("vec", t), c = rt.svgData.vec[1]) : ((m = _(m = rt.makeOrd({
+                                var m, u;
+                                "\\vec" === n.label ? (m = Ze.staticSvg("vec", t), u = Ze.svgData.vec[1]) : ((m = H(m = Ze.makeOrd({
                                     mode: n.mode,
                                     text: n.label
-                                }, t, "textord"))).italic = 0, c = m.width), l = rt.makeSpan(["accent-body"], [m]);
-                                var u = "\\textcircled" === n.label;
-                                u && (l.classes.push("accent-full"), h = i.height);
-                                var p = o;
-                                u || (p -= c / 2), l.style.left = p + "em", "\\textcircled" === n.label && (l.style.top = ".2em"), l = rt.makeVList({
+                                }, t, "textord"))).italic = 0, u = m.width), l = Ze.makeSpan(["accent-body"], [m]);
+                                var p = "\\textcircled" === n.label;
+                                p && (l.classes.push("accent-full"), h = i.height);
+                                var d = o;
+                                p || (d -= u / 2), l.style.left = d + "em", "\\textcircled" === n.label && (l.style.top = ".2em"), l = Ze.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: i
                                     }, {
                                         type: "kern",
                                         size: -h
                                     }, {
                                         type: "elem",
                                         elem: l
                                     }]
                                 }, t)
                             }
-                            var d = rt.makeSpan(["mord", "accent"], [l], t);
-                            return a ? (a.children[0] = d, a.height = Math.max(d.height, a.height), a.classes[0] = "mord", a) : d
+                            var f = Ze.makeSpan(["mord", "accent"], [l], t);
+                            return a ? (a.children[0] = f, a.height = Math.max(f.height, a.height), a.classes[0] = "mord", a) : f
                         },
-                        $t = function(e, t) {
-                            var r = e.isStretchy ? Gt(e.label) : new Nt.MathNode("mo", [It(e.label, e.mode)]),
-                                n = new Nt.MathNode("mover", [Pt(e.base, t), r]);
+                        Gt = function(e, t) {
+                            var r = e.isStretchy ? Pt(e.label) : new zt.MathNode("mo", [At(e.label, e.mode)]),
+                                n = new zt.MathNode("mover", [Nt(e.base, t), r]);
                             return n.setAttribute("accent", "true"), n
                         },
-                        Zt = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map((function(e) {
+                        Yt = new RegExp(["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring"].map((function(e) {
                             return "\\" + e
                         })).join("|"));
-                    ct({
+                    it({
                         type: "accent",
                         names: ["\\acute", "\\grave", "\\ddot", "\\tilde", "\\bar", "\\breve", "\\check", "\\hat", "\\vec", "\\dot", "\\mathring", "\\widecheck", "\\widehat", "\\widetilde", "\\overrightarrow", "\\overleftarrow", "\\Overrightarrow", "\\overleftrightarrow", "\\overgroup", "\\overlinesegment", "\\overleftharpoon", "\\overrightharpoon"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = t[0],
-                                n = !Zt.test(e.funcName),
+                                n = !Yt.test(e.funcName),
                                 a = !n || "\\widehat" === e.funcName || "\\widetilde" === e.funcName || "\\widecheck" === e.funcName;
                             return {
                                 type: "accent",
                                 mode: e.parser.mode,
                                 label: e.funcName,
                                 isStretchy: n,
                                 isShifty: a,
                                 base: r
                             }
                         },
-                        htmlBuilder: jt,
-                        mathmlBuilder: $t
-                    }), ct({
+                        htmlBuilder: Ut,
+                        mathmlBuilder: Gt
+                    }), it({
                         type: "accent",
                         names: ["\\'", "\\`", "\\^", "\\~", "\\=", "\\u", "\\.", '\\"', "\\r", "\\H", "\\v", "\\textcircled"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0,
                             allowedInMath: !1
                         },
@@ -3985,17 +3989,17 @@
                                 mode: e.parser.mode,
                                 label: e.funcName,
                                 isStretchy: !1,
                                 isShifty: !0,
                                 base: r
                             }
                         },
-                        htmlBuilder: jt,
-                        mathmlBuilder: $t
-                    }), ct({
+                        htmlBuilder: Ut,
+                        mathmlBuilder: Gt
+                    }), it({
                         type: "accentUnder",
                         names: ["\\underleftarrow", "\\underrightarrow", "\\underleftrightarrow", "\\undergroup", "\\underlinesegment", "\\utilde"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
@@ -4005,45 +4009,45 @@
                                 type: "accentUnder",
                                 mode: r.mode,
                                 label: n,
                                 base: a
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = zt(e.base, t),
-                                n = Yt(e, t),
+                            var r = yt(e.base, t),
+                                n = Dt(e, t),
                                 a = "\\utilde" === e.label ? .12 : 0,
-                                i = rt.makeVList({
+                                i = Ze.makeVList({
                                     positionType: "top",
                                     positionData: r.height,
                                     children: [{
                                         type: "elem",
                                         elem: n,
                                         wrapperClasses: ["svg-align"]
                                     }, {
                                         type: "kern",
                                         size: a
                                     }, {
                                         type: "elem",
                                         elem: r
                                     }]
                                 }, t);
-                            return rt.makeSpan(["mord", "accentunder"], [i], t)
+                            return Ze.makeSpan(["mord", "accentunder"], [i], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = Gt(e.label),
-                                n = new Nt.MathNode("munder", [Pt(e.base, t), r]);
+                            var r = Pt(e.label),
+                                n = new zt.MathNode("munder", [Nt(e.base, t), r]);
                             return n.setAttribute("accentunder", "true"), n
                         }
                     });
-                    var Kt = function(e) {
-                        var t = new Nt.MathNode("mpadded", e ? [e] : []);
+                    var _t = function(e) {
+                        var t = new zt.MathNode("mpadded", e ? [e] : []);
                         return t.setAttribute("width", "+0.6em"), t.setAttribute("lspace", "0.3em"), t
                     };
-                    ct({
+                    it({
                         type: "xArrow",
                         names: ["\\xleftarrow", "\\xrightarrow", "\\xLeftarrow", "\\xRightarrow", "\\xleftrightarrow", "\\xLeftrightarrow", "\\xhookleftarrow", "\\xhookrightarrow", "\\xmapsto", "\\xrightharpoondown", "\\xrightharpoonup", "\\xleftharpoondown", "\\xleftharpoonup", "\\xrightleftharpoons", "\\xleftrightharpoons", "\\xlongequal", "\\xtwoheadrightarrow", "\\xtwoheadleftarrow", "\\xtofrom", "\\xrightleftarrows", "\\xrightequilibrium", "\\xleftequilibrium"],
                         props: {
                             numArgs: 1,
                             numOptionalArgs: 1
                         },
                         handler: function(e, t, r) {
@@ -4056,22 +4060,22 @@
                                 body: t[0],
                                 below: r[0]
                             }
                         },
                         htmlBuilder: function(e, t) {
                             var r, n = t.style,
                                 a = t.havingStyle(n.sup()),
-                                i = rt.wrapFragment(zt(e.body, a, t), t);
-                            i.classes.push("x-arrow-pad"), e.below && (a = t.havingStyle(n.sub()), (r = rt.wrapFragment(zt(e.below, a, t), t)).classes.push("x-arrow-pad"));
-                            var o, s = Yt(e, t),
+                                i = Ze.wrapFragment(yt(e.body, a, t), t);
+                            i.classes.push("x-arrow-pad"), e.below && (a = t.havingStyle(n.sub()), (r = Ze.wrapFragment(yt(e.below, a, t), t)).classes.push("x-arrow-pad"));
+                            var o, s = Dt(e, t),
                                 l = -t.fontMetrics().axisHeight + .5 * s.height,
                                 h = -t.fontMetrics().axisHeight - .5 * s.height - .111;
                             if ((i.depth > .25 || "\\xleftequilibrium" === e.label) && (h -= i.depth), r) {
                                 var m = -t.fontMetrics().axisHeight + r.height + .5 * s.height + .111;
-                                o = rt.makeVList({
+                                o = Ze.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
                                         elem: i,
                                         shift: h
                                     }, {
                                         type: "elem",
@@ -4079,116 +4083,116 @@
                                         shift: l
                                     }, {
                                         type: "elem",
                                         elem: r,
                                         shift: m
                                     }]
                                 }, t)
-                            } else o = rt.makeVList({
+                            } else o = Ze.makeVList({
                                 positionType: "individualShift",
                                 children: [{
                                     type: "elem",
                                     elem: i,
                                     shift: h
                                 }, {
                                     type: "elem",
                                     elem: s,
                                     shift: l
                                 }]
                             }, t);
-                            return o.children[0].children[0].children[1].classes.push("svg-align"), rt.makeSpan(["mrel", "x-arrow"], [o], t)
+                            return o.children[0].children[0].children[1].classes.push("svg-align"), Ze.makeSpan(["mrel", "x-arrow"], [o], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r, n = Gt(e.label);
+                            var r, n = Pt(e.label);
                             if (e.body) {
-                                var a = Kt(Pt(e.body, t));
+                                var a = _t(Nt(e.body, t));
                                 if (e.below) {
-                                    var i = Kt(Pt(e.below, t));
-                                    r = new Nt.MathNode("munderover", [n, i, a])
-                                } else r = new Nt.MathNode("mover", [n, a])
+                                    var i = _t(Nt(e.below, t));
+                                    r = new zt.MathNode("munderover", [n, i, a])
+                                } else r = new zt.MathNode("mover", [n, a])
                             } else if (e.below) {
-                                var o = Kt(Pt(e.below, t));
-                                r = new Nt.MathNode("munder", [n, o])
-                            } else r = Kt(), r = new Nt.MathNode("mover", [n, r]);
+                                var o = _t(Nt(e.below, t));
+                                r = new zt.MathNode("munder", [n, o])
+                            } else r = _t(), r = new zt.MathNode("mover", [n, r]);
                             return r
                         }
-                    }), ct({
+                    }), it({
                         type: "textord",
                         names: ["\\@char"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
-                            for (var r = e.parser, n = _t(t[0], "ordgroup").body, a = "", i = 0; i < n.length; i++) a += _t(n[i], "textord").text;
+                            for (var r = e.parser, n = Ht(t[0], "ordgroup").body, a = "", i = 0; i < n.length; i++) a += Ht(n[i], "textord").text;
                             var s = parseInt(a);
                             if (isNaN(s)) throw new o("\\@char has non-numeric argument " + a);
                             return {
                                 type: "textord",
                                 mode: r.mode,
                                 text: String.fromCharCode(s)
                             }
                         }
                     });
-                    var Jt = function(e, t) {
-                            var r = yt(e.body, t.withColor(e.color), !1);
-                            return rt.makeFragment(r)
-                        },
-                        Qt = function(e, t) {
-                            var r = Et(e.body, t.withColor(e.color)),
-                                n = new Nt.MathNode("mstyle", r);
+                    var Wt = function(e, t) {
+                            var r = pt(e.body, t.withColor(e.color), !1);
+                            return Ze.makeFragment(r)
+                        },
+                        Xt = function(e, t) {
+                            var r = Ct(e.body, t.withColor(e.color)),
+                                n = new zt.MathNode("mstyle", r);
                             return n.setAttribute("mathcolor", e.color), n
                         };
-                    ct({
+                    it({
                         type: "color",
                         names: ["\\textcolor"],
                         props: {
                             numArgs: 2,
                             allowedInText: !0,
                             greediness: 3,
                             argTypes: ["color", "original"]
                         },
                         handler: function(e, t) {
                             var r = e.parser,
-                                n = _t(t[0], "color-token").color,
+                                n = Ht(t[0], "color-token").color,
                                 a = t[1];
                             return {
                                 type: "color",
                                 mode: r.mode,
                                 color: n,
-                                body: pt(a)
+                                body: st(a)
                             }
                         },
-                        htmlBuilder: Jt,
-                        mathmlBuilder: Qt
-                    }), ct({
+                        htmlBuilder: Wt,
+                        mathmlBuilder: Xt
+                    }), it({
                         type: "color",
                         names: ["\\color"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0,
                             greediness: 3,
                             argTypes: ["color"]
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.breakOnTokenText,
-                                a = _t(t[0], "color-token").color;
+                                a = Ht(t[0], "color-token").color;
                             r.gullet.macros.set("\\current@color", a);
                             var i = r.parseExpression(!0, n);
                             return {
                                 type: "color",
                                 mode: r.mode,
                                 color: a,
                                 body: i
                             }
                         },
-                        htmlBuilder: Jt,
-                        mathmlBuilder: Qt
-                    }), ct({
+                        htmlBuilder: Wt,
+                        mathmlBuilder: Xt
+                    }), it({
                         type: "cr",
                         names: ["\\cr", "\\newline"],
                         props: {
                             numArgs: 0,
                             numOptionalArgs: 1,
                             argTypes: ["size"],
                             allowedInText: !0
@@ -4200,67 +4204,67 @@
                                 o = "\\cr" === a,
                                 s = !1;
                             return o || (s = !n.settings.displayMode || !n.settings.useStrictBehavior("newLineInDisplayMode", "In LaTeX, \\\\ or \\newline does nothing in display mode")), {
                                 type: "cr",
                                 mode: n.mode,
                                 newLine: s,
                                 newRow: o,
-                                size: i && _t(i, "size").value
+                                size: i && Ht(i, "size").value
                             }
                         },
                         htmlBuilder: function(e, t) {
                             if (e.newRow) throw new o("\\cr valid only within a tabular/array environment");
-                            var r = rt.makeSpan(["mspace"], [], t);
-                            return e.newLine && (r.classes.push("newline"), e.size && (r.style.marginTop = _e(e.size, t) + "em")), r
+                            var r = Ze.makeSpan(["mspace"], [], t);
+                            return e.newLine && (r.classes.push("newline"), e.size && (r.style.marginTop = He(e.size, t) + "em")), r
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mspace");
-                            return e.newLine && (r.setAttribute("linebreak", "newline"), e.size && r.setAttribute("height", _e(e.size, t) + "em")), r
+                            var r = new zt.MathNode("mspace");
+                            return e.newLine && (r.setAttribute("linebreak", "newline"), e.size && r.setAttribute("height", He(e.size, t) + "em")), r
                         }
                     });
-                    var er = {
+                    var jt = {
                             "\\global": "\\global",
                             "\\long": "\\\\globallong",
                             "\\\\globallong": "\\\\globallong",
                             "\\def": "\\gdef",
                             "\\gdef": "\\gdef",
                             "\\edef": "\\xdef",
                             "\\xdef": "\\xdef",
                             "\\let": "\\\\globallet",
                             "\\futurelet": "\\\\globalfuture"
                         },
-                        tr = function(e) {
+                        $t = function(e) {
                             var t = e.text;
                             if (/^(?:[\\{}$&#^_]|EOF)$/.test(t)) throw new o("Expected a control sequence", e);
                             return t
                         },
-                        rr = function(e, t, r, n) {
+                        Zt = function(e, t, r, n) {
                             var a = e.gullet.macros.get(r.text);
                             null == a && (r.noexpand = !0, a = {
                                 tokens: [r],
                                 numArgs: 0,
                                 unexpandable: !e.gullet.isExpandable(r.text)
                             }), e.gullet.macros.set(t, a, n)
                         };
-                    ct({
+                    it({
                         type: "internal",
                         names: ["\\global", "\\long", "\\\\globallong"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e) {
                             var t = e.parser,
                                 r = e.funcName;
                             t.consumeSpaces();
                             var n = t.fetch();
-                            if (er[n.text]) return "\\global" !== r && "\\\\globallong" !== r || (n.text = er[n.text]), _t(t.parseFunction(), "internal");
+                            if (jt[n.text]) return "\\global" !== r && "\\\\globallong" !== r || (n.text = jt[n.text]), Ht(t.parseFunction(), "internal");
                             throw new o("Invalid token after macro prefix", n)
                         }
-                    }), ct({
+                    }), it({
                         type: "internal",
                         names: ["\\def", "\\gdef", "\\edef", "\\xdef"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e) {
@@ -4275,157 +4279,159 @@
                                 if (!/^[1-9]$/.test(n[0].text)) throw new o('Invalid argument number "' + n[0].text + '"');
                                 if (i++, parseInt(n[0].text) !== i) throw new o('Argument number "' + n[0].text + '" out of order');
                                 n = t.gullet.consumeArgs(1)[0]
                             }
                             return "\\edef" !== r && "\\xdef" !== r || (n = t.gullet.expandTokens(n)).reverse(), t.gullet.macros.set(a, {
                                 tokens: n,
                                 numArgs: i
-                            }, r === er[r]), {
+                            }, r === jt[r]), {
                                 type: "internal",
                                 mode: t.mode
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "internal",
                         names: ["\\let", "\\\\globallet"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e) {
                             var t = e.parser,
                                 r = e.funcName,
-                                n = tr(t.gullet.popToken());
+                                n = $t(t.gullet.popToken());
                             t.gullet.consumeSpaces();
                             var a = function(e) {
                                 var t = e.gullet.popToken();
                                 return "=" === t.text && " " === (t = e.gullet.popToken()).text && (t = e.gullet.popToken()), t
                             }(t);
-                            return rr(t, n, a, "\\\\globallet" === r), {
+                            return Zt(t, n, a, "\\\\globallet" === r), {
                                 type: "internal",
                                 mode: t.mode
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "internal",
                         names: ["\\futurelet", "\\\\globalfuture"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e) {
                             var t = e.parser,
                                 r = e.funcName,
-                                n = tr(t.gullet.popToken()),
+                                n = $t(t.gullet.popToken()),
                                 a = t.gullet.popToken(),
                                 i = t.gullet.popToken();
-                            return rr(t, n, i, "\\\\globalfuture" === r), t.gullet.pushToken(i), t.gullet.pushToken(a), {
+                            return Zt(t, n, i, "\\\\globalfuture" === r), t.gullet.pushToken(i), t.gullet.pushToken(a), {
                                 type: "internal",
                                 mode: t.mode
                             }
                         }
                     });
-                    var nr = function(e, t, r) {
-                            var n = $(ee.math[e] && ee.math[e].replace || e, t, r);
+                    var Kt = function(e, t, r) {
+                            var n = G(j.math[e] && j.math[e].replace || e, t, r);
                             if (!n) throw new Error("Unsupported symbol " + e + " and font size " + t + ".");
                             return n
                         },
-                        ar = function(e, t, r, n) {
+                        Jt = function(e, t, r, n) {
                             var a = r.havingBaseStyle(t),
-                                i = rt.makeSpan(n.concat(a.sizingClasses(r)), [e], r),
+                                i = Ze.makeSpan(n.concat(a.sizingClasses(r)), [e], r),
                                 o = a.sizeMultiplier / r.sizeMultiplier;
                             return i.height *= o, i.depth *= o, i.maxFontSize = a.sizeMultiplier, i
                         },
-                        ir = function(e, t, r) {
+                        Qt = function(e, t, r) {
                             var n = t.havingBaseStyle(r),
                                 a = (1 - t.sizeMultiplier / n.sizeMultiplier) * t.fontMetrics().axisHeight;
                             e.classes.push("delimcenter"), e.style.top = a + "em", e.height -= a, e.depth += a
                         },
-                        or = function(e, t, r, n, a, i) {
+                        er = function(e, t, r, n, a, i) {
                             var o = function(e, t, r, n) {
-                                    return rt.makeSymbol(e, "Size" + t + "-Regular", r, n)
+                                    return Ze.makeSymbol(e, "Size" + t + "-Regular", r, n)
                                 }(e, t, a, n),
-                                s = ar(rt.makeSpan(["delimsizing", "size" + t], [o], n), T.TEXT, n, i);
-                            return r && ir(s, n, T.TEXT), s
+                                s = Jt(Ze.makeSpan(["delimsizing", "size" + t], [o], n), w.TEXT, n, i);
+                            return r && Qt(s, n, w.TEXT), s
                         },
-                        sr = function(e, t, r) {
-                            return {
+                        tr = function(e, t, r) {
+                            var n;
+                            return n = "Size1-Regular" === t ? "delim-size1" : "delim-size4", {
                                 type: "elem",
-                                elem: rt.makeSpan(["delimsizinginner", "Size1-Regular" === t ? "delim-size1" : "delim-size4"], [rt.makeSpan([], [rt.makeSymbol(e, t, r)])])
+                                elem: Ze.makeSpan(["delimsizinginner", n], [Ze.makeSpan([], [Ze.makeSymbol(e, t, r)])])
                             }
                         },
-                        lr = {
+                        rr = {
                             type: "kern",
                             size: -.005
                         },
-                        hr = function(e, t, r, n, a, i) {
+                        nr = function(e, t, r, n, a, i) {
                             var o, s, l, h;
                             o = l = h = e, s = null;
                             var m = "Size1-Regular";
                             "\\uparrow" === e ? l = h = "⏐" : "\\Uparrow" === e ? l = h = "‖" : "\\downarrow" === e ? o = l = "⏐" : "\\Downarrow" === e ? o = l = "‖" : "\\updownarrow" === e ? (o = "\\uparrow", l = "⏐", h = "\\downarrow") : "\\Updownarrow" === e ? (o = "\\Uparrow", l = "‖", h = "\\Downarrow") : "[" === e || "\\lbrack" === e ? (o = "⎡", l = "⎢", h = "⎣", m = "Size4-Regular") : "]" === e || "\\rbrack" === e ? (o = "⎤", l = "⎥", h = "⎦", m = "Size4-Regular") : "\\lfloor" === e || "⌊" === e ? (l = o = "⎢", h = "⎣", m = "Size4-Regular") : "\\lceil" === e || "⌈" === e ? (o = "⎡", l = h = "⎢", m = "Size4-Regular") : "\\rfloor" === e || "⌋" === e ? (l = o = "⎥", h = "⎦", m = "Size4-Regular") : "\\rceil" === e || "⌉" === e ? (o = "⎤", l = h = "⎥", m = "Size4-Regular") : "(" === e || "\\lparen" === e ? (o = "⎛", l = "⎜", h = "⎝", m = "Size4-Regular") : ")" === e || "\\rparen" === e ? (o = "⎞", l = "⎟", h = "⎠", m = "Size4-Regular") : "\\{" === e || "\\lbrace" === e ? (o = "⎧", s = "⎨", h = "⎩", l = "⎪", m = "Size4-Regular") : "\\}" === e || "\\rbrace" === e ? (o = "⎫", s = "⎬", h = "⎭", l = "⎪", m = "Size4-Regular") : "\\lgroup" === e || "⟮" === e ? (o = "⎧", h = "⎩", l = "⎪", m = "Size4-Regular") : "\\rgroup" === e || "⟯" === e ? (o = "⎫", h = "⎭", l = "⎪", m = "Size4-Regular") : "\\lmoustache" === e || "⎰" === e ? (o = "⎧", h = "⎭", l = "⎪", m = "Size4-Regular") : "\\rmoustache" !== e && "⎱" !== e || (o = "⎫", h = "⎩", l = "⎪", m = "Size4-Regular");
-                            var c = nr(o, m, a),
+                            var c = Kt(o, m, a),
                                 u = c.height + c.depth,
-                                p = nr(l, m, a),
+                                p = Kt(l, m, a),
                                 d = p.height + p.depth,
-                                f = nr(h, m, a),
+                                f = Kt(h, m, a),
                                 g = f.height + f.depth,
                                 v = 0,
                                 b = 1;
                             if (null !== s) {
-                                var y = nr(s, m, a);
+                                var y = Kt(s, m, a);
                                 v = y.height + y.depth, b = 2
                             }
                             var x = u + g + v,
-                                w = Math.max(0, Math.ceil((t - x) / (b * d))),
-                                k = x + w * b * d,
-                                S = n.fontMetrics().axisHeight;
-                            r && (S *= n.sizeMultiplier);
-                            var M = k / 2 - S,
-                                z = .005 * (w + 1) - d,
-                                A = [];
-                            if (A.push(sr(h, m, a)), null === s)
-                                for (var B = 0; B < w; B++) A.push(lr), A.push(sr(l, m, a));
+                                k = Math.max(0, Math.ceil((t - x) / (b * d))),
+                                S = x + k * b * d,
+                                M = n.fontMetrics().axisHeight;
+                            r && (M *= n.sizeMultiplier);
+                            var z = S / 2 - M,
+                                A = .005 * (k + 1) - d,
+                                T = [];
+                            if (T.push(tr(h, m, a)), null === s)
+                                for (var B = 0; B < k; B++) T.push(rr), T.push(tr(l, m, a));
                             else {
-                                for (var C = 0; C < w; C++) A.push(lr), A.push(sr(l, m, a));
-                                A.push({
+                                for (var C = 0; C < k; C++) T.push(rr), T.push(tr(l, m, a));
+                                T.push({
                                     type: "kern",
-                                    size: z
-                                }), A.push(sr(l, m, a)), A.push(lr), A.push(sr(s, m, a));
-                                for (var q = 0; q < w; q++) A.push(lr), A.push(sr(l, m, a))
+                                    size: A
+                                }), T.push(tr(l, m, a)), T.push(rr), T.push(tr(s, m, a));
+                                for (var q = 0; q < k; q++) T.push(rr), T.push(tr(l, m, a))
                             }
-                            if ("⎜" !== l && "⎟" !== l || 0 !== w) A.push({
+                            if ("⎜" !== l && "⎟" !== l || 0 !== k) T.push({
                                 type: "kern",
-                                size: z
-                            }), A.push(sr(l, m, a)), A.push(lr);
+                                size: A
+                            }), T.push(tr(l, m, a)), T.push(rr);
                             else {
-                                var N = rt.svgData.leftParenInner[2] / 2;
-                                A.push({
+                                var N = Ze.svgData.leftParenInner[2] / 2;
+                                T.push({
                                     type: "kern",
                                     size: -N
                                 });
-                                var I = rt.staticSvg("⎜" === l ? "leftParenInner" : "rightParenInner", n);
-                                A.push({
+                                var I = "⎜" === l ? "leftParenInner" : "rightParenInner",
+                                    O = Ze.staticSvg(I, n);
+                                T.push({
                                     type: "elem",
-                                    elem: I
-                                }), A.push({
+                                    elem: O
+                                }), T.push({
                                     type: "kern",
                                     size: -N
                                 })
                             }
-                            A.push(sr(o, m, a));
-                            var O = n.havingBaseStyle(T.TEXT),
-                                R = rt.makeVList({
+                            T.push(tr(o, m, a));
+                            var R = n.havingBaseStyle(w.TEXT),
+                                E = Ze.makeVList({
                                     positionType: "bottom",
-                                    positionData: M,
-                                    children: A
-                                }, O);
-                            return ar(rt.makeSpan(["delimsizing", "mult"], [R], O), T.TEXT, n, i)
+                                    positionData: z,
+                                    children: T
+                                }, R);
+                            return Jt(Ze.makeSpan(["delimsizing", "mult"], [E], R), w.TEXT, n, i)
                         },
-                        mr = .08,
-                        cr = function(e, t, r, n, a) {
+                        ar = .08,
+                        ir = function(e, t, r, n, a) {
                             var i = function(e, t, r) {
                                     t *= 1e3;
                                     var n = "";
                                     switch (e) {
                                         case "sqrtMain":
                                             n = function(e, t) {
                                                 return "M95," + (622 + e + 80) + "\nc-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14\nc0,-2,0.3,-3.3,1,-4c1.3,-2.7,23.83,-20.7,67.5,-54\nc44.2,-33.3,65.8,-50.3,66.5,-51c1.3,-1.3,3,-2,5,-2c4.7,0,8.7,3.3,12,10\ns173,378,173,378c0.7,0,35.3,-71,104,-213c68.7,-142,137.5,-285,206.5,-429\nc69,-144,104.5,-217.7,106.5,-221\nl" + e / 2.075 + " -" + e + "\nc5.3,-9.3,12,-14,20,-14\nH400000v" + (40 + e) + "H845.2724\ns-225.272,467,-225.272,467s-235,486,-235,486c-2.7,4.7,-9,7,-19,7\nc-6,0,-10,-1,-12,-3s-194,-422,-194,-422s-65,47,-65,47z\nM" + (834 + e) + " 80h400000v" + (40 + e) + "h-400000z"
@@ -4454,70 +4460,70 @@
                                         case "sqrtTall":
                                             n = function(e, t, r) {
                                                 return "M702 " + (e + 80) + "H400000" + (40 + e) + "\nH742v" + (r - 54 - 80 - e) + "l-4 4-4 4c-.667.7 -2 1.5-4 2.5s-4.167 1.833-6.5 2.5-5.5 1-9.5 1\nh-12l-28-84c-16.667-52-96.667 -294.333-240-727l-212 -643 -85 170\nc-4-3.333-8.333-7.667-13 -13l-13-13l77-155 77-156c66 199.333 139 419.667\n219 661 l218 661zM702 80H400000v" + (40 + e) + "H742z"
                                             }(t, 0, r)
                                     }
                                     return n
                                 }(e, n, r),
-                                o = new G(e, i),
-                                s = new U([o], {
+                                o = new P(e, i),
+                                s = new L([o], {
                                     width: "400em",
                                     height: t + "em",
                                     viewBox: "0 0 400000 " + r,
                                     preserveAspectRatio: "xMinYMin slice"
                                 });
-                            return rt.makeSvgSpan(["hide-tail"], [s], a)
+                            return Ze.makeSvgSpan(["hide-tail"], [s], a)
                         },
-                        ur = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "⌊", "⌋", "\\lceil", "\\rceil", "⌈", "⌉", "\\surd"],
-                        pr = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "⟮", "⟯", "\\lmoustache", "\\rmoustache", "⎰", "⎱"],
-                        dr = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
-                        fr = [0, 1.2, 1.8, 2.4, 3],
-                        gr = [{
+                        or = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "⌊", "⌋", "\\lceil", "\\rceil", "⌈", "⌉", "\\surd"],
+                        sr = ["\\uparrow", "\\downarrow", "\\updownarrow", "\\Uparrow", "\\Downarrow", "\\Updownarrow", "|", "\\|", "\\vert", "\\Vert", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "⟮", "⟯", "\\lmoustache", "\\rmoustache", "⎰", "⎱"],
+                        lr = ["<", ">", "\\langle", "\\rangle", "/", "\\backslash", "\\lt", "\\gt"],
+                        hr = [0, 1.2, 1.8, 2.4, 3],
+                        mr = [{
                             type: "small",
-                            style: T.SCRIPTSCRIPT
+                            style: w.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: T.SCRIPT
+                            style: w.SCRIPT
                         }, {
                             type: "small",
-                            style: T.TEXT
+                            style: w.TEXT
                         }, {
                             type: "large",
                             size: 1
                         }, {
                             type: "large",
                             size: 2
                         }, {
                             type: "large",
                             size: 3
                         }, {
                             type: "large",
                             size: 4
                         }],
-                        vr = [{
+                        cr = [{
                             type: "small",
-                            style: T.SCRIPTSCRIPT
+                            style: w.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: T.SCRIPT
+                            style: w.SCRIPT
                         }, {
                             type: "small",
-                            style: T.TEXT
+                            style: w.TEXT
                         }, {
                             type: "stack"
                         }],
-                        br = [{
+                        ur = [{
                             type: "small",
-                            style: T.SCRIPTSCRIPT
+                            style: w.SCRIPTSCRIPT
                         }, {
                             type: "small",
-                            style: T.SCRIPT
+                            style: w.SCRIPT
                         }, {
                             type: "small",
-                            style: T.TEXT
+                            style: w.TEXT
                         }, {
                             type: "large",
                             size: 1
                         }, {
                             type: "large",
                             size: 2
                         }, {
@@ -4525,52 +4531,52 @@
                             size: 3
                         }, {
                             type: "large",
                             size: 4
                         }, {
                             type: "stack"
                         }],
-                        yr = function(e) {
+                        pr = function(e) {
                             if ("small" === e.type) return "Main-Regular";
                             if ("large" === e.type) return "Size" + e.size + "-Regular";
                             if ("stack" === e.type) return "Size4-Regular";
                             throw new Error("Add support for delim type '" + e.type + "' here.")
                         },
-                        xr = function(e, t, r, n) {
+                        dr = function(e, t, r, n) {
                             for (var a = Math.min(2, 3 - n.style.size); a < r.length && "stack" !== r[a].type; a++) {
-                                var i = nr(e, yr(r[a]), "math"),
+                                var i = Kt(e, pr(r[a]), "math"),
                                     o = i.height + i.depth;
                                 if ("small" === r[a].type && (o *= n.havingBaseStyle(r[a].style).sizeMultiplier), o > t) return r[a]
                             }
                             return r[r.length - 1]
                         },
-                        wr = function(e, t, r, n, a, i) {
+                        fr = function(e, t, r, n, a, i) {
                             var o;
-                            "<" === e || "\\lt" === e || "⟨" === e ? e = "\\langle" : ">" !== e && "\\gt" !== e && "⟩" !== e || (e = "\\rangle"), o = c(dr, e) ? gr : c(ur, e) ? br : vr;
-                            var s = xr(e, t, o, n);
+                            "<" === e || "\\lt" === e || "⟨" === e ? e = "\\langle" : ">" !== e && "\\gt" !== e && "⟩" !== e || (e = "\\rangle"), o = c.contains(lr, e) ? mr : c.contains(or, e) ? ur : cr;
+                            var s = dr(e, t, o, n);
                             return "small" === s.type ? function(e, t, r, n, a, i) {
-                                var o = rt.makeSymbol(e, "Main-Regular", a, n),
-                                    s = ar(o, t, n, i);
-                                return r && ir(s, n, t), s
-                            }(e, s.style, r, n, a, i) : "large" === s.type ? or(e, s.size, r, n, a, i) : hr(e, t, r, n, a, i)
-                        },
-                        kr = function(e, t, r, n, a) {
-                            if ("<" === e || "\\lt" === e || "⟨" === e ? e = "\\langle" : ">" !== e && "\\gt" !== e && "⟩" !== e || (e = "\\rangle"), c(ur, e) || c(dr, e)) return or(e, t, !1, r, n, a);
-                            if (c(pr, e)) return hr(e, fr[t], !1, r, n, a);
+                                var o = Ze.makeSymbol(e, "Main-Regular", a, n),
+                                    s = Jt(o, t, n, i);
+                                return r && Qt(s, n, t), s
+                            }(e, s.style, r, n, a, i) : "large" === s.type ? er(e, s.size, r, n, a, i) : nr(e, t, r, n, a, i)
+                        },
+                        gr = function(e, t, r, n, a) {
+                            if ("<" === e || "\\lt" === e || "⟨" === e ? e = "\\langle" : ">" !== e && "\\gt" !== e && "⟩" !== e || (e = "\\rangle"), c.contains(or, e) || c.contains(lr, e)) return er(e, t, !1, r, n, a);
+                            if (c.contains(sr, e)) return nr(e, hr[t], !1, r, n, a);
                             throw new o("Illegal delimiter: '" + e + "'")
                         },
-                        Sr = wr,
-                        Mr = function(e, t, r, n, a, i) {
+                        vr = fr,
+                        br = function(e, t, r, n, a, i) {
                             var o = n.fontMetrics().axisHeight * n.sizeMultiplier,
                                 s = 5 / n.fontMetrics().ptPerEm,
                                 l = Math.max(t - o, r + o),
                                 h = Math.max(l / 500 * 901, 2 * l - s);
-                            return wr(e, h, !0, n, a, i)
+                            return fr(e, h, !0, n, a, i)
                         },
-                        zr = {
+                        yr = {
                             "\\bigl": {
                                 mclass: "mopen",
                                 size: 1
                             },
                             "\\Bigl": {
                                 mclass: "mopen",
                                 size: 2
@@ -4628,220 +4634,220 @@
                                 size: 3
                             },
                             "\\Bigg": {
                                 mclass: "mord",
                                 size: 4
                             }
                         },
-                        Ar = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "⌊", "⌋", "\\lceil", "\\rceil", "⌈", "⌉", "<", ">", "\\langle", "⟨", "\\rangle", "⟩", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "⟮", "⟯", "\\lmoustache", "\\rmoustache", "⎰", "⎱", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
+                        xr = ["(", "\\lparen", ")", "\\rparen", "[", "\\lbrack", "]", "\\rbrack", "\\{", "\\lbrace", "\\}", "\\rbrace", "\\lfloor", "\\rfloor", "⌊", "⌋", "\\lceil", "\\rceil", "⌈", "⌉", "<", ">", "\\langle", "⟨", "\\rangle", "⟩", "\\lt", "\\gt", "\\lvert", "\\rvert", "\\lVert", "\\rVert", "\\lgroup", "\\rgroup", "⟮", "⟯", "\\lmoustache", "\\rmoustache", "⎰", "⎱", "/", "\\backslash", "|", "\\vert", "\\|", "\\Vert", "\\uparrow", "\\Uparrow", "\\downarrow", "\\Downarrow", "\\updownarrow", "\\Updownarrow", "."];
 
-                    function Tr(e, t) {
-                        var r = Xt(e);
-                        if (r && c(Ar, r.text)) return r;
+                    function wr(e, t) {
+                        var r = Vt(e);
+                        if (r && c.contains(xr, r.text)) return r;
                         throw new o(r ? "Invalid delimiter '" + r.text + "' after '" + t.funcName + "'" : "Invalid delimiter type '" + e.type + "'", e)
                     }
 
-                    function Br(e) {
+                    function kr(e) {
                         if (!e.body) throw new Error("Bug: The leftright ParseNode wasn't fully parsed.")
                     }
-                    ct({
+                    it({
                         type: "delimsizing",
                         names: ["\\bigl", "\\Bigl", "\\biggl", "\\Biggl", "\\bigr", "\\Bigr", "\\biggr", "\\Biggr", "\\bigm", "\\Bigm", "\\biggm", "\\Biggm", "\\big", "\\Big", "\\bigg", "\\Bigg"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
-                            var r = Tr(t[0], e);
+                            var r = wr(t[0], e);
                             return {
                                 type: "delimsizing",
                                 mode: e.parser.mode,
-                                size: zr[e.funcName].size,
-                                mclass: zr[e.funcName].mclass,
+                                size: yr[e.funcName].size,
+                                mclass: yr[e.funcName].mclass,
                                 delim: r.text
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            return "." === e.delim ? rt.makeSpan([e.mclass]) : kr(e.delim, e.size, t, e.mode, [e.mclass])
+                            return "." === e.delim ? Ze.makeSpan([e.mclass]) : gr(e.delim, e.size, t, e.mode, [e.mclass])
                         },
                         mathmlBuilder: function(e) {
                             var t = [];
-                            "." !== e.delim && t.push(It(e.delim, e.mode));
-                            var r = new Nt.MathNode("mo", t);
+                            "." !== e.delim && t.push(At(e.delim, e.mode));
+                            var r = new zt.MathNode("mo", t);
                             return "mopen" === e.mclass || "mclose" === e.mclass ? r.setAttribute("fence", "true") : r.setAttribute("fence", "false"), r
                         }
-                    }), ct({
+                    }), it({
                         type: "leftright-right",
                         names: ["\\right"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser.gullet.macros.get("\\current@color");
                             if (r && "string" != typeof r) throw new o("\\current@color set to non-string in \\right");
                             return {
                                 type: "leftright-right",
                                 mode: e.parser.mode,
-                                delim: Tr(t[0], e).text,
+                                delim: wr(t[0], e).text,
                                 color: r
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "leftright",
                         names: ["\\left"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
-                            var r = Tr(t[0], e),
+                            var r = wr(t[0], e),
                                 n = e.parser;
                             ++n.leftrightDepth;
                             var a = n.parseExpression(!1);
                             --n.leftrightDepth, n.expect("\\right", !1);
-                            var i = _t(n.parseFunction(), "leftright-right");
+                            var i = Ht(n.parseFunction(), "leftright-right");
                             return {
                                 type: "leftright",
                                 mode: n.mode,
                                 body: a,
                                 left: r.text,
                                 right: i.delim,
                                 rightColor: i.color
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            Br(e);
-                            for (var r, n, a = yt(e.body, t, !0, ["mopen", "mclose"]), i = 0, o = 0, s = !1, l = 0; l < a.length; l++) a[l].isMiddle ? s = !0 : (i = Math.max(a[l].height, i), o = Math.max(a[l].depth, o));
-                            if (i *= t.sizeMultiplier, o *= t.sizeMultiplier, r = "." === e.left ? Mt(t, ["mopen"]) : Mr(e.left, i, o, t, e.mode, ["mopen"]), a.unshift(r), s)
+                            kr(e);
+                            for (var r, n, a = pt(e.body, t, !0, ["mopen", "mclose"]), i = 0, o = 0, s = !1, l = 0; l < a.length; l++) a[l].isMiddle ? s = !0 : (i = Math.max(a[l].height, i), o = Math.max(a[l].depth, o));
+                            if (i *= t.sizeMultiplier, o *= t.sizeMultiplier, r = "." === e.left ? bt(t, ["mopen"]) : br(e.left, i, o, t, e.mode, ["mopen"]), a.unshift(r), s)
                                 for (var h = 1; h < a.length; h++) {
                                     var m = a[h].isMiddle;
-                                    m && (a[h] = Mr(m.delim, i, o, m.options, e.mode, []))
+                                    m && (a[h] = br(m.delim, i, o, m.options, e.mode, []))
                                 }
-                            if ("." === e.right) n = Mt(t, ["mclose"]);
+                            if ("." === e.right) n = bt(t, ["mclose"]);
                             else {
                                 var c = e.rightColor ? t.withColor(e.rightColor) : t;
-                                n = Mr(e.right, i, o, c, e.mode, ["mclose"])
+                                n = br(e.right, i, o, c, e.mode, ["mclose"])
                             }
-                            return a.push(n), rt.makeSpan(["minner"], a, t)
+                            return a.push(n), Ze.makeSpan(["minner"], a, t)
                         },
                         mathmlBuilder: function(e, t) {
-                            Br(e);
-                            var r = Et(e.body, t);
+                            kr(e);
+                            var r = Ct(e.body, t);
                             if ("." !== e.left) {
-                                var n = new Nt.MathNode("mo", [It(e.left, e.mode)]);
+                                var n = new zt.MathNode("mo", [At(e.left, e.mode)]);
                                 n.setAttribute("fence", "true"), r.unshift(n)
                             }
                             if ("." !== e.right) {
-                                var a = new Nt.MathNode("mo", [It(e.right, e.mode)]);
+                                var a = new zt.MathNode("mo", [At(e.right, e.mode)]);
                                 a.setAttribute("fence", "true"), e.rightColor && a.setAttribute("mathcolor", e.rightColor), r.push(a)
                             }
-                            return Ot(r)
+                            return Tt(r)
                         }
-                    }), ct({
+                    }), it({
                         type: "middle",
                         names: ["\\middle"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
-                            var r = Tr(t[0], e);
+                            var r = wr(t[0], e);
                             if (!e.parser.leftrightDepth) throw new o("\\middle without preceding \\left", r);
                             return {
                                 type: "middle",
                                 mode: e.parser.mode,
                                 delim: r.text
                             }
                         },
                         htmlBuilder: function(e, t) {
                             var r;
-                            if ("." === e.delim) r = Mt(t, []);
+                            if ("." === e.delim) r = bt(t, []);
                             else {
-                                r = kr(e.delim, 1, t, e.mode, []);
+                                r = gr(e.delim, 1, t, e.mode, []);
                                 var n = {
                                     delim: e.delim,
                                     options: t
                                 };
                                 r.isMiddle = n
                             }
                             return r
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = "\\vert" === e.delim || "|" === e.delim ? It("|", "text") : It(e.delim, e.mode),
-                                n = new Nt.MathNode("mo", [r]);
+                            var r = "\\vert" === e.delim || "|" === e.delim ? At("|", "text") : At(e.delim, e.mode),
+                                n = new zt.MathNode("mo", [r]);
                             return n.setAttribute("fence", "true"), n.setAttribute("lspace", "0.05em"), n.setAttribute("rspace", "0.05em"), n
                         }
                     });
-                    var Cr = function(e, t) {
-                            var r, n, a = rt.wrapFragment(zt(e.body, t), t),
+                    var Sr = function(e, t) {
+                            var r, n, a = Ze.wrapFragment(yt(e.body, t), t),
                                 i = e.label.substr(1),
                                 o = t.sizeMultiplier,
                                 s = 0,
-                                l = g(e.body);
-                            if ("sout" === i)(r = rt.makeSpan(["stretchy", "sout"])).height = t.fontMetrics().defaultRuleThickness / o, s = -.5 * t.fontMetrics().xHeight;
+                                l = c.isCharacterBox(e.body);
+                            if ("sout" === i)(r = Ze.makeSpan(["stretchy", "sout"])).height = t.fontMetrics().defaultRuleThickness / o, s = -.5 * t.fontMetrics().xHeight;
                             else {
                                 /cancel/.test(i) ? l || a.classes.push("cancel-pad") : a.classes.push("boxpad");
                                 var h = 0,
                                     m = 0;
                                 /box/.test(i) ? (m = Math.max(t.fontMetrics().fboxrule, t.minRuleThickness), h = t.fontMetrics().fboxsep + ("colorbox" === i ? 0 : m)) : h = l ? .2 : 0, r = function(e, t, r, n) {
                                     var a, i = e.height + e.depth + 2 * r;
                                     if (/fbox|color/.test(t)) {
-                                        if (a = rt.makeSpan(["stretchy", t], [], n), "fbox" === t) {
+                                        if (a = Ze.makeSpan(["stretchy", t], [], n), "fbox" === t) {
                                             var o = n.color && n.getColor();
                                             o && (a.style.borderColor = o)
                                         }
                                     } else {
                                         var s = [];
-                                        /^[bx]cancel$/.test(t) && s.push(new Y({
+                                        /^[bx]cancel$/.test(t) && s.push(new D({
                                             x1: "0",
                                             y1: "0",
                                             x2: "100%",
                                             y2: "100%",
                                             "stroke-width": "0.046em"
-                                        })), /^x?cancel$/.test(t) && s.push(new Y({
+                                        })), /^x?cancel$/.test(t) && s.push(new D({
                                             x1: "0",
                                             y1: "100%",
                                             x2: "100%",
                                             y2: "0",
                                             "stroke-width": "0.046em"
                                         }));
-                                        var l = new U(s, {
+                                        var l = new L(s, {
                                             width: "100%",
                                             height: i + "em"
                                         });
-                                        a = rt.makeSvgSpan([], [l], n)
+                                        a = Ze.makeSvgSpan([], [l], n)
                                     }
                                     return a.height = i, a.style.height = i + "em", a
                                 }(a, i, h, t), /fbox|boxed|fcolorbox/.test(i) && (r.style.borderStyle = "solid", r.style.borderWidth = m + "em"), s = a.depth + h, e.backgroundColor && (r.style.backgroundColor = e.backgroundColor, e.borderColor && (r.style.borderColor = e.borderColor))
                             }
-                            return n = e.backgroundColor ? rt.makeVList({
+                            return n = e.backgroundColor ? Ze.makeVList({
                                 positionType: "individualShift",
                                 children: [{
                                     type: "elem",
                                     elem: r,
                                     shift: s
                                 }, {
                                     type: "elem",
                                     elem: a,
                                     shift: 0
                                 }]
-                            }, t) : rt.makeVList({
+                            }, t) : Ze.makeVList({
                                 positionType: "individualShift",
                                 children: [{
                                     type: "elem",
                                     elem: a,
                                     shift: 0
                                 }, {
                                     type: "elem",
                                     elem: r,
                                     shift: s,
                                     wrapperClasses: /cancel/.test(i) ? ["svg-align"] : []
                                 }]
-                            }, t), /cancel/.test(i) && (n.height = a.height, n.depth = a.depth), /cancel/.test(i) && !l ? rt.makeSpan(["mord", "cancel-lap"], [n], t) : rt.makeSpan(["mord"], [n], t)
+                            }, t), /cancel/.test(i) && (n.height = a.height, n.depth = a.depth), /cancel/.test(i) && !l ? Ze.makeSpan(["mord", "cancel-lap"], [n], t) : Ze.makeSpan(["mord"], [n], t)
                         },
-                        qr = function(e, t) {
+                        Mr = function(e, t) {
                             var r = 0,
-                                n = new Nt.MathNode(e.label.indexOf("colorbox") > -1 ? "mpadded" : "menclose", [Pt(e.body, t)]);
+                                n = new zt.MathNode(e.label.indexOf("colorbox") > -1 ? "mpadded" : "menclose", [Nt(e.body, t)]);
                             switch (e.label) {
                                 case "\\cancel":
                                     n.setAttribute("notation", "updiagonalstrike");
                                     break;
                                 case "\\bcancel":
                                     n.setAttribute("notation", "downdiagonalstrike");
                                     break;
@@ -4859,65 +4865,65 @@
                                     }
                                     break;
                                 case "\\xcancel":
                                     n.setAttribute("notation", "updiagonalstrike downdiagonalstrike")
                             }
                             return e.backgroundColor && n.setAttribute("mathbackground", e.backgroundColor), n
                         };
-                    ct({
+                    it({
                         type: "enclose",
                         names: ["\\colorbox"],
                         props: {
                             numArgs: 2,
                             allowedInText: !0,
                             greediness: 3,
                             argTypes: ["color", "text"]
                         },
                         handler: function(e, t, r) {
                             var n = e.parser,
                                 a = e.funcName,
-                                i = _t(t[0], "color-token").color,
+                                i = Ht(t[0], "color-token").color,
                                 o = t[1];
                             return {
                                 type: "enclose",
                                 mode: n.mode,
                                 label: a,
                                 backgroundColor: i,
                                 body: o
                             }
                         },
-                        htmlBuilder: Cr,
-                        mathmlBuilder: qr
-                    }), ct({
+                        htmlBuilder: Sr,
+                        mathmlBuilder: Mr
+                    }), it({
                         type: "enclose",
                         names: ["\\fcolorbox"],
                         props: {
                             numArgs: 3,
                             allowedInText: !0,
                             greediness: 3,
                             argTypes: ["color", "color", "text"]
                         },
                         handler: function(e, t, r) {
                             var n = e.parser,
                                 a = e.funcName,
-                                i = _t(t[0], "color-token").color,
-                                o = _t(t[1], "color-token").color,
+                                i = Ht(t[0], "color-token").color,
+                                o = Ht(t[1], "color-token").color,
                                 s = t[2];
                             return {
                                 type: "enclose",
                                 mode: n.mode,
                                 label: a,
                                 backgroundColor: o,
                                 borderColor: i,
                                 body: s
                             }
                         },
-                        htmlBuilder: Cr,
-                        mathmlBuilder: qr
-                    }), ct({
+                        htmlBuilder: Sr,
+                        mathmlBuilder: Mr
+                    }), it({
                         type: "enclose",
                         names: ["\\fbox"],
                         props: {
                             numArgs: 1,
                             argTypes: ["hbox"],
                             allowedInText: !0
                         },
@@ -4925,15 +4931,15 @@
                             return {
                                 type: "enclose",
                                 mode: e.parser.mode,
                                 label: "\\fbox",
                                 body: t[0]
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "enclose",
                         names: ["\\cancel", "\\bcancel", "\\xcancel", "\\sout"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t, r) {
                             var n = e.parser,
@@ -4942,40 +4948,40 @@
                             return {
                                 type: "enclose",
                                 mode: n.mode,
                                 label: a,
                                 body: i
                             }
                         },
-                        htmlBuilder: Cr,
-                        mathmlBuilder: qr
+                        htmlBuilder: Sr,
+                        mathmlBuilder: Mr
                     });
-                    var Nr = {};
+                    var zr = {};
 
-                    function Ir(e) {
+                    function Ar(e) {
                         for (var t = e.type, r = e.names, n = e.props, a = e.handler, i = e.htmlBuilder, o = e.mathmlBuilder, s = {
                                 type: t,
                                 numArgs: n.numArgs || 0,
                                 greediness: 1,
                                 allowedInText: !1,
                                 numOptionalArgs: 0,
                                 handler: a
-                            }, l = 0; l < r.length; ++l) Nr[r[l]] = s;
-                        i && (ht[t] = i), o && (mt[t] = o)
+                            }, l = 0; l < r.length; ++l) zr[r[l]] = s;
+                        i && (nt[t] = i), o && (at[t] = o)
                     }
 
-                    function Or(e) {
+                    function Tr(e) {
                         var t = [];
                         e.consumeSpaces();
                         for (var r = e.fetch().text;
                             "\\hline" === r || "\\hdashline" === r;) e.consume(), t.push("\\hdashline" === r), e.consumeSpaces(), r = e.fetch().text;
                         return t
                     }
 
-                    function Rr(e, t, r) {
+                    function Br(e, t, r) {
                         var n = t.hskipBeforeAndAfter,
                             a = t.addJot,
                             i = t.cols,
                             s = t.arraystretch,
                             l = t.colSeparationType;
                         if (e.gullet.beginGroup(), e.gullet.macros.set("\\\\", "\\cr"), !s) {
                             var h = e.gullet.expandMacroAsText("\\arraystretch");
@@ -4983,15 +4989,15 @@
                             else if (!(s = parseFloat(h)) || s < 0) throw new o("Invalid \\arraystretch: " + h)
                         }
                         e.gullet.beginGroup();
                         var m = [],
                             c = [m],
                             u = [],
                             p = [];
-                        for (p.push(Or(e));;) {
+                        for (p.push(Tr(e));;) {
                             var d = e.parseExpression(!1, "\\cr");
                             e.gullet.endGroup(), e.gullet.beginGroup(), d = {
                                 type: "ordgroup",
                                 mode: e.mode,
                                 body: d
                             }, r && (d = {
                                 type: "styling",
@@ -5003,16 +5009,16 @@
                             if ("&" === f) e.consume();
                             else {
                                 if ("\\end" === f) {
                                     1 === m.length && "styling" === d.type && 0 === d.body[0].body.length && c.pop(), p.length < c.length + 1 && p.push([]);
                                     break
                                 }
                                 if ("\\cr" !== f) throw new o("Expected & or \\\\ or \\cr or \\end", e.nextToken);
-                                var g = _t(e.parseFunction(), "cr");
-                                u.push(g.size), p.push(Or(e)), m = [], c.push(m)
+                                var g = Ht(e.parseFunction(), "cr");
+                                u.push(g.size), p.push(Tr(e)), m = [], c.push(m)
                             }
                         }
                         return e.gullet.endGroup(), e.gullet.endGroup(), {
                             type: "array",
                             mode: e.mode,
                             addJot: a,
                             arraystretch: s,
@@ -5021,89 +5027,89 @@
                             rowGaps: u,
                             hskipBeforeAndAfter: n,
                             hLinesBeforeRow: p,
                             colSeparationType: l
                         }
                     }
 
-                    function Er(e) {
+                    function Cr(e) {
                         return "d" === e.substr(0, 1) ? "display" : "text"
                     }
-                    var Lr = function(e, t) {
+                    var qr = function(e, t) {
                             var r, n, a = e.body.length,
                                 i = e.hLinesBeforeRow,
                                 s = 0,
                                 l = new Array(a),
                                 h = [],
                                 m = Math.max(t.fontMetrics().arrayRuleWidth, t.minRuleThickness),
-                                c = 1 / t.fontMetrics().ptPerEm,
-                                p = 5 * c;
-                            e.colSeparationType && "small" === e.colSeparationType && (p = t.havingStyle(T.SCRIPT).sizeMultiplier / t.sizeMultiplier * .2778);
-                            var d = 12 * c,
-                                f = 3 * c,
+                                u = 1 / t.fontMetrics().ptPerEm,
+                                p = 5 * u;
+                            e.colSeparationType && "small" === e.colSeparationType && (p = t.havingStyle(w.SCRIPT).sizeMultiplier / t.sizeMultiplier * .2778);
+                            var d = 12 * u,
+                                f = 3 * u,
                                 g = e.arraystretch * d,
                                 v = .7 * g,
                                 b = .3 * g,
                                 y = 0;
 
                             function x(e) {
                                 for (var t = 0; t < e.length; ++t) t > 0 && (y += .25), h.push({
                                     pos: y,
                                     isDashed: e[t]
                                 })
                             }
                             for (x(i[0]), r = 0; r < e.body.length; ++r) {
-                                var w = e.body[r],
-                                    k = v,
-                                    S = b;
-                                s < w.length && (s = w.length);
-                                var M = new Array(w.length);
-                                for (n = 0; n < w.length; ++n) {
-                                    var z = zt(w[n], t);
-                                    S < z.depth && (S = z.depth), k < z.height && (k = z.height), M[n] = z
+                                var k = e.body[r],
+                                    S = v,
+                                    M = b;
+                                s < k.length && (s = k.length);
+                                var z = new Array(k.length);
+                                for (n = 0; n < k.length; ++n) {
+                                    var A = yt(k[n], t);
+                                    M < A.depth && (M = A.depth), S < A.height && (S = A.height), z[n] = A
                                 }
-                                var A = e.rowGaps[r],
+                                var T = e.rowGaps[r],
                                     B = 0;
-                                A && (B = _e(A, t)) > 0 && (S < (B += b) && (S = B), B = 0), e.addJot && (S += f), M.height = k, M.depth = S, y += k, M.pos = y, y += S + B, l[r] = M, x(i[r + 1])
+                                T && (B = He(T, t)) > 0 && (M < (B += b) && (M = B), B = 0), e.addJot && (M += f), z.height = S, z.depth = M, y += S, z.pos = y, y += M + B, l[r] = z, x(i[r + 1])
                             }
                             var C, q, N = y / 2 + t.fontMetrics().axisHeight,
                                 I = e.cols || [],
                                 O = [];
                             for (n = 0, q = 0; n < s || q < I.length; ++n, ++q) {
                                 for (var R = I[q] || {}, E = !0;
                                     "separator" === R.type;) {
-                                    if (E || ((C = rt.makeSpan(["arraycolsep"], [])).style.width = t.fontMetrics().doubleRuleSep + "em", O.push(C)), "|" !== R.separator && ":" !== R.separator) throw new o("Invalid separator type: " + R.separator);
+                                    if (E || ((C = Ze.makeSpan(["arraycolsep"], [])).style.width = t.fontMetrics().doubleRuleSep + "em", O.push(C)), "|" !== R.separator && ":" !== R.separator) throw new o("Invalid separator type: " + R.separator);
                                     var L = "|" === R.separator ? "solid" : "dashed",
-                                        P = rt.makeSpan(["vertical-separator"], [], t);
+                                        P = Ze.makeSpan(["vertical-separator"], [], t);
                                     P.style.height = y + "em", P.style.borderRightWidth = m + "em", P.style.borderRightStyle = L, P.style.margin = "0 -" + m / 2 + "em", P.style.verticalAlign = -(y - N) + "em", O.push(P), R = I[++q] || {}, E = !1
                                 }
                                 if (!(n >= s)) {
                                     var D = void 0;
-                                    (n > 0 || e.hskipBeforeAndAfter) && 0 !== (D = u(R.pregap, p)) && ((C = rt.makeSpan(["arraycolsep"], [])).style.width = D + "em", O.push(C));
+                                    (n > 0 || e.hskipBeforeAndAfter) && 0 !== (D = c.deflt(R.pregap, p)) && ((C = Ze.makeSpan(["arraycolsep"], [])).style.width = D + "em", O.push(C));
                                     var H = [];
                                     for (r = 0; r < a; ++r) {
                                         var F = l[r],
                                             V = F[n];
                                         if (V) {
                                             var U = F.pos - N;
                                             V.depth = F.depth, V.height = F.height, H.push({
                                                 type: "elem",
                                                 elem: V,
                                                 shift: U
                                             })
                                         }
                                     }
-                                    H = rt.makeVList({
+                                    H = Ze.makeVList({
                                         positionType: "individualShift",
                                         children: H
-                                    }, t), H = rt.makeSpan(["col-align-" + (R.align || "c")], [H]), O.push(H), (n < s - 1 || e.hskipBeforeAndAfter) && 0 !== (D = u(R.postgap, p)) && ((C = rt.makeSpan(["arraycolsep"], [])).style.width = D + "em", O.push(C))
+                                    }, t), H = Ze.makeSpan(["col-align-" + (R.align || "c")], [H]), O.push(H), (n < s - 1 || e.hskipBeforeAndAfter) && 0 !== (D = c.deflt(R.postgap, p)) && ((C = Ze.makeSpan(["arraycolsep"], [])).style.width = D + "em", O.push(C))
                                 }
                             }
-                            if (l = rt.makeSpan(["mtable"], O), h.length > 0) {
-                                for (var G = rt.makeLineSpan("hline", t, m), Y = rt.makeLineSpan("hdashline", t, m), _ = [{
+                            if (l = Ze.makeSpan(["mtable"], O), h.length > 0) {
+                                for (var G = Ze.makeLineSpan("hline", t, m), Y = Ze.makeLineSpan("hdashline", t, m), _ = [{
                                         type: "elem",
                                         elem: l,
                                         shift: 0
                                     }]; h.length > 0;) {
                                     var W = h.pop(),
                                         X = W.pos - N;
                                     W.isDashed ? _.push({
@@ -5112,77 +5118,77 @@
                                         shift: X
                                     }) : _.push({
                                         type: "elem",
                                         elem: G,
                                         shift: X
                                     })
                                 }
-                                l = rt.makeVList({
+                                l = Ze.makeVList({
                                     positionType: "individualShift",
                                     children: _
                                 }, t)
                             }
-                            return rt.makeSpan(["mord"], [l], t)
+                            return Ze.makeSpan(["mord"], [l], t)
                         },
-                        Pr = {
+                        Nr = {
                             c: "center ",
                             l: "left ",
                             r: "right "
                         },
-                        Dr = function(e, t) {
-                            var r = new Nt.MathNode("mtable", e.body.map((function(e) {
-                                    return new Nt.MathNode("mtr", e.map((function(e) {
-                                        return new Nt.MathNode("mtd", [Pt(e, t)])
+                        Ir = function(e, t) {
+                            var r = new zt.MathNode("mtable", e.body.map((function(e) {
+                                    return new zt.MathNode("mtr", e.map((function(e) {
+                                        return new zt.MathNode("mtd", [Nt(e, t)])
                                     })))
                                 }))),
                                 n = .5 === e.arraystretch ? .1 : .16 + e.arraystretch - 1 + (e.addJot ? .09 : 0);
                             r.setAttribute("rowspacing", n + "em");
                             var a = "",
                                 i = "";
                             if (e.cols && e.cols.length > 0) {
                                 var o = e.cols,
                                     s = "",
                                     l = !1,
                                     h = 0,
                                     m = o.length;
                                 "separator" === o[0].type && (a += "top ", h = 1), "separator" === o[o.length - 1].type && (a += "bottom ", m -= 1);
-                                for (var c = h; c < m; c++) "align" === o[c].type ? (i += Pr[o[c].align], l && (s += "none "), l = !0) : "separator" === o[c].type && l && (s += "|" === o[c].separator ? "solid " : "dashed ", l = !1);
+                                for (var c = h; c < m; c++) "align" === o[c].type ? (i += Nr[o[c].align], l && (s += "none "), l = !0) : "separator" === o[c].type && l && (s += "|" === o[c].separator ? "solid " : "dashed ", l = !1);
                                 r.setAttribute("columnalign", i.trim()), /[sd]/.test(s) && r.setAttribute("columnlines", s.trim())
                             }
                             if ("align" === e.colSeparationType) {
                                 for (var u = e.cols || [], p = "", d = 1; d < u.length; d++) p += d % 2 ? "0em " : "1em ";
                                 r.setAttribute("columnspacing", p.trim())
                             } else "alignat" === e.colSeparationType ? r.setAttribute("columnspacing", "0em") : "small" === e.colSeparationType ? r.setAttribute("columnspacing", "0.2778em") : r.setAttribute("columnspacing", "1em");
                             var f = "",
                                 g = e.hLinesBeforeRow;
                             a += g[0].length > 0 ? "left " : "", a += g[g.length - 1].length > 0 ? "right " : "";
                             for (var v = 1; v < g.length - 1; v++) f += 0 === g[v].length ? "none " : g[v][0] ? "dashed " : "solid ";
-                            return /[sd]/.test(f) && r.setAttribute("rowlines", f.trim()), "" !== a && (r = new Nt.MathNode("menclose", [r])).setAttribute("notation", a.trim()), e.arraystretch && e.arraystretch < 1 && (r = new Nt.MathNode("mstyle", [r])).setAttribute("scriptlevel", "1"), r
+                            return /[sd]/.test(f) && r.setAttribute("rowlines", f.trim()), "" !== a && (r = new zt.MathNode("menclose", [r])).setAttribute("notation", a.trim()), e.arraystretch && e.arraystretch < 1 && (r = new zt.MathNode("mstyle", [r])).setAttribute("scriptlevel", "1"), r
                         },
-                        Hr = function(e, t) {
+                        Or = function(e, t) {
                             var r, n = [],
-                                a = Rr(e.parser, {
+                                a = Br(e.parser, {
                                     cols: n,
                                     addJot: !0
                                 }, "display"),
                                 i = 0,
                                 s = {
                                     type: "ordgroup",
                                     mode: e.mode,
                                     body: []
                                 };
                             if (t[0] && "ordgroup" === t[0].type) {
-                                for (var l = "", h = 0; h < t[0].body.length; h++) l += _t(t[0].body[h], "textord").text;
+                                for (var l = "", h = 0; h < t[0].body.length; h++) l += Ht(t[0].body[h], "textord").text;
                                 r = Number(l), i = 2 * r
                             }
                             var m = !i;
                             a.body.forEach((function(e) {
                                 for (var t = 1; t < e.length; t += 2) {
-                                    var n = _t(e[t], "styling");
-                                    _t(n.body[0], "ordgroup").body.unshift(s)
+                                    var n = Ht(e[t], "styling");
+                                    Ht(n.body[0], "ordgroup").body.unshift(s)
                                 }
                                 if (m) i < e.length && (i = e.length);
                                 else {
                                     var a = e.length / 2;
                                     if (r < a) throw new o("Too many math in a row: expected " + r + ", but got " + a, e[0])
                                 }
                             }));
@@ -5194,24 +5200,24 @@
                                     align: u,
                                     pregap: p,
                                     postgap: 0
                                 }
                             }
                             return a.colSeparationType = m ? "align" : "alignat", a
                         };
-                    Ir({
+                    Ar({
                         type: "array",
                         names: ["array", "darray"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = {
-                                cols: (Xt(t[0]) ? [t[0]] : _t(t[0], "ordgroup").body).map((function(e) {
-                                    var t = Wt(e).text;
+                                cols: (Vt(t[0]) ? [t[0]] : Ht(t[0], "ordgroup").body).map((function(e) {
+                                    var t = Ft(e).text;
                                     if (-1 !== "lcr".indexOf(t)) return {
                                         type: "align",
                                         align: t
                                     };
                                     if ("|" === t) return {
                                         type: "separator",
                                         separator: "|"
@@ -5220,359 +5226,359 @@
                                         type: "separator",
                                         separator: ":"
                                     };
                                     throw new o("Unknown column alignment: " + t, e)
                                 })),
                                 hskipBeforeAndAfter: !0
                             };
-                            return Rr(e.parser, r, Er(e.envName))
+                            return Br(e.parser, r, Cr(e.envName))
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["matrix", "pmatrix", "bmatrix", "Bmatrix", "vmatrix", "Vmatrix"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
                             var t = {
                                     matrix: null,
                                     pmatrix: ["(", ")"],
                                     bmatrix: ["[", "]"],
                                     Bmatrix: ["\\{", "\\}"],
                                     vmatrix: ["|", "|"],
                                     Vmatrix: ["\\Vert", "\\Vert"]
                                 } [e.envName],
-                                r = Rr(e.parser, {
+                                r = Br(e.parser, {
                                     hskipBeforeAndAfter: !1
-                                }, Er(e.envName));
+                                }, Cr(e.envName));
                             return t ? {
                                 type: "leftright",
                                 mode: e.mode,
                                 body: [r],
                                 left: t[0],
                                 right: t[1],
                                 rightColor: void 0
                             } : r
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["smallmatrix"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
-                            var t = Rr(e.parser, {
+                            var t = Br(e.parser, {
                                 arraystretch: .5
                             }, "script");
                             return t.colSeparationType = "small", t
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["subarray"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
-                            var r = (Xt(t[0]) ? [t[0]] : _t(t[0], "ordgroup").body).map((function(e) {
-                                var t = Wt(e).text;
+                            var r = (Vt(t[0]) ? [t[0]] : Ht(t[0], "ordgroup").body).map((function(e) {
+                                var t = Ft(e).text;
                                 if (-1 !== "lc".indexOf(t)) return {
                                     type: "align",
                                     align: t
                                 };
                                 throw new o("Unknown column alignment: " + t, e)
                             }));
                             if (r.length > 1) throw new o("{subarray} can contain only one column");
                             var n = {
                                 cols: r,
                                 hskipBeforeAndAfter: !1,
                                 arraystretch: .5
                             };
-                            if ((n = Rr(e.parser, n, "script")).body.length > 0 && n.body[0].length > 1) throw new o("{subarray} can contain only one column");
+                            if ((n = Br(e.parser, n, "script")).body.length > 0 && n.body[0].length > 1) throw new o("{subarray} can contain only one column");
                             return n
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["cases", "dcases", "rcases", "drcases"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
-                            var t = Rr(e.parser, {
+                            var t = Br(e.parser, {
                                 arraystretch: 1.2,
                                 cols: [{
                                     type: "align",
                                     align: "l",
                                     pregap: 0,
                                     postgap: 1
                                 }, {
                                     type: "align",
                                     align: "l",
                                     pregap: 0,
                                     postgap: 0
                                 }]
-                            }, Er(e.envName));
+                            }, Cr(e.envName));
                             return {
                                 type: "leftright",
                                 mode: e.mode,
                                 body: [t],
                                 left: e.envName.indexOf("r") > -1 ? "." : "\\{",
                                 right: e.envName.indexOf("r") > -1 ? "\\}" : ".",
                                 rightColor: void 0
                             }
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["aligned"],
                         props: {
                             numArgs: 0
                         },
-                        handler: Hr,
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        handler: Or,
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["gathered"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
-                            return Rr(e.parser, {
+                            return Br(e.parser, {
                                 cols: [{
                                     type: "align",
                                     align: "c"
                                 }],
                                 addJot: !0
                             }, "display")
                         },
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), Ir({
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), Ar({
                         type: "array",
                         names: ["alignedat"],
                         props: {
                             numArgs: 1
                         },
-                        handler: Hr,
-                        htmlBuilder: Lr,
-                        mathmlBuilder: Dr
-                    }), ct({
+                        handler: Or,
+                        htmlBuilder: qr,
+                        mathmlBuilder: Ir
+                    }), it({
                         type: "text",
                         names: ["\\hline", "\\hdashline"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
                             allowedInMath: !0
                         },
                         handler: function(e, t) {
                             throw new o(e.funcName + " valid only within array environment")
                         }
                     });
-                    var Fr = Nr;
-                    ct({
+                    var Rr = zr;
+                    it({
                         type: "environment",
                         names: ["\\begin", "\\end"],
                         props: {
                             numArgs: 1,
                             argTypes: ["text"]
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
                                 a = t[0];
                             if ("ordgroup" !== a.type) throw new o("Invalid environment name", a);
-                            for (var i = "", s = 0; s < a.body.length; ++s) i += _t(a.body[s], "textord").text;
+                            for (var i = "", s = 0; s < a.body.length; ++s) i += Ht(a.body[s], "textord").text;
                             if ("\\begin" === n) {
-                                if (!Fr.hasOwnProperty(i)) throw new o("No such environment: " + i, a);
-                                var l = Fr[i],
+                                if (!Rr.hasOwnProperty(i)) throw new o("No such environment: " + i, a);
+                                var l = Rr[i],
                                     h = r.parseArguments("\\begin{" + i + "}", l),
                                     m = h.args,
                                     c = h.optArgs,
                                     u = {
                                         mode: r.mode,
                                         envName: i,
                                         parser: r
                                     },
                                     p = l.handler(u, m, c);
                                 r.expect("\\end", !1);
                                 var d = r.nextToken,
-                                    f = _t(r.parseFunction(), "environment");
+                                    f = Ht(r.parseFunction(), "environment");
                                 if (f.name !== i) throw new o("Mismatch: \\begin{" + i + "} matched by \\end{" + f.name + "}", d);
                                 return p
                             }
                             return {
                                 type: "environment",
                                 mode: r.mode,
                                 name: i,
                                 nameGroup: a
                             }
                         }
                     });
-                    var Vr = rt.makeSpan;
+                    var Er = Ze.makeSpan;
 
-                    function Ur(e, t) {
-                        var r = yt(e.body, t, !0);
-                        return Vr([e.mclass], r, t)
+                    function Lr(e, t) {
+                        var r = pt(e.body, t, !0);
+                        return Er([e.mclass], r, t)
                     }
 
-                    function Gr(e, t) {
-                        var r, n = Et(e.body, t);
-                        return "minner" === e.mclass ? Nt.newDocumentFragment(n) : ("mord" === e.mclass ? e.isCharacterBox ? (r = n[0]).type = "mi" : r = new Nt.MathNode("mi", n) : (e.isCharacterBox ? (r = n[0]).type = "mo" : r = new Nt.MathNode("mo", n), "mbin" === e.mclass ? (r.attributes.lspace = "0.22em", r.attributes.rspace = "0.22em") : "mpunct" === e.mclass ? (r.attributes.lspace = "0em", r.attributes.rspace = "0.17em") : "mopen" !== e.mclass && "mclose" !== e.mclass || (r.attributes.lspace = "0em", r.attributes.rspace = "0em")), r)
+                    function Pr(e, t) {
+                        var r, n = Ct(e.body, t);
+                        return "minner" === e.mclass ? zt.newDocumentFragment(n) : ("mord" === e.mclass ? e.isCharacterBox ? (r = n[0]).type = "mi" : r = new zt.MathNode("mi", n) : (e.isCharacterBox ? (r = n[0]).type = "mo" : r = new zt.MathNode("mo", n), "mbin" === e.mclass ? (r.attributes.lspace = "0.22em", r.attributes.rspace = "0.22em") : "mpunct" === e.mclass ? (r.attributes.lspace = "0em", r.attributes.rspace = "0.17em") : "mopen" !== e.mclass && "mclose" !== e.mclass || (r.attributes.lspace = "0em", r.attributes.rspace = "0em")), r)
                     }
-                    ct({
+                    it({
                         type: "mclass",
                         names: ["\\mathord", "\\mathbin", "\\mathrel", "\\mathopen", "\\mathclose", "\\mathpunct", "\\mathinner"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
                                 a = t[0];
                             return {
                                 type: "mclass",
                                 mode: r.mode,
                                 mclass: "m" + n.substr(5),
-                                body: pt(a),
-                                isCharacterBox: g(a)
+                                body: st(a),
+                                isCharacterBox: c.isCharacterBox(a)
                             }
                         },
-                        htmlBuilder: Ur,
-                        mathmlBuilder: Gr
+                        htmlBuilder: Lr,
+                        mathmlBuilder: Pr
                     });
-                    var Yr = function(e) {
+                    var Dr = function(e) {
                         var t = "ordgroup" === e.type && e.body.length ? e.body[0] : e;
                         return "atom" !== t.type || "bin" !== t.family && "rel" !== t.family ? "mord" : "m" + t.family
                     };
-                    ct({
+                    it({
                         type: "mclass",
                         names: ["\\@binrel"],
                         props: {
                             numArgs: 2
                         },
                         handler: function(e, t) {
                             return {
                                 type: "mclass",
                                 mode: e.parser.mode,
-                                mclass: Yr(t[0]),
+                                mclass: Dr(t[0]),
                                 body: [t[1]],
-                                isCharacterBox: g(t[1])
+                                isCharacterBox: c.isCharacterBox(t[1])
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "mclass",
                         names: ["\\stackrel", "\\overset", "\\underset"],
                         props: {
                             numArgs: 2
                         },
                         handler: function(e, t) {
                             var r, n = e.parser,
                                 a = e.funcName,
                                 i = t[1],
                                 o = t[0];
-                            r = "\\stackrel" !== a ? Yr(i) : "mrel";
+                            r = "\\stackrel" !== a ? Dr(i) : "mrel";
                             var s = {
                                     type: "op",
                                     mode: i.mode,
                                     limits: !0,
                                     alwaysHandleSupSub: !0,
                                     parentIsSupSub: !1,
                                     symbol: !1,
                                     suppressBaseShift: "\\stackrel" !== a,
-                                    body: pt(i)
+                                    body: st(i)
                                 },
                                 l = {
                                     type: "supsub",
                                     mode: o.mode,
                                     base: s,
                                     sup: "\\underset" === a ? null : o,
                                     sub: "\\underset" === a ? o : null
                                 };
                             return {
                                 type: "mclass",
                                 mode: n.mode,
                                 mclass: r,
                                 body: [l],
-                                isCharacterBox: g(l)
+                                isCharacterBox: c.isCharacterBox(l)
                             }
                         },
-                        htmlBuilder: Ur,
-                        mathmlBuilder: Gr
+                        htmlBuilder: Lr,
+                        mathmlBuilder: Pr
                     });
-                    var _r = function(e, t) {
+                    var Hr = function(e, t) {
                             var r = e.font,
                                 n = t.withFont(r);
-                            return zt(e.body, n)
+                            return yt(e.body, n)
                         },
-                        Wr = function(e, t) {
+                        Fr = function(e, t) {
                             var r = e.font,
                                 n = t.withFont(r);
-                            return Pt(e.body, n)
+                            return Nt(e.body, n)
                         },
-                        Xr = {
+                        Vr = {
                             "\\Bbb": "\\mathbb",
                             "\\bold": "\\mathbf",
                             "\\frak": "\\mathfrak",
                             "\\bm": "\\boldsymbol"
                         };
-                    ct({
+                    it({
                         type: "font",
                         names: ["\\mathrm", "\\mathit", "\\mathbf", "\\mathnormal", "\\mathbb", "\\mathcal", "\\mathfrak", "\\mathscr", "\\mathsf", "\\mathtt", "\\Bbb", "\\bold", "\\frak"],
                         props: {
                             numArgs: 1,
                             greediness: 2
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
                                 a = t[0],
                                 i = n;
-                            return i in Xr && (i = Xr[i]), {
+                            return i in Vr && (i = Vr[i]), {
                                 type: "font",
                                 mode: r.mode,
                                 font: i.slice(1),
                                 body: a
                             }
                         },
-                        htmlBuilder: _r,
-                        mathmlBuilder: Wr
-                    }), ct({
+                        htmlBuilder: Hr,
+                        mathmlBuilder: Fr
+                    }), it({
                         type: "mclass",
                         names: ["\\boldsymbol", "\\bm"],
                         props: {
                             numArgs: 1,
                             greediness: 2
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = t[0],
-                                a = g(n);
+                                a = c.isCharacterBox(n);
                             return {
                                 type: "mclass",
                                 mode: r.mode,
-                                mclass: Yr(n),
+                                mclass: Dr(n),
                                 body: [{
                                     type: "font",
                                     mode: r.mode,
                                     font: "boldsymbol",
                                     body: n
                                 }],
                                 isCharacterBox: a
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "font",
                         names: ["\\rm", "\\sf", "\\tt", "\\bf", "\\it", "\\cal"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
@@ -5588,98 +5594,100 @@
                                 body: {
                                     type: "ordgroup",
                                     mode: r.mode,
                                     body: o
                                 }
                             }
                         },
-                        htmlBuilder: _r,
-                        mathmlBuilder: Wr
+                        htmlBuilder: Hr,
+                        mathmlBuilder: Fr
                     });
-                    var jr = function(e, t) {
+                    var Ur = function(e, t) {
                             var r = t;
-                            return "display" === e ? r = r.id >= T.SCRIPT.id ? r.text() : T.DISPLAY : "text" === e && r.size === T.DISPLAY.size ? r = T.TEXT : "script" === e ? r = T.SCRIPT : "scriptscript" === e && (r = T.SCRIPTSCRIPT), r
+                            return "display" === e ? r = r.id >= w.SCRIPT.id ? r.text() : w.DISPLAY : "text" === e && r.size === w.DISPLAY.size ? r = w.TEXT : "script" === e ? r = w.SCRIPT : "scriptscript" === e && (r = w.SCRIPTSCRIPT), r
                         },
-                        $r = function(e, t) {
-                            var r, n = jr(e.size, t.style),
+                        Gr = function(e, t) {
+                            var r, n = Ur(e.size, t.style),
                                 a = n.fracNum(),
                                 i = n.fracDen();
                             r = t.havingStyle(a);
-                            var o = zt(e.numer, r, t);
+                            var o = yt(e.numer, r, t);
                             if (e.continued) {
                                 var s = 8.5 / t.fontMetrics().ptPerEm,
                                     l = 3.5 / t.fontMetrics().ptPerEm;
                                 o.height = o.height < s ? s : o.height, o.depth = o.depth < l ? l : o.depth
                             }
                             r = t.havingStyle(i);
-                            var h, m, c, u, p, d, f, g, v, b, y = zt(e.denom, r, t);
-                            if (e.hasBarLine ? (e.barSize ? (m = _e(e.barSize, t), h = rt.makeLineSpan("frac-line", t, m)) : h = rt.makeLineSpan("frac-line", t), m = h.height, c = h.height) : (h = null, m = 0, c = t.fontMetrics().defaultRuleThickness), n.size === T.DISPLAY.size || "display" === e.size ? (u = t.fontMetrics().num1, p = m > 0 ? 3 * c : 7 * c, d = t.fontMetrics().denom1) : (m > 0 ? (u = t.fontMetrics().num2, p = c) : (u = t.fontMetrics().num3, p = 3 * c), d = t.fontMetrics().denom2), h) {
+                            var h, m, c, u, p, d, f, g, v, b, y = yt(e.denom, r, t);
+                            if (e.hasBarLine ? (e.barSize ? (m = He(e.barSize, t), h = Ze.makeLineSpan("frac-line", t, m)) : h = Ze.makeLineSpan("frac-line", t), m = h.height, c = h.height) : (h = null, m = 0, c = t.fontMetrics().defaultRuleThickness), n.size === w.DISPLAY.size || "display" === e.size ? (u = t.fontMetrics().num1, p = m > 0 ? 3 * c : 7 * c, d = t.fontMetrics().denom1) : (m > 0 ? (u = t.fontMetrics().num2, p = c) : (u = t.fontMetrics().num3, p = 3 * c), d = t.fontMetrics().denom2), h) {
                                 var x = t.fontMetrics().axisHeight;
-                                u - o.depth - (x + .5 * m) < p && (u += p - (u - o.depth - (x + .5 * m))), x - .5 * m - (y.height - d) < p && (d += p - (x - .5 * m - (y.height - d))), f = rt.makeVList({
+                                u - o.depth - (x + .5 * m) < p && (u += p - (u - o.depth - (x + .5 * m))), x - .5 * m - (y.height - d) < p && (d += p - (x - .5 * m - (y.height - d)));
+                                var k = -(x - .5 * m);
+                                f = Ze.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
                                         elem: y,
                                         shift: d
                                     }, {
                                         type: "elem",
                                         elem: h,
-                                        shift: -(x - .5 * m)
+                                        shift: k
                                     }, {
                                         type: "elem",
                                         elem: o,
                                         shift: -u
                                     }]
                                 }, t)
                             } else {
-                                var w = u - o.depth - (y.height - d);
-                                w < p && (u += .5 * (p - w), d += .5 * (p - w)), f = rt.makeVList({
+                                var S = u - o.depth - (y.height - d);
+                                S < p && (u += .5 * (p - S), d += .5 * (p - S)), f = Ze.makeVList({
                                     positionType: "individualShift",
                                     children: [{
                                         type: "elem",
                                         elem: y,
                                         shift: d
                                     }, {
                                         type: "elem",
                                         elem: o,
                                         shift: -u
                                     }]
                                 }, t)
                             }
-                            return r = t.havingStyle(n), f.height *= r.sizeMultiplier / t.sizeMultiplier, f.depth *= r.sizeMultiplier / t.sizeMultiplier, g = n.size === T.DISPLAY.size ? t.fontMetrics().delim1 : t.fontMetrics().delim2, v = null == e.leftDelim ? Mt(t, ["mopen"]) : Sr(e.leftDelim, g, !0, t.havingStyle(n), e.mode, ["mopen"]), b = e.continued ? rt.makeSpan([]) : null == e.rightDelim ? Mt(t, ["mclose"]) : Sr(e.rightDelim, g, !0, t.havingStyle(n), e.mode, ["mclose"]), rt.makeSpan(["mord"].concat(r.sizingClasses(t)), [v, rt.makeSpan(["mfrac"], [f]), b], t)
+                            return r = t.havingStyle(n), f.height *= r.sizeMultiplier / t.sizeMultiplier, f.depth *= r.sizeMultiplier / t.sizeMultiplier, g = n.size === w.DISPLAY.size ? t.fontMetrics().delim1 : t.fontMetrics().delim2, v = null == e.leftDelim ? bt(t, ["mopen"]) : vr(e.leftDelim, g, !0, t.havingStyle(n), e.mode, ["mopen"]), b = e.continued ? Ze.makeSpan([]) : null == e.rightDelim ? bt(t, ["mclose"]) : vr(e.rightDelim, g, !0, t.havingStyle(n), e.mode, ["mclose"]), Ze.makeSpan(["mord"].concat(r.sizingClasses(t)), [v, Ze.makeSpan(["mfrac"], [f]), b], t)
                         },
-                        Zr = function(e, t) {
-                            var r = new Nt.MathNode("mfrac", [Pt(e.numer, t), Pt(e.denom, t)]);
+                        Yr = function(e, t) {
+                            var r = new zt.MathNode("mfrac", [Nt(e.numer, t), Nt(e.denom, t)]);
                             if (e.hasBarLine) {
                                 if (e.barSize) {
-                                    var n = _e(e.barSize, t);
+                                    var n = He(e.barSize, t);
                                     r.setAttribute("linethickness", n + "em")
                                 }
                             } else r.setAttribute("linethickness", "0px");
-                            var a = jr(e.size, t.style);
+                            var a = Ur(e.size, t.style);
                             if (a.size !== t.style.size) {
-                                r = new Nt.MathNode("mstyle", [r]);
-                                var i = a.size === T.DISPLAY.size ? "true" : "false";
+                                r = new zt.MathNode("mstyle", [r]);
+                                var i = a.size === w.DISPLAY.size ? "true" : "false";
                                 r.setAttribute("displaystyle", i), r.setAttribute("scriptlevel", "0")
                             }
                             if (null != e.leftDelim || null != e.rightDelim) {
                                 var o = [];
                                 if (null != e.leftDelim) {
-                                    var s = new Nt.MathNode("mo", [new Nt.TextNode(e.leftDelim.replace("\\", ""))]);
+                                    var s = new zt.MathNode("mo", [new zt.TextNode(e.leftDelim.replace("\\", ""))]);
                                     s.setAttribute("fence", "true"), o.push(s)
                                 }
                                 if (o.push(r), null != e.rightDelim) {
-                                    var l = new Nt.MathNode("mo", [new Nt.TextNode(e.rightDelim.replace("\\", ""))]);
+                                    var l = new zt.MathNode("mo", [new zt.TextNode(e.rightDelim.replace("\\", ""))]);
                                     l.setAttribute("fence", "true"), o.push(l)
                                 }
-                                return Ot(o)
+                                return Tt(o)
                             }
                             return r
                         };
-                    ct({
+                    it({
                         type: "genfrac",
                         names: ["\\cfrac", "\\dfrac", "\\frac", "\\tfrac", "\\dbinom", "\\binom", "\\tbinom", "\\\\atopfrac", "\\\\bracefrac", "\\\\brackfrac"],
                         props: {
                             numArgs: 2,
                             greediness: 2
                         },
                         handler: function(e, t) {
@@ -5733,17 +5741,17 @@
                                 hasBarLine: r,
                                 leftDelim: s,
                                 rightDelim: l,
                                 size: h,
                                 barSize: null
                             }
                         },
-                        htmlBuilder: $r,
-                        mathmlBuilder: Zr
-                    }), ct({
+                        htmlBuilder: Gr,
+                        mathmlBuilder: Yr
+                    }), it({
                         type: "infix",
                         names: ["\\over", "\\choose", "\\atop", "\\brace", "\\brack"],
                         props: {
                             numArgs: 0,
                             infix: !0
                         },
                         handler: function(e) {
@@ -5773,92 +5781,92 @@
                                 type: "infix",
                                 mode: r.mode,
                                 replaceWith: t,
                                 token: a
                             }
                         }
                     });
-                    var Kr = ["display", "text", "script", "scriptscript"],
-                        Jr = function(e) {
+                    var _r = ["display", "text", "script", "scriptscript"],
+                        Wr = function(e) {
                             var t = null;
                             return e.length > 0 && (t = "." === (t = e) ? null : t), t
                         };
-                    ct({
+                    it({
                         type: "genfrac",
                         names: ["\\genfrac"],
                         props: {
                             numArgs: 6,
                             greediness: 6,
                             argTypes: ["math", "math", "size", "text", "math", "math"]
                         },
                         handler: function(e, t) {
                             var r, n = e.parser,
                                 a = t[4],
                                 i = t[5],
-                                o = "atom" === t[0].type && "open" === t[0].family ? Jr(t[0].text) : null,
-                                s = "atom" === t[1].type && "close" === t[1].family ? Jr(t[1].text) : null,
-                                l = _t(t[2], "size"),
+                                o = "atom" === t[0].type && "open" === t[0].family ? Wr(t[0].text) : null,
+                                s = "atom" === t[1].type && "close" === t[1].family ? Wr(t[1].text) : null,
+                                l = Ht(t[2], "size"),
                                 h = null;
                             r = !!l.isBlank || (h = l.value).number > 0;
                             var m = "auto",
                                 c = t[3];
                             if ("ordgroup" === c.type) {
                                 if (c.body.length > 0) {
-                                    var u = _t(c.body[0], "textord");
-                                    m = Kr[Number(u.text)]
+                                    var u = Ht(c.body[0], "textord");
+                                    m = _r[Number(u.text)]
                                 }
-                            } else c = _t(c, "textord"), m = Kr[Number(c.text)];
+                            } else c = Ht(c, "textord"), m = _r[Number(c.text)];
                             return {
                                 type: "genfrac",
                                 mode: n.mode,
                                 numer: a,
                                 denom: i,
                                 continued: !1,
                                 hasBarLine: r,
                                 barSize: h,
                                 leftDelim: o,
                                 rightDelim: s,
                                 size: m
                             }
                         },
-                        htmlBuilder: $r,
-                        mathmlBuilder: Zr
-                    }), ct({
+                        htmlBuilder: Gr,
+                        mathmlBuilder: Yr
+                    }), it({
                         type: "infix",
                         names: ["\\above"],
                         props: {
                             numArgs: 1,
                             argTypes: ["size"],
                             infix: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = (e.funcName, e.token);
                             return {
                                 type: "infix",
                                 mode: r.mode,
                                 replaceWith: "\\\\abovefrac",
-                                size: _t(t[0], "size").value,
+                                size: Ht(t[0], "size").value,
                                 token: n
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "genfrac",
                         names: ["\\\\abovefrac"],
                         props: {
                             numArgs: 3,
                             argTypes: ["math", "size", "math"]
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = (e.funcName, t[0]),
                                 a = function(e) {
                                     if (!e) throw new Error("Expected non-null, but got " + String(e));
                                     return e
-                                }(_t(t[1], "infix").size),
+                                }(Ht(t[1], "infix").size),
                                 i = t[2],
                                 o = a.number > 0;
                             return {
                                 type: "genfrac",
                                 mode: r.mode,
                                 numer: n,
                                 denom: i,
@@ -5866,79 +5874,79 @@
                                 hasBarLine: o,
                                 barSize: a,
                                 leftDelim: null,
                                 rightDelim: null,
                                 size: "auto"
                             }
                         },
-                        htmlBuilder: $r,
-                        mathmlBuilder: Zr
+                        htmlBuilder: Gr,
+                        mathmlBuilder: Yr
                     });
-                    var Qr = function(e, t) {
+                    var Xr = function(e, t) {
                         var r, n, a = t.style;
-                        "supsub" === e.type ? (r = e.sup ? zt(e.sup, t.havingStyle(a.sup()), t) : zt(e.sub, t.havingStyle(a.sub()), t), n = _t(e.base, "horizBrace")) : n = _t(e, "horizBrace");
-                        var i, o = zt(n.base, t.havingBaseStyle(T.DISPLAY)),
-                            s = Yt(n, t);
-                        if (n.isOver ? (i = rt.makeVList({
+                        "supsub" === e.type ? (r = e.sup ? yt(e.sup, t.havingStyle(a.sup()), t) : yt(e.sub, t.havingStyle(a.sub()), t), n = Ht(e.base, "horizBrace")) : n = Ht(e, "horizBrace");
+                        var i, o = yt(n.base, t.havingBaseStyle(w.DISPLAY)),
+                            s = Dt(n, t);
+                        if (n.isOver ? (i = Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: o
                                 }, {
                                     type: "kern",
                                     size: .1
                                 }, {
                                     type: "elem",
                                     elem: s
                                 }]
-                            }, t)).children[0].children[0].children[1].classes.push("svg-align") : (i = rt.makeVList({
+                            }, t)).children[0].children[0].children[1].classes.push("svg-align") : (i = Ze.makeVList({
                                 positionType: "bottom",
                                 positionData: o.depth + .1 + s.height,
                                 children: [{
                                     type: "elem",
                                     elem: s
                                 }, {
                                     type: "kern",
                                     size: .1
                                 }, {
                                     type: "elem",
                                     elem: o
                                 }]
                             }, t)).children[0].children[0].children[0].classes.push("svg-align"), r) {
-                            var l = rt.makeSpan(["mord", n.isOver ? "mover" : "munder"], [i], t);
-                            i = n.isOver ? rt.makeVList({
+                            var l = Ze.makeSpan(["mord", n.isOver ? "mover" : "munder"], [i], t);
+                            i = n.isOver ? Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: l
                                 }, {
                                     type: "kern",
                                     size: .2
                                 }, {
                                     type: "elem",
                                     elem: r
                                 }]
-                            }, t) : rt.makeVList({
+                            }, t) : Ze.makeVList({
                                 positionType: "bottom",
                                 positionData: l.depth + .2 + r.height + r.depth,
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }, {
                                     type: "kern",
                                     size: .2
                                 }, {
                                     type: "elem",
                                     elem: l
                                 }]
                             }, t)
                         }
-                        return rt.makeSpan(["mord", n.isOver ? "mover" : "munder"], [i], t)
+                        return Ze.makeSpan(["mord", n.isOver ? "mover" : "munder"], [i], t)
                     };
-                    ct({
+                    it({
                         type: "horizBrace",
                         names: ["\\overbrace", "\\underbrace"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
@@ -5947,60 +5955,60 @@
                                 type: "horizBrace",
                                 mode: r.mode,
                                 label: n,
                                 isOver: /^\\over/.test(n),
                                 base: t[0]
                             }
                         },
-                        htmlBuilder: Qr,
+                        htmlBuilder: Xr,
                         mathmlBuilder: function(e, t) {
-                            var r = Gt(e.label);
-                            return new Nt.MathNode(e.isOver ? "mover" : "munder", [Pt(e.base, t), r])
+                            var r = Pt(e.label);
+                            return new zt.MathNode(e.isOver ? "mover" : "munder", [Nt(e.base, t), r])
                         }
-                    }), ct({
+                    }), it({
                         type: "href",
                         names: ["\\href"],
                         props: {
                             numArgs: 2,
                             argTypes: ["url", "original"],
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = t[1],
-                                a = _t(t[0], "url").url;
+                                a = Ht(t[0], "url").url;
                             return r.settings.isTrusted({
                                 command: "\\href",
                                 url: a
                             }) ? {
                                 type: "href",
                                 mode: r.mode,
                                 href: a,
-                                body: pt(n)
+                                body: st(n)
                             } : r.formatUnsupportedCmd("\\href")
                         },
                         htmlBuilder: function(e, t) {
-                            var r = yt(e.body, t, !1);
-                            return rt.makeAnchor(e.href, [], r, t)
+                            var r = pt(e.body, t, !1);
+                            return Ze.makeAnchor(e.href, [], r, t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = Lt(e.body, t);
-                            return r instanceof Ct || (r = new Ct("mrow", [r])), r.setAttribute("href", e.href), r
+                            var r = qt(e.body, t);
+                            return r instanceof St || (r = new St("mrow", [r])), r.setAttribute("href", e.href), r
                         }
-                    }), ct({
+                    }), it({
                         type: "href",
                         names: ["\\url"],
                         props: {
                             numArgs: 1,
                             argTypes: ["url"],
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
-                                n = _t(t[0], "url").url;
+                                n = Ht(t[0], "url").url;
                             if (!r.settings.isTrusted({
                                     command: "\\url",
                                     url: n
                                 })) return r.formatUnsupportedCmd("\\url");
                             for (var a = [], i = 0; i < n.length; i++) {
                                 var o = n[i];
                                 "~" === o && (o = "\\textasciitilde"), a.push({
@@ -6015,29 +6023,29 @@
                                 font: "\\texttt",
                                 body: a
                             };
                             return {
                                 type: "href",
                                 mode: r.mode,
                                 href: n,
-                                body: pt(s)
+                                body: st(s)
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "html",
                         names: ["\\htmlClass", "\\htmlId", "\\htmlStyle", "\\htmlData"],
                         props: {
                             numArgs: 2,
                             argTypes: ["raw", "original"],
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r, n = e.parser,
                                 a = e.funcName,
-                                i = (e.token, _t(t[0], "raw").string),
+                                i = (e.token, Ht(t[0], "raw").string),
                                 s = t[1];
                             n.settings.strict && n.settings.reportNonstrict("htmlExtension", "HTML extension is disabled on strict mode");
                             var l = {};
                             switch (a) {
                                 case "\\htmlClass":
                                     l.class = i, r = {
                                         command: "\\htmlClass",
@@ -6070,66 +6078,66 @@
                                 default:
                                     throw new Error("Unrecognized html command")
                             }
                             return n.settings.isTrusted(r) ? {
                                 type: "html",
                                 mode: n.mode,
                                 attributes: l,
-                                body: pt(s)
+                                body: st(s)
                             } : n.formatUnsupportedCmd(a)
                         },
                         htmlBuilder: function(e, t) {
-                            var r = yt(e.body, t, !1),
+                            var r = pt(e.body, t, !1),
                                 n = ["enclosing"];
                             e.attributes.class && n.push.apply(n, e.attributes.class.trim().split(/\s+/));
-                            var a = rt.makeSpan(n, r, t);
+                            var a = Ze.makeSpan(n, r, t);
                             for (var i in e.attributes) "class" !== i && e.attributes.hasOwnProperty(i) && a.setAttribute(i, e.attributes[i]);
                             return a
                         },
                         mathmlBuilder: function(e, t) {
-                            return Lt(e.body, t)
+                            return qt(e.body, t)
                         }
-                    }), ct({
+                    }), it({
                         type: "htmlmathml",
                         names: ["\\html@mathml"],
                         props: {
                             numArgs: 2,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             return {
                                 type: "htmlmathml",
                                 mode: e.parser.mode,
-                                html: pt(t[0]),
-                                mathml: pt(t[1])
+                                html: st(t[0]),
+                                mathml: st(t[1])
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = yt(e.html, t, !1);
-                            return rt.makeFragment(r)
+                            var r = pt(e.html, t, !1);
+                            return Ze.makeFragment(r)
                         },
                         mathmlBuilder: function(e, t) {
-                            return Lt(e.mathml, t)
+                            return qt(e.mathml, t)
                         }
                     });
-                    var en = function(e) {
+                    var jr = function(e) {
                         if (/^[-+]? *(\d+(\.\d*)?|\.\d+)$/.test(e)) return {
                             number: +e,
                             unit: "bp"
                         };
                         var t = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(e);
                         if (!t) throw new o("Invalid size: '" + e + "' in \\includegraphics");
                         var r = {
                             number: +(t[1] + t[2]),
                             unit: t[3]
                         };
-                        if (!Ye(r)) throw new o("Invalid unit: '" + r.unit + "' in \\includegraphics.");
+                        if (!De(r)) throw new o("Invalid unit: '" + r.unit + "' in \\includegraphics.");
                         return r
                     };
-                    ct({
+                    it({
                         type: "includegraphics",
                         names: ["\\includegraphics"],
                         props: {
                             numArgs: 1,
                             numOptionalArgs: 1,
                             argTypes: ["raw", "url"],
                             allowedInText: !1
@@ -6146,105 +6154,105 @@
                                 },
                                 s = {
                                     number: 0,
                                     unit: "em"
                                 },
                                 l = "";
                             if (r[0])
-                                for (var h = _t(r[0], "raw").string.split(","), m = 0; m < h.length; m++) {
+                                for (var h = Ht(r[0], "raw").string.split(","), m = 0; m < h.length; m++) {
                                     var c = h[m].split("=");
                                     if (2 === c.length) {
                                         var u = c[1].trim();
                                         switch (c[0].trim()) {
                                             case "alt":
                                                 l = u;
                                                 break;
                                             case "width":
-                                                a = en(u);
+                                                a = jr(u);
                                                 break;
                                             case "height":
-                                                i = en(u);
+                                                i = jr(u);
                                                 break;
                                             case "totalheight":
-                                                s = en(u);
+                                                s = jr(u);
                                                 break;
                                             default:
                                                 throw new o("Invalid key: '" + c[0] + "' in \\includegraphics.")
                                         }
                                     }
                                 }
-                            var p = _t(t[0], "url").url;
+                            var p = Ht(t[0], "url").url;
                             return "" === l && (l = (l = (l = p).replace(/^.*[\\/]/, "")).substring(0, l.lastIndexOf("."))), n.settings.isTrusted({
                                 command: "\\includegraphics",
                                 url: p
                             }) ? {
                                 type: "includegraphics",
                                 mode: n.mode,
                                 alt: l,
                                 width: a,
                                 height: i,
                                 totalheight: s,
                                 src: p
                             } : n.formatUnsupportedCmd("\\includegraphics")
                         },
                         htmlBuilder: function(e, t) {
-                            var r = _e(e.height, t),
+                            var r = He(e.height, t),
                                 n = 0;
-                            e.totalheight.number > 0 && (n = _e(e.totalheight, t) - r, n = Number(n.toFixed(2)));
+                            e.totalheight.number > 0 && (n = He(e.totalheight, t) - r, n = Number(n.toFixed(2)));
                             var a = 0;
-                            e.width.number > 0 && (a = _e(e.width, t));
+                            e.width.number > 0 && (a = He(e.width, t));
                             var i = {
                                 height: r + n + "em"
                             };
                             a > 0 && (i.width = a + "em"), n > 0 && (i.verticalAlign = -n + "em");
-                            var o = new H(e.src, e.alt, i);
+                            var o = new O(e.src, e.alt, i);
                             return o.height = r, o.depth = n, o
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mglyph", []);
+                            var r = new zt.MathNode("mglyph", []);
                             r.setAttribute("alt", e.alt);
-                            var n = _e(e.height, t),
+                            var n = He(e.height, t),
                                 a = 0;
-                            if (e.totalheight.number > 0 && (a = (a = _e(e.totalheight, t) - n).toFixed(2), r.setAttribute("valign", "-" + a + "em")), r.setAttribute("height", n + a + "em"), e.width.number > 0) {
-                                var i = _e(e.width, t);
+                            if (e.totalheight.number > 0 && (a = (a = He(e.totalheight, t) - n).toFixed(2), r.setAttribute("valign", "-" + a + "em")), r.setAttribute("height", n + a + "em"), e.width.number > 0) {
+                                var i = He(e.width, t);
                                 r.setAttribute("width", i + "em")
                             }
                             return r.setAttribute("src", e.src), r
                         }
-                    }), ct({
+                    }), it({
                         type: "kern",
                         names: ["\\kern", "\\mkern", "\\hskip", "\\mskip"],
                         props: {
                             numArgs: 1,
                             argTypes: ["size"],
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
-                                a = _t(t[0], "size");
+                                a = Ht(t[0], "size");
                             if (r.settings.strict) {
                                 var i = "m" === n[1],
                                     o = "mu" === a.value.unit;
                                 i ? (o || r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + n + " supports only mu units, not " + a.value.unit + " units"), "math" !== r.mode && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + n + " works only in math mode")) : o && r.settings.reportNonstrict("mathVsTextUnits", "LaTeX's " + n + " doesn't support mu units")
                             }
                             return {
                                 type: "kern",
                                 mode: r.mode,
                                 dimension: a.value
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            return rt.makeGlue(e.dimension, t)
+                            return Ze.makeGlue(e.dimension, t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = _e(e.dimension, t);
-                            return new Nt.SpaceNode(r)
+                            var r = He(e.dimension, t);
+                            return new zt.SpaceNode(r)
                         }
-                    }), ct({
+                    }), it({
                         type: "lap",
                         names: ["\\mathllap", "\\mathrlap", "\\mathclap"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
@@ -6256,29 +6264,29 @@
                                 mode: r.mode,
                                 alignment: n.slice(5),
                                 body: a
                             }
                         },
                         htmlBuilder: function(e, t) {
                             var r;
-                            "clap" === e.alignment ? (r = rt.makeSpan([], [zt(e.body, t)]), r = rt.makeSpan(["inner"], [r], t)) : r = rt.makeSpan(["inner"], [zt(e.body, t)]);
-                            var n = rt.makeSpan(["fix"], []),
-                                a = rt.makeSpan([e.alignment], [r, n], t),
-                                i = rt.makeSpan(["strut"]);
-                            return i.style.height = a.height + a.depth + "em", i.style.verticalAlign = -a.depth + "em", a.children.unshift(i), a = rt.makeSpan(["thinbox"], [a], t), rt.makeSpan(["mord", "vbox"], [a], t)
+                            "clap" === e.alignment ? (r = Ze.makeSpan([], [yt(e.body, t)]), r = Ze.makeSpan(["inner"], [r], t)) : r = Ze.makeSpan(["inner"], [yt(e.body, t)]);
+                            var n = Ze.makeSpan(["fix"], []),
+                                a = Ze.makeSpan([e.alignment], [r, n], t),
+                                i = Ze.makeSpan(["strut"]);
+                            return i.style.height = a.height + a.depth + "em", i.style.verticalAlign = -a.depth + "em", a.children.unshift(i), a = Ze.makeSpan(["thinbox"], [a], t), Ze.makeSpan(["mord", "vbox"], [a], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mpadded", [Pt(e.body, t)]);
+                            var r = new zt.MathNode("mpadded", [Nt(e.body, t)]);
                             if ("rlap" !== e.alignment) {
                                 var n = "llap" === e.alignment ? "-1" : "-0.5";
                                 r.setAttribute("lspace", n + "width")
                             }
                             return r.setAttribute("width", "0px"), r
                         }
-                    }), ct({
+                    }), it({
                         type: "styling",
                         names: ["\\(", "$"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
                             allowedInMath: !1
                         },
@@ -6292,85 +6300,85 @@
                             return n.expect(i), n.switchMode(a), {
                                 type: "styling",
                                 mode: n.mode,
                                 style: "text",
                                 body: o
                             }
                         }
-                    }), ct({
+                    }), it({
                         type: "text",
                         names: ["\\)", "\\]"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0,
                             allowedInMath: !1
                         },
                         handler: function(e, t) {
                             throw new o("Mismatched " + e.funcName)
                         }
                     });
-                    var tn = function(e, t) {
+                    var $r = function(e, t) {
                         switch (t.style.size) {
-                            case T.DISPLAY.size:
+                            case w.DISPLAY.size:
                                 return e.display;
-                            case T.TEXT.size:
+                            case w.TEXT.size:
                                 return e.text;
-                            case T.SCRIPT.size:
+                            case w.SCRIPT.size:
                                 return e.script;
-                            case T.SCRIPTSCRIPT.size:
+                            case w.SCRIPTSCRIPT.size:
                                 return e.scriptscript;
                             default:
                                 return e.text
                         }
                     };
-                    ct({
+                    it({
                         type: "mathchoice",
                         names: ["\\mathchoice"],
                         props: {
                             numArgs: 4
                         },
                         handler: function(e, t) {
                             return {
                                 type: "mathchoice",
                                 mode: e.parser.mode,
-                                display: pt(t[0]),
-                                text: pt(t[1]),
-                                script: pt(t[2]),
-                                scriptscript: pt(t[3])
+                                display: st(t[0]),
+                                text: st(t[1]),
+                                script: st(t[2]),
+                                scriptscript: st(t[3])
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = tn(e, t),
-                                n = yt(r, t, !1);
-                            return rt.makeFragment(n)
+                            var r = $r(e, t),
+                                n = pt(r, t, !1);
+                            return Ze.makeFragment(n)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = tn(e, t);
-                            return Lt(r, t)
+                            var r = $r(e, t);
+                            return qt(r, t)
                         }
                     });
-                    var rn = function(e, t, r, n, a, i, o) {
+                    var Zr = function(e, t, r, n, a, i, o) {
                             var s, l, h;
-                            if (e = rt.makeSpan([], [e]), t) {
-                                var m = zt(t, n.havingStyle(a.sup()), n);
+                            if (e = Ze.makeSpan([], [e]), t) {
+                                var m = yt(t, n.havingStyle(a.sup()), n);
                                 l = {
                                     elem: m,
                                     kern: Math.max(n.fontMetrics().bigOpSpacing1, n.fontMetrics().bigOpSpacing3 - m.depth)
                                 }
                             }
                             if (r) {
-                                var c = zt(r, n.havingStyle(a.sub()), n);
+                                var c = yt(r, n.havingStyle(a.sub()), n);
                                 s = {
                                     elem: c,
                                     kern: Math.max(n.fontMetrics().bigOpSpacing2, n.fontMetrics().bigOpSpacing4 - c.height)
                                 }
                             }
                             if (l && s) {
                                 var u = n.fontMetrics().bigOpSpacing5 + s.elem.height + s.elem.depth + s.kern + e.depth + o;
-                                h = rt.makeVList({
+                                h = Ze.makeVList({
                                     positionType: "bottom",
                                     positionData: u,
                                     children: [{
                                         type: "kern",
                                         size: n.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
@@ -6392,15 +6400,15 @@
                                     }, {
                                         type: "kern",
                                         size: n.fontMetrics().bigOpSpacing5
                                     }]
                                 }, n)
                             } else if (s) {
                                 var p = e.height - o;
-                                h = rt.makeVList({
+                                h = Ze.makeVList({
                                     positionType: "top",
                                     positionData: p,
                                     children: [{
                                         type: "kern",
                                         size: n.fontMetrics().bigOpSpacing5
                                     }, {
                                         type: "elem",
@@ -6413,15 +6421,15 @@
                                         type: "elem",
                                         elem: e
                                     }]
                                 }, n)
                             } else {
                                 if (!l) return e;
                                 var d = e.depth + o;
-                                h = rt.makeVList({
+                                h = Ze.makeVList({
                                     positionType: "bottom",
                                     positionData: d,
                                     children: [{
                                         type: "elem",
                                         elem: e
                                     }, {
                                         type: "kern",
@@ -6432,127 +6440,127 @@
                                         marginLeft: i + "em"
                                     }, {
                                         type: "kern",
                                         size: n.fontMetrics().bigOpSpacing5
                                     }]
                                 }, n)
                             }
-                            return rt.makeSpan(["mop", "op-limits"], [h], n)
+                            return Ze.makeSpan(["mop", "op-limits"], [h], n)
                         },
-                        nn = ["\\smallint"],
-                        an = function(e, t) {
+                        Kr = ["\\smallint"],
+                        Jr = function(e, t) {
                             var r, n, a, i = !1;
-                            "supsub" === e.type ? (r = e.sup, n = e.sub, a = _t(e.base, "op"), i = !0) : a = _t(e, "op");
+                            "supsub" === e.type ? (r = e.sup, n = e.sub, a = Ht(e.base, "op"), i = !0) : a = Ht(e, "op");
                             var o, s = t.style,
                                 l = !1;
-                            if (s.size === T.DISPLAY.size && a.symbol && !c(nn, a.name) && (l = !0), a.symbol) {
+                            if (s.size === w.DISPLAY.size && a.symbol && !c.contains(Kr, a.name) && (l = !0), a.symbol) {
                                 var h = l ? "Size2-Regular" : "Size1-Regular",
                                     m = "";
-                                if ("\\oiint" !== a.name && "\\oiiint" !== a.name || (m = a.name.substr(1), a.name = "oiint" === m ? "\\iint" : "\\iiint"), o = rt.makeSymbol(a.name, h, "math", t, ["mop", "op-symbol", l ? "large-op" : "small-op"]), m.length > 0) {
+                                if ("\\oiint" !== a.name && "\\oiiint" !== a.name || (m = a.name.substr(1), a.name = "oiint" === m ? "\\iint" : "\\iiint"), o = Ze.makeSymbol(a.name, h, "math", t, ["mop", "op-symbol", l ? "large-op" : "small-op"]), m.length > 0) {
                                     var u = o.italic,
-                                        p = rt.staticSvg(m + "Size" + (l ? "2" : "1"), t);
-                                    o = rt.makeVList({
+                                        p = Ze.staticSvg(m + "Size" + (l ? "2" : "1"), t);
+                                    o = Ze.makeVList({
                                         positionType: "individualShift",
                                         children: [{
                                             type: "elem",
                                             elem: o,
                                             shift: 0
                                         }, {
                                             type: "elem",
                                             elem: p,
                                             shift: l ? .08 : 0
                                         }]
                                     }, t), a.name = "\\" + m, o.classes.unshift("mop"), o.italic = u
                                 }
                             } else if (a.body) {
-                                var d = yt(a.body, t, !0);
-                                1 === d.length && d[0] instanceof V ? (o = d[0]).classes[0] = "mop" : o = rt.makeSpan(["mop"], rt.tryCombineChars(d), t)
+                                var d = pt(a.body, t, !0);
+                                1 === d.length && d[0] instanceof E ? (o = d[0]).classes[0] = "mop" : o = Ze.makeSpan(["mop"], Ze.tryCombineChars(d), t)
                             } else {
-                                for (var f = [], g = 1; g < a.name.length; g++) f.push(rt.mathsym(a.name[g], a.mode, t));
-                                o = rt.makeSpan(["mop"], f, t)
+                                for (var f = [], g = 1; g < a.name.length; g++) f.push(Ze.mathsym(a.name[g], a.mode, t));
+                                o = Ze.makeSpan(["mop"], f, t)
                             }
                             var v = 0,
                                 b = 0;
-                            return (o instanceof V || "\\oiint" === a.name || "\\oiiint" === a.name) && !a.suppressBaseShift && (v = (o.height - o.depth) / 2 - t.fontMetrics().axisHeight, b = o.italic), i ? rn(o, r, n, t, s, b, v) : (v && (o.style.position = "relative", o.style.top = v + "em"), o)
+                            return (o instanceof E || "\\oiint" === a.name || "\\oiiint" === a.name) && !a.suppressBaseShift && (v = (o.height - o.depth) / 2 - t.fontMetrics().axisHeight, b = o.italic), i ? Zr(o, r, n, t, s, b, v) : (v && (o.style.position = "relative", o.style.top = v + "em"), o)
                         },
-                        on = function(e, t) {
+                        Qr = function(e, t) {
                             var r;
-                            if (e.symbol) r = new Ct("mo", [It(e.name, e.mode)]), c(nn, e.name) && r.setAttribute("largeop", "false");
-                            else if (e.body) r = new Ct("mo", Et(e.body, t));
+                            if (e.symbol) r = new St("mo", [At(e.name, e.mode)]), c.contains(Kr, e.name) && r.setAttribute("largeop", "false");
+                            else if (e.body) r = new St("mo", Ct(e.body, t));
                             else {
-                                r = new Ct("mi", [new qt(e.name.slice(1))]);
-                                var n = new Ct("mo", [It("⁡", "text")]);
-                                r = e.parentIsSupSub ? new Ct("mo", [r, n]) : Bt([r, n])
+                                r = new St("mi", [new Mt(e.name.slice(1))]);
+                                var n = new St("mo", [At("⁡", "text")]);
+                                r = e.parentIsSupSub ? new St("mo", [r, n]) : kt([r, n])
                             }
                             return r
                         },
-                        sn = {
+                        en = {
                             "∏": "\\prod",
                             "∐": "\\coprod",
                             "∑": "\\sum",
                             "⋀": "\\bigwedge",
                             "⋁": "\\bigvee",
                             "⋂": "\\bigcap",
                             "⋃": "\\bigcup",
                             "⨀": "\\bigodot",
                             "⨁": "\\bigoplus",
                             "⨂": "\\bigotimes",
                             "⨄": "\\biguplus",
                             "⨆": "\\bigsqcup"
                         };
-                    ct({
+                    it({
                         type: "op",
                         names: ["\\coprod", "\\bigvee", "\\bigwedge", "\\biguplus", "\\bigcap", "\\bigcup", "\\intop", "\\prod", "\\sum", "\\bigotimes", "\\bigoplus", "\\bigodot", "\\bigsqcup", "\\smallint", "∏", "∐", "∑", "⋀", "⋁", "⋂", "⋃", "⨀", "⨁", "⨂", "⨄", "⨆"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName;
-                            return 1 === n.length && (n = sn[n]), {
+                            return 1 === n.length && (n = en[n]), {
                                 type: "op",
                                 mode: r.mode,
                                 limits: !0,
                                 parentIsSupSub: !1,
                                 symbol: !0,
                                 name: n
                             }
                         },
-                        htmlBuilder: an,
-                        mathmlBuilder: on
-                    }), ct({
+                        htmlBuilder: Jr,
+                        mathmlBuilder: Qr
+                    }), it({
                         type: "op",
                         names: ["\\mathop"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = t[0];
                             return {
                                 type: "op",
                                 mode: r.mode,
                                 limits: !1,
                                 parentIsSupSub: !1,
                                 symbol: !1,
-                                body: pt(n)
+                                body: st(n)
                             }
                         },
-                        htmlBuilder: an,
-                        mathmlBuilder: on
+                        htmlBuilder: Jr,
+                        mathmlBuilder: Qr
                     });
-                    var ln = {
+                    var tn = {
                         "∫": "\\int",
                         "∬": "\\iint",
                         "∭": "\\iiint",
                         "∮": "\\oint",
                         "∯": "\\oiint",
                         "∰": "\\oiiint"
                     };
-                    ct({
+                    it({
                         type: "op",
                         names: ["\\arcsin", "\\arccos", "\\arctan", "\\arctg", "\\arcctg", "\\arg", "\\ch", "\\cos", "\\cosec", "\\cosh", "\\cot", "\\cotg", "\\coth", "\\csc", "\\ctg", "\\cth", "\\deg", "\\dim", "\\exp", "\\hom", "\\ker", "\\lg", "\\ln", "\\log", "\\sec", "\\sin", "\\sinh", "\\sh", "\\tan", "\\tanh", "\\tg", "\\th"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
                             var t = e.parser,
@@ -6562,17 +6570,17 @@
                                 mode: t.mode,
                                 limits: !1,
                                 parentIsSupSub: !1,
                                 symbol: !1,
                                 name: r
                             }
                         },
-                        htmlBuilder: an,
-                        mathmlBuilder: on
-                    }), ct({
+                        htmlBuilder: Jr,
+                        mathmlBuilder: Qr
+                    }), it({
                         type: "op",
                         names: ["\\det", "\\gcd", "\\inf", "\\lim", "\\max", "\\min", "\\Pr", "\\sup"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
                             var t = e.parser,
@@ -6582,122 +6590,122 @@
                                 mode: t.mode,
                                 limits: !0,
                                 parentIsSupSub: !1,
                                 symbol: !1,
                                 name: r
                             }
                         },
-                        htmlBuilder: an,
-                        mathmlBuilder: on
-                    }), ct({
+                        htmlBuilder: Jr,
+                        mathmlBuilder: Qr
+                    }), it({
                         type: "op",
                         names: ["\\int", "\\iint", "\\iiint", "\\oint", "\\oiint", "\\oiiint", "∫", "∬", "∭", "∮", "∯", "∰"],
                         props: {
                             numArgs: 0
                         },
                         handler: function(e) {
                             var t = e.parser,
                                 r = e.funcName;
-                            return 1 === r.length && (r = ln[r]), {
+                            return 1 === r.length && (r = tn[r]), {
                                 type: "op",
                                 mode: t.mode,
                                 limits: !1,
                                 parentIsSupSub: !1,
                                 symbol: !0,
                                 name: r
                             }
                         },
-                        htmlBuilder: an,
-                        mathmlBuilder: on
+                        htmlBuilder: Jr,
+                        mathmlBuilder: Qr
                     });
-                    var hn = function(e, t) {
+                    var rn = function(e, t) {
                         var r, n, a, i, o = !1;
-                        if ("supsub" === e.type ? (r = e.sup, n = e.sub, a = _t(e.base, "operatorname"), o = !0) : a = _t(e, "operatorname"), a.body.length > 0) {
+                        if ("supsub" === e.type ? (r = e.sup, n = e.sub, a = Ht(e.base, "operatorname"), o = !0) : a = Ht(e, "operatorname"), a.body.length > 0) {
                             for (var s = a.body.map((function(e) {
                                     var t = e.text;
                                     return "string" == typeof t ? {
                                         type: "textord",
                                         mode: e.mode,
                                         text: t
                                     } : e
-                                })), l = yt(s, t.withFont("mathrm"), !0), h = 0; h < l.length; h++) {
+                                })), l = pt(s, t.withFont("mathrm"), !0), h = 0; h < l.length; h++) {
                                 var m = l[h];
-                                m instanceof V && (m.text = m.text.replace(/\u2212/, "-").replace(/\u2217/, "*"))
+                                m instanceof E && (m.text = m.text.replace(/\u2212/, "-").replace(/\u2217/, "*"))
                             }
-                            i = rt.makeSpan(["mop"], l, t)
-                        } else i = rt.makeSpan(["mop"], [], t);
-                        return o ? rn(i, r, n, t, t.style, 0, 0) : i
+                            i = Ze.makeSpan(["mop"], l, t)
+                        } else i = Ze.makeSpan(["mop"], [], t);
+                        return o ? Zr(i, r, n, t, t.style, 0, 0) : i
                     };
 
-                    function mn(e, t, r) {
-                        for (var n = yt(e, t, !1), a = t.sizeMultiplier / r.sizeMultiplier, i = 0; i < n.length; i++) {
+                    function nn(e, t, r) {
+                        for (var n = pt(e, t, !1), a = t.sizeMultiplier / r.sizeMultiplier, i = 0; i < n.length; i++) {
                             var o = n[i].classes.indexOf("sizing");
                             o < 0 ? Array.prototype.push.apply(n[i].classes, t.sizingClasses(r)) : n[i].classes[o + 1] === "reset-size" + t.size && (n[i].classes[o + 1] = "reset-size" + r.size), n[i].height *= a, n[i].depth *= a
                         }
-                        return rt.makeFragment(n)
+                        return Ze.makeFragment(n)
                     }
-                    ct({
+                    it({
                         type: "operatorname",
                         names: ["\\operatorname", "\\operatorname*"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
                                 a = t[0];
                             return {
                                 type: "operatorname",
                                 mode: r.mode,
-                                body: pt(a),
+                                body: st(a),
                                 alwaysHandleSupSub: "\\operatorname*" === n,
                                 limits: !1,
                                 parentIsSupSub: !1
                             }
                         },
-                        htmlBuilder: hn,
+                        htmlBuilder: rn,
                         mathmlBuilder: function(e, t) {
-                            for (var r = Et(e.body, t.withFont("mathrm")), n = !0, a = 0; a < r.length; a++) {
+                            for (var r = Ct(e.body, t.withFont("mathrm")), n = !0, a = 0; a < r.length; a++) {
                                 var i = r[a];
-                                if (i instanceof Nt.SpaceNode);
-                                else if (i instanceof Nt.MathNode) switch (i.type) {
+                                if (i instanceof zt.SpaceNode);
+                                else if (i instanceof zt.MathNode) switch (i.type) {
                                     case "mi":
                                     case "mn":
                                     case "ms":
                                     case "mspace":
                                     case "mtext":
                                         break;
                                     case "mo":
                                         var o = i.children[0];
-                                        1 === i.children.length && o instanceof Nt.TextNode ? o.text = o.text.replace(/\u2212/, "-").replace(/\u2217/, "*") : n = !1;
+                                        1 === i.children.length && o instanceof zt.TextNode ? o.text = o.text.replace(/\u2212/, "-").replace(/\u2217/, "*") : n = !1;
                                         break;
                                     default:
                                         n = !1
                                 } else n = !1
                             }
                             if (n) {
                                 var s = r.map((function(e) {
                                     return e.toText()
                                 })).join("");
-                                r = [new Nt.TextNode(s)]
+                                r = [new zt.TextNode(s)]
                             }
-                            var l = new Nt.MathNode("mi", r);
+                            var l = new zt.MathNode("mi", r);
                             l.setAttribute("mathvariant", "normal");
-                            var h = new Nt.MathNode("mo", [It("⁡", "text")]);
-                            return e.parentIsSupSub ? new Nt.MathNode("mo", [l, h]) : Nt.newDocumentFragment([l, h])
+                            var h = new zt.MathNode("mo", [At("⁡", "text")]);
+                            return e.parentIsSupSub ? new zt.MathNode("mo", [l, h]) : zt.newDocumentFragment([l, h])
                         }
-                    }), ut({
+                    }), ot({
                         type: "ordgroup",
                         htmlBuilder: function(e, t) {
-                            return e.semisimple ? rt.makeFragment(yt(e.body, t, !1)) : rt.makeSpan(["mord"], yt(e.body, t, !0), t)
+                            return e.semisimple ? Ze.makeFragment(pt(e.body, t, !1)) : Ze.makeSpan(["mord"], pt(e.body, t, !0), t)
                         },
                         mathmlBuilder: function(e, t) {
-                            return Lt(e.body, t, !0)
+                            return qt(e.body, t, !0)
                         }
-                    }), ct({
+                    }), it({
                         type: "overline",
                         names: ["\\overline"],
                         props: {
                             numArgs: 1
                         },
                         handler: function(e, t) {
                             var r = e.parser,
@@ -6705,18 +6713,18 @@
                             return {
                                 type: "overline",
                                 mode: r.mode,
                                 body: n
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = zt(e.body, t.havingCrampedStyle()),
-                                n = rt.makeLineSpan("overline-line", t),
+                            var r = yt(e.body, t.havingCrampedStyle()),
+                                n = Ze.makeLineSpan("overline-line", t),
                                 a = t.fontMetrics().defaultRuleThickness,
-                                i = rt.makeVList({
+                                i = Ze.makeVList({
                                     positionType: "firstBaseline",
                                     children: [{
                                         type: "elem",
                                         elem: r
                                     }, {
                                         type: "kern",
                                         size: 3 * a
@@ -6724,47 +6732,47 @@
                                         type: "elem",
                                         elem: n
                                     }, {
                                         type: "kern",
                                         size: a
                                     }]
                                 }, t);
-                            return rt.makeSpan(["mord", "overline"], [i], t)
+                            return Ze.makeSpan(["mord", "overline"], [i], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mo", [new Nt.TextNode("‾")]);
+                            var r = new zt.MathNode("mo", [new zt.TextNode("‾")]);
                             r.setAttribute("stretchy", "true");
-                            var n = new Nt.MathNode("mover", [Pt(e.body, t), r]);
+                            var n = new zt.MathNode("mover", [Nt(e.body, t), r]);
                             return n.setAttribute("accent", "true"), n
                         }
-                    }), ct({
+                    }), it({
                         type: "phantom",
                         names: ["\\phantom"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = t[0];
                             return {
                                 type: "phantom",
                                 mode: r.mode,
-                                body: pt(n)
+                                body: st(n)
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = yt(e.body, t.withPhantom(), !1);
-                            return rt.makeFragment(r)
+                            var r = pt(e.body, t.withPhantom(), !1);
+                            return Ze.makeFragment(r)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = Et(e.body, t);
-                            return new Nt.MathNode("mphantom", r)
+                            var r = Ct(e.body, t);
+                            return new zt.MathNode("mphantom", r)
                         }
-                    }), ct({
+                    }), it({
                         type: "hphantom",
                         names: ["\\hphantom"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
@@ -6773,32 +6781,32 @@
                             return {
                                 type: "hphantom",
                                 mode: r.mode,
                                 body: n
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = rt.makeSpan([], [zt(e.body, t.withPhantom())]);
+                            var r = Ze.makeSpan([], [yt(e.body, t.withPhantom())]);
                             if (r.height = 0, r.depth = 0, r.children)
                                 for (var n = 0; n < r.children.length; n++) r.children[n].height = 0, r.children[n].depth = 0;
-                            return r = rt.makeVList({
+                            return r = Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }]
-                            }, t), rt.makeSpan(["mord"], [r], t)
+                            }, t), Ze.makeSpan(["mord"], [r], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = Et(pt(e.body), t),
-                                n = new Nt.MathNode("mphantom", r),
-                                a = new Nt.MathNode("mpadded", [n]);
+                            var r = Ct(st(e.body), t),
+                                n = new zt.MathNode("mphantom", r),
+                                a = new zt.MathNode("mpadded", [n]);
                             return a.setAttribute("height", "0px"), a.setAttribute("depth", "0px"), a
                         }
-                    }), ct({
+                    }), it({
                         type: "vphantom",
                         names: ["\\vphantom"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
@@ -6807,142 +6815,142 @@
                             return {
                                 type: "vphantom",
                                 mode: r.mode,
                                 body: n
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = rt.makeSpan(["inner"], [zt(e.body, t.withPhantom())]),
-                                n = rt.makeSpan(["fix"], []);
-                            return rt.makeSpan(["mord", "rlap"], [r, n], t)
+                            var r = Ze.makeSpan(["inner"], [yt(e.body, t.withPhantom())]),
+                                n = Ze.makeSpan(["fix"], []);
+                            return Ze.makeSpan(["mord", "rlap"], [r, n], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = Et(pt(e.body), t),
-                                n = new Nt.MathNode("mphantom", r),
-                                a = new Nt.MathNode("mpadded", [n]);
+                            var r = Ct(st(e.body), t),
+                                n = new zt.MathNode("mphantom", r),
+                                a = new zt.MathNode("mpadded", [n]);
                             return a.setAttribute("width", "0px"), a
                         }
-                    }), ct({
+                    }), it({
                         type: "raisebox",
                         names: ["\\raisebox"],
                         props: {
                             numArgs: 2,
                             argTypes: ["size", "hbox"],
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.parser,
-                                n = _t(t[0], "size").value,
+                                n = Ht(t[0], "size").value,
                                 a = t[1];
                             return {
                                 type: "raisebox",
                                 mode: r.mode,
                                 dy: n,
                                 body: a
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = zt(e.body, t),
-                                n = _e(e.dy, t);
-                            return rt.makeVList({
+                            var r = yt(e.body, t),
+                                n = He(e.dy, t);
+                            return Ze.makeVList({
                                 positionType: "shift",
                                 positionData: -n,
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }]
                             }, t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mpadded", [Pt(e.body, t)]),
+                            var r = new zt.MathNode("mpadded", [Nt(e.body, t)]),
                                 n = e.dy.number + e.dy.unit;
                             return r.setAttribute("voffset", n), r
                         }
-                    }), ct({
+                    }), it({
                         type: "rule",
                         names: ["\\rule"],
                         props: {
                             numArgs: 2,
                             numOptionalArgs: 1,
                             argTypes: ["size", "size", "size"]
                         },
                         handler: function(e, t, r) {
                             var n = e.parser,
                                 a = r[0],
-                                i = _t(t[0], "size"),
-                                o = _t(t[1], "size");
+                                i = Ht(t[0], "size"),
+                                o = Ht(t[1], "size");
                             return {
                                 type: "rule",
                                 mode: n.mode,
-                                shift: a && _t(a, "size").value,
+                                shift: a && Ht(a, "size").value,
                                 width: i.value,
                                 height: o.value
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = rt.makeSpan(["mord", "rule"], [], t),
-                                n = _e(e.width, t),
-                                a = _e(e.height, t),
-                                i = e.shift ? _e(e.shift, t) : 0;
+                            var r = Ze.makeSpan(["mord", "rule"], [], t),
+                                n = He(e.width, t),
+                                a = He(e.height, t),
+                                i = e.shift ? He(e.shift, t) : 0;
                             return r.style.borderRightWidth = n + "em", r.style.borderTopWidth = a + "em", r.style.bottom = i + "em", r.width = n, r.height = a + i, r.depth = -i, r.maxFontSize = 1.125 * a * t.sizeMultiplier, r
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = _e(e.width, t),
-                                n = _e(e.height, t),
-                                a = e.shift ? _e(e.shift, t) : 0,
+                            var r = He(e.width, t),
+                                n = He(e.height, t),
+                                a = e.shift ? He(e.shift, t) : 0,
                                 i = t.color && t.getColor() || "black",
-                                o = new Nt.MathNode("mspace");
+                                o = new zt.MathNode("mspace");
                             o.setAttribute("mathbackground", i), o.setAttribute("width", r + "em"), o.setAttribute("height", n + "em");
-                            var s = new Nt.MathNode("mpadded", [o]);
+                            var s = new zt.MathNode("mpadded", [o]);
                             return a >= 0 ? s.setAttribute("height", "+" + a + "em") : (s.setAttribute("height", a + "em"), s.setAttribute("depth", "+" + -a + "em")), s.setAttribute("voffset", a + "em"), s
                         }
                     });
-                    var cn = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
-                    ct({
+                    var an = ["\\tiny", "\\sixptsize", "\\scriptsize", "\\footnotesize", "\\small", "\\normalsize", "\\large", "\\Large", "\\LARGE", "\\huge", "\\Huge"];
+                    it({
                         type: "sizing",
-                        names: cn,
+                        names: an,
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             var r = e.breakOnTokenText,
                                 n = e.funcName,
                                 a = e.parser,
                                 i = a.parseExpression(!1, r);
                             return {
                                 type: "sizing",
                                 mode: a.mode,
-                                size: cn.indexOf(n) + 1,
+                                size: an.indexOf(n) + 1,
                                 body: i
                             }
                         },
                         htmlBuilder: function(e, t) {
                             var r = t.havingSize(e.size);
-                            return mn(e.body, r, t)
+                            return nn(e.body, r, t)
                         },
                         mathmlBuilder: function(e, t) {
                             var r = t.havingSize(e.size),
-                                n = Et(e.body, r),
-                                a = new Nt.MathNode("mstyle", n);
+                                n = Ct(e.body, r),
+                                a = new zt.MathNode("mstyle", n);
                             return a.setAttribute("mathsize", r.sizeMultiplier + "em"), a
                         }
-                    }), ct({
+                    }), it({
                         type: "smash",
                         names: ["\\smash"],
                         props: {
                             numArgs: 1,
                             numOptionalArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t, r) {
                             var n = e.parser,
                                 a = !1,
                                 i = !1,
-                                o = r[0] && _t(r[0], "ordgroup");
+                                o = r[0] && Ht(r[0], "ordgroup");
                             if (o)
                                 for (var s = "", l = 0; l < o.body.length; ++l)
                                     if ("t" === (s = o.body[l].text)) a = !0;
                                     else {
                                         if ("b" !== s) {
                                             a = !1, i = !1;
                                             break
@@ -6956,34 +6964,34 @@
                                 mode: n.mode,
                                 body: h,
                                 smashHeight: a,
                                 smashDepth: i
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = rt.makeSpan([], [zt(e.body, t)]);
+                            var r = Ze.makeSpan([], [yt(e.body, t)]);
                             if (!e.smashHeight && !e.smashDepth) return r;
                             if (e.smashHeight && (r.height = 0, r.children))
                                 for (var n = 0; n < r.children.length; n++) r.children[n].height = 0;
                             if (e.smashDepth && (r.depth = 0, r.children))
                                 for (var a = 0; a < r.children.length; a++) r.children[a].depth = 0;
-                            var i = rt.makeVList({
+                            var i = Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: r
                                 }]
                             }, t);
-                            return rt.makeSpan(["mord"], [i], t)
+                            return Ze.makeSpan(["mord"], [i], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mpadded", [Pt(e.body, t)]);
+                            var r = new zt.MathNode("mpadded", [Nt(e.body, t)]);
                             return e.smashHeight && r.setAttribute("height", "0px"), e.smashDepth && r.setAttribute("depth", "0px"), r
                         }
-                    }), ct({
+                    }), it({
                         type: "sqrt",
                         names: ["\\sqrt"],
                         props: {
                             numArgs: 1,
                             numOptionalArgs: 1
                         },
                         handler: function(e, t, r) {
@@ -6994,42 +7002,42 @@
                                 type: "sqrt",
                                 mode: n.mode,
                                 body: i,
                                 index: a
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = zt(e.body, t.havingCrampedStyle());
-                            0 === r.height && (r.height = t.fontMetrics().xHeight), r = rt.wrapFragment(r, t);
+                            var r = yt(e.body, t.havingCrampedStyle());
+                            0 === r.height && (r.height = t.fontMetrics().xHeight), r = Ze.wrapFragment(r, t);
                             var n = t.fontMetrics().defaultRuleThickness,
                                 a = n;
-                            t.style.id < T.TEXT.id && (a = t.fontMetrics().xHeight);
+                            t.style.id < w.TEXT.id && (a = t.fontMetrics().xHeight);
                             var i = n + a / 4,
                                 o = function(e, t) {
                                     var r, n, a = t.havingBaseSizing(),
-                                        i = xr("\\surd", e * a.sizeMultiplier, br, a),
+                                        i = dr("\\surd", e * a.sizeMultiplier, ur, a),
                                         o = a.sizeMultiplier,
                                         s = Math.max(0, t.minRuleThickness - t.fontMetrics().sqrtRuleThickness),
                                         l = 0,
                                         h = 0,
                                         m = 0;
-                                    return "small" === i.type ? (e < 1 ? o = 1 : e < 1.4 && (o = .7), h = (1 + s) / o, (r = cr("sqrtMain", l = (1 + s + mr) / o, m = 1e3 + 1e3 * s + 80, s, t)).style.minWidth = "0.853em", n = .833 / o) : "large" === i.type ? (m = 1080 * fr[i.size], h = (fr[i.size] + s) / o, l = (fr[i.size] + s + mr) / o, (r = cr("sqrtSize" + i.size, l, m, s, t)).style.minWidth = "1.02em", n = 1 / o) : (l = e + s + mr, h = e + s, m = Math.floor(1e3 * e + s) + 80, (r = cr("sqrtTall", l, m, s, t)).style.minWidth = "0.742em", n = 1.056), r.height = h, r.style.height = l + "em", {
+                                    return "small" === i.type ? (e < 1 ? o = 1 : e < 1.4 && (o = .7), h = (1 + s) / o, (r = ir("sqrtMain", l = (1 + s + ar) / o, m = 1e3 + 1e3 * s + 80, s, t)).style.minWidth = "0.853em", n = .833 / o) : "large" === i.type ? (m = 1080 * hr[i.size], h = (hr[i.size] + s) / o, l = (hr[i.size] + s + ar) / o, (r = ir("sqrtSize" + i.size, l, m, s, t)).style.minWidth = "1.02em", n = 1 / o) : (l = e + s + ar, h = e + s, m = Math.floor(1e3 * e + s) + 80, (r = ir("sqrtTall", l, m, s, t)).style.minWidth = "0.742em", n = 1.056), r.height = h, r.style.height = l + "em", {
                                         span: r,
                                         advanceWidth: n,
                                         ruleWidth: (t.fontMetrics().sqrtRuleThickness + s) * o
                                     }
                                 }(r.height + r.depth + i + n, t),
                                 s = o.span,
                                 l = o.ruleWidth,
                                 h = o.advanceWidth,
                                 m = s.height - l;
                             m > r.height + r.depth + i && (i = (i + m - r.height - r.depth) / 2);
                             var c = s.height - r.height - i - l;
                             r.style.paddingLeft = h + "em";
-                            var u = rt.makeVList({
+                            var u = Ze.makeVList({
                                 positionType: "firstBaseline",
                                 children: [{
                                     type: "elem",
                                     elem: r,
                                     wrapperClasses: ["svg-align"]
                                 }, {
                                     type: "kern",
@@ -7039,43 +7047,43 @@
                                     elem: s
                                 }, {
                                     type: "kern",
                                     size: l
                                 }]
                             }, t);
                             if (e.index) {
-                                var p = t.havingStyle(T.SCRIPTSCRIPT),
-                                    d = zt(e.index, p, t),
+                                var p = t.havingStyle(w.SCRIPTSCRIPT),
+                                    d = yt(e.index, p, t),
                                     f = .6 * (u.height - u.depth),
-                                    g = rt.makeVList({
+                                    g = Ze.makeVList({
                                         positionType: "shift",
                                         positionData: -f,
                                         children: [{
                                             type: "elem",
                                             elem: d
                                         }]
                                     }, t),
-                                    v = rt.makeSpan(["root"], [g]);
-                                return rt.makeSpan(["mord", "sqrt"], [v, u], t)
+                                    v = Ze.makeSpan(["root"], [g]);
+                                return Ze.makeSpan(["mord", "sqrt"], [v, u], t)
                             }
-                            return rt.makeSpan(["mord", "sqrt"], [u], t)
+                            return Ze.makeSpan(["mord", "sqrt"], [u], t)
                         },
                         mathmlBuilder: function(e, t) {
                             var r = e.body,
                                 n = e.index;
-                            return n ? new Nt.MathNode("mroot", [Pt(r, t), Pt(n, t)]) : new Nt.MathNode("msqrt", [Pt(r, t)])
+                            return n ? new zt.MathNode("mroot", [Nt(r, t), Nt(n, t)]) : new zt.MathNode("msqrt", [Nt(r, t)])
                         }
                     });
-                    var un = {
-                        display: T.DISPLAY,
-                        text: T.TEXT,
-                        script: T.SCRIPT,
-                        scriptscript: T.SCRIPTSCRIPT
+                    var on = {
+                        display: w.DISPLAY,
+                        text: w.TEXT,
+                        script: w.SCRIPT,
+                        scriptscript: w.SCRIPTSCRIPT
                     };
-                    ct({
+                    it({
                         type: "styling",
                         names: ["\\displaystyle", "\\textstyle", "\\scriptstyle", "\\scriptscriptstyle"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
@@ -7088,239 +7096,242 @@
                                 type: "styling",
                                 mode: a.mode,
                                 style: o,
                                 body: i
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = un[e.style],
+                            var r = on[e.style],
                                 n = t.havingStyle(r).withFont("");
-                            return mn(e.body, n, t)
+                            return nn(e.body, n, t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = un[e.style],
+                            var r = on[e.style],
                                 n = t.havingStyle(r),
-                                a = Et(e.body, n),
-                                i = new Nt.MathNode("mstyle", a),
+                                a = Ct(e.body, n),
+                                i = new zt.MathNode("mstyle", a),
                                 o = {
                                     display: ["0", "true"],
                                     text: ["0", "false"],
                                     script: ["1", "false"],
                                     scriptscript: ["2", "false"]
                                 } [e.style];
                             return i.setAttribute("scriptlevel", o[0]), i.setAttribute("displaystyle", o[1]), i
                         }
-                    }), ut({
+                    }), ot({
                         type: "supsub",
                         htmlBuilder: function(e, t) {
                             var r = function(e, t) {
                                 var r = e.base;
-                                return r ? "op" === r.type ? r.limits && (t.style.size === T.DISPLAY.size || r.alwaysHandleSupSub) ? an : null : "operatorname" === r.type ? r.alwaysHandleSupSub && (t.style.size === T.DISPLAY.size || r.limits) ? hn : null : "accent" === r.type ? g(r.base) ? jt : null : "horizBrace" === r.type && !e.sub === r.isOver ? Qr : null : null
+                                return r ? "op" === r.type ? r.limits && (t.style.size === w.DISPLAY.size || r.alwaysHandleSupSub) ? Jr : null : "operatorname" === r.type ? r.alwaysHandleSupSub && (t.style.size === w.DISPLAY.size || r.limits) ? rn : null : "accent" === r.type ? c.isCharacterBox(r.base) ? Ut : null : "horizBrace" === r.type && !e.sub === r.isOver ? Xr : null : null
                             }(e, t);
                             if (r) return r(e, t);
                             var n, a, i, o = e.base,
                                 s = e.sup,
                                 l = e.sub,
-                                h = zt(o, t),
+                                h = yt(o, t),
                                 m = t.fontMetrics(),
-                                c = 0,
                                 u = 0,
-                                p = o && g(o);
+                                p = 0,
+                                d = o && c.isCharacterBox(o);
                             if (s) {
-                                var d = t.havingStyle(t.style.sup());
-                                n = zt(s, d, t), p || (c = h.height - d.fontMetrics().supDrop * d.sizeMultiplier / t.sizeMultiplier)
+                                var f = t.havingStyle(t.style.sup());
+                                n = yt(s, f, t), d || (u = h.height - f.fontMetrics().supDrop * f.sizeMultiplier / t.sizeMultiplier)
                             }
                             if (l) {
-                                var f = t.havingStyle(t.style.sub());
-                                a = zt(l, f, t), p || (u = h.depth + f.fontMetrics().subDrop * f.sizeMultiplier / t.sizeMultiplier)
+                                var g = t.havingStyle(t.style.sub());
+                                a = yt(l, g, t), d || (p = h.depth + g.fontMetrics().subDrop * g.sizeMultiplier / t.sizeMultiplier)
                             }
-                            i = t.style === T.DISPLAY ? m.sup1 : t.style.cramped ? m.sup3 : m.sup2;
+                            i = t.style === w.DISPLAY ? m.sup1 : t.style.cramped ? m.sup3 : m.sup2;
                             var v, b = t.sizeMultiplier,
                                 y = .5 / m.ptPerEm / b + "em",
                                 x = null;
                             if (a) {
-                                var w = e.base && "op" === e.base.type && e.base.name && ("\\oiint" === e.base.name || "\\oiiint" === e.base.name);
-                                (h instanceof V || w) && (x = -h.italic + "em")
+                                var k = e.base && "op" === e.base.type && e.base.name && ("\\oiint" === e.base.name || "\\oiiint" === e.base.name);
+                                (h instanceof E || k) && (x = -h.italic + "em")
                             }
                             if (n && a) {
-                                c = Math.max(c, i, n.depth + .25 * m.xHeight), u = Math.max(u, m.sub2);
-                                var k = 4 * m.defaultRuleThickness;
-                                if (c - n.depth - (a.height - u) < k) {
-                                    u = k - (c - n.depth) + a.height;
-                                    var S = .8 * m.xHeight - (c - n.depth);
-                                    S > 0 && (c += S, u -= S)
+                                u = Math.max(u, i, n.depth + .25 * m.xHeight), p = Math.max(p, m.sub2);
+                                var S = 4 * m.defaultRuleThickness;
+                                if (u - n.depth - (a.height - p) < S) {
+                                    p = S - (u - n.depth) + a.height;
+                                    var M = .8 * m.xHeight - (u - n.depth);
+                                    M > 0 && (u += M, p -= M)
                                 }
-                                v = rt.makeVList({
+                                var z = [{
+                                    type: "elem",
+                                    elem: a,
+                                    shift: p,
+                                    marginRight: y,
+                                    marginLeft: x
+                                }, {
+                                    type: "elem",
+                                    elem: n,
+                                    shift: -u,
+                                    marginRight: y
+                                }];
+                                v = Ze.makeVList({
                                     positionType: "individualShift",
-                                    children: [{
-                                        type: "elem",
-                                        elem: a,
-                                        shift: u,
-                                        marginRight: y,
-                                        marginLeft: x
-                                    }, {
-                                        type: "elem",
-                                        elem: n,
-                                        shift: -c,
-                                        marginRight: y
-                                    }]
+                                    children: z
                                 }, t)
                             } else if (a) {
-                                u = Math.max(u, m.sub1, a.height - .8 * m.xHeight), v = rt.makeVList({
+                                p = Math.max(p, m.sub1, a.height - .8 * m.xHeight);
+                                var A = [{
+                                    type: "elem",
+                                    elem: a,
+                                    marginLeft: x,
+                                    marginRight: y
+                                }];
+                                v = Ze.makeVList({
                                     positionType: "shift",
-                                    positionData: u,
-                                    children: [{
-                                        type: "elem",
-                                        elem: a,
-                                        marginLeft: x,
-                                        marginRight: y
-                                    }]
+                                    positionData: p,
+                                    children: A
                                 }, t)
                             } else {
                                 if (!n) throw new Error("supsub must have either sup or sub.");
-                                c = Math.max(c, i, n.depth + .25 * m.xHeight), v = rt.makeVList({
+                                u = Math.max(u, i, n.depth + .25 * m.xHeight), v = Ze.makeVList({
                                     positionType: "shift",
-                                    positionData: -c,
+                                    positionData: -u,
                                     children: [{
                                         type: "elem",
                                         elem: n,
                                         marginRight: y
                                     }]
                                 }, t)
                             }
-                            var M = St(h, "right") || "mord";
-                            return rt.makeSpan([M], [h, rt.makeSpan(["msupsub"], [v])], t)
+                            var T = vt(h, "right") || "mord";
+                            return Ze.makeSpan([T], [h, Ze.makeSpan(["msupsub"], [v])], t)
                         },
                         mathmlBuilder: function(e, t) {
                             var r, n = !1;
                             e.base && "horizBrace" === e.base.type && !!e.sup === e.base.isOver && (n = !0, r = e.base.isOver), !e.base || "op" !== e.base.type && "operatorname" !== e.base.type || (e.base.parentIsSupSub = !0);
-                            var a, i = [Pt(e.base, t)];
-                            if (e.sub && i.push(Pt(e.sub, t)), e.sup && i.push(Pt(e.sup, t)), n) a = r ? "mover" : "munder";
+                            var a, i = [Nt(e.base, t)];
+                            if (e.sub && i.push(Nt(e.sub, t)), e.sup && i.push(Nt(e.sup, t)), n) a = r ? "mover" : "munder";
                             else if (e.sub)
                                 if (e.sup) {
                                     var o = e.base;
-                                    a = o && "op" === o.type && o.limits && t.style === T.DISPLAY || o && "operatorname" === o.type && o.alwaysHandleSupSub && (t.style === T.DISPLAY || o.limits) ? "munderover" : "msubsup"
+                                    a = o && "op" === o.type && o.limits && t.style === w.DISPLAY || o && "operatorname" === o.type && o.alwaysHandleSupSub && (t.style === w.DISPLAY || o.limits) ? "munderover" : "msubsup"
                                 } else {
                                     var s = e.base;
-                                    a = s && "op" === s.type && s.limits && (t.style === T.DISPLAY || s.alwaysHandleSupSub) || s && "operatorname" === s.type && s.alwaysHandleSupSub && (s.limits || t.style === T.DISPLAY) ? "munder" : "msub"
+                                    a = s && "op" === s.type && s.limits && (t.style === w.DISPLAY || s.alwaysHandleSupSub) || s && "operatorname" === s.type && s.alwaysHandleSupSub && (s.limits || t.style === w.DISPLAY) ? "munder" : "msub"
                                 }
                             else {
                                 var l = e.base;
-                                a = l && "op" === l.type && l.limits && (t.style === T.DISPLAY || l.alwaysHandleSupSub) || l && "operatorname" === l.type && l.alwaysHandleSupSub && (l.limits || t.style === T.DISPLAY) ? "mover" : "msup"
+                                a = l && "op" === l.type && l.limits && (t.style === w.DISPLAY || l.alwaysHandleSupSub) || l && "operatorname" === l.type && l.alwaysHandleSupSub && (l.limits || t.style === w.DISPLAY) ? "mover" : "msup"
                             }
-                            return new Nt.MathNode(a, i)
+                            return new zt.MathNode(a, i)
                         }
-                    }), ut({
+                    }), ot({
                         type: "atom",
                         htmlBuilder: function(e, t) {
-                            return rt.mathsym(e.text, e.mode, t, ["m" + e.family])
+                            return Ze.mathsym(e.text, e.mode, t, ["m" + e.family])
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mo", [It(e.text, e.mode)]);
+                            var r = new zt.MathNode("mo", [At(e.text, e.mode)]);
                             if ("bin" === e.family) {
-                                var n = Rt(e, t);
+                                var n = Bt(e, t);
                                 "bold-italic" === n && r.setAttribute("mathvariant", n)
                             } else "punct" === e.family ? r.setAttribute("separator", "true") : "open" !== e.family && "close" !== e.family || r.setAttribute("stretchy", "false");
                             return r
                         }
                     });
-                    var pn = {
+                    var sn = {
                         mi: "italic",
                         mn: "normal",
                         mtext: "normal"
                     };
-                    ut({
+                    ot({
                         type: "mathord",
                         htmlBuilder: function(e, t) {
-                            return rt.makeOrd(e, t, "mathord")
+                            return Ze.makeOrd(e, t, "mathord")
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mi", [It(e.text, e.mode, t)]),
-                                n = Rt(e, t) || "italic";
-                            return n !== pn[r.type] && r.setAttribute("mathvariant", n), r
+                            var r = new zt.MathNode("mi", [At(e.text, e.mode, t)]),
+                                n = Bt(e, t) || "italic";
+                            return n !== sn[r.type] && r.setAttribute("mathvariant", n), r
                         }
-                    }), ut({
+                    }), ot({
                         type: "textord",
                         htmlBuilder: function(e, t) {
-                            return rt.makeOrd(e, t, "textord")
+                            return Ze.makeOrd(e, t, "textord")
                         },
                         mathmlBuilder: function(e, t) {
-                            var r, n = It(e.text, e.mode, t),
-                                a = Rt(e, t) || "normal";
-                            return r = "text" === e.mode ? new Nt.MathNode("mtext", [n]) : /[0-9]/.test(e.text) ? new Nt.MathNode("mn", [n]) : "\\prime" === e.text ? new Nt.MathNode("mo", [n]) : new Nt.MathNode("mi", [n]), a !== pn[r.type] && r.setAttribute("mathvariant", a), r
+                            var r, n = At(e.text, e.mode, t),
+                                a = Bt(e, t) || "normal";
+                            return r = "text" === e.mode ? new zt.MathNode("mtext", [n]) : /[0-9]/.test(e.text) ? new zt.MathNode("mn", [n]) : "\\prime" === e.text ? new zt.MathNode("mo", [n]) : new zt.MathNode("mi", [n]), a !== sn[r.type] && r.setAttribute("mathvariant", a), r
                         }
                     });
-                    var dn = {
+                    var ln = {
                             "\\nobreak": "nobreak",
                             "\\allowbreak": "allowbreak"
                         },
-                        fn = {
+                        hn = {
                             " ": {},
                             "\\ ": {},
                             "~": {
                                 className: "nobreak"
                             },
                             "\\space": {},
                             "\\nobreakspace": {
                                 className: "nobreak"
                             }
                         };
-                    ut({
+                    ot({
                         type: "spacing",
                         htmlBuilder: function(e, t) {
-                            if (fn.hasOwnProperty(e.text)) {
-                                var r = fn[e.text].className || "";
+                            if (hn.hasOwnProperty(e.text)) {
+                                var r = hn[e.text].className || "";
                                 if ("text" === e.mode) {
-                                    var n = rt.makeOrd(e, t, "textord");
+                                    var n = Ze.makeOrd(e, t, "textord");
                                     return n.classes.push(r), n
                                 }
-                                return rt.makeSpan(["mspace", r], [rt.mathsym(e.text, e.mode, t)], t)
+                                return Ze.makeSpan(["mspace", r], [Ze.mathsym(e.text, e.mode, t)], t)
                             }
-                            if (dn.hasOwnProperty(e.text)) return rt.makeSpan(["mspace", dn[e.text]], [], t);
+                            if (ln.hasOwnProperty(e.text)) return Ze.makeSpan(["mspace", ln[e.text]], [], t);
                             throw new o('Unknown type of space "' + e.text + '"')
                         },
                         mathmlBuilder: function(e, t) {
-                            if (!fn.hasOwnProperty(e.text)) {
-                                if (dn.hasOwnProperty(e.text)) return new Nt.MathNode("mspace");
+                            if (!hn.hasOwnProperty(e.text)) {
+                                if (ln.hasOwnProperty(e.text)) return new zt.MathNode("mspace");
                                 throw new o('Unknown type of space "' + e.text + '"')
                             }
-                            return new Nt.MathNode("mtext", [new Nt.TextNode(" ")])
+                            return new zt.MathNode("mtext", [new zt.TextNode(" ")])
                         }
                     });
-                    var gn = function() {
-                        var e = new Nt.MathNode("mtd", []);
+                    var mn = function() {
+                        var e = new zt.MathNode("mtd", []);
                         return e.setAttribute("width", "50%"), e
                     };
-                    ut({
+                    ot({
                         type: "tag",
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mtable", [new Nt.MathNode("mtr", [gn(), new Nt.MathNode("mtd", [Lt(e.body, t)]), gn(), new Nt.MathNode("mtd", [Lt(e.tag, t)])])]);
+                            var r = new zt.MathNode("mtable", [new zt.MathNode("mtr", [mn(), new zt.MathNode("mtd", [qt(e.body, t)]), mn(), new zt.MathNode("mtd", [qt(e.tag, t)])])]);
                             return r.setAttribute("width", "100%"), r
                         }
                     });
-                    var vn = {
+                    var cn = {
                             "\\text": void 0,
                             "\\textrm": "textrm",
                             "\\textsf": "textsf",
                             "\\texttt": "texttt",
                             "\\textnormal": "textrm"
                         },
-                        bn = {
+                        un = {
                             "\\textbf": "textbf",
                             "\\textmd": "textmd"
                         },
-                        yn = {
+                        pn = {
                             "\\textit": "textit",
                             "\\textup": "textup"
                         },
-                        xn = function(e, t) {
+                        dn = function(e, t) {
                             var r = e.font;
-                            return r ? vn[r] ? t.withTextFontFamily(vn[r]) : bn[r] ? t.withTextFontWeight(bn[r]) : t.withTextFontShape(yn[r]) : t
+                            return r ? cn[r] ? t.withTextFontFamily(cn[r]) : un[r] ? t.withTextFontWeight(un[r]) : t.withTextFontShape(pn[r]) : t
                         };
-                    ct({
+                    it({
                         type: "text",
                         names: ["\\text", "\\textrm", "\\textsf", "\\texttt", "\\textnormal", "\\textbf", "\\textmd", "\\textit", "\\textup"],
                         props: {
                             numArgs: 1,
                             argTypes: ["text"],
                             greediness: 2,
                             allowedInText: !0
@@ -7328,46 +7339,46 @@
                         handler: function(e, t) {
                             var r = e.parser,
                                 n = e.funcName,
                                 a = t[0];
                             return {
                                 type: "text",
                                 mode: r.mode,
-                                body: pt(a),
+                                body: st(a),
                                 font: n
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = xn(e, t),
-                                n = yt(e.body, r, !0);
-                            return rt.makeSpan(["mord", "text"], rt.tryCombineChars(n), r)
+                            var r = dn(e, t),
+                                n = pt(e.body, r, !0);
+                            return Ze.makeSpan(["mord", "text"], Ze.tryCombineChars(n), r)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = xn(e, t);
-                            return Lt(e.body, r)
+                            var r = dn(e, t);
+                            return qt(e.body, r)
                         }
-                    }), ct({
+                    }), it({
                         type: "underline",
                         names: ["\\underline"],
                         props: {
                             numArgs: 1,
                             allowedInText: !0
                         },
                         handler: function(e, t) {
                             return {
                                 type: "underline",
                                 mode: e.parser.mode,
                                 body: t[0]
                             }
                         },
                         htmlBuilder: function(e, t) {
-                            var r = zt(e.body, t),
-                                n = rt.makeLineSpan("underline-line", t),
+                            var r = yt(e.body, t),
+                                n = Ze.makeLineSpan("underline-line", t),
                                 a = t.fontMetrics().defaultRuleThickness,
-                                i = rt.makeVList({
+                                i = Ze.makeVList({
                                     positionType: "top",
                                     positionData: r.height,
                                     children: [{
                                         type: "kern",
                                         size: a
                                     }, {
                                         type: "elem",
@@ -7376,54 +7387,59 @@
                                         type: "kern",
                                         size: 3 * a
                                     }, {
                                         type: "elem",
                                         elem: r
                                     }]
                                 }, t);
-                            return rt.makeSpan(["mord", "underline"], [i], t)
+                            return Ze.makeSpan(["mord", "underline"], [i], t)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.MathNode("mo", [new Nt.TextNode("‾")]);
+                            var r = new zt.MathNode("mo", [new zt.TextNode("‾")]);
                             r.setAttribute("stretchy", "true");
-                            var n = new Nt.MathNode("munder", [Pt(e.body, t), r]);
+                            var n = new zt.MathNode("munder", [Nt(e.body, t), r]);
                             return n.setAttribute("accentunder", "true"), n
                         }
-                    }), ct({
+                    }), it({
                         type: "verb",
                         names: ["\\verb"],
                         props: {
                             numArgs: 0,
                             allowedInText: !0
                         },
                         handler: function(e, t, r) {
                             throw new o("\\verb ended by end of line instead of matching delimiter")
                         },
                         htmlBuilder: function(e, t) {
-                            for (var r = wn(e), n = [], a = t.havingStyle(t.style.text()), i = 0; i < r.length; i++) {
+                            for (var r = fn(e), n = [], a = t.havingStyle(t.style.text()), i = 0; i < r.length; i++) {
                                 var o = r[i];
-                                "~" === o && (o = "\\textasciitilde"), n.push(rt.makeSymbol(o, "Typewriter-Regular", e.mode, a, ["mord", "texttt"]))
+                                "~" === o && (o = "\\textasciitilde"), n.push(Ze.makeSymbol(o, "Typewriter-Regular", e.mode, a, ["mord", "texttt"]))
                             }
-                            return rt.makeSpan(["mord", "text"].concat(a.sizingClasses(t)), rt.tryCombineChars(n), a)
+                            return Ze.makeSpan(["mord", "text"].concat(a.sizingClasses(t)), Ze.tryCombineChars(n), a)
                         },
                         mathmlBuilder: function(e, t) {
-                            var r = new Nt.TextNode(wn(e)),
-                                n = new Nt.MathNode("mtext", [r]);
+                            var r = new zt.TextNode(fn(e)),
+                                n = new zt.MathNode("mtext", [r]);
                             return n.setAttribute("mathvariant", "monospace"), n
                         }
                     });
-                    var wn = function(e) {
+                    var fn = function(e) {
                             return e.body.replace(/ /g, e.star ? "␣" : " ")
                         },
-                        kn = lt,
-                        Sn = new RegExp("^(\\\\[a-zA-Z@]+)[ \r\n\t]*$"),
-                        Mn = new RegExp("[̀-ͯ]+$"),
-                        zn = function() {
+                        gn = rt,
+                        vn = "[ \r\n\t]",
+                        bn = "\\\\[a-zA-Z@]+",
+                        yn = "" + bn + vn + "*",
+                        xn = new RegExp("^(" + bn + ")" + vn + "*$"),
+                        wn = "[̀-ͯ]",
+                        kn = new RegExp(wn + "+$"),
+                        Sn = "(" + vn + "+)|([!-\\[\\]-‧‪-퟿豈-￿]" + wn + "*|[\ud800-\udbff][\udc00-\udfff]" + wn + "*|\\\\verb\\*([^]).*?\\3|\\\\verb([^*a-zA-Z]).*?\\4|\\\\operatorname\\*|" + yn + "|\\\\[^\ud800-\udfff])",
+                        Mn = function() {
                             function e(e, t) {
-                                this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = e, this.settings = t, this.tokenRegex = new RegExp("([ \r\n\t]+)|([!-\\[\\]-‧‪-퟿豈-￿][̀-ͯ]*|[\ud800-\udbff][\udc00-\udfff][̀-ͯ]*|\\\\verb\\*([^]).*?\\3|\\\\verb([^*a-zA-Z]).*?\\4|\\\\operatorname\\*|\\\\[a-zA-Z@]+[ \r\n\t]*|\\\\[^\ud800-\udfff])", "g"), this.catcodes = {
+                                this.input = void 0, this.settings = void 0, this.tokenRegex = void 0, this.catcodes = void 0, this.input = e, this.settings = t, this.tokenRegex = new RegExp(Sn, "g"), this.catcodes = {
                                     "%": 14
                                 }
                             }
                             var t = e.prototype;
                             return t.setCatcode = function(e, t) {
                                 this.catcodes[e] = t
                             }, t.lex = function() {
@@ -7433,19 +7449,19 @@
                                 var r = this.tokenRegex.exec(e);
                                 if (null === r || r.index !== t) throw new o("Unexpected character: '" + e[t] + "'", new a(e[t], new n(this, t, t + 1)));
                                 var i = r[2] || " ";
                                 if (14 === this.catcodes[i]) {
                                     var s = e.indexOf("\n", this.tokenRegex.lastIndex);
                                     return -1 === s ? (this.tokenRegex.lastIndex = e.length, this.settings.reportNonstrict("commentAtEnd", "% comment has no terminating newline; LaTeX would fail because of commenting the end of math mode (e.g. $)")) : this.tokenRegex.lastIndex = s + 1, this.lex()
                                 }
-                                var l = i.match(Sn);
+                                var l = i.match(xn);
                                 return l && (i = l[1]), new a(i, new n(this, t, this.tokenRegex.lastIndex))
                             }, e
                         }(),
-                        An = function() {
+                        zn = function() {
                             function e(e, t) {
                                 void 0 === e && (e = {}), void 0 === t && (t = {}), this.current = void 0, this.builtins = void 0, this.undefStack = void 0, this.current = t, this.builtins = e, this.undefStack = []
                             }
                             var t = e.prototype;
                             return t.beginGroup = function() {
                                 this.undefStack.push({})
                             }, t.endGroup = function() {
@@ -7463,64 +7479,64 @@
                                 } else {
                                     var a = this.undefStack[this.undefStack.length - 1];
                                     a && !a.hasOwnProperty(e) && (a[e] = this.current[e])
                                 }
                                 this.current[e] = t
                             }, e
                         }(),
-                        Tn = {},
-                        Bn = Tn;
+                        An = {},
+                        Tn = An;
 
-                    function Cn(e, t) {
-                        Tn[e] = t
+                    function Bn(e, t) {
+                        An[e] = t
                     }
-                    Cn("\\noexpand", (function(e) {
+                    Bn("\\noexpand", (function(e) {
                         var t = e.popToken();
                         return e.isExpandable(t.text) && (t.noexpand = !0, t.treatAsRelax = !0), {
                             tokens: [t],
                             numArgs: 0
                         }
-                    })), Cn("\\expandafter", (function(e) {
+                    })), Bn("\\expandafter", (function(e) {
                         var t = e.popToken();
                         return e.expandOnce(!0), {
                             tokens: [t],
                             numArgs: 0
                         }
-                    })), Cn("\\@firstoftwo", (function(e) {
+                    })), Bn("\\@firstoftwo", (function(e) {
                         return {
                             tokens: e.consumeArgs(2)[0],
                             numArgs: 0
                         }
-                    })), Cn("\\@secondoftwo", (function(e) {
+                    })), Bn("\\@secondoftwo", (function(e) {
                         return {
                             tokens: e.consumeArgs(2)[1],
                             numArgs: 0
                         }
-                    })), Cn("\\@ifnextchar", (function(e) {
+                    })), Bn("\\@ifnextchar", (function(e) {
                         var t = e.consumeArgs(3);
                         e.consumeSpaces();
                         var r = e.future();
                         return 1 === t[0].length && t[0][0].text === r.text ? {
                             tokens: t[1],
                             numArgs: 0
                         } : {
                             tokens: t[2],
                             numArgs: 0
                         }
-                    })), Cn("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), Cn("\\TextOrMath", (function(e) {
+                    })), Bn("\\@ifstar", "\\@ifnextchar *{\\@firstoftwo{#1}}"), Bn("\\TextOrMath", (function(e) {
                         var t = e.consumeArgs(2);
                         return "text" === e.mode ? {
                             tokens: t[0],
                             numArgs: 0
                         } : {
                             tokens: t[1],
                             numArgs: 0
                         }
                     }));
-                    var qn = {
+                    var Cn = {
                         0: 0,
                         1: 1,
                         2: 2,
                         3: 3,
                         4: 4,
                         5: 5,
                         6: 6,
@@ -7536,33 +7552,33 @@
                         d: 13,
                         D: 13,
                         e: 14,
                         E: 14,
                         f: 15,
                         F: 15
                     };
-                    Cn("\\char", (function(e) {
+                    Bn("\\char", (function(e) {
                         var t, r = e.popToken(),
                             n = "";
                         if ("'" === r.text) t = 8, r = e.popToken();
                         else if ('"' === r.text) t = 16, r = e.popToken();
                         else if ("`" === r.text)
                             if ("\\" === (r = e.popToken()).text[0]) n = r.text.charCodeAt(1);
                             else {
                                 if ("EOF" === r.text) throw new o("\\char` missing argument");
                                 n = r.text.charCodeAt(0)
                             }
                         else t = 10;
                         if (t) {
-                            if (null == (n = qn[r.text]) || n >= t) throw new o("Invalid base-" + t + " digit " + r.text);
-                            for (var a; null != (a = qn[e.future().text]) && a < t;) n *= t, n += a, e.popToken()
+                            if (null == (n = Cn[r.text]) || n >= t) throw new o("Invalid base-" + t + " digit " + r.text);
+                            for (var a; null != (a = Cn[e.future().text]) && a < t;) n *= t, n += a, e.popToken()
                         }
                         return "\\@char{" + n + "}"
                     }));
-                    var Nn = function(e, t, r) {
+                    var qn = function(e, t, r) {
                         var n = e.consumeArgs(1)[0];
                         if (1 !== n.length) throw new o("\\newcommand's first argument must be a macro name");
                         var a = n[0].text,
                             i = e.isDefined(a);
                         if (i && !t) throw new o("\\newcommand{" + a + "} attempting to redefine " + a + "; use \\renewcommand");
                         if (!i && !r) throw new o("\\renewcommand{" + a + "} when command " + a + " does not yet exist; use \\newcommand");
                         var s = 0;
@@ -7573,36 +7589,36 @@
                             s = parseInt(l), n = e.consumeArgs(1)[0]
                         }
                         return e.macros.set(a, {
                             tokens: n,
                             numArgs: s
                         }), ""
                     };
-                    Cn("\\newcommand", (function(e) {
-                        return Nn(e, !1, !0)
-                    })), Cn("\\renewcommand", (function(e) {
-                        return Nn(e, !0, !1)
-                    })), Cn("\\providecommand", (function(e) {
-                        return Nn(e, !0, !0)
-                    })), Cn("\\message", (function(e) {
+                    Bn("\\newcommand", (function(e) {
+                        return qn(e, !1, !0)
+                    })), Bn("\\renewcommand", (function(e) {
+                        return qn(e, !0, !1)
+                    })), Bn("\\providecommand", (function(e) {
+                        return qn(e, !0, !0)
+                    })), Bn("\\message", (function(e) {
                         var t = e.consumeArgs(1)[0];
                         return console.log(t.reverse().map((function(e) {
                             return e.text
                         })).join("")), ""
-                    })), Cn("\\errmessage", (function(e) {
+                    })), Bn("\\errmessage", (function(e) {
                         var t = e.consumeArgs(1)[0];
                         return console.error(t.reverse().map((function(e) {
                             return e.text
                         })).join("")), ""
-                    })), Cn("\\show", (function(e) {
+                    })), Bn("\\show", (function(e) {
                         var t = e.popToken(),
                             r = t.text;
-                        return console.log(t, e.macros.get(r), kn[r], ee.math[r], ee.text[r]), ""
-                    })), Cn("\\bgroup", "{"), Cn("\\egroup", "}"), Cn("\\lq", "`"), Cn("\\rq", "'"), Cn("\\aa", "\\r a"), Cn("\\AA", "\\r A"), Cn("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`©}"), Cn("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), Cn("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`®}"), Cn("ℬ", "\\mathscr{B}"), Cn("ℰ", "\\mathscr{E}"), Cn("ℱ", "\\mathscr{F}"), Cn("ℋ", "\\mathscr{H}"), Cn("ℐ", "\\mathscr{I}"), Cn("ℒ", "\\mathscr{L}"), Cn("ℳ", "\\mathscr{M}"), Cn("ℛ", "\\mathscr{R}"), Cn("ℭ", "\\mathfrak{C}"), Cn("ℌ", "\\mathfrak{H}"), Cn("ℨ", "\\mathfrak{Z}"), Cn("\\Bbbk", "\\Bbb{k}"), Cn("·", "\\cdotp"), Cn("\\llap", "\\mathllap{\\textrm{#1}}"), Cn("\\rlap", "\\mathrlap{\\textrm{#1}}"), Cn("\\clap", "\\mathclap{\\textrm{#1}}"), Cn("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), Cn("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`≠}}"), Cn("\\ne", "\\neq"), Cn("≠", "\\neq"), Cn("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`∉}}"), Cn("∉", "\\notin"), Cn("≘", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`≘}}"), Cn("≙", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`≘}}"), Cn("≚", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`≚}}"), Cn("≛", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`≛}}"), Cn("≝", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`≝}}"), Cn("≞", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`≞}}"), Cn("≟", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`≟}}"), Cn("⟂", "\\perp"), Cn("‼", "\\mathclose{!\\mkern-0.8mu!}"), Cn("∌", "\\notni"), Cn("⌜", "\\ulcorner"), Cn("⌝", "\\urcorner"), Cn("⌞", "\\llcorner"), Cn("⌟", "\\lrcorner"), Cn("©", "\\copyright"), Cn("®", "\\textregistered"), Cn("️", "\\textregistered"), Cn("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), Cn("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), Cn("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), Cn("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), Cn("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), Cn("⋮", "\\vdots"), Cn("\\varGamma", "\\mathit{\\Gamma}"), Cn("\\varDelta", "\\mathit{\\Delta}"), Cn("\\varTheta", "\\mathit{\\Theta}"), Cn("\\varLambda", "\\mathit{\\Lambda}"), Cn("\\varXi", "\\mathit{\\Xi}"), Cn("\\varPi", "\\mathit{\\Pi}"), Cn("\\varSigma", "\\mathit{\\Sigma}"), Cn("\\varUpsilon", "\\mathit{\\Upsilon}"), Cn("\\varPhi", "\\mathit{\\Phi}"), Cn("\\varPsi", "\\mathit{\\Psi}"), Cn("\\varOmega", "\\mathit{\\Omega}"), Cn("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), Cn("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu"), Cn("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), Cn("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), Cn("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), Cn("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
-                    var In = {
+                        return console.log(t, e.macros.get(r), gn[r], j.math[r], j.text[r]), ""
+                    })), Bn("\\bgroup", "{"), Bn("\\egroup", "}"), Bn("\\lq", "`"), Bn("\\rq", "'"), Bn("\\aa", "\\r a"), Bn("\\AA", "\\r A"), Bn("\\textcopyright", "\\html@mathml{\\textcircled{c}}{\\char`©}"), Bn("\\copyright", "\\TextOrMath{\\textcopyright}{\\text{\\textcopyright}}"), Bn("\\textregistered", "\\html@mathml{\\textcircled{\\scriptsize R}}{\\char`®}"), Bn("ℬ", "\\mathscr{B}"), Bn("ℰ", "\\mathscr{E}"), Bn("ℱ", "\\mathscr{F}"), Bn("ℋ", "\\mathscr{H}"), Bn("ℐ", "\\mathscr{I}"), Bn("ℒ", "\\mathscr{L}"), Bn("ℳ", "\\mathscr{M}"), Bn("ℛ", "\\mathscr{R}"), Bn("ℭ", "\\mathfrak{C}"), Bn("ℌ", "\\mathfrak{H}"), Bn("ℨ", "\\mathfrak{Z}"), Bn("\\Bbbk", "\\Bbb{k}"), Bn("·", "\\cdotp"), Bn("\\llap", "\\mathllap{\\textrm{#1}}"), Bn("\\rlap", "\\mathrlap{\\textrm{#1}}"), Bn("\\clap", "\\mathclap{\\textrm{#1}}"), Bn("\\not", '\\html@mathml{\\mathrel{\\mathrlap\\@not}}{\\char"338}'), Bn("\\neq", "\\html@mathml{\\mathrel{\\not=}}{\\mathrel{\\char`≠}}"), Bn("\\ne", "\\neq"), Bn("≠", "\\neq"), Bn("\\notin", "\\html@mathml{\\mathrel{{\\in}\\mathllap{/\\mskip1mu}}}{\\mathrel{\\char`∉}}"), Bn("∉", "\\notin"), Bn("≘", "\\html@mathml{\\mathrel{=\\kern{-1em}\\raisebox{0.4em}{$\\scriptsize\\frown$}}}{\\mathrel{\\char`≘}}"), Bn("≙", "\\html@mathml{\\stackrel{\\tiny\\wedge}{=}}{\\mathrel{\\char`≘}}"), Bn("≚", "\\html@mathml{\\stackrel{\\tiny\\vee}{=}}{\\mathrel{\\char`≚}}"), Bn("≛", "\\html@mathml{\\stackrel{\\scriptsize\\star}{=}}{\\mathrel{\\char`≛}}"), Bn("≝", "\\html@mathml{\\stackrel{\\tiny\\mathrm{def}}{=}}{\\mathrel{\\char`≝}}"), Bn("≞", "\\html@mathml{\\stackrel{\\tiny\\mathrm{m}}{=}}{\\mathrel{\\char`≞}}"), Bn("≟", "\\html@mathml{\\stackrel{\\tiny?}{=}}{\\mathrel{\\char`≟}}"), Bn("⟂", "\\perp"), Bn("‼", "\\mathclose{!\\mkern-0.8mu!}"), Bn("∌", "\\notni"), Bn("⌜", "\\ulcorner"), Bn("⌝", "\\urcorner"), Bn("⌞", "\\llcorner"), Bn("⌟", "\\lrcorner"), Bn("©", "\\copyright"), Bn("®", "\\textregistered"), Bn("️", "\\textregistered"), Bn("\\ulcorner", '\\html@mathml{\\@ulcorner}{\\mathop{\\char"231c}}'), Bn("\\urcorner", '\\html@mathml{\\@urcorner}{\\mathop{\\char"231d}}'), Bn("\\llcorner", '\\html@mathml{\\@llcorner}{\\mathop{\\char"231e}}'), Bn("\\lrcorner", '\\html@mathml{\\@lrcorner}{\\mathop{\\char"231f}}'), Bn("\\vdots", "\\mathord{\\varvdots\\rule{0pt}{15pt}}"), Bn("⋮", "\\vdots"), Bn("\\varGamma", "\\mathit{\\Gamma}"), Bn("\\varDelta", "\\mathit{\\Delta}"), Bn("\\varTheta", "\\mathit{\\Theta}"), Bn("\\varLambda", "\\mathit{\\Lambda}"), Bn("\\varXi", "\\mathit{\\Xi}"), Bn("\\varPi", "\\mathit{\\Pi}"), Bn("\\varSigma", "\\mathit{\\Sigma}"), Bn("\\varUpsilon", "\\mathit{\\Upsilon}"), Bn("\\varPhi", "\\mathit{\\Phi}"), Bn("\\varPsi", "\\mathit{\\Psi}"), Bn("\\varOmega", "\\mathit{\\Omega}"), Bn("\\substack", "\\begin{subarray}{c}#1\\end{subarray}"), Bn("\\colon", "\\nobreak\\mskip2mu\\mathpunct{}\\mathchoice{\\mkern-3mu}{\\mkern-3mu}{}{}{:}\\mskip6mu"), Bn("\\boxed", "\\fbox{$\\displaystyle{#1}$}"), Bn("\\iff", "\\DOTSB\\;\\Longleftrightarrow\\;"), Bn("\\implies", "\\DOTSB\\;\\Longrightarrow\\;"), Bn("\\impliedby", "\\DOTSB\\;\\Longleftarrow\\;");
+                    var Nn = {
                         ",": "\\dotsc",
                         "\\not": "\\dotsb",
                         "+": "\\dotsb",
                         "=": "\\dotsb",
                         "<": "\\dotsb",
                         ">": "\\dotsb",
                         "-": "\\dotsb",
@@ -7643,20 +7659,20 @@
                         "\\oint": "\\dotsi",
                         "\\iint": "\\dotsi",
                         "\\iiint": "\\dotsi",
                         "\\iiiint": "\\dotsi",
                         "\\idotsint": "\\dotsi",
                         "\\DOTSX": "\\dotsx"
                     };
-                    Cn("\\dots", (function(e) {
+                    Bn("\\dots", (function(e) {
                         var t = "\\dotso",
                             r = e.expandAfterFuture().text;
-                        return r in In ? t = In[r] : ("\\not" === r.substr(0, 4) || r in ee.math && c(["bin", "rel"], ee.math[r].group)) && (t = "\\dotsb"), t
+                        return r in Nn ? t = Nn[r] : ("\\not" === r.substr(0, 4) || r in j.math && c.contains(["bin", "rel"], j.math[r].group)) && (t = "\\dotsb"), t
                     }));
-                    var On = {
+                    var In = {
                         ")": !0,
                         "]": !0,
                         "\\rbrack": !0,
                         "\\}": !0,
                         "\\rbrace": !0,
                         "\\rangle": !0,
                         "\\rceil": !0,
@@ -7669,41 +7685,41 @@
                         "\\Bigr": !0,
                         "\\Biggr": !0,
                         $: !0,
                         ";": !0,
                         ".": !0,
                         ",": !0
                     };
-                    Cn("\\dotso", (function(e) {
-                        return e.future().text in On ? "\\ldots\\," : "\\ldots"
-                    })), Cn("\\dotsc", (function(e) {
+                    Bn("\\dotso", (function(e) {
+                        return e.future().text in In ? "\\ldots\\," : "\\ldots"
+                    })), Bn("\\dotsc", (function(e) {
                         var t = e.future().text;
-                        return t in On && "," !== t ? "\\ldots\\," : "\\ldots"
-                    })), Cn("\\cdots", (function(e) {
-                        return e.future().text in On ? "\\@cdots\\," : "\\@cdots"
-                    })), Cn("\\dotsb", "\\cdots"), Cn("\\dotsm", "\\cdots"), Cn("\\dotsi", "\\!\\cdots"), Cn("\\dotsx", "\\ldots\\,"), Cn("\\DOTSI", "\\relax"), Cn("\\DOTSB", "\\relax"), Cn("\\DOTSX", "\\relax"), Cn("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), Cn("\\,", "\\tmspace+{3mu}{.1667em}"), Cn("\\thinspace", "\\,"), Cn("\\>", "\\mskip{4mu}"), Cn("\\:", "\\tmspace+{4mu}{.2222em}"), Cn("\\medspace", "\\:"), Cn("\\;", "\\tmspace+{5mu}{.2777em}"), Cn("\\thickspace", "\\;"), Cn("\\!", "\\tmspace-{3mu}{.1667em}"), Cn("\\negthinspace", "\\!"), Cn("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), Cn("\\negthickspace", "\\tmspace-{5mu}{.277em}"), Cn("\\enspace", "\\kern.5em "), Cn("\\enskip", "\\hskip.5em\\relax"), Cn("\\quad", "\\hskip1em\\relax"), Cn("\\qquad", "\\hskip2em\\relax"), Cn("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), Cn("\\tag@paren", "\\tag@literal{({#1})}"), Cn("\\tag@literal", (function(e) {
+                        return t in In && "," !== t ? "\\ldots\\," : "\\ldots"
+                    })), Bn("\\cdots", (function(e) {
+                        return e.future().text in In ? "\\@cdots\\," : "\\@cdots"
+                    })), Bn("\\dotsb", "\\cdots"), Bn("\\dotsm", "\\cdots"), Bn("\\dotsi", "\\!\\cdots"), Bn("\\dotsx", "\\ldots\\,"), Bn("\\DOTSI", "\\relax"), Bn("\\DOTSB", "\\relax"), Bn("\\DOTSX", "\\relax"), Bn("\\tmspace", "\\TextOrMath{\\kern#1#3}{\\mskip#1#2}\\relax"), Bn("\\,", "\\tmspace+{3mu}{.1667em}"), Bn("\\thinspace", "\\,"), Bn("\\>", "\\mskip{4mu}"), Bn("\\:", "\\tmspace+{4mu}{.2222em}"), Bn("\\medspace", "\\:"), Bn("\\;", "\\tmspace+{5mu}{.2777em}"), Bn("\\thickspace", "\\;"), Bn("\\!", "\\tmspace-{3mu}{.1667em}"), Bn("\\negthinspace", "\\!"), Bn("\\negmedspace", "\\tmspace-{4mu}{.2222em}"), Bn("\\negthickspace", "\\tmspace-{5mu}{.277em}"), Bn("\\enspace", "\\kern.5em "), Bn("\\enskip", "\\hskip.5em\\relax"), Bn("\\quad", "\\hskip1em\\relax"), Bn("\\qquad", "\\hskip2em\\relax"), Bn("\\tag", "\\@ifstar\\tag@literal\\tag@paren"), Bn("\\tag@paren", "\\tag@literal{({#1})}"), Bn("\\tag@literal", (function(e) {
                         if (e.macros.get("\\df@tag")) throw new o("Multiple \\tag");
                         return "\\gdef\\df@tag{\\text{#1}}"
-                    })), Cn("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), Cn("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), Cn("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), Cn("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), Cn("\\pmb", "\\html@mathml{\\@binrel{#1}{\\mathrlap{#1}\\kern0.5px#1}}{\\mathbf{#1}}"), Cn("\\\\", "\\newline"), Cn("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
-                    var Rn = W["Main-Regular"]["T".charCodeAt(0)][1] - .7 * W["Main-Regular"]["A".charCodeAt(0)][1] + "em";
-                    Cn("\\LaTeX", "\\textrm{\\html@mathml{L\\kern-.36em\\raisebox{" + Rn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{LaTeX}}"), Cn("\\KaTeX", "\\textrm{\\html@mathml{K\\kern-.17em\\raisebox{" + Rn + "}{\\scriptstyle A}\\kern-.15em\\TeX}{KaTeX}}"), Cn("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), Cn("\\@hspace", "\\hskip #1\\relax"), Cn("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), Cn("\\ordinarycolon", ":"), Cn("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), Cn("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), Cn("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), Cn("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), Cn("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), Cn("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), Cn("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), Cn("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), Cn("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), Cn("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), Cn("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), Cn("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), Cn("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), Cn("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), Cn("∷", "\\dblcolon"), Cn("∹", "\\eqcolon"), Cn("≔", "\\coloneqq"), Cn("≕", "\\eqqcolon"), Cn("⩴", "\\Coloneqq"), Cn("\\ratio", "\\vcentcolon"), Cn("\\coloncolon", "\\dblcolon"), Cn("\\colonequals", "\\coloneqq"), Cn("\\coloncolonequals", "\\Coloneqq"), Cn("\\equalscolon", "\\eqqcolon"), Cn("\\equalscoloncolon", "\\Eqqcolon"), Cn("\\colonminus", "\\coloneq"), Cn("\\coloncolonminus", "\\Coloneq"), Cn("\\minuscolon", "\\eqcolon"), Cn("\\minuscoloncolon", "\\Eqcolon"), Cn("\\coloncolonapprox", "\\Colonapprox"), Cn("\\coloncolonsim", "\\Colonsim"), Cn("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Cn("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Cn("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Cn("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Cn("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`∌}}"), Cn("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), Cn("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), Cn("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{≩}"), Cn("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{≨}"), Cn("\\ngeqq", "\\html@mathml{\\@ngeqq}{≱}"), Cn("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{≱}"), Cn("\\nleqq", "\\html@mathml{\\@nleqq}{≰}"), Cn("\\nleqslant", "\\html@mathml{\\@nleqslant}{≰}"), Cn("\\nshortmid", "\\html@mathml{\\@nshortmid}{∤}"), Cn("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{∦}"), Cn("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{⊈}"), Cn("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{⊉}"), Cn("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{⊊}"), Cn("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{⫋}"), Cn("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{⊋}"), Cn("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{⫌}"), Cn("\\imath", "\\html@mathml{\\@imath}{ı}"), Cn("\\jmath", "\\html@mathml{\\@jmath}{ȷ}"), Cn("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`⟦}}"), Cn("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`⟧}}"), Cn("⟦", "\\llbracket"), Cn("⟧", "\\rrbracket"), Cn("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`⦃}}"), Cn("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`⦄}}"), Cn("⦃", "\\lBrace"), Cn("⦄", "\\rBrace"), Cn("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`⦵}}"), Cn("⦵", "\\minuso"), Cn("\\darr", "\\downarrow"), Cn("\\dArr", "\\Downarrow"), Cn("\\Darr", "\\Downarrow"), Cn("\\lang", "\\langle"), Cn("\\rang", "\\rangle"), Cn("\\uarr", "\\uparrow"), Cn("\\uArr", "\\Uparrow"), Cn("\\Uarr", "\\Uparrow"), Cn("\\N", "\\mathbb{N}"), Cn("\\R", "\\mathbb{R}"), Cn("\\Z", "\\mathbb{Z}"), Cn("\\alef", "\\aleph"), Cn("\\alefsym", "\\aleph"), Cn("\\Alpha", "\\mathrm{A}"), Cn("\\Beta", "\\mathrm{B}"), Cn("\\bull", "\\bullet"), Cn("\\Chi", "\\mathrm{X}"), Cn("\\clubs", "\\clubsuit"), Cn("\\cnums", "\\mathbb{C}"), Cn("\\Complex", "\\mathbb{C}"), Cn("\\Dagger", "\\ddagger"), Cn("\\diamonds", "\\diamondsuit"), Cn("\\empty", "\\emptyset"), Cn("\\Epsilon", "\\mathrm{E}"), Cn("\\Eta", "\\mathrm{H}"), Cn("\\exist", "\\exists"), Cn("\\harr", "\\leftrightarrow"), Cn("\\hArr", "\\Leftrightarrow"), Cn("\\Harr", "\\Leftrightarrow"), Cn("\\hearts", "\\heartsuit"), Cn("\\image", "\\Im"), Cn("\\infin", "\\infty"), Cn("\\Iota", "\\mathrm{I}"), Cn("\\isin", "\\in"), Cn("\\Kappa", "\\mathrm{K}"), Cn("\\larr", "\\leftarrow"), Cn("\\lArr", "\\Leftarrow"), Cn("\\Larr", "\\Leftarrow"), Cn("\\lrarr", "\\leftrightarrow"), Cn("\\lrArr", "\\Leftrightarrow"), Cn("\\Lrarr", "\\Leftrightarrow"), Cn("\\Mu", "\\mathrm{M}"), Cn("\\natnums", "\\mathbb{N}"), Cn("\\Nu", "\\mathrm{N}"), Cn("\\Omicron", "\\mathrm{O}"), Cn("\\plusmn", "\\pm"), Cn("\\rarr", "\\rightarrow"), Cn("\\rArr", "\\Rightarrow"), Cn("\\Rarr", "\\Rightarrow"), Cn("\\real", "\\Re"), Cn("\\reals", "\\mathbb{R}"), Cn("\\Reals", "\\mathbb{R}"), Cn("\\Rho", "\\mathrm{P}"), Cn("\\sdot", "\\cdot"), Cn("\\sect", "\\S"), Cn("\\spades", "\\spadesuit"), Cn("\\sub", "\\subset"), Cn("\\sube", "\\subseteq"), Cn("\\supe", "\\supseteq"), Cn("\\Tau", "\\mathrm{T}"), Cn("\\thetasym", "\\vartheta"), Cn("\\weierp", "\\wp"), Cn("\\Zeta", "\\mathrm{Z}"), Cn("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), Cn("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), Cn("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), Cn("\\bra", "\\mathinner{\\langle{#1}|}"), Cn("\\ket", "\\mathinner{|{#1}\\rangle}"), Cn("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), Cn("\\Bra", "\\left\\langle#1\\right|"), Cn("\\Ket", "\\left|#1\\right\\rangle"), Cn("\\blue", "\\textcolor{##6495ed}{#1}"), Cn("\\orange", "\\textcolor{##ffa500}{#1}"), Cn("\\pink", "\\textcolor{##ff00af}{#1}"), Cn("\\red", "\\textcolor{##df0030}{#1}"), Cn("\\green", "\\textcolor{##28ae7b}{#1}"), Cn("\\gray", "\\textcolor{gray}{#1}"), Cn("\\purple", "\\textcolor{##9d38bd}{#1}"), Cn("\\blueA", "\\textcolor{##ccfaff}{#1}"), Cn("\\blueB", "\\textcolor{##80f6ff}{#1}"), Cn("\\blueC", "\\textcolor{##63d9ea}{#1}"), Cn("\\blueD", "\\textcolor{##11accd}{#1}"), Cn("\\blueE", "\\textcolor{##0c7f99}{#1}"), Cn("\\tealA", "\\textcolor{##94fff5}{#1}"), Cn("\\tealB", "\\textcolor{##26edd5}{#1}"), Cn("\\tealC", "\\textcolor{##01d1c1}{#1}"), Cn("\\tealD", "\\textcolor{##01a995}{#1}"), Cn("\\tealE", "\\textcolor{##208170}{#1}"), Cn("\\greenA", "\\textcolor{##b6ffb0}{#1}"), Cn("\\greenB", "\\textcolor{##8af281}{#1}"), Cn("\\greenC", "\\textcolor{##74cf70}{#1}"), Cn("\\greenD", "\\textcolor{##1fab54}{#1}"), Cn("\\greenE", "\\textcolor{##0d923f}{#1}"), Cn("\\goldA", "\\textcolor{##ffd0a9}{#1}"), Cn("\\goldB", "\\textcolor{##ffbb71}{#1}"), Cn("\\goldC", "\\textcolor{##ff9c39}{#1}"), Cn("\\goldD", "\\textcolor{##e07d10}{#1}"), Cn("\\goldE", "\\textcolor{##a75a05}{#1}"), Cn("\\redA", "\\textcolor{##fca9a9}{#1}"), Cn("\\redB", "\\textcolor{##ff8482}{#1}"), Cn("\\redC", "\\textcolor{##f9685d}{#1}"), Cn("\\redD", "\\textcolor{##e84d39}{#1}"), Cn("\\redE", "\\textcolor{##bc2612}{#1}"), Cn("\\maroonA", "\\textcolor{##ffbde0}{#1}"), Cn("\\maroonB", "\\textcolor{##ff92c6}{#1}"), Cn("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), Cn("\\maroonD", "\\textcolor{##ca337c}{#1}"), Cn("\\maroonE", "\\textcolor{##9e034e}{#1}"), Cn("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), Cn("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), Cn("\\purpleC", "\\textcolor{##aa87ff}{#1}"), Cn("\\purpleD", "\\textcolor{##7854ab}{#1}"), Cn("\\purpleE", "\\textcolor{##543b78}{#1}"), Cn("\\mintA", "\\textcolor{##f5f9e8}{#1}"), Cn("\\mintB", "\\textcolor{##edf2df}{#1}"), Cn("\\mintC", "\\textcolor{##e0e5cc}{#1}"), Cn("\\grayA", "\\textcolor{##f6f7f7}{#1}"), Cn("\\grayB", "\\textcolor{##f0f1f2}{#1}"), Cn("\\grayC", "\\textcolor{##e3e5e6}{#1}"), Cn("\\grayD", "\\textcolor{##d6d8da}{#1}"), Cn("\\grayE", "\\textcolor{##babec2}{#1}"), Cn("\\grayF", "\\textcolor{##888d93}{#1}"), Cn("\\grayG", "\\textcolor{##626569}{#1}"), Cn("\\grayH", "\\textcolor{##3b3e40}{#1}"), Cn("\\grayI", "\\textcolor{##21242c}{#1}"), Cn("\\kaBlue", "\\textcolor{##314453}{#1}"), Cn("\\kaGreen", "\\textcolor{##71B307}{#1}");
-                    var En = {
+                    })), Bn("\\bmod", "\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}\\mathbin{\\rm mod}\\mathchoice{\\mskip1mu}{\\mskip1mu}{\\mskip5mu}{\\mskip5mu}"), Bn("\\pod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern8mu}{\\mkern8mu}{\\mkern8mu}(#1)"), Bn("\\pmod", "\\pod{{\\rm mod}\\mkern6mu#1}"), Bn("\\mod", "\\allowbreak\\mathchoice{\\mkern18mu}{\\mkern12mu}{\\mkern12mu}{\\mkern12mu}{\\rm mod}\\,\\,#1"), Bn("\\pmb", "\\html@mathml{\\@binrel{#1}{\\mathrlap{#1}\\kern0.5px#1}}{\\mathbf{#1}}"), Bn("\\\\", "\\newline"), Bn("\\TeX", "\\textrm{\\html@mathml{T\\kern-.1667em\\raisebox{-.5ex}{E}\\kern-.125emX}{TeX}}");
+                    var On = F["Main-Regular"]["T".charCodeAt(0)][1] - .7 * F["Main-Regular"]["A".charCodeAt(0)][1] + "em";
+                    Bn("\\LaTeX", "\\textrm{\\html@mathml{L\\kern-.36em\\raisebox{" + On + "}{\\scriptstyle A}\\kern-.15em\\TeX}{LaTeX}}"), Bn("\\KaTeX", "\\textrm{\\html@mathml{K\\kern-.17em\\raisebox{" + On + "}{\\scriptstyle A}\\kern-.15em\\TeX}{KaTeX}}"), Bn("\\hspace", "\\@ifstar\\@hspacer\\@hspace"), Bn("\\@hspace", "\\hskip #1\\relax"), Bn("\\@hspacer", "\\rule{0pt}{0pt}\\hskip #1\\relax"), Bn("\\ordinarycolon", ":"), Bn("\\vcentcolon", "\\mathrel{\\mathop\\ordinarycolon}"), Bn("\\dblcolon", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-.9mu}\\vcentcolon}}{\\mathop{\\char"2237}}'), Bn("\\coloneqq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2254}}'), Bn("\\Coloneqq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}=}}{\\mathop{\\char"2237\\char"3d}}'), Bn("\\coloneq", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"3a\\char"2212}}'), Bn("\\Coloneq", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\mathrel{-}}}{\\mathop{\\char"2237\\char"2212}}'), Bn("\\eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2255}}'), Bn("\\Eqqcolon", '\\html@mathml{\\mathrel{=\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"3d\\char"2237}}'), Bn("\\eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\vcentcolon}}{\\mathop{\\char"2239}}'), Bn("\\Eqcolon", '\\html@mathml{\\mathrel{\\mathrel{-}\\mathrel{\\mkern-1.2mu}\\dblcolon}}{\\mathop{\\char"2212\\char"2237}}'), Bn("\\colonapprox", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"3a\\char"2248}}'), Bn("\\Colonapprox", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\approx}}{\\mathop{\\char"2237\\char"2248}}'), Bn("\\colonsim", '\\html@mathml{\\mathrel{\\vcentcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"3a\\char"223c}}'), Bn("\\Colonsim", '\\html@mathml{\\mathrel{\\dblcolon\\mathrel{\\mkern-1.2mu}\\sim}}{\\mathop{\\char"2237\\char"223c}}'), Bn("∷", "\\dblcolon"), Bn("∹", "\\eqcolon"), Bn("≔", "\\coloneqq"), Bn("≕", "\\eqqcolon"), Bn("⩴", "\\Coloneqq"), Bn("\\ratio", "\\vcentcolon"), Bn("\\coloncolon", "\\dblcolon"), Bn("\\colonequals", "\\coloneqq"), Bn("\\coloncolonequals", "\\Coloneqq"), Bn("\\equalscolon", "\\eqqcolon"), Bn("\\equalscoloncolon", "\\Eqqcolon"), Bn("\\colonminus", "\\coloneq"), Bn("\\coloncolonminus", "\\Coloneq"), Bn("\\minuscolon", "\\eqcolon"), Bn("\\minuscoloncolon", "\\Eqcolon"), Bn("\\coloncolonapprox", "\\Colonapprox"), Bn("\\coloncolonsim", "\\Colonsim"), Bn("\\simcolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Bn("\\simcoloncolon", "\\mathrel{\\sim\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Bn("\\approxcolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\vcentcolon}"), Bn("\\approxcoloncolon", "\\mathrel{\\approx\\mathrel{\\mkern-1.2mu}\\dblcolon}"), Bn("\\notni", "\\html@mathml{\\not\\ni}{\\mathrel{\\char`∌}}"), Bn("\\limsup", "\\DOTSB\\operatorname*{lim\\,sup}"), Bn("\\liminf", "\\DOTSB\\operatorname*{lim\\,inf}"), Bn("\\gvertneqq", "\\html@mathml{\\@gvertneqq}{≩}"), Bn("\\lvertneqq", "\\html@mathml{\\@lvertneqq}{≨}"), Bn("\\ngeqq", "\\html@mathml{\\@ngeqq}{≱}"), Bn("\\ngeqslant", "\\html@mathml{\\@ngeqslant}{≱}"), Bn("\\nleqq", "\\html@mathml{\\@nleqq}{≰}"), Bn("\\nleqslant", "\\html@mathml{\\@nleqslant}{≰}"), Bn("\\nshortmid", "\\html@mathml{\\@nshortmid}{∤}"), Bn("\\nshortparallel", "\\html@mathml{\\@nshortparallel}{∦}"), Bn("\\nsubseteqq", "\\html@mathml{\\@nsubseteqq}{⊈}"), Bn("\\nsupseteqq", "\\html@mathml{\\@nsupseteqq}{⊉}"), Bn("\\varsubsetneq", "\\html@mathml{\\@varsubsetneq}{⊊}"), Bn("\\varsubsetneqq", "\\html@mathml{\\@varsubsetneqq}{⫋}"), Bn("\\varsupsetneq", "\\html@mathml{\\@varsupsetneq}{⊋}"), Bn("\\varsupsetneqq", "\\html@mathml{\\@varsupsetneqq}{⫌}"), Bn("\\imath", "\\html@mathml{\\@imath}{ı}"), Bn("\\jmath", "\\html@mathml{\\@jmath}{ȷ}"), Bn("\\llbracket", "\\html@mathml{\\mathopen{[\\mkern-3.2mu[}}{\\mathopen{\\char`⟦}}"), Bn("\\rrbracket", "\\html@mathml{\\mathclose{]\\mkern-3.2mu]}}{\\mathclose{\\char`⟧}}"), Bn("⟦", "\\llbracket"), Bn("⟧", "\\rrbracket"), Bn("\\lBrace", "\\html@mathml{\\mathopen{\\{\\mkern-3.2mu[}}{\\mathopen{\\char`⦃}}"), Bn("\\rBrace", "\\html@mathml{\\mathclose{]\\mkern-3.2mu\\}}}{\\mathclose{\\char`⦄}}"), Bn("⦃", "\\lBrace"), Bn("⦄", "\\rBrace"), Bn("\\minuso", "\\mathbin{\\html@mathml{{\\mathrlap{\\mathchoice{\\kern{0.145em}}{\\kern{0.145em}}{\\kern{0.1015em}}{\\kern{0.0725em}}\\circ}{-}}}{\\char`⦵}}"), Bn("⦵", "\\minuso"), Bn("\\darr", "\\downarrow"), Bn("\\dArr", "\\Downarrow"), Bn("\\Darr", "\\Downarrow"), Bn("\\lang", "\\langle"), Bn("\\rang", "\\rangle"), Bn("\\uarr", "\\uparrow"), Bn("\\uArr", "\\Uparrow"), Bn("\\Uarr", "\\Uparrow"), Bn("\\N", "\\mathbb{N}"), Bn("\\R", "\\mathbb{R}"), Bn("\\Z", "\\mathbb{Z}"), Bn("\\alef", "\\aleph"), Bn("\\alefsym", "\\aleph"), Bn("\\Alpha", "\\mathrm{A}"), Bn("\\Beta", "\\mathrm{B}"), Bn("\\bull", "\\bullet"), Bn("\\Chi", "\\mathrm{X}"), Bn("\\clubs", "\\clubsuit"), Bn("\\cnums", "\\mathbb{C}"), Bn("\\Complex", "\\mathbb{C}"), Bn("\\Dagger", "\\ddagger"), Bn("\\diamonds", "\\diamondsuit"), Bn("\\empty", "\\emptyset"), Bn("\\Epsilon", "\\mathrm{E}"), Bn("\\Eta", "\\mathrm{H}"), Bn("\\exist", "\\exists"), Bn("\\harr", "\\leftrightarrow"), Bn("\\hArr", "\\Leftrightarrow"), Bn("\\Harr", "\\Leftrightarrow"), Bn("\\hearts", "\\heartsuit"), Bn("\\image", "\\Im"), Bn("\\infin", "\\infty"), Bn("\\Iota", "\\mathrm{I}"), Bn("\\isin", "\\in"), Bn("\\Kappa", "\\mathrm{K}"), Bn("\\larr", "\\leftarrow"), Bn("\\lArr", "\\Leftarrow"), Bn("\\Larr", "\\Leftarrow"), Bn("\\lrarr", "\\leftrightarrow"), Bn("\\lrArr", "\\Leftrightarrow"), Bn("\\Lrarr", "\\Leftrightarrow"), Bn("\\Mu", "\\mathrm{M}"), Bn("\\natnums", "\\mathbb{N}"), Bn("\\Nu", "\\mathrm{N}"), Bn("\\Omicron", "\\mathrm{O}"), Bn("\\plusmn", "\\pm"), Bn("\\rarr", "\\rightarrow"), Bn("\\rArr", "\\Rightarrow"), Bn("\\Rarr", "\\Rightarrow"), Bn("\\real", "\\Re"), Bn("\\reals", "\\mathbb{R}"), Bn("\\Reals", "\\mathbb{R}"), Bn("\\Rho", "\\mathrm{P}"), Bn("\\sdot", "\\cdot"), Bn("\\sect", "\\S"), Bn("\\spades", "\\spadesuit"), Bn("\\sub", "\\subset"), Bn("\\sube", "\\subseteq"), Bn("\\supe", "\\supseteq"), Bn("\\Tau", "\\mathrm{T}"), Bn("\\thetasym", "\\vartheta"), Bn("\\weierp", "\\wp"), Bn("\\Zeta", "\\mathrm{Z}"), Bn("\\argmin", "\\DOTSB\\operatorname*{arg\\,min}"), Bn("\\argmax", "\\DOTSB\\operatorname*{arg\\,max}"), Bn("\\plim", "\\DOTSB\\mathop{\\operatorname{plim}}\\limits"), Bn("\\bra", "\\mathinner{\\langle{#1}|}"), Bn("\\ket", "\\mathinner{|{#1}\\rangle}"), Bn("\\braket", "\\mathinner{\\langle{#1}\\rangle}"), Bn("\\Bra", "\\left\\langle#1\\right|"), Bn("\\Ket", "\\left|#1\\right\\rangle"), Bn("\\blue", "\\textcolor{##6495ed}{#1}"), Bn("\\orange", "\\textcolor{##ffa500}{#1}"), Bn("\\pink", "\\textcolor{##ff00af}{#1}"), Bn("\\red", "\\textcolor{##df0030}{#1}"), Bn("\\green", "\\textcolor{##28ae7b}{#1}"), Bn("\\gray", "\\textcolor{gray}{#1}"), Bn("\\purple", "\\textcolor{##9d38bd}{#1}"), Bn("\\blueA", "\\textcolor{##ccfaff}{#1}"), Bn("\\blueB", "\\textcolor{##80f6ff}{#1}"), Bn("\\blueC", "\\textcolor{##63d9ea}{#1}"), Bn("\\blueD", "\\textcolor{##11accd}{#1}"), Bn("\\blueE", "\\textcolor{##0c7f99}{#1}"), Bn("\\tealA", "\\textcolor{##94fff5}{#1}"), Bn("\\tealB", "\\textcolor{##26edd5}{#1}"), Bn("\\tealC", "\\textcolor{##01d1c1}{#1}"), Bn("\\tealD", "\\textcolor{##01a995}{#1}"), Bn("\\tealE", "\\textcolor{##208170}{#1}"), Bn("\\greenA", "\\textcolor{##b6ffb0}{#1}"), Bn("\\greenB", "\\textcolor{##8af281}{#1}"), Bn("\\greenC", "\\textcolor{##74cf70}{#1}"), Bn("\\greenD", "\\textcolor{##1fab54}{#1}"), Bn("\\greenE", "\\textcolor{##0d923f}{#1}"), Bn("\\goldA", "\\textcolor{##ffd0a9}{#1}"), Bn("\\goldB", "\\textcolor{##ffbb71}{#1}"), Bn("\\goldC", "\\textcolor{##ff9c39}{#1}"), Bn("\\goldD", "\\textcolor{##e07d10}{#1}"), Bn("\\goldE", "\\textcolor{##a75a05}{#1}"), Bn("\\redA", "\\textcolor{##fca9a9}{#1}"), Bn("\\redB", "\\textcolor{##ff8482}{#1}"), Bn("\\redC", "\\textcolor{##f9685d}{#1}"), Bn("\\redD", "\\textcolor{##e84d39}{#1}"), Bn("\\redE", "\\textcolor{##bc2612}{#1}"), Bn("\\maroonA", "\\textcolor{##ffbde0}{#1}"), Bn("\\maroonB", "\\textcolor{##ff92c6}{#1}"), Bn("\\maroonC", "\\textcolor{##ed5fa6}{#1}"), Bn("\\maroonD", "\\textcolor{##ca337c}{#1}"), Bn("\\maroonE", "\\textcolor{##9e034e}{#1}"), Bn("\\purpleA", "\\textcolor{##ddd7ff}{#1}"), Bn("\\purpleB", "\\textcolor{##c6b9fc}{#1}"), Bn("\\purpleC", "\\textcolor{##aa87ff}{#1}"), Bn("\\purpleD", "\\textcolor{##7854ab}{#1}"), Bn("\\purpleE", "\\textcolor{##543b78}{#1}"), Bn("\\mintA", "\\textcolor{##f5f9e8}{#1}"), Bn("\\mintB", "\\textcolor{##edf2df}{#1}"), Bn("\\mintC", "\\textcolor{##e0e5cc}{#1}"), Bn("\\grayA", "\\textcolor{##f6f7f7}{#1}"), Bn("\\grayB", "\\textcolor{##f0f1f2}{#1}"), Bn("\\grayC", "\\textcolor{##e3e5e6}{#1}"), Bn("\\grayD", "\\textcolor{##d6d8da}{#1}"), Bn("\\grayE", "\\textcolor{##babec2}{#1}"), Bn("\\grayF", "\\textcolor{##888d93}{#1}"), Bn("\\grayG", "\\textcolor{##626569}{#1}"), Bn("\\grayH", "\\textcolor{##3b3e40}{#1}"), Bn("\\grayI", "\\textcolor{##21242c}{#1}"), Bn("\\kaBlue", "\\textcolor{##314453}{#1}"), Bn("\\kaGreen", "\\textcolor{##71B307}{#1}");
+                    var Rn = {
                             "\\relax": !0,
                             "^": !0,
                             _: !0,
                             "\\limits": !0,
                             "\\nolimits": !0
                         },
-                        Ln = function() {
+                        En = function() {
                             function e(e, t, r) {
-                                this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = t, this.expansionCount = 0, this.feed(e), this.macros = new An(Bn, t.macros), this.mode = r, this.stack = []
+                                this.settings = void 0, this.expansionCount = void 0, this.lexer = void 0, this.macros = void 0, this.stack = void 0, this.mode = void 0, this.settings = t, this.expansionCount = 0, this.feed(e), this.macros = new zn(Tn, t.macros), this.mode = r, this.stack = []
                             }
                             var t = e.prototype;
                             return t.feed = function(e) {
-                                this.lexer = new zn(e, this.settings)
+                                this.lexer = new Mn(e, this.settings)
                             }, t.switchMode = function(e) {
                                 this.mode = e
                             }, t.beginGroup = function() {
                                 this.macros.beginGroup()
                             }, t.endGroup = function() {
                                 this.macros.endGroup()
                             }, t.future = function() {
@@ -7790,30 +7806,30 @@
                                 var t = this.macros.get(e);
                                 if (null == t) return t;
                                 var r = "function" == typeof t ? t(this) : t;
                                 if ("string" == typeof r) {
                                     var n = 0;
                                     if (-1 !== r.indexOf("#"))
                                         for (var a = r.replace(/##/g, ""); - 1 !== a.indexOf("#" + (n + 1));) ++n;
-                                    for (var i = new zn(r, this.settings), o = [], s = i.lex();
+                                    for (var i = new Mn(r, this.settings), o = [], s = i.lex();
                                         "EOF" !== s.text;) o.push(s), s = i.lex();
                                     return o.reverse(), {
                                         tokens: o,
                                         numArgs: n
                                     }
                                 }
                                 return r
                             }, t.isDefined = function(e) {
-                                return this.macros.has(e) || kn.hasOwnProperty(e) || ee.math.hasOwnProperty(e) || ee.text.hasOwnProperty(e) || En.hasOwnProperty(e)
+                                return this.macros.has(e) || gn.hasOwnProperty(e) || j.math.hasOwnProperty(e) || j.text.hasOwnProperty(e) || Rn.hasOwnProperty(e)
                             }, t.isExpandable = function(e) {
                                 var t = this.macros.get(e);
-                                return null != t ? "string" == typeof t || "function" == typeof t || !t.unexpandable : kn.hasOwnProperty(e)
+                                return null != t ? "string" == typeof t || "function" == typeof t || !t.unexpandable : gn.hasOwnProperty(e)
                             }, e
                         }(),
-                        Pn = {
+                        Ln = {
                             "́": {
                                 text: "\\'",
                                 math: "\\acute"
                             },
                             "̀": {
                                 text: "\\`",
                                 math: "\\grave"
@@ -7850,15 +7866,15 @@
                                 text: "\\r",
                                 math: "\\mathring"
                             },
                             "̋": {
                                 text: "\\H"
                             }
                         },
-                        Dn = {
+                        Pn = {
                             á: "á",
                             à: "à",
                             ä: "ä",
                             ǟ: "ǟ",
                             ã: "ã",
                             ā: "ā",
                             ă: "ă",
@@ -8170,17 +8186,17 @@
                             Ὺ: "Ὺ",
                             Ϋ: "Ϋ",
                             Ῡ: "Ῡ",
                             Ῠ: "Ῠ",
                             Ώ: "Ώ",
                             Ὼ: "Ὼ"
                         },
-                        Hn = function() {
+                        Dn = function() {
                             function e(e, t) {
-                                this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new Ln(e, t, this.mode), this.settings = t, this.leftrightDepth = 0
+                                this.mode = void 0, this.gullet = void 0, this.settings = void 0, this.leftrightDepth = void 0, this.nextToken = void 0, this.mode = "math", this.gullet = new En(e, t, this.mode), this.settings = t, this.leftrightDepth = 0
                             }
                             var t = e.prototype;
                             return t.expect = function(e, t) {
                                 if (void 0 === t && (t = !0), this.fetch().text !== e) throw new o("Expected '" + e + "', got '" + this.fetch().text + "'", this.fetch());
                                 t && this.consume()
                             }, t.consume = function() {
                                 this.nextToken = null
@@ -8194,15 +8210,15 @@
                                 return this.expect("EOF"), this.settings.globalGroup || this.gullet.endGroup(), e
                             }, t.parseExpression = function(t, r) {
                                 for (var n = [];;) {
                                     "math" === this.mode && this.consumeSpaces();
                                     var a = this.fetch();
                                     if (-1 !== e.endOfExpression.indexOf(a.text)) break;
                                     if (r && a.text === r) break;
-                                    if (t && kn[a.text] && kn[a.text].infix) break;
+                                    if (t && gn[a.text] && gn[a.text].infix) break;
                                     var i = this.parseAtom(r);
                                     if (!i) break;
                                     "internal" !== i.type && n.push(i)
                                 }
                                 return "text" === this.mode && this.formLigatures(n), this.handleInfixNodes(n)
                             }, t.handleInfixNodes = function(e) {
                                 for (var t, r = -1, n = 0; n < e.length; n++)
@@ -8293,15 +8309,15 @@
                                     base: n,
                                     sup: t,
                                     sub: r
                                 } : n
                             }, t.parseFunction = function(e, t, r) {
                                 var n = this.fetch(),
                                     a = n.text,
-                                    i = kn[a];
+                                    i = gn[a];
                                 if (!i) return null;
                                 if (this.consume(), null != r && i.greediness <= r) throw new o("Got function '" + a + "' with no arguments" + (t ? " as " + t : ""), n);
                                 if ("text" === this.mode && !i.allowedInText) throw new o("Can't use function '" + a + "' in text mode", n);
                                 if ("math" === this.mode && !1 === i.allowedInMath) throw new o("Can't use function '" + a + "' in math mode", n);
                                 var s = this.parseArguments(a, i),
                                     l = s.args,
                                     h = s.optArgs;
@@ -8309,15 +8325,15 @@
                             }, t.callFunction = function(e, t, r, n, a) {
                                 var i = {
                                         funcName: e,
                                         parser: this,
                                         token: n,
                                         breakOnTokenText: a
                                     },
-                                    s = kn[e];
+                                    s = gn[e];
                                 if (s && s.handler) return s.handler(i, t, r);
                                 throw new o("No function handler for " + e)
                             }, t.parseArguments = function(e, t) {
                                 var r = t.numArgs + t.numOptionalArgs;
                                 if (0 === r) return {
                                     args: [],
                                     optArgs: []
@@ -8425,15 +8441,15 @@
                                 e || 0 !== t.text.length || (t.text = "0pt", r = !0);
                                 var n = /([-+]?) *(\d+(?:\.\d*)?|\.\d+) *([a-z]{2})/.exec(t.text);
                                 if (!n) throw new o("Invalid size: '" + t.text + "'", t);
                                 var a = {
                                     number: +(n[1] + n[2]),
                                     unit: n[3]
                                 };
-                                if (!Ye(a)) throw new o("Invalid unit: '" + a.unit + "'", t);
+                                if (!De(a)) throw new o("Invalid unit: '" + a.unit + "'", t);
                                 return {
                                     type: "size",
                                     mode: this.mode,
                                     value: a,
                                     isBlank: r
                                 }
                             }, t.parseUrlGroup = function(e, t) {
@@ -8461,15 +8477,15 @@
                                         type: "ordgroup",
                                         mode: this.mode,
                                         loc: n.range(c, f),
                                         body: d,
                                         semisimple: "\\begingroup" === u || void 0
                                     }
                                 } else if (r) m = null;
-                                else if (null == (m = this.parseFunction(i, t, a) || this.parseSymbol()) && "\\" === u[0] && !En.hasOwnProperty(u)) {
+                                else if (null == (m = this.parseFunction(i, t, a) || this.parseSymbol()) && "\\" === u[0] && !Rn.hasOwnProperty(u)) {
                                     if (this.settings.throwOnError) throw new o("Undefined control sequence: " + u, c);
                                     m = this.formatUnsupportedCmd(u), this.consume()
                                 }
                                 return s && this.switchMode(h), m
                             }, t.formLigatures = function(e) {
                                 for (var t = e.length - 1, r = 0; r < t; ++r) {
                                     var a = e[r],
@@ -8502,21 +8518,21 @@
                                     return {
                                         type: "verb",
                                         mode: "text",
                                         body: r = r.slice(1, -1),
                                         star: a
                                     }
                                 }
-                                Dn.hasOwnProperty(t[0]) && !ee[this.mode][t[0]] && (this.settings.strict && "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + t[0] + '" used in math mode', e), t = Dn[t[0]] + t.substr(1));
-                                var i, s = Mn.exec(t);
-                                if (s && ("i" === (t = t.substring(0, s.index)) ? t = "ı" : "j" === t && (t = "ȷ")), ee[this.mode][t]) {
-                                    this.settings.strict && "math" === this.mode && Ie.indexOf(t) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + t[0] + '" used in math mode', e);
-                                    var l, h = ee[this.mode][t].group,
+                                Pn.hasOwnProperty(t[0]) && !j[this.mode][t[0]] && (this.settings.strict && "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Accented Unicode text character "' + t[0] + '" used in math mode', e), t = Pn[t[0]] + t.substr(1));
+                                var i, s = kn.exec(t);
+                                if (s && ("i" === (t = t.substring(0, s.index)) ? t = "ı" : "j" === t && (t = "ȷ")), j[this.mode][t]) {
+                                    this.settings.strict && "math" === this.mode && Ae.indexOf(t) >= 0 && this.settings.reportNonstrict("unicodeTextInMathMode", 'Latin-1/Unicode text character "' + t[0] + '" used in math mode', e);
+                                    var l, h = j[this.mode][t].group,
                                         m = n.range(e);
-                                    if (K.hasOwnProperty(h)) {
+                                    if (_.hasOwnProperty(h)) {
                                         var c = h;
                                         l = {
                                             type: "atom",
                                             mode: this.mode,
                                             family: c,
                                             loc: m,
                                             text: t
@@ -8526,131 +8542,131 @@
                                         mode: this.mode,
                                         loc: m,
                                         text: t
                                     };
                                     i = l
                                 } else {
                                     if (!(t.charCodeAt(0) >= 128)) return null;
-                                    this.settings.strict && (q(t.charCodeAt(0)) ? "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Unicode text character "' + t[0] + '" used in math mode', e) : this.settings.reportNonstrict("unknownSymbol", 'Unrecognized Unicode character "' + t[0] + '" (' + t.charCodeAt(0) + ")", e)), i = {
+                                    this.settings.strict && (M(t.charCodeAt(0)) ? "math" === this.mode && this.settings.reportNonstrict("unicodeTextInMathMode", 'Unicode text character "' + t[0] + '" used in math mode', e) : this.settings.reportNonstrict("unknownSymbol", 'Unrecognized Unicode character "' + t[0] + '" (' + t.charCodeAt(0) + ")", e)), i = {
                                         type: "textord",
                                         mode: "text",
                                         loc: n.range(e),
                                         text: t
                                     }
                                 }
                                 if (this.consume(), s)
                                     for (var u = 0; u < s[0].length; u++) {
                                         var p = s[0][u];
-                                        if (!Pn[p]) throw new o("Unknown accent ' " + p + "'", e);
-                                        var d = Pn[p][this.mode];
+                                        if (!Ln[p]) throw new o("Unknown accent ' " + p + "'", e);
+                                        var d = Ln[p][this.mode];
                                         if (!d) throw new o("Accent " + p + " unsupported in " + this.mode + " mode", e);
                                         i = {
                                             type: "accent",
                                             mode: this.mode,
                                             loc: n.range(e),
                                             label: d,
                                             isStretchy: !1,
                                             isShifty: !0,
                                             base: i
                                         }
                                     }
                                 return i
                             }, e
                         }();
-                    Hn.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"], Hn.endOfGroup = {
+                    Dn.endOfExpression = ["}", "\\endgroup", "\\end", "\\right", "&"], Dn.endOfGroup = {
                         "[": "]",
                         "{": "}",
                         "\\begingroup": "\\endgroup"
-                    }, Hn.SUPSUB_GREEDINESS = 1;
-                    var Fn = function(e, t) {
+                    }, Dn.SUPSUB_GREEDINESS = 1;
+                    var Hn = function(e, t) {
                             if (!("string" == typeof e || e instanceof String)) throw new TypeError("KaTeX can only parse string typed expression");
-                            var r = new Hn(e, t);
+                            var r = new Dn(e, t);
                             delete r.gullet.macros.current["\\df@tag"];
                             var n = r.parse();
                             if (r.gullet.macros.get("\\df@tag")) {
                                 if (!t.displayMode) throw new o("\\tag works only in display equations");
                                 r.gullet.feed("\\df@tag"), n = [{
                                     type: "tag",
                                     mode: "text",
                                     body: n,
                                     tag: r.parse()
                                 }]
                             }
                             return n
                         },
-                        Vn = function(e, t, r) {
+                        Fn = function(e, t, r) {
                             t.textContent = "";
-                            var n = Gn(e, r).toNode();
+                            var n = Un(e, r).toNode();
                             t.appendChild(n)
                         };
-                    "undefined" != typeof document && "CSS1Compat" !== document.compatMode && ("undefined" != typeof console && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Vn = function() {
+                    "undefined" != typeof document && "CSS1Compat" !== document.compatMode && ("undefined" != typeof console && console.warn("Warning: KaTeX doesn't work in quirks mode. Make sure your website has a suitable doctype."), Fn = function() {
                         throw new o("KaTeX doesn't work in quirks mode.")
                     });
-                    var Un = function(e, t, r) {
+                    var Vn = function(e, t, r) {
                             if (r.throwOnError || !(e instanceof o)) throw e;
-                            var n = rt.makeSpan(["katex-error"], [new V(t)]);
+                            var n = Ze.makeSpan(["katex-error"], [new E(t)]);
                             return n.setAttribute("title", e.toString()), n.setAttribute("style", "color:" + r.errorColor), n
                         },
-                        Gn = function(e, t) {
-                            var r = new b(t);
+                        Un = function(e, t) {
+                            var r = new u(t);
                             try {
                                 return function(e, t, r) {
-                                    var n, a = Ht(r);
-                                    if ("mathml" === r.output) return Dt(e, t, a, r.displayMode, !0);
+                                    var n, a = Ot(r);
+                                    if ("mathml" === r.output) return It(e, t, a, r.displayMode, !0);
                                     if ("html" === r.output) {
-                                        var i = Tt(e, a);
-                                        n = rt.makeSpan(["katex"], [i])
+                                        var i = wt(e, a);
+                                        n = Ze.makeSpan(["katex"], [i])
                                     } else {
-                                        var o = Dt(e, t, a, r.displayMode, !1),
-                                            s = Tt(e, a);
-                                        n = rt.makeSpan(["katex"], [o, s])
+                                        var o = It(e, t, a, r.displayMode, !1),
+                                            s = wt(e, a);
+                                        n = Ze.makeSpan(["katex"], [o, s])
                                     }
-                                    return Ft(n, r)
-                                }(Fn(e, r), e, r)
+                                    return Rt(n, r)
+                                }(Hn(e, r), e, r)
                             } catch (t) {
-                                return Un(t, e, r)
+                                return Vn(t, e, r)
                             }
                         },
-                        Yn = {
+                        Gn = {
                             version: "0.12.0",
-                            render: Vn,
+                            render: Fn,
                             renderToString: function(e, t) {
-                                return Gn(e, t).toMarkup()
+                                return Un(e, t).toMarkup()
                             },
                             ParseError: o,
                             __parse: function(e, t) {
-                                var r = new b(t);
-                                return Fn(e, r)
+                                var r = new u(t);
+                                return Hn(e, r)
                             },
-                            __renderToDomTree: Gn,
+                            __renderToDomTree: Un,
                             __renderToHTMLTree: function(e, t) {
-                                var r = new b(t);
+                                var r = new u(t);
                                 try {
                                     return function(e, t, r) {
-                                        var n = Tt(e, Ht(r)),
-                                            a = rt.makeSpan(["katex"], [n]);
-                                        return Ft(a, r)
-                                    }(Fn(e, r), 0, r)
+                                        var n = wt(e, Ot(r)),
+                                            a = Ze.makeSpan(["katex"], [n]);
+                                        return Rt(a, r)
+                                    }(Hn(e, r), 0, r)
                                 } catch (t) {
-                                    return Un(t, e, r)
+                                    return Vn(t, e, r)
                                 }
                             },
                             __setFontMetrics: function(e, t) {
-                                W[e] = t
+                                F[e] = t
                             },
-                            __defineSymbol: te,
-                            __defineMacro: Cn,
+                            __defineSymbol: $,
+                            __defineMacro: Bn,
                             __domTree: {
-                                Span: P,
-                                Anchor: D,
-                                SymbolNode: V,
-                                SvgNode: U,
-                                PathNode: G,
-                                LineNode: Y
+                                Span: N,
+                                Anchor: I,
+                                SymbolNode: E,
+                                SvgNode: L,
+                                PathNode: P,
+                                LineNode: D
                             }
                         };
-                    t.default = Yn
+                    t.default = Gn
                 }]).default
             }, e.exports = t()
         }
     }
 ]);
```

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/66034ad79f0f68739b7be69771748a1c61d524d4dbba570905318595151377ad.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/66034ad79f0f68739b7b.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/697b1c9f6e11e42800664b58d06173e96548f87ad8b96a37cb01fa4b897dff9b.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/697b1c9f6e11e4280066.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/7b7be7af132561e043a429328fcde231634bfeace1c9e3024887fc4a6f09b6bf.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/7b7be7af132561e043a4.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/82880d882256c6098e5c4a8bdb8f67fbbccb42bf33a5b68e3662bd9bf1f34448.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/82880d882256c6098e5c.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/9339484861f622622c4d4fecffcb05da810407cc23305e8799bc1100329223b9.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/9339484861f622622c4d.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/a4f24d9b4244d4341ba0214cac621ec5727218df842af6de8e228aae985b5512.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/a4f24d9b4244d4341ba0.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/a70a4daf27a074dbc86ca6b186306b852792929da734394fbc62ad3b788aefe5.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/a70a4daf27a074dbc86c.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/ae44802f0b88aca9a5b0150990c7dbd2c51bcf725da05cfb71f878c476017711.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/ae44802f0b88aca9a5b0.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/af1d60bcfc57febf32ab10cc5467219f76117ef82fa663f92db22194f376b424.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/af1d60bcfc57febf32ab.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/b40a2796e46b2f558dcb5158bc76ffd7d5a7cbe35c0662a7599c9e1a88ae4e3c.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/b40a2796e46b2f558dcb.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/c3d1c2c8c0455af0db352e704e4fd4c5ae692cb3b895b6be752f5a89bf3b93f5.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/c3d1c2c8c0455af0db35.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/cb6b7776d09864b2dc99c1ae5ee3659a7115db75b6ed660def2161968a2437c2.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/cb6b7776d09864b2dc99.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/cc796f5fea153a7134e5050fad1bcccadee89d52ace60d498f6fc1f1e069032e.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/cc796f5fea153a7134e5.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/dc8093175e397ea58bed6a7bcc810e05e2125742763f1599babaa926461a32cb.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/dc8093175e397ea58bed.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/deba64bdc3911c01e7bee8c1c9c736d3f5859eaea0d91d5a793a140b21d6b1c6.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/deba64bdc3911c01e7be.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/df5e2dff7ff874a1c50566b93ea32bdf9b219fb1646240ad61ad332c950cfa9d.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/df5e2dff7ff874a1c505.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/e5d73a831c38e3782f1698d94716025e26a59d34272bcf9ac7ab188d2cc9af16.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/e5d73a831c38e3782f16.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/e818e3cd8065e949ca547607045e1cca24912d02f1b44d3efcac67ba6320f619.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/e818e3cd8065e949ca54.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/eab76eab40c7dd342bc38c05d008b96a3a603f6c0bf635701ed1c6b2f0c12fcd.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/eab76eab40c7dd342bc3.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/eebf6eacab4b4238f927271da3bc942970ba7dcdeb6226a0b893dba3f73801ef.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/eebf6eacab4b4238f927.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f1527a373f9e2f3b9b9a44d5a9f4fcc225fe15b9c64735b434de8a5d93fcdf12.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f1527a373f9e2f3b9b9a.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f5b0e1ff158f892d45bbd24799d83b3f046ea492b248674a7d2e26787ff9f5bd.woff` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f5b0e1ff158f892d45bb.woff`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f6f61cab7740ef34b23a8e941760bf54a5c3e8975d70d5cea3c244bbf699fad9.woff2` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f6f61cab7740ef34b23a.woff2`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/f7184e0f0eb9ebd69d81acbd01bbd2519b82f4a4701530d40e47154680d07a02.ttf` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/f7184e0f0eb9ebd69d81.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/remoteEntry.ed329d57579564c8b6bc.js` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/remoteEntry.704fe5b2eb7ee9890e7f.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, u, l, s, d, f, c, p, h, v, b, g, m = {
-            8097: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, s, f, d, c, p, h, v, b, g, m = {
+            9956: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(533), t.e(704)]).then((() => () => t(6704))),
-                        "./extension": () => Promise.all([t.e(533), t.e(704)]).then((() => () => t(6704))),
-                        "./style": () => Promise.all([t.e(533), t.e(643)]).then((() => () => t(6643)))
+                        "./index": () => t.e(537).then((() => () => t(9537))),
+                        "./extension": () => t.e(537).then((() => () => t(9537))),
+                        "./style": () => Promise.all([t.e(689), t.e(643)]).then((() => () => t(6643)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         y = {};
 
     function x(e) {
         var r = y[e];
@@ -43,83 +43,83 @@
         }), r
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        533: "d6b9fd7a31727b57ec5a",
-        643: "bb10b0cf3cac77c8d13d",
-        654: "37cda6b64b789e43ffac",
-        704: "654ced8aac282e7771a2"
+        537: "320d67943944ccaf87fc",
+        643: "a63dec0bcc09cf695f3a",
+        654: "e293e14ee956f393cfa0",
+        689: "a2a55bd7baeb48f90f2c"
     } [e] + ".js?v=" + {
-        533: "d6b9fd7a31727b57ec5a",
-        643: "bb10b0cf3cac77c8d13d",
-        654: "37cda6b64b789e43ffac",
-        704: "654ced8aac282e7771a2"
+        537: "320d67943944ccaf87fc",
+        643: "a63dec0bcc09cf695f3a",
+        654: "e293e14ee956f393cfa0",
+        689: "a2a55bd7baeb48f90f2c"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/katex-extension:", x.l = (t, n, a, o) => {
+    }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@jupyterlab/katex-extension:", x.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
-            if (void 0 !== a)
+            if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var d = l[s];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         x.S = {};
         var e = {},
             r = {};
         x.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 x.o(x.S, t) || (x.S[t] = {});
-                var o = x.S[t],
+                var a = x.S[t],
                     i = "@jupyterlab/katex-extension",
                     u = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            u = a[r];
-                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (a[r] = {
+                        var o = a[e] = a[e] || {},
+                            u = o[r];
+                        (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("@jupyterlab/katex-extension", "3.3.0", (() => Promise.all([x.e(533), x.e(704)]).then((() => () => x(6704))))), u("katex", "0.12.0", (() => x.e(654).then((() => () => x(6654)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@jupyterlab/katex-extension", "3.4.0", (() => x.e(537).then((() => () => x(9537))))), u("katex", "0.12.0", (() => x.e(654).then((() => () => x(6654)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -133,152 +133,153 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
             var i = r[n],
                 u = (typeof i)[0];
-            if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(u = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
         var i = [];
-        for (o = 1; o < e.length; o++) {
-            var u = e[o];
-            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : a(u))
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
+                o = n < 0;
+            o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, d, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(s = r[i]))[0])) return !l || ("u" == f ? u > n && !a : "" == f != a);
-                if ("u" == d) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == d)
+                    if (d == f)
                         if (u <= n) {
                             if (s != e[u]) return !1
                         } else {
-                            if (a ? s > e[u] : s < e[u]) return !1;
+                            if (o ? s > e[u] : s < e[u]) return !1;
                             s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || u <= n) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < f != a) return !1;
+                    if (u <= n || f < d != o) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = u(e, t);
-        return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), f(e[t][a])
-    }, d = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
-        var o = x.I(r);
-        return o && o.then ? o.then(e.bind(e, r, x.S[r], t, n, a)) : e(r, x.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
-        var o = r && x.o(r, t) && d(r, t, n);
-        return o ? f(o) : a()
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+        var o = u(e, t);
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), d(e[t][o])
+    }, f = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, o) {
+        var a = x.I(r);
+        return a && a.then ? a.then(e.bind(e, r, x.S[r], t, n, o)) : e(r, x.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), h = c(((e, r, t, n, o) => {
+        var a = r && x.o(r, t) && f(r, t, n);
+        return a ? d(a) : o()
     })), v = {}, b = {
-        2736: () => p("default", "@jupyterlab/rendermime", [1, 3, 2, 8]),
-        4674: () => p("default", "@jupyterlab/settingregistry", [1, 3, 2, 8]),
+        1486: () => p("default", "@jupyterlab/rendermime", [1, 4, 0, 0]),
+        6629: () => p("default", "@jupyterlab/settingregistry", [1, 4, 0, 0]),
         8509: () => h("default", "katex", [2, 0, 12, 0], (() => x.e(654).then((() => () => x(6654)))))
     }, g = {
-        704: [2736, 4674, 8509]
+        537: [1486, 6629, 8509]
     }, x.f.consumes = (e, r) => {
         x.o(g, e) && g[e].forEach((e => {
             if (x.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
                     }
                 },
                 n = r => {
                     delete v[e], x.m[e] = t => {
                         throw delete x.c[e], r
                     }
                 };
             try {
-                var a = b[e]();
-                a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                var o = b[e]();
+                o.then ? r.push(v[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
+        x.b = document.baseURI || self.location.href;
         var e = {
             582: 0
         };
         x.f.j = (r, t) => {
             var n = x.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var o = x.p + x.u(r),
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = x.p + x.u(r),
                         i = new Error;
-                    x.l(o, (t => {
+                    x.l(a, (t => {
                         if (x.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                o = t && t.target && t.target.src;
-                            i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [o, i, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (o.some((r => 0 !== e[r]))) {
+                if (a.some((r => 0 !== e[r]))) {
                     for (n in i) x.o(i, n) && (x.m[n] = i[n]);
                     u && u(x)
                 }
-                for (r && r(t); l < o.length; l++) a = o[l], x.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyterlab_katex_extension = self.webpackChunk_jupyterlab_katex_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })();
-    var w = x(8097);
+    })(), x.nc = void 0;
+    var w = x(9956);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyterlab/katex-extension"] = w
 })();
```

### Comparing `jupyterlab-katex-3.3.0/jupyterlab-katex/labextension/static/third-party-licenses.json` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/static/third-party-licenses.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333333%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.7.3'}, 2: {'versionInfo': '3.3.2'}}"}*

```diff
@@ -1,22 +1,22 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.7.3"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2013-2019 Khan Academy and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "katex",
             "versionInfo": "0.12.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.2"
         }
     ]
 }
```

### Comparing `jupyterlab-katex-3.3.0/package.json` & `jupyterlab_katex-3.4.0/jupyterlab_katex/labextension/schemas/@jupyterlab/katex-extension/package.json.orig`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9152649176954734%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.0.0 || ^4.0.0', '@jupyterlab/rendermime': "*

 * *                   "'^3.0.0 || ^4.0.0', '@jupyterlab/rendermime-interfaces': '^3.0.0 || ^3.8.0', "*

 * *                   "'@jupyterlab/settingregistry': '^3.0.0 || ^4.0.0'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4.0.0', 'rimraf': '^4.4.1', 'typescript': "*

 * *                      "'~5.0.2', '@types/json-schema': '^7.0.11', "*

 * *                      "'@typescript-eslint/eslint-plugin': '^5.55.0', '@typescript- […]*

```diff
@@ -3,45 +3,62 @@
         "email": "jupyter@googlegroups.com",
         "name": "Project Jupyter"
     },
     "bugs": {
         "url": "https://github.com/jupyterlab/jupyter-renderers/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.2.8",
-        "@jupyterlab/rendermime": "^3.2.8",
-        "@jupyterlab/rendermime-interfaces": "^3.2.8",
-        "@jupyterlab/settingregistry": "^3.2.8",
+        "@jupyterlab/application": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime": "^3.0.0 || ^4.0.0",
+        "@jupyterlab/rendermime-interfaces": "^3.0.0 || ^3.8.0",
+        "@jupyterlab/settingregistry": "^3.0.0 || ^4.0.0",
         "katex": "^0.12.0"
     },
     "description": "KaTeX math renderer for JupyterLab",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.2.8",
+        "@jupyterlab/builder": "^4.0.0",
+        "@types/json-schema": "^7.0.11",
         "@types/katex": "^0.11.0",
+        "@typescript-eslint/eslint-plugin": "^5.55.0",
+        "@typescript-eslint/parser": "^5.55.0",
+        "css-loader": "^6.7.1",
+        "eslint": "^8.36.0",
+        "eslint-config-prettier": "^8.7.0",
+        "eslint-plugin-prettier": "^4.2.1",
         "npm-run-all": "^4.1.5",
-        "rimraf": "^3.0.2",
-        "typescript": "~4.1.3"
+        "prettier": "^2.8.7",
+        "rimraf": "^4.4.1",
+        "source-map-loader": "^1.0.2",
+        "style-loader": "^3.3.1",
+        "stylelint": "^14.9.1",
+        "stylelint-config-prettier": "^9.0.4",
+        "stylelint-config-recommended": "^8.0.0",
+        "stylelint-config-standard": "^26.0.0",
+        "stylelint-prettier": "^2.0.0",
+        "typescript": "~5.0.2",
+        "yjs": "^13.5.40"
     },
     "directories": {
         "lib": "lib/"
     },
     "files": [
         "lib/*.d.ts",
         "lib/*.js",
         "schema/*.json",
         "style/*.*",
         "style/index.js"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-renderers",
     "jupyterlab": {
         "disabledExtensions": [
+            "@jupyterlab/mathjax-extension:plugin",
             "@jupyterlab/mathjax2-extension:plugin"
         ],
         "extension": true,
-        "outputDir": "jupyterlab-katex/labextension",
+        "outputDir": "jupyterlab_katex/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension",
         "katex"
@@ -50,30 +67,36 @@
     "main": "lib/index.js",
     "name": "@jupyterlab/katex-extension",
     "repository": {
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-renderers.git"
     },
     "scripts": {
-        "build": "jlpm run build:lib && jlpm run build:labextension:dev",
+        "build": "jlpm build:lib && jlpm build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
-        "build:lib": "tsc",
-        "build:prod": "jlpm run build:lib && jlpm run build:labextension",
-        "clean": "jlpm run clean:lib",
-        "clean:all": "jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:dist",
-        "clean:dist": "rimraf dist",
-        "clean:labextension": "rimraf ./jupyterlab-katex/labextension",
+        "build:lib": "tsc --sourceMap",
+        "build:lib:prod": "tsc",
+        "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
+        "clean": "jlpm clean:lib",
+        "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
+        "clean:labextension": "rimraf jupyterlab_katex/labextension jupyterlab_katex/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
-        "eslint": "eslint . --ext .ts,.tsx --fix",
-        "eslint:check": "eslint . --ext .ts,.tsx",
-        "install:extension": "jupyter labextension develop --overwrite .",
-        "prepack": "npm run clean && npm run build",
-        "prepare": "jlpm run clean && jlpm run build:prod",
+        "clean:lintcache": "rimraf .eslintcache .stylelintcache",
+        "eslint": "jlpm eslint:check --fix",
+        "eslint:check": "eslint . --cache --ext .ts,.tsx",
+        "install:extension": "jlpm build",
+        "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
+        "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
+        "prettier": "jlpm prettier:base --write --list-different",
+        "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
+        "prettier:check": "jlpm prettier:base --check",
+        "stylelint": "jlpm stylelint:check --fix",
+        "stylelint:check": "stylelint --cache \"style/**/*.css\"",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
-        "watch:src": "tsc -w"
+        "watch:src": "tsc -w --sourceMap"
     },
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "3.3.0"
+    "version": "3.4.0"
 }
```

### Comparing `jupyterlab-katex-3.3.0/src/autorender.ts` & `jupyterlab_katex-3.4.0/src/autorender.ts`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
       nextIndex = text.indexOf(leftDelim);
       if (nextIndex !== -1) {
         currIndex = nextIndex;
         finalData.push({
           type: 'text',
           data: text.slice(0, currIndex),
-          display,
+          display
         });
         lookingForLeft = false;
       }
 
       // eslint-disable-next-line no-constant-condition
       while (true) {
         if (lookingForLeft) {
@@ -69,15 +69,15 @@
           if (nextIndex === -1) {
             break;
           }
 
           finalData.push({
             type: 'text',
             data: text.slice(currIndex, nextIndex),
-            display,
+            display
           });
 
           currIndex = nextIndex;
         } else {
           nextIndex = findEndOfMath(
             rightDelim,
             text,
@@ -87,27 +87,27 @@
             break;
           }
 
           finalData.push({
             type: 'math',
             data: text.slice(currIndex + leftDelim.length, nextIndex),
             rawData: text.slice(currIndex, nextIndex + rightDelim.length),
-            display: display,
+            display: display
           });
 
           currIndex = nextIndex + rightDelim.length;
         }
 
         lookingForLeft = !lookingForLeft;
       }
 
       finalData.push({
         type: 'text',
         data: text.slice(currIndex),
-        display,
+        display
       });
     } else {
       finalData.push(startData[i]);
     }
   }
   return finalData;
 }
@@ -141,29 +141,32 @@
       const math = data[i].data;
       // Override any display mode defined in the settings with that
       // defined by the text itself
       optionsCopy.displayMode = data[i].display;
       try {
         katex.render(math, span, optionsCopy);
       } catch (err) {
-        fragment.appendChild(document.createTextNode(data[i].rawData));
+        console.error(
+          `Failed to render mathematical expression with Katex:\n${err}`
+        );
+        fragment.appendChild(document.createTextNode(data[i].rawData ?? ''));
         continue;
       }
       fragment.appendChild(span);
     }
   }
   return fragment;
 }
 
 function renderElem(elem: Node, optionsCopy: IAutoRenderOptions) {
   for (let i = 0; i < elem.childNodes.length; i++) {
     const childNode = elem.childNodes[i];
     if (childNode.nodeType === 3) {
       // Text node
-      const frag = renderMathInText(childNode.textContent, optionsCopy);
+      const frag = renderMathInText(childNode.textContent ?? '', optionsCopy);
       i += frag.childNodes.length - 1;
       elem.replaceChild(frag, childNode);
     } else if (childNode.nodeType === 1) {
       // Element node
       const shouldRender =
         optionsCopy.ignoredTags.indexOf(childNode.nodeName.toLowerCase()) ===
         -1;
@@ -195,20 +198,20 @@
 
 const defaultAutoRenderOptions: IAutoRenderOptions = {
   delimiters: [
     { left: '$$', right: '$$', display: true },
     { left: '\\[', right: '\\]', display: true },
     { left: '\\(', right: '\\)', display: false },
     { left: '$', right: '$', display: false },
-    { left: '\\begin{equation}', right: '\\end{equation}', display: true },
+    { left: '\\begin{equation}', right: '\\end{equation}', display: true }
   ],
 
   ignoredTags: ['script', 'noscript', 'style', 'textarea', 'pre', 'code'],
   errorColor: '#CC0000',
-  throwOnError: false,
+  throwOnError: false
 };
 
 export function renderMathInElement(
   elem: HTMLElement,
   options: Partial<IAutoRenderOptions> = {}
 ): void {
   if (!elem) {
```

### Comparing `jupyterlab-katex-3.3.0/src/index.ts` & `jupyterlab_katex-3.4.0/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 // Copyright (c) Jupyter Development Team.
 // Distributed under the terms of the Modified BSD License.
 
 import {
   JupyterFrontEnd,
-  JupyterFrontEndPlugin,
+  JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { ILatexTypesetter } from '@jupyterlab/rendermime';
 
 import { IRenderMime } from '@jupyterlab/rendermime-interfaces';
 
-import { IMacros, renderMathInElement } from './autorender';
-
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 
-import '../style/index.css';
+import { IMacros, renderMathInElement } from './autorender';
 
 const katexPluginId = '@jupyterlab/katex-extension:plugin';
 
 interface IOptions {
   macros?: IMacros;
 }
 
@@ -53,20 +51,20 @@
     function updateSettings(settings: ISettingRegistry.ISettings): void {
       const macros = settings.get('macros').composite as IMacros;
       options.macros = macros;
     }
 
     settingRegistry
       .load(katexPluginId)
-      .then((settings) => {
+      .then(settings => {
         settings.changed.connect(updateSettings);
         updateSettings(settings);
       })
       .catch((reason: Error) => {
         console.error(reason.message);
       });
     return new KatexTypesetter();
   },
-  autoStart: true,
+  autoStart: true
 };
 
 export default katexPlugin;
```

### Comparing `jupyterlab-katex-3.3.0/style/base.css` & `jupyterlab_katex-3.4.0/style/base.css`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-/*-----------------------------------------------------------------------------
+/* -----------------------------------------------------------------------------
 | Copyright (c) Jupyter Development Team.
 | Distributed under the terms of the Modified BSD License.
-|----------------------------------------------------------------------------*/
+|---------------------------------------------------------------------------- */
 
-@import url('~katex/dist/katex.css');
+@import '~katex/dist/katex.css';
+
+/* stylelint-disable selector-class-pattern */
 
 /**
  * Note: the KaTeX CSS doesn't apply a height property
  * to its SVG objects, so it can be overridden by low-
  * specificity rules elsewhere on the page. This
  * is a workaround for that behavior.
  */
```

### Comparing `jupyterlab-katex-3.3.0/tsconfig.json` & `jupyterlab_katex-3.4.0/tsconfig.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9802631578947368%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, 'target': 'ES2018', 'types': ['jest']}"}*

```diff
@@ -12,15 +12,17 @@
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "strict": true,
-        "strictNullChecks": false,
-        "target": "es2017",
-        "types": []
+        "strictNullChecks": true,
+        "target": "ES2018",
+        "types": [
+            "jest"
+        ]
     },
     "include": [
         "src/*"
     ]
 }
```

