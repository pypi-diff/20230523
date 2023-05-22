# Comparing `tmp/claudia-0.0.8.tar.gz` & `tmp/claudia-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claudia-0.0.8.tar", last modified: Sat May 20 01:37:06 2023, max compression
+gzip compressed data, was "claudia-0.0.9.tar", last modified: Mon May 22 22:47:31 2023, max compression
```

## Comparing `claudia-0.0.8.tar` & `claudia-0.0.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.488944 claudia-0.0.8/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.8/LICENSE
--rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-20 01:37:06.488716 claudia-0.0.8/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     4935 2023-05-20 01:17:00.000000 claudia-0.0.8/README.md
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.467866 claudia-0.0.8/claudia.egg-info/
--rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/PKG-INFO
--rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/SOURCES.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/dependency_links.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/entry_points.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/requires.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-20 01:37:06.000000 claudia-0.0.8/claudia.egg-info/top_level.txt
--rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-20 01:37:06.489017 claudia-0.0.8/setup.cfg
--rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-20 01:23:01.000000 claudia-0.0.8/setup.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.459775 claudia-0.0.8/src/
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.469394 claudia-0.0.8/src/claudia/
--rw-r--r--   0 ksaxena    (502) staff       (20)     3184 2023-05-20 01:12:37.000000 claudia-0.0.8/src/claudia/README.md
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    11978 2023-05-20 01:33:06.000000 claudia-0.0.8/src/claudia/claudia.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.470973 claudia-0.0.8/src/claudia/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/features/nft_burn_mint.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/features/payments.feature
--rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/features/trustline.feature
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.473461 claudia-0.0.8/src/claudia/javascript/
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/cleanup
--rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/cucumber.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.473733 claudia-0.0.8/src/claudia/javascript/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/context.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.474118 claudia-0.0.8/src/claudia/javascript/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/lib/ObjFactory.js
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.476070 claudia-0.0.8/src/claudia/javascript/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/steps/common.js
--rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/steps/constants.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/steps/nft_mint_burn.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/steps/payments.js
--rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/features/steps/trustline.js
--rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/package-lock.json
--rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/package.json
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/javascript/runTest
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.476734 claudia-0.0.8/src/claudia/network_setup/
--rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/Dockerfile
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.477537 claudia-0.0.8/src/claudia/network_setup/configs/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled.cfg
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.478196 claudia-0.0.8/src/claudia/network_setup/configs/rippled_1/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_1/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_1/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.478797 claudia-0.0.8/src/claudia/network_setup/configs/rippled_2/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_2/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_2/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.479334 claudia-0.0.8/src/claudia/network_setup/configs/rippled_3/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_3/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_3/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.480003 claudia-0.0.8/src/claudia/network_setup/configs/rippled_4/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_4/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_4/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.480709 claudia-0.0.8/src/claudia/network_setup/configs/rippled_5/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_5/rippled.cfg
--rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/rippled_5/validators.txt
--rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/configs/validators.txt
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.482157 claudia-0.0.8/src/claudia/network_setup/lib/
--rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/lib/build_rippled.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/lib/rippled_network.yml
--rw-rw-r--   0 ksaxena    (502) staff       (20)     8966 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/lib/setup_helper.sh
--rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/lib/validate_network.py
--rw-rw-r--   0 ksaxena    (502) staff       (20)     3784 2023-05-18 02:32:34.000000 claudia-0.0.8/src/claudia/network_setup/setup.sh
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.483928 claudia-0.0.8/src/claudia/python/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/behave.ini
--rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/cleanup
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.484842 claudia-0.0.8/src/claudia/python/features/
--rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/__init__.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/environment.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.485654 claudia-0.0.8/src/claudia/python/features/exceptions/
--rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/exceptions/InvalidInputException.py
--rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.486395 claudia-0.0.8/src/claudia/python/features/lib/
--rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/lib/Helpers.py
--rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/lib/ObjFactory.py
-drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-20 01:37:06.488216 claudia-0.0.8/src/claudia/python/features/steps/
--rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/steps/common.py
--rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/steps/constants.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/steps/nft_mint_burn.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/steps/payments.py
--rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/features/steps/trustline.py
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/runSetup
--rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-15 18:14:02.000000 claudia-0.0.8/src/claudia/python/runTest
--rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-19 20:42:19.000000 claudia-0.0.8/src/claudia/requirements.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.041493 claudia-0.0.9/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1073 2023-05-11 10:47:00.000000 claudia-0.0.9/LICENSE
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-22 22:47:31.041286 claudia-0.0.9/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     4935 2023-05-20 01:17:00.000000 claudia-0.0.9/README.md
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.016780 claudia-0.0.9/claudia.egg-info/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3533 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/PKG-INFO
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2610 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/SOURCES.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        1 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/dependency_links.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/entry_points.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/requires.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)        8 2023-05-22 22:47:30.000000 claudia-0.0.9/claudia.egg-info/top_level.txt
+-rw-r--r--   0 ksaxena    (502) staff       (20)       38 2023-05-22 22:47:31.041576 claudia-0.0.9/setup.cfg
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1477 2023-05-22 19:16:03.000000 claudia-0.0.9/setup.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.009898 claudia-0.0.9/src/
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.018624 claudia-0.0.9/src/claudia/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     3184 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/README.md
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    13074 2023-05-22 22:45:51.000000 claudia-0.0.9/src/claudia/claudia.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.019898 claudia-0.0.9/src/claudia/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    14321 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/nft_burn_mint.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)     5371 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/payments.feature
+-rw-r--r--   0 ksaxena    (502) staff       (20)    11071 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/features/trustline.feature
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.022337 claudia-0.0.9/src/claudia/javascript/
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      118 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/cleanup
+-rw-r--r--   0 ksaxena    (502) staff       (20)      145 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/cucumber.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.022698 claudia-0.0.9/src/claudia/javascript/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     1226 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/context.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.023935 claudia-0.0.9/src/claudia/javascript/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2106 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/lib/ObjFactory.js
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.026052 claudia-0.0.9/src/claudia/javascript/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    38728 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/common.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)      300 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/constants.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    71153 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/nft_mint_burn.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    19024 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/payments.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)    59478 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/features/steps/trustline.js
+-rw-r--r--   0 ksaxena    (502) staff       (20)   129466 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/package-lock.json
+-rw-r--r--   0 ksaxena    (502) staff       (20)      221 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/package.json
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      869 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     4674 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/javascript/runTest
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.027301 claudia-0.0.9/src/claudia/network_setup/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      251 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/Dockerfile
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.028414 claudia-0.0.9/src/claudia/network_setup/configs/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1520 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled.cfg
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.029182 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2150 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.029997 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.030851 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2191 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.031551 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2190 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.032268 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2226 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/rippled.cfg
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      278 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/validators.txt
+-rw-rw-r--   0 ksaxena    (502) staff       (20)      279 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/configs/validators.txt
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.033877 claudia-0.0.9/src/claudia/network_setup/lib/
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     1619 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/build_rippled.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     2161 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/rippled_network.yml
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     9944 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/setup_helper.sh
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     5094 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/lib/validate_network.py
+-rw-rw-r--   0 ksaxena    (502) staff       (20)     3800 2023-05-22 22:00:05.000000 claudia-0.0.9/src/claudia/network_setup/setup.sh
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.036032 claudia-0.0.9/src/claudia/python/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      107 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/behave.ini
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)      123 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/cleanup
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.037077 claudia-0.0.9/src/claudia/python/features/
+-rw-r--r--   0 ksaxena    (502) staff       (20)        0 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/__init__.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     2977 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/environment.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.037804 claudia-0.0.9/src/claudia/python/features/exceptions/
+-rw-r--r--   0 ksaxena    (502) staff       (20)       49 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/exceptions/InvalidInputException.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)       60 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/exceptions/UnconfiguredEnvironmentException.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.038633 claudia-0.0.9/src/claudia/python/features/lib/
+-rw-r--r--   0 ksaxena    (502) staff       (20)      301 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/lib/Helpers.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)     7674 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/lib/ObjFactory.py
+drwxr-xr-x   0 ksaxena    (502) staff       (20)        0 2023-05-22 22:47:31.040792 claudia-0.0.9/src/claudia/python/features/steps/
+-rw-r--r--   0 ksaxena    (502) staff       (20)    24750 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/common.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)      251 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/constants.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    66340 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/nft_mint_burn.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    21822 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/payments.py
+-rw-r--r--   0 ksaxena    (502) staff       (20)    54620 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/features/steps/trustline.py
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     1381 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/runSetup
+-rwxr-xr-x   0 ksaxena    (502) staff       (20)     5634 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/python/runTest
+-rw-r--r--   0 ksaxena    (502) staff       (20)       88 2023-05-22 18:05:18.000000 claudia-0.0.9/src/claudia/requirements.txt
```

### Comparing `claudia-0.0.8/LICENSE` & `claudia-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/PKG-INFO` & `claudia-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.8/README.md` & `claudia-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/claudia.egg-info/PKG-INFO` & `claudia-0.0.9/claudia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claudia
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run XRPL Automated Tests
 Home-page: https://xrpl.org/
 Download-URL: https://gitlab.ops.ripple.com/xrpledger/xrpl-nocode-automation
 Author: Kausty Saxena
 Author-email: ksaxena@ripple.com
 Keywords: ripple xrpl python javascript
 Description-Content-Type: text/markdown
