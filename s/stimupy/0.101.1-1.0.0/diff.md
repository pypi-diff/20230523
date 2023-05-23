# Comparing `tmp/stimupy-0.101.1.tar.gz` & `tmp/stimupy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimupy-0.101.1.tar", last modified: Sat May 20 14:38:57 2023, max compression
+gzip compressed data, was "stimupy-1.0.0.tar", last modified: Tue May 23 16:37:48 2023, max compression
```

## Comparing `stimupy-0.101.1.tar` & `stimupy-1.0.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.449014 stimupy-0.101.1/
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-05-20 14:38:35.000000 stimupy-0.101.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 14:38:35.000000 stimupy-0.101.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24162 2023-05-20 14:38:57.449014 stimupy-0.101.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-20 14:38:35.000000 stimupy-0.101.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-20 14:38:45.000000 stimupy-0.101.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:38:57.449014 stimupy-0.101.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.437014 stimupy-0.101.1/stimupy/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-20 14:38:45.000000 stimupy-0.101.1/stimupy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.437014 stimupy-0.101.1/stimupy/components/
--rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/angulars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/gaussians.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/radials.py
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28406 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/components/waves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/logos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.441014 stimupy-0.101.1/stimupy/noises/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/noises/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/noises/binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/noises/narrowbands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/noises/naturals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/noises/whites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.441014 stimupy-0.101.1/stimupy/papers/
--rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/RHS2007.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65164 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/bindmann2004.py
--rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/domijan2015.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/example.py
--rw-r--r--   0 runner    (1001) docker     (123)    64666 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/modelfest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/modelfest_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    56134 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/modelfest_natural_scene.tif
--rw-r--r--   0 runner    (1001) docker     (123)    56498 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/modelfest_noise.tif
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/murray2020.mat
--rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/murray2020.py
--rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/white1981.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/papers/white1985.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.445014 stimupy-0.101.1/stimupy/stimuli/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/benarys.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/bullseyes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16184 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/checkerboards.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/cornsweets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/cubes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/delboeufs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/dungeons.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/gabors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/gratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/hermanns.py
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/mondrians.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/mueller_lyers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/pinwheels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/plaids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/ponzos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/rings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/sbcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32499 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/todorovics.py
--rw-r--r--   0 runner    (1001) docker     (123)    58832 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/waves.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/wedding_cakes.py
--rw-r--r--   0 runner    (1001) docker     (123)    31912 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/stimuli/whites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.449014 stimupy-0.101.1/stimupy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/color_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/contrast_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-20 14:38:35.000000 stimupy-0.101.1/stimupy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.437014 stimupy-0.101.1/stimupy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24162 2023-05-20 14:38:57.000000 stimupy-0.101.1/stimupy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-20 14:38:57.000000 stimupy-0.101.1/stimupy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:38:57.000000 stimupy-0.101.1/stimupy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-20 14:38:57.000000 stimupy-0.101.1/stimupy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 14:38:57.000000 stimupy-0.101.1/stimupy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:38:57.449014 stimupy-0.101.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_overviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_resolve_resolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_valid_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_validate_resolution_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-20 14:38:35.000000 stimupy-0.101.1/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.293286 stimupy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-05-23 16:37:24.000000 stimupy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 16:37:24.000000 stimupy-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-05-23 16:37:48.293286 stimupy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-23 16:37:24.000000 stimupy-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-23 16:37:36.000000 stimupy-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 16:37:48.293286 stimupy-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.277286 stimupy-1.0.0/stimupy/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 16:37:36.000000 stimupy-1.0.0/stimupy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.281286 stimupy-1.0.0/stimupy/components/
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/angulars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7958 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/gaussians.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10450 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/radials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28406 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/components/waves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/logos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.281286 stimupy-1.0.0/stimupy/noises/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/noises/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/noises/binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/noises/narrowbands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/noises/naturals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/noises/whites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.285286 stimupy-1.0.0/stimupy/papers/
+-rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/RHS2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65164 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/bindmann2004.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43233 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/domijan2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64666 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/modelfest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/modelfest_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    56134 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/modelfest_natural_scene.tif
+-rw-r--r--   0 runner    (1001) docker     (123)    56498 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/modelfest_noise.tif
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/murray2020.mat
+-rw-r--r--   0 runner    (1001) docker     (123)    22926 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/murray2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19273 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/white1981.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/papers/white1985.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.289286 stimupy-1.0.0/stimupy/stimuli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/benarys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/bullseyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16184 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/checkerboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/cornsweets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/cubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/delboeufs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/dungeons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/gabors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/gratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/hermanns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/mondrians.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/mueller_lyers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/pinwheels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/plaids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/ponzos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/rings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/sbcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32499 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/todorovics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58832 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/waves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/wedding_cakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32032 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/stimuli/whites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.289286 stimupy-1.0.0/stimupy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/color_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/contrast_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-23 16:37:24.000000 stimupy-1.0.0/stimupy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.277286 stimupy-1.0.0/stimupy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-05-23 16:37:48.000000 stimupy-1.0.0/stimupy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-23 16:37:48.000000 stimupy-1.0.0/stimupy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:37:48.000000 stimupy-1.0.0/stimupy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 16:37:48.000000 stimupy-1.0.0/stimupy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 16:37:48.000000 stimupy-1.0.0/stimupy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:37:48.289286 stimupy-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_overviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_resolve_resolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_valid_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_validate_resolution_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 16:37:24.000000 stimupy-1.0.0/tests/test_waves.py
```

### Comparing `stimupy-0.101.1/LICENSE` & `stimupy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/PKG-INFO` & `stimupy-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimupy
-Version: 0.101.1
+Version: 1.0.0
 Summary: Stimuli for vision science, as image arrays
 Author: Matko Matic, Guillermo Aguilar, Marianne Maertens
 Author-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 Maintainer-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
