# Comparing `tmp/module_qc_analysis_tools-1.3.1rc8.tar.gz` & `tmp/module_qc_analysis_tools-2.0.0.tar.gz`

## Comparing `module_qc_analysis_tools-1.3.1rc8.tar` & `module_qc_analysis_tools-2.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.flake8
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitmodules
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/_version.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    22396 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
--rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/TUNING.py
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/__main__.py
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/globals.py
--rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/load_yarr_scans.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/main.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/overwrite_config.py
--rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/update_chip_config.py
--rw-r--r--   0        0        0     4804 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/analysis_cuts.json
--rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/pixel_classification.json
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/info_schema.json
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
--rw-r--r--   0        0        0    33126 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/analysis.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/classification.py
--rw-r--r--   0        0        0    36639 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/misc.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/LICENSE
--rw-r--r--   0        0        0    25306 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/README.md
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/pyproject.toml
--rw-r--r--   0        0        0    27430 2020-02-02 00:00:00.000000 module_qc_analysis_tools-1.3.1rc8/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.flake8
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitmodules
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tbump.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/_version.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    12036 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0     9548 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py
+-rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/TUNING.py
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/globals.py
+-rwxr-xr-x   0        0        0     8167 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/load_yarr_scans.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/main.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/overwrite_config.py
+-rw-r--r--   0        0        0     8646 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/update_chip_config.py
+-rw-r--r--   0        0        0     7376 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/analysis_cuts.json
+-rw-r--r--   0        0        0     5212 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/pixel_classification.json
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/info_schema.json
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_yarr_schema.json
+-rw-r--r--   0        0        0    33358 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/analysis.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/classification.py
+-rw-r--r--   0        0        0    36639 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/misc.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/tests/test_package.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/LICENSE
+-rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/README.md
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    27421 2020-02-02 00:00:00.000000 module_qc_analysis_tools-2.0.0/PKG-INFO
```

### Comparing `module_qc_analysis_tools-1.3.1rc8/.gitlab-ci.yml` & `module_qc_analysis_tools-2.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/.pre-commit-config.yaml` & `module_qc_analysis_tools-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/tbump.toml` & `module_qc_analysis_tools-2.0.0/tbump.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e31 7263 3822 0a0a  t = "1.3.1rc8"..
-00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
-00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
-00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
-00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
-00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
-00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
-00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
-00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
-000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
-000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
-000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
-000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
-000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
-000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
-00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
-00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
-00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
-00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
-00000140: 2242 756d 7020 7665 7273 696f 6e3a 2031  "Bump version: 1
-00000150: 2e33 2e31 7263 3820 e286 9220 7b6e 6577  .3.1rc8 ... {new
-00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
-00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
-00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
-00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
-000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
-000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
-000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
-000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
-000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
-000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
-00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
-00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
-00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
-00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
-00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
-00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
-00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
-00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
-00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
-00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
-000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
-000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
-000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
-000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
-000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
-000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
-00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
-00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
-00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
-00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
-00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
-00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
-00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
-00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
-00000380: 2222 0a                                  "".
+00000010: 7420 3d20 2232 2e30 2e30 220a 0a23 2045  t = "2.0.0"..# E
+00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
+00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
+00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
+00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
+00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
+00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
+00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
+00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
+000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
+000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
+000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
+000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
+000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
+000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
+00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
+00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
+00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
+00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
+00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 302e  mp version: 2.0.
+00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
+00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
+00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
+00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
+00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
+000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
+000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
+000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
+000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
+000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
+00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
+00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
+00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
+00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
+00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
+00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
+00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
+00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
+00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
+00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
+000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
+000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
+000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
+000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
+000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
+000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
+00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
+00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
+00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
+00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
+00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
+00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
+00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
+00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
```

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/ANALOG_READBACK.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,24 +206,31 @@
     fig.savefig(output_dir.joinpath(f"{chipname}_ROSC_vs_VDDD_{plot_name}.png"))
     plt.close(fig)
 
 
 def plot_rosc_vs_vddd(rosc, vdd, chipname, output_dir, fit_method):
     p1_list = []
     p0_list = []
+    maxres_list = []
 
     # Get SLOP and OFFSET
     for _i, rosc_i in enumerate(rosc):
-        p1, p0 = (
-            linear_fit(vdd, rosc_i)
-            if fit_method == "root"
-            else linear_fit_np(vdd, rosc_i)
-        )
+        if fit_method == "root":
+            p1, p0 = linear_fit(vdd, rosc_i)
+        elif fit_method == "numpy":
+            p1, p0 = linear_fit_np(vdd, rosc_i)
+
+        # Calculate predicted values
+        predicted_rosc = p1 * np.array(vdd) + p0
+        # Calculate residuals
+        max_res = abs(max(rosc_i - predicted_rosc, key=abs))
+
         p1_list.append(p1)
         p0_list.append(p0)
+        maxres_list.append(max_res)
 
     # Define names
     bank_AB_name = [
         "CLK 0",
         "CLK 4",
         "Inv 0",
         "Inv 4",
@@ -315,15 +322,15 @@
         p1_list[34:],
         p0_list[34:],
         "Bank B Inj-cap-loaded 4-input NAND 4",
         chipname,
         output_dir,
     )
 
-    return p1_list, p0_list
+    return p1_list, p0_list, maxres_list
 
 
 @app.command()
 def main(
     input_meas: Path = OPTIONS["input_meas"],
     base_output_dir: Path = OPTIONS["output_dir"],
     qc_criteria_path: Path = OPTIONS["qc_criteria"],
@@ -534,35 +541,39 @@
                 )
                 plot_vdd_vs_trim(
                     trimD, vddd, "VDDD", output_name_vddd, chipname, fit_method.value
                 )
 
                 # Plot ROSC vs VDDD
                 rosc_list = [
-                    calculated_data[f"ROSC{i}"]["Values"].tolist() for i in range(1, 42)
+                    calculated_data[f"ROSC{i}"]["Values"].tolist() for i in range(42)
                 ]
-                p1_list, p0_list = plot_rosc_vs_vddd(
+                p1_list, p0_list, maxres_list = plot_rosc_vs_vddd(
                     rosc_list,
                     vddd,
                     chipname,
                     output_dir,
                     fit_method.value,
                 )
 
                 # Add parameters for output file
                 data[chipname].add_parameter("AR_VDDA_VS_TRIM", round_list(vdda, 4))
                 data[chipname].add_parameter("AR_VDDD_VS_TRIM", round_list(vddd, 4))
                 data[chipname].add_parameter("AR_ROSC_SLOPE", round_list(p1_list, 4))
                 data[chipname].add_parameter("AR_ROSC_OFFSET", round_list(p0_list, 4))
+                data[chipname].add_parameter(
+                    "AR_ROSC_MAX_RESIDUAL", round_list(maxres_list, 4)
+                )
 
                 # Load values to dictionary for QC analysis
                 tmpresults.update({"AR_VDDA_VS_TRIM": round_list(vdda, 4)})
                 tmpresults.update({"AR_VDDD_VS_TRIM": round_list(vddd, 4)})
                 tmpresults.update({"AR_ROSC_SLOPE": round_list(p1_list, 4)})
                 tmpresults.update({"AR_ROSC_OFFSET": round_list(p0_list, 4)})
+                tmpresults.update({"AR_ROSC_MAX_RESIDUAL": round_list(maxres_list, 4)})
             else:
                 log.warning(
                     bcolors.WARNING
                     + f"{filename}.json does not have any required subtestType. Skipping."
                     + bcolors.ENDC
                 )
                 continue
@@ -587,15 +598,15 @@
             log.addHandler(chiplog)
             passes_qc, summary = perform_qc_analysis(
                 test_type,
                 qc_config,
                 layer,
                 results.get(key),
             )
-            print_result_summary(summary, test_type, output_dir, chipname)
+            print_result_summary(summary, test_type, output_dir, key)
             if passes_qc == -1:
                 log.error(
                     bcolors.ERROR
                     + f" QC analysis for {key} was NOT successful. Please fix and re-run. Continuing to next chip.."
                     + bcolors.ENDC
                 )
                 continue
```

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/IV_MEASURE.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/LP_MODE.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MASS_MEASUREMENT.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/MIN_HEALTH_TEST.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/PIXEL_FAILURE_ANALYSIS.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/SLDO.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/TUNING.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/TUNING.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/VISUAL_INSPECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/globals.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/load_yarr_scans.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/load_yarr_scans.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/main.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/overwrite_config.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/overwrite_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/cli/update_chip_config.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/cli/update_chip_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/pixel_classification.json` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/pixel_classification.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/info_schema.json` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/info_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/data/schema/input_chipconfig_schema.json`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/analysis.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,19 +257,22 @@
 
 def perform_qc_analysis_AR_ROSC(_test_type, qc_config, _layer_name, results, key):
     # QC analysis for ROSC_VS_VDDD
     pass_rosc_vs_vddd_test = True
 
     cell_text = np.empty(0)
 
-    lower_bound = qc_config[0]
-    upper_bound = qc_config[1]
-
     for i in range(len(results)):
         tmp_pass_qc = True
+        lower_bound = (
+            qc_config[0] if "RESIDUAL" in key else qc_config.get(f"ROSC{i}")[0]
+        )
+        upper_bound = (
+            qc_config[1] if "RESIDUAL" in key else qc_config.get(f"ROSC{i}")[1]
+        )
         if (results[i] < lower_bound) or (results[i] > upper_bound):
             tmp_pass_qc = False
         if tmp_pass_qc:
             print_output_pass(f"{key}_{i}", results[i], lower_bound, upper_bound)
         else:
             print_output_fail(f"{key}_{i}", results[i], lower_bound, upper_bound)
         cell_text = np.append(
@@ -339,15 +342,15 @@
                 key,
             )
             cell_text = np.append(cell_text, new_cell_text)
             passes_qc_overall = passes_qc_overall and passes_qc_test
             continue
 
         # Handle AR_ROSC_SLOPE and AR_ROSC_OFFSET separately
-        if ("AR_ROSC_SLOPE" in key) or ("AR_ROSC_OFFSET" in key):
+        if "AR_ROSC" in key:
             passes_qc_test, new_cell_text = perform_qc_analysis_AR_ROSC(
                 test_type,
                 qc_selections.get(key),
                 layer_name,
                 results.get(key),
                 key,
             )
@@ -509,17 +512,17 @@
 
     # Temporary solution to avoid error when indexing array that doesn't exist
     if not results.get("AR_VDDA_VS_TRIM"):
         results.update({"AR_VDDA_VS_TRIM": [-1] * 16})
     if not results.get("AR_VDDD_VS_TRIM"):
         results.update({"AR_VDDD_VS_TRIM": [-1] * 16})
     if not results.get("AR_ROSC_SLOPE"):
-        results.update({"AR_ROSC_SLOPE": [-1] * 41})
+        results.update({"AR_ROSC_SLOPE": [-1] * 42})
     if not results.get("AR_ROSC_OFFSET"):
-        results.update({"AR_ROSC_OFFSET": [-1] * 41})
+        results.update({"AR_ROSC_OFFSET": [-1] * 42})
     if not results.get("AR_NOMINAL_SETTINGS"):
         results.update({"AR_NOMINAL_SETTINGS": [-1] * 72})
     analysis_version = results.get("property").get("ANALYSIS_VERSION")
     meas_version = results.get("Metadata").get("MEASUREMENT_VERSION")
 
     url = {
         "ADC_CALIBRATION": f"https://docs.google.com/forms/d/e/1FAIpQLSegDYRQ1Foe5eTuSOVZUXe0d1f_Bh5v3rhsffCnu9DUDFR69A/formResponse?usp=pp_url\
@@ -568,15 +571,15 @@
 	&entry.1592726943={results.get('LP_VINA')}\
 	&entry.422835427={results.get('LP_VIND')}\
 	&entry.1218296463={results.get('LP_VOFFS')}\
 	&entry.1682731027={results.get('LP_IINA')}\
 	&entry.784021623={results.get('LP_IIND')}\
 	&entry.1188204940={results.get('LP_ISHUNTA')}\
 	&entry.1456818826={results.get('LP_ISHUNTD')}\
-        &entry.1355617557={results.get('LP_DIGITAL_FAIL')}",
+	&entry.1355617557={results.get('LP_DIGITAL_FAIL')}",
         "OVERVOLTAGE_PROTECTION": f"https://docs.google.com/forms/d/e/1FAIpQLSc0lwqev5Yyozmnn3gkdnTOoH9BbSdjOuL7CAbhQOZ2rTJINg/formResponse?usp=pp_url\
 	&entry.1920584355={timestamp}\
 	&entry.104853658={outputDF.get('serialNumber')}\
 	&entry.1282466276={outputDF.get('passed')}\
 	&entry.141409196={analysis_version}\
 	&entry.1579707472={meas_version}\
 	&entry.913205750={layer}\
@@ -766,14 +769,15 @@
 	&entry.1335702676={results.get('AR_ROSC_SLOPE')[34]}\
 	&entry.1182244852={results.get('AR_ROSC_SLOPE')[35]}\
 	&entry.869372092={results.get('AR_ROSC_SLOPE')[36]}\
 	&entry.1109476155={results.get('AR_ROSC_SLOPE')[37]}\
 	&entry.696844799={results.get('AR_ROSC_SLOPE')[38]}\
 	&entry.881044474={results.get('AR_ROSC_SLOPE')[39]}\
 	&entry.210472674={results.get('AR_ROSC_SLOPE')[40]}\
+	&entry.1561547505={results.get('AR_ROSC_SLOPE')[41]}\
 	&entry.294359514={results.get('AR_ROSC_OFFSET')[0]}\
 	&entry.218278347={results.get('AR_ROSC_OFFSET')[1]}\
 	&entry.1296340612={results.get('AR_ROSC_OFFSET')[2]}\
 	&entry.325246147={results.get('AR_ROSC_OFFSET')[3]}\
 	&entry.1461792727={results.get('AR_ROSC_OFFSET')[4]}\
 	&entry.147717067={results.get('AR_ROSC_OFFSET')[5]}\
 	&entry.308162325={results.get('AR_ROSC_OFFSET')[6]}\
@@ -806,15 +810,16 @@
 	&entry.987149730={results.get('AR_ROSC_OFFSET')[33]}\
 	&entry.1559814776={results.get('AR_ROSC_OFFSET')[34]}\
 	&entry.1700713522={results.get('AR_ROSC_OFFSET')[35]}\
 	&entry.417646576={results.get('AR_ROSC_OFFSET')[36]}\
 	&entry.1968942403={results.get('AR_ROSC_OFFSET')[37]}\
 	&entry.1596668024={results.get('AR_ROSC_OFFSET')[38]}\
 	&entry.2058648829={results.get('AR_ROSC_OFFSET')[39]}\
-	&entry.1785914={results.get('AR_ROSC_OFFSET')[40]}",
+	&entry.1785914={results.get('AR_ROSC_OFFSET')[40]}\
+	&entry.1316032248={results.get('AR_ROSC_OFFSET')[41]}",
     }
     log.info(
         bcolors.WARNING
         + "Copy the following URL into a browser to submit these results: \n"
         + url.get(outputDF.get("testType")).replace("\t", "")
         + "\n"
         + "View submitted results at: https://docs.google.com/spreadsheets/d/1pw_07F94fg2GJQr8wlvhaRUV63uhsAuBt_S1FEFBzBU/view"
```

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/classification.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/classification.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/src/module_qc_analysis_tools/utils/misc.py` & `module_qc_analysis_tools-2.0.0/src/module_qc_analysis_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/tests/test_cli.py` & `module_qc_analysis_tools-2.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/.gitignore` & `module_qc_analysis_tools-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/LICENSE` & `module_qc_analysis_tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/README.md` & `module_qc_analysis_tools-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-analysis-tools v1.3.1rc8
+# module-qc-analysis-tools v2.0.0
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -71,15 +71,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc8
+python -m pip install -U pip module-qc-analysis-tools==2.0.0
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

### Comparing `module_qc_analysis_tools-1.3.1rc8/pyproject.toml` & `module_qc_analysis_tools-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_analysis_tools-1.3.1rc8/PKG-INFO` & `module_qc_analysis_tools-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-analysis-tools
-Version: 1.3.1rc8
+Version: 2.0.0
 Summary: Module qc analysis tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-analysis-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -34,15 +34,15 @@
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: matplotlib
 Requires-Dist: module-qc-data-tools>=1.0.6
 Requires-Dist: numpy
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# module-qc-analysis-tools v1.3.1rc8
+# module-qc-analysis-tools v2.0.0
 
 A general python tool for running ITkPixV1.1 module QC test analysis. An
 overview of the steps in the module QC procedure is documented in the
 [Electrical specification and QC procedures for ITkPixV1.1 modules](https://gitlab.cern.ch/atlas-itk/pixel/module/itkpix-electrical-qc/)
 document and in
 [this spreadsheet](https://docs.google.com/spreadsheets/d/1qGzrCl4iD9362RwKlstZASbhphV_qTXPeBC-VSttfgE/edit#gid=989740987).
 The analysis scripts in this repository require input files with measurement
@@ -111,15 +111,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-analysis-tools==1.3.1rc8
+python -m pip install -U pip module-qc-analysis-tools==2.0.0
 ```
 
 Note that users should use the latest python version (check python version via
 `python3 -V`). Python3.7 is the minimum requirement for developers. See
 [For Developer](#for-developer) section.
 
 ## Scripts
```