```

### Comparing `claudia-0.0.8/claudia.egg-info/SOURCES.txt` & `claudia-0.0.9/claudia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/setup.py` & `claudia-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         requirements = content.split('\n')
 
     return requirements
 
 
 setup(
     name='claudia',
-    version='0.0.8',
+    version='0.0.9',
     description='Run XRPL Automated Tests',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     author="Kausty Saxena",
     author_email="ksaxena@ripple.com",
     keywords="ripple xrpl python javascript",
     url='https://xrpl.org/',
```

### Comparing `claudia-0.0.8/src/claudia/README.md` & `claudia-0.0.9/src/claudia/README.md`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/claudia.py` & `claudia-0.0.9/src/claudia/claudia.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,38 +105,52 @@
         - pip
         - docker
     2. Pull down a fresh copy of rippled code base from https://github.com/XRPLF/rippled
     3. Optional: Following depedencies are only required if you intend to run Javascript tests:
         - node
         - npm
     
-        More information can be found in the 'General prerequisite' section here: https://pypi.org/project/claudia
+        More detailed information can be found under the 'General prerequisite' section here: https://pypi.org/project/claudia
     """
     click.echo(message)
 
 @rippled.command()
 @click.option('--repo', required=True, help="The path to a local rippled repo")
 def build(repo):
     """Build rippled from source"""
+    if not os.path.isabs(repo) or not os.path.exists(repo):
+        click.echo(" - ERROR: Rippled repository path '{}' is not correct. Please provide correct absolute path!".format(repo))
+        return
     set_to_project_root_wd()
     command = "sh network_setup/setup.sh --buildRippled --rippledRepo {}".format(repo)
     subprocess.call(command, shell=True)
 
 
 @rippled.command()
+def version():
+    """View rippled version info"""
+    set_to_project_root_wd()
+    command = "sh network_setup/setup.sh --rippledVersion"
+    subprocess.call(command, shell=True)
+
+
+@rippled.command()
 def install():
     """Install rippled packages"""
     click.echo("Currently not supported")
 
 
 @network.command()
 @click.option('--repo', required=True,
-              help="path to rippled repo")
+              help="The path to a local rippled repo")
 def start(repo):
     """Start a new rippled network"""
+    if not os.path.isabs(repo) or not os.path.exists(repo):
+        click.echo(" - ERROR: Rippled repository path '{}' is not correct. Please provide correct absolute path!".format(repo))
+        return
     set_to_project_root_wd()
     command = "sh ./network_setup/setup.sh --networkStart  --rippledRepo {}".format(repo)
     subprocess.call(command, shell=True)
 
 
 @network.command()
 def stop():
@@ -189,14 +203,26 @@
         if (client_type != 'websocket'):
             raise Exception("Client Type {} is not supported with {} library client.".format(client_type, lib))
         print_explorer_message(network)
         javascript(context, network, tag, feature, invalidate_cache)
     else:
         raise Exception("Invalid library type: {}".format(lib))
 
+
+@run.command()
+@click.option('--testname', default='everything', help="The unit test which needs to be selected. If not provided, all tests are selected.")
+def unittests(testname):
+    """Launch Rippled Unit tests"""
+    set_to_project_root_wd()
+    if(testname == ''):
+        command = "sh network_setup/setup.sh --runUnittests"
+    else:
+        command = "sh network_setup/setup.sh --runUnittests {}".format(testname)
+    subprocess.call(command, shell=True)
+
 # @run.command()
 # @click.pass_context
 # @click.argument("text")
 # def customcommand(context, text):
 #     """Run a debug command"""
 #     click.echo("Running command: {}".format(text))
 #     subprocess.call(text, shell=True)
```

### Comparing `claudia-0.0.8/src/claudia/features/nft_burn_mint.feature` & `claudia-0.0.9/src/claudia/features/nft_burn_mint.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/features/payments.feature` & `claudia-0.0.9/src/claudia/features/payments.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/features/trustline.feature` & `claudia-0.0.9/src/claudia/features/trustline.feature`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/context.js` & `claudia-0.0.9/src/claudia/javascript/features/context.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/lib/ObjFactory.js` & `claudia-0.0.9/src/claudia/javascript/features/lib/ObjFactory.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/steps/common.js` & `claudia-0.0.9/src/claudia/javascript/features/steps/common.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/steps/nft_mint_burn.js` & `claudia-0.0.9/src/claudia/javascript/features/steps/nft_mint_burn.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/steps/payments.js` & `claudia-0.0.9/src/claudia/javascript/features/steps/payments.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/features/steps/trustline.js` & `claudia-0.0.9/src/claudia/javascript/features/steps/trustline.js`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/package-lock.json` & `claudia-0.0.9/src/claudia/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/runSetup` & `claudia-0.0.9/src/claudia/javascript/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/javascript/runTest` & `claudia-0.0.9/src/claudia/javascript/runTest`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled_1/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled_1/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled_2/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled_2/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled_3/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled_3/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled_4/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled_4/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/configs/rippled_5/rippled.cfg` & `claudia-0.0.9/src/claudia/network_setup/configs/rippled_5/rippled.cfg`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/lib/build_rippled.sh` & `claudia-0.0.9/src/claudia/network_setup/lib/build_rippled.sh`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/lib/rippled_network.yml` & `claudia-0.0.9/src/claudia/network_setup/lib/rippled_network.yml`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/lib/setup_helper.sh` & `claudia-0.0.9/src/claudia/network_setup/lib/setup_helper.sh`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 RIPPLED_NODE_CONTAINER_NAME=rippled_node
 RIPPLED_BUILD_CONTAINER_NAME=rippled_build
 MAC_CHROME_BROWSER="/Applications/Google Chrome.app"
 LINUX_CHROME_BROWSER="chrome"
 EXPLORER_URL="https://custom.xrpl.org/localhost:6001"
 
 BUILD_DIR_NAME="linux_build"
+CONFIGS_DIR_NAME="configs"
 CONTAINER_HOME="/root"
 RIPPLED_BUILD_CONTAINER_SCRIPT_DIR="${CONTAINER_HOME}/network_setup"
 RIPPLED_BUILD_CONTAINER_LOG_DIR="${CONTAINER_HOME}/logs"
 RIPPLED_BUILD_CONTAINER_BUILD_SCRIPT="${RIPPLED_BUILD_CONTAINER_SCRIPT_DIR}/lib/build_rippled.sh"
 RIPPLED_BUILD_CONTAINER_RIPPLED_HOME="${CONTAINER_HOME}/rippled"
 RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC="${RIPPLED_BUILD_CONTAINER_RIPPLED_HOME}/${BUILD_DIR_NAME}/rippled"
 RIPPLED_NODE_DOCKER_FILE="${SCRIPT_PATH}"
@@ -41,14 +42,22 @@
 rippled_exec_not_found() {
   echo "rippled binary '${rippled_exec}' not found"
   echo " - Is rippled built successfully?"
   echo " - Is the path to rippled repo correct?"
   exit 1
 }
 
+is_rippled_built_successfully() {
+  docker exec ${RIPPLED_BUILD_CONTAINER_NAME} "${RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC}" --version > /dev/null 2>&1
+  if [ "$?" -ne 0 ]; then
+    echo "Error: 'rippled' not built successfully"
+    exit 1
+  fi
+}
+
 install_os_packages() {
   echo "- Install OS packages"
   time_now="$(date +%Y%m%d_%H%M%S)"
   log_file="${LOG_DIR}/${time_now}_prerequisite.log"
 
   apt -y update >>"${log_file}" 2>&1 && \
   DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata >>"${log_file}" 2>&1 && \
@@ -164,61 +173,36 @@
     if [ ! "$(docker ps -aq --filter name=${RIPPLED_BUILD_CONTAINER_NAME})" ]; then
       docker run \
         --name "${RIPPLED_BUILD_CONTAINER_NAME}" -i -d \
         -v "${rippled_repo}":"${RIPPLED_BUILD_CONTAINER_RIPPLED_HOME}" \
         -v "${host_script_dir}":"${RIPPLED_BUILD_CONTAINER_SCRIPT_DIR}" \
         -v "${LOG_BASE_DIR}":"${RIPPLED_BUILD_CONTAINER_LOG_DIR}" \
         "${DOCKER_IMAGE}" > /dev/null 2>&1
+    elif [ "$(docker ps -aq --filter name=${RIPPLED_BUILD_CONTAINER_NAME} --filter status=exited)" ]; then
+      docker start "${RIPPLED_BUILD_CONTAINER_NAME}"
     fi
+
     docker exec ${RIPPLED_BUILD_CONTAINER_NAME} \
       sh "${RIPPLED_BUILD_CONTAINER_BUILD_SCRIPT}" --installMode "${install_mode}" --logDir "${LOG_DIR}"
-    build_status=$?
-
-    exit_on_error $build_status
-  fi
-}
-
-docker_run_unittests() {
-  run_unittests_opt="$1"
-  if [ "${run_unittests_opt}" = "true" ]; then
-    if [ -f "${rippled_exec}" ]; then
-      echo "- Run unittests"
-
-      docker exec ${RIPPLED_BUILD_CONTAINER_NAME} "${RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC}" --unittest
-      exit_on_error $?
-    else
-      rippled_exec_not_found
-    fi
-  fi
-}
-
-docker_rippled_version() {
-  get_rippled_version_opt="$1"
-  if [ "${get_rippled_version_opt}" = "true" ]; then
-    if [ -f "${rippled_exec}" ]; then
-      docker exec ${RIPPLED_BUILD_CONTAINER_NAME} "${RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC}" --version
-      exit_on_error $?
-    else
-      rippled_exec_not_found
-    fi
+    exit_on_error $?
   fi
 }
 
 start_network() {
   start_network_opt="$1"
   host_script_dir="$2"
   if [ "${start_network_opt}" = "true" ]; then
     if [ -f "${rippled_exec}" ]; then
       echo "- Setup network"
 
-      docker rm $(docker ps --filter name=rippled --filter status=exited -q) > /dev/null 2>&1
+      docker rm $(docker ps --filter name=${RIPPLED_NODE_CONTAINER_NAME} --filter status=exited -q) > /dev/null 2>&1
       docker build --quiet -t ${RIPPLED_NODE_CONTAINER_NAME} "${RIPPLED_NODE_DOCKER_FILE}" > /dev/null 2>&1
 
       export RIPPLED_BUILD_DIR="${rippled_build_path}"
-      export RIPPLED_CONFIG_DIR="${host_script_dir}/configs"
+      export RIPPLED_CONFIG_DIR="${host_script_dir}/${CONFIGS_DIR_NAME}"
       docker-compose -f "${DOCKER_NETWORK_CONFIG}" down > /dev/null 2>&1
       docker-compose -f "${DOCKER_NETWORK_CONFIG}" up -d > /dev/null 2>&1
     else
       rippled_exec_not_found
     fi
   fi
 }
@@ -255,7 +239,39 @@
 
     if [ -d "${WEB_BROWSER}" ] || [ -f "${WEB_BROWSER}" ]; then
       /usr/bin/open -a "${WEB_BROWSER}" "${EXPLORER_URL}"
       echo ""
     fi
   fi
 }