@@ -307,15 +307,18 @@
 for creating new and existing visual stimuli
 commonly used in the study of contrast, brightness, lightness,
 and other aspects of visual perception.
 </p>
 
 <p align=center>
 
-[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml) [![](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![JOSS Status](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d/status.svg)](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d)
+[![PyPI version](https://img.shields.io/pypi/v/stimupy)](https://pypi.org/project/stimupy/)
+[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml)
+[![Py versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![Documentation Status](https://readthedocs.org/projects/stimupy/badge/?version=latest)](https://stimupy.readthedocs.io/en/latest/?badge=latest)
 </p>
 
 <p align=center>
 <img src=docs/logo.png width=400>
 </p>
 
@@ -404,18 +407,17 @@
 
 If you want to contribute yourself, see [contributing](https://stimupy.readthedocs.io/en/latest/contributing/contribute.html)
 
 
 ---
 ## Installation
 
-For now, `pip` can install directly from GitHub (the `main` branch)
-GitHub repository
+`pip` can install `stimupy` directly PyPI:
 ```python
-pip install https://github.com/computational-psychology/stimupy/zipball/main
+pip install stimupy
 ```
 
 OR (for developers), install from source:
 1. Clone the repository from GitHub:
 
     ```bash
     git clone git@github.com:computational-psychology/stimupy.git
```

### Comparing `stimupy-0.101.1/README.md` & `stimupy-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 for creating new and existing visual stimuli
 commonly used in the study of contrast, brightness, lightness,
 and other aspects of visual perception.
 </p>
 
 <p align=center>
 
-[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml) [![](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![JOSS Status](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d/status.svg)](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d)
+[![PyPI version](https://img.shields.io/pypi/v/stimupy)](https://pypi.org/project/stimupy/)
+[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml)
+[![Py versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![Documentation Status](https://readthedocs.org/projects/stimupy/badge/?version=latest)](https://stimupy.readthedocs.io/en/latest/?badge=latest)
 </p>
 
 <p align=center>
 <img src=docs/logo.png width=400>
 </p>
 
@@ -102,18 +105,17 @@
 
 If you want to contribute yourself, see [contributing](https://stimupy.readthedocs.io/en/latest/contributing/contribute.html)
 
 
 ---
 ## Installation
 
-For now, `pip` can install directly from GitHub (the `main` branch)
-GitHub repository
+`pip` can install `stimupy` directly PyPI:
 ```python
-pip install https://github.com/computational-psychology/stimupy/zipball/main
+pip install stimupy
 ```
 
 OR (for developers), install from source:
 1. Clone the repository from GitHub:
 
     ```bash
     git clone git@github.com:computational-psychology/stimupy.git
```

### Comparing `stimupy-0.101.1/pyproject.toml` & `stimupy-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   {name = "Guillermo Aguilar"},
   {name = "Marianne Maertens"},
 ]
 maintainers = [
   {name = "Lynn Schmittwilken", email = "l.schmittwilken@tu-berlin.de"},
   {name = "Joris Vincent", email = "j.vincent@tu-berlin.de"},
 ]
-version = "0.101.1"
+version = "1.0.0"
 
 requires-python = ">=3.6"
 dependencies = [
   "numpy",
   "scipy",
   "matplotlib",
   "pandas",
@@ -76,15 +76,15 @@
 
 [tool.semantic_release]
 version_source = "commit"               # source for version
 version_variable = [                    # version location(s)
   "pyproject.toml:version",             # in this pyproject.toml
   "stimupy/__init__.py:__version__"     # in the init.py, so that stimupy.__version__ works
 ]
-major_on_zero = false                   # don't auto-bump to v1.0.0 yet
+major_on_zero = true                    # don't auto-bump to v1.0.0 yet
 patch_without_tag = false               # if nothing triggers a patch, bump?
 commit_version_number = true            # commit changes to version number?
 commit_subject = "v{version}"
 
 branch = "main"                         # build dists (only) from "main" branch
 build_command = "pipx run build"        # use PyPAs build to generate distribution packages (sdist, wheel)
 upload_to_release = true                # upload sdist, wheel to release-tag
```

### Comparing `stimupy-0.101.1/stimupy/components/__init__.py` & `stimupy-1.0.0/stimupy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/angulars.py` & `stimupy-1.0.0/stimupy/components/angulars.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/edges.py` & `stimupy-1.0.0/stimupy/components/edges.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/frames.py` & `stimupy-1.0.0/stimupy/components/frames.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/gaussians.py` & `stimupy-1.0.0/stimupy/components/gaussians.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/lines.py` & `stimupy-1.0.0/stimupy/components/lines.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/radials.py` & `stimupy-1.0.0/stimupy/components/radials.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/shapes.py` & `stimupy-1.0.0/stimupy/components/shapes.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/components/waves.py` & `stimupy-1.0.0/stimupy/components/waves.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/logos.py` & `stimupy-1.0.0/stimupy/logos.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/noises/__init__.py` & `stimupy-1.0.0/stimupy/noises/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/noises/binaries.py` & `stimupy-1.0.0/stimupy/noises/binaries.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/noises/narrowbands.py` & `stimupy-1.0.0/stimupy/noises/narrowbands.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/noises/naturals.py` & `stimupy-1.0.0/stimupy/noises/naturals.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/noises/whites.py` & `stimupy-1.0.0/stimupy/noises/whites.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/RHS2007.py` & `stimupy-1.0.0/stimupy/papers/RHS2007.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/bindmann2004.py` & `stimupy-1.0.0/stimupy/papers/bindmann2004.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/domijan2015.py` & `stimupy-1.0.0/stimupy/papers/domijan2015.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/example.py` & `stimupy-1.0.0/stimupy/papers/example.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/modelfest.py` & `stimupy-1.0.0/stimupy/papers/modelfest.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/modelfest_data.csv` & `stimupy-1.0.0/stimupy/papers/modelfest_data.csv`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/modelfest_natural_scene.tif` & `stimupy-1.0.0/stimupy/papers/modelfest_natural_scene.tif`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/modelfest_noise.tif` & `stimupy-1.0.0/stimupy/papers/modelfest_noise.tif`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/murray2020.mat` & `stimupy-1.0.0/stimupy/papers/murray2020.mat`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/murray2020.py` & `stimupy-1.0.0/stimupy/papers/murray2020.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/white1981.py` & `stimupy-1.0.0/stimupy/papers/white1981.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/papers/white1985.py` & `stimupy-1.0.0/stimupy/papers/white1985.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/__init__.py` & `stimupy-1.0.0/stimupy/stimuli/__init__.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/benarys.py` & `stimupy-1.0.0/stimupy/stimuli/benarys.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/bullseyes.py` & `stimupy-1.0.0/stimupy/stimuli/bullseyes.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/checkerboards.py` & `stimupy-1.0.0/stimupy/stimuli/checkerboards.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/cornsweets.py` & `stimupy-1.0.0/stimupy/stimuli/cornsweets.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/cubes.py` & `stimupy-1.0.0/stimupy/stimuli/cubes.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/delboeufs.py` & `stimupy-1.0.0/stimupy/stimuli/delboeufs.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/dungeons.py` & `stimupy-1.0.0/stimupy/stimuli/dungeons.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/gabors.py` & `stimupy-1.0.0/stimupy/stimuli/gabors.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/gratings.py` & `stimupy-1.0.0/stimupy/stimuli/gratings.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/hermanns.py` & `stimupy-1.0.0/stimupy/stimuli/hermanns.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/mondrians.py` & `stimupy-1.0.0/stimupy/stimuli/mondrians.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/mueller_lyers.py` & `stimupy-1.0.0/stimupy/stimuli/mueller_lyers.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/pinwheels.py` & `stimupy-1.0.0/stimupy/stimuli/pinwheels.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/plaids.py` & `stimupy-1.0.0/stimupy/stimuli/plaids.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/ponzos.py` & `stimupy-1.0.0/stimupy/stimuli/ponzos.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/rings.py` & `stimupy-1.0.0/stimupy/stimuli/rings.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/sbcs.py` & `stimupy-1.0.0/stimupy/stimuli/sbcs.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/todorovics.py` & `stimupy-1.0.0/stimupy/stimuli/todorovics.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/waves.py` & `stimupy-1.0.0/stimupy/stimuli/waves.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/wedding_cakes.py` & `stimupy-1.0.0/stimupy/stimuli/wedding_cakes.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/stimuli/whites.py` & `stimupy-1.0.0/stimupy/stimuli/whites.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,14 @@
     References
     ----------
     White, M. (1979).
         A new effect of pattern on perceived lightness.
         Perception, 8(4), 413-416.
         https://doi.org/10.1068/p080413
     """
-    if target_heights is None:
-        raise ValueError("generalized() missing argument 'target_heights' which is not 'None'")
 
     # Spatial square-wave grating
     stim = squarewave(
         visual_size=visual_size,
         ppd=ppd,
         shape=shape,
         frequency=frequency,
@@ -121,14 +119,19 @@
     if isinstance(intensity_target, (int, float)):
         intensity_target = (intensity_target,)
     if isinstance(target_heights, (int, float)):
         target_heights = (target_heights,)
     if isinstance(target_center_offsets, (int, float)):
         target_center_offsets = (target_center_offsets,)
 
+    if len(target_indices) != 0 and target_heights is None:
+        raise ValueError("generalized() missing argument 'target_heights' which is not 'None'")
+    if len(target_indices) == 0 and target_heights is None:
+        target_heights = (0,)
+
     intensity_target = tuple(
         itertools.islice(itertools.cycle(intensity_target), len(target_indices))
     )
     target_heights = tuple(itertools.islice(itertools.cycle(target_heights), len(target_indices)))
     target_center_offsets = tuple(
         itertools.islice(itertools.cycle(target_center_offsets), len(target_indices))
     )
```

### Comparing `stimupy-0.101.1/stimupy/utils/color_conversions.py` & `stimupy-1.0.0/stimupy/utils/color_conversions.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/contrast_conversions.py` & `stimupy-1.0.0/stimupy/utils/contrast_conversions.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/export.py` & `stimupy-1.0.0/stimupy/utils/export.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/filters.py` & `stimupy-1.0.0/stimupy/utils/filters.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/masks.py` & `stimupy-1.0.0/stimupy/utils/masks.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/pad.py` & `stimupy-1.0.0/stimupy/utils/pad.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/plotting.py` & `stimupy-1.0.0/stimupy/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/resolution.py` & `stimupy-1.0.0/stimupy/utils/resolution.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy/utils/utils.py` & `stimupy-1.0.0/stimupy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/stimupy.egg-info/PKG-INFO` & `stimupy-1.0.0/stimupy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimupy
-Version: 0.101.1
+Version: 1.0.0
 Summary: Stimuli for vision science, as image arrays
 Author: Matko Matic, Guillermo Aguilar, Marianne Maertens
 Author-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 Maintainer-email: Lynn Schmittwilken <l.schmittwilken@tu-berlin.de>, Joris Vincent <j.vincent@tu-berlin.de>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
@@ -307,15 +307,18 @@
 for creating new and existing visual stimuli
 commonly used in the study of contrast, brightness, lightness,
 and other aspects of visual perception.
 </p>
 
 <p align=center>
 
-[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml) [![](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
+[![JOSS Status](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d/status.svg)](https://joss.theoj.org/papers/af54c793f6f4c02a4af6a8b5f6f57e9d)
+[![PyPI version](https://img.shields.io/pypi/v/stimupy)](https://pypi.org/project/stimupy/)
+[![Tests](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml/badge.svg)](https://github.com/computational-psychology/stimupy/actions/workflows/test.yml)
+[![Py versions](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![Documentation Status](https://readthedocs.org/projects/stimupy/badge/?version=latest)](https://stimupy.readthedocs.io/en/latest/?badge=latest)
 </p>
 
 <p align=center>
 <img src=docs/logo.png width=400>
 </p>
 
@@ -404,18 +407,17 @@
 
 If you want to contribute yourself, see [contributing](https://stimupy.readthedocs.io/en/latest/contributing/contribute.html)
 
 
 ---
 ## Installation
 
-For now, `pip` can install directly from GitHub (the `main` branch)
-GitHub repository
+`pip` can install `stimupy` directly PyPI:
 ```python
-pip install https://github.com/computational-psychology/stimupy/zipball/main
+pip install stimupy
 ```
 
 OR (for developers), install from source:
 1. Clone the repository from GitHub:
 
     ```bash
     git clone git@github.com:computational-psychology/stimupy.git
```

### Comparing `stimupy-0.101.1/stimupy.egg-info/SOURCES.txt` & `stimupy-1.0.0/stimupy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/tests/test_pad.py` & `stimupy-1.0.0/tests/test_pad.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/tests/test_resolve_resolutions.py` & `stimupy-1.0.0/tests/test_resolve_resolutions.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/tests/test_valid_resolution.py` & `stimupy-1.0.0/tests/test_valid_resolution.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/tests/test_validate_resolution_components.py` & `stimupy-1.0.0/tests/test_validate_resolution_components.py`

 * *Files identical despite different names*

### Comparing `stimupy-0.101.1/tests/test_waves.py` & `stimupy-1.0.0/tests/test_waves.py`

 * *Files identical despite different names*