+
+docker_run_unittests() {
+  run_unittests_opt="$1"
+  filtered_unittests_to_run="$2"
+  if [ "${run_unittests_opt}" = "true" ]; then
+    echo "- Run unittests"
+
+    if [ ! "$(docker ps -aq --filter name=${RIPPLED_BUILD_CONTAINER_NAME})" ]; then
+      docker run \
+        --name "${RIPPLED_BUILD_CONTAINER_NAME}" -i -d \
+        -v "${rippled_repo}":"${RIPPLED_BUILD_CONTAINER_RIPPLED_HOME}" \
+        -v "${host_script_dir}":"${RIPPLED_BUILD_CONTAINER_SCRIPT_DIR}" \
+        -v "${LOG_BASE_DIR}":"${RIPPLED_BUILD_CONTAINER_LOG_DIR}" \
+        "${DOCKER_IMAGE}" > /dev/null 2>&1
+    elif [ "$(docker ps -aq --filter name=${RIPPLED_BUILD_CONTAINER_NAME} --filter status=exited)" ]; then
+      docker start "${RIPPLED_BUILD_CONTAINER_NAME}"
+    fi
+
+    is_rippled_built_successfully
+    docker exec ${RIPPLED_BUILD_CONTAINER_NAME} "${RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC}" --unittest "${filtered_unittests_to_run}"
+    exit_on_error $?
+  fi
+}
+
+docker_rippled_version() {
+  get_rippled_version_opt="$1"
+  if [ "${get_rippled_version_opt}" = "true" ]; then
+    is_rippled_built_successfully
+    docker exec ${RIPPLED_BUILD_CONTAINER_NAME} "${RIPPLED_BUILD_CONTAINER_RIPPLED_EXEC}" --version
+    exit_on_error $?
+  fi
+}
```

### Comparing `claudia-0.0.8/src/claudia/network_setup/lib/validate_network.py` & `claudia-0.0.9/src/claudia/network_setup/lib/validate_network.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/network_setup/setup.sh` & `claudia-0.0.9/src/claudia/network_setup/setup.sh`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/bin/sh
 
 
-# TODO: install_prerequisites in a dedicated docker image?
 # TODO: Add firefox support in prepare()
 
 SCRIPT_PATH="$(cd -- "$(dirname "$0")" >/dev/null 2>&1 ; pwd -P)"
 install="install"
 build="build"
 build_rippled_opt="false"
 get_rippled_version_opt="false"
@@ -17,14 +16,15 @@
 install_mode="${build}"
 rippled_repo="${HOME}/rippled"
 LOG_BASE_DIR="${HOME}/logs"
 LOG_DIR="${LOG_BASE_DIR}/logs_$(date +%Y%m%d_%H%M%S)"
 SCRIPT_HELPER="${SCRIPT_PATH}/lib/setup_helper.sh"
 WORK_DIR="/tmp/work_dir"
 ALT_HOST_SCRIPT_DIR="/tmp/network_setup"
+filtered_unittests_to_run=""
 
 trap cleanup EXIT
 
 
 usage() {
   echo ""
   echo "Usage: $0 [Optional parameters]"
@@ -37,17 +37,15 @@
   echo "  --networkStop (Stop local rippled network)>"
   echo "  --networkStatus (Get local rippled network status)>"
 
   exit 1
 }
 
 cleanup() {
-  if [ -d "${WORK_DIR}" ]; then
-    /bin/rm -rf "${WORK_DIR}" "${ALT_HOST_SCRIPT_DIR}"
-  fi
+  /bin/rm -rf "${WORK_DIR}" "${ALT_HOST_SCRIPT_DIR}"
 }
 
 prepare_workspace() {
   if [ "${build_rippled_opt}" = "true" ]; then
     if [ ! -d "${rippled_repo}" ]; then
       echo "rippled repo '${rippled_repo}' not found. Check help"
       exit 1
@@ -75,15 +73,14 @@
       exit 1
     fi
   done
 
   host_script_dir="${SCRIPT_PATH}"
   is_script_in_home=$(echo "${PWD}" | grep "^${HOME}")
   if [ -z "${is_script_in_home}" ]; then
-    echo "Copying scripts to ${ALT_HOST_SCRIPT_DIR}"  # TODO: remove this line
     /bin/cp -r "${host_script_dir}" "$(dirname "${ALT_HOST_SCRIPT_DIR}")"
     host_script_dir="${ALT_HOST_SCRIPT_DIR}"
   fi
 
   . "${SCRIPT_HELPER}"
 }
 
@@ -110,14 +107,19 @@
 
   --rippledVersion)
     get_rippled_version_opt="true"
     ;;
 
   --runUnittests)
     run_unittests_opt="true"
+    next_param=$(echo "$2" | grep "^--")
+    if [ -z "${next_param}" ]; then
+      filtered_unittests_to_run="$2"
+      shift
+    fi
     ;;
 
   --networkStart)
     start_network_opt="true"
     validate_network_opt="true"
     launch_explorer_opt="true"
     ;;
@@ -137,11 +139,11 @@
   shift
 done
 
 prepare_workspace
 stop_network "${stop_network_opt}"
 docker_build_rippled "${build_rippled_opt}" "${install_mode}" "${host_script_dir}"
 docker_rippled_version "${get_rippled_version_opt}"
-docker_run_unittests "${run_unittests_opt}"
+docker_run_unittests "${run_unittests_opt}" "${filtered_unittests_to_run}"
 start_network "${start_network_opt}" "${host_script_dir}"
 validate_network "${validate_network_opt}"
 launch_explorer "${launch_explorer_opt}"
```

### Comparing `claudia-0.0.8/src/claudia/python/features/environment.py` & `claudia-0.0.9/src/claudia/python/features/environment.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/features/lib/ObjFactory.py` & `claudia-0.0.9/src/claudia/python/features/lib/ObjFactory.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/features/steps/common.py` & `claudia-0.0.9/src/claudia/python/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/features/steps/nft_mint_burn.py` & `claudia-0.0.9/src/claudia/python/features/steps/nft_mint_burn.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/features/steps/payments.py` & `claudia-0.0.9/src/claudia/python/features/steps/payments.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/features/steps/trustline.py` & `claudia-0.0.9/src/claudia/python/features/steps/trustline.py`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/runSetup` & `claudia-0.0.9/src/claudia/python/runSetup`

 * *Files identical despite different names*

### Comparing `claudia-0.0.8/src/claudia/python/runTest` & `claudia-0.0.9/src/claudia/python/runTest`

 * *Files identical despite different names*

