# Comparing `tmp/module_qc_tools-1.3.2rc1.tar.gz` & `tmp/module_qc_tools-2.0.0.tar.gz`

## Comparing `module_qc_tools-1.3.2rc1.tar` & `module_qc_tools-2.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitmodules
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/tbump.toml
--rw-r--r--   0        0        0    40218 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/ADC_CALIBRATION/2023-05-16_222258/20UPGXM1234567.json
--rw-r--r--   0        0        0   311634 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/ANALOG_READBACK/2023-05-16_222258/20UPGXM1234567.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/INJECTION_CAPACITANCE/2023-05-16_222259/20UPGXM1234567.json
--rw-r--r--   0        0        0    27194 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/LP_MODE/2023-05-16_222257/20UPGXM1234567.json
--rw-r--r--   0        0        0    23798 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/OVERVOLTAGE_PROTECTION/2023-05-16_222254/20UPGXM1234567.json
--rw-r--r--   0        0        0    75478 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/SLDO/2023-05-16_222255/20UPGXM1234567.json
--rw-r--r--   0        0        0   140202 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/Measurements/VCAL_CALIBRATION/2023-05-16_222245/20UPGXM1234567.json
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/emulator/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    21900 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0    17516 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/emulator_merged_vmux.json
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_merged_vmux.json
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_separate_vmux.json
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/LP_MODE.json
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0     5157 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/config.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/LICENSE
--rw-r--r--   0        0        0    28359 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/README.md
--rw-r--r--   0        0        0     4330 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/pyproject.toml
--rw-r--r--   0        0        0    30484 2020-02-02 00:00:00.000000 module_qc_tools-1.3.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitmodules
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/tbump.toml
+-rw-r--r--   0        0        0    40206 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/ADC_CALIBRATION/2023-05-23_144715/20UPGXM1234567.json
+-rw-r--r--   0        0        0   311598 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/ANALOG_READBACK/2023-05-23_144719/20UPGXM1234567.json
+-rw-r--r--   0        0        0    22334 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/INJECTION_CAPACITANCE/2023-05-23_144710/20UPGXM1234567.json
+-rw-r--r--   0        0        0    27182 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/LP_MODE/2023-05-23_144908/20UPGXM1234567.json
+-rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/OVERVOLTAGE_PROTECTION/2023-05-23_144903/20UPGXM1234567.json
+-rw-r--r--   0        0        0    75466 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/SLDO/2023-05-23_144651/20UPGXM1234567.json
+-rw-r--r--   0        0        0   140154 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/Measurements/VCAL_CALIBRATION/2023-05-23_144703/20UPGXM1234567.json
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/emulator/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    22166 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0    10519 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0    18660 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/LP_MODE.json
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    26090 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/data/schema/config.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    12555 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/LICENSE
+-rw-r--r--   0        0        0    28528 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/README.md
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 module_qc_tools-2.0.0/PKG-INFO
```

### Comparing `module_qc_tools-1.3.2rc1/.gitlab-ci.yml` & `module_qc_tools-2.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/.pre-commit-config.yaml` & `module_qc_tools-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/tbump.toml` & `module_qc_tools-2.0.0/tbump.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e33 2e32 7263 3122 0a0a  t = "1.3.2rc1"..
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
-00000150: 2e33 2e32 7263 3120 e286 9220 7b6e 6577  .3.2rc1 ... {new
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

### Comparing `module_qc_tools-1.3.2rc1/Measurements/ADC_CALIBRATION/2023-05-16_222258/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/ADC_CALIBRATION/2023-05-23_144715/20UPGXM1234567.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853237, 'TimeEnd': 1684853404}}}}",*

 * * '1': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853237, 'TimeEnd': 1684853404}}}}",*

 * * '2': "{0: {'results': {'property': {'ADC_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853237, 'TimeEnd': 1684853404}}}}",*

 * * '3': "{0: {'results': {'prop […]*

```diff
@@ -246,20 +246,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275961,
-                    "TimeStart": 1684275780
+                    "TimeEnd": 1684853404,
+                    "TimeStart": 1684853237
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -510,20 +510,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275961,
-                    "TimeStart": 1684275780
+                    "TimeEnd": 1684853404,
+                    "TimeStart": 1684853237
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -774,20 +774,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275961,
-                    "TimeStart": 1684275780
+                    "TimeEnd": 1684853404,
+                    "TimeStart": 1684853237
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ],
@@ -1038,20 +1038,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275961,
-                    "TimeStart": 1684275780
+                    "TimeEnd": 1684853404,
+                    "TimeStart": 1684853237
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "ADC_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/ANALOG_READBACK/2023-05-16_222258/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/ANALOG_READBACK/2023-05-23_144719/20UPGXM1234567.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'ANALOG_READBACK_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853241, 'TimeEnd': 1684853804}}}, 1: {'results': {'property': "*

 * *      "{'ANALOG_READBACK_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': {'TimeStart': 1684853331, "*

 * *      "'TimeEnd': 1684853804}}}, 2: {'results': {'property': "*

 * *      "{'ANALOG_READBACK_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': {'TimeStart': 1684853728, "*

 * *      "'TimeEnd': 1684853804}}}}",*

 * * '1': "{0: {'results': {'proper […]*

```diff
@@ -450,20 +450,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853241
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -1063,20 +1063,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275858
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853331
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -2178,20 +2178,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684276196
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853728
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -2646,20 +2646,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853241
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -3259,20 +3259,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275858
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853331
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -4374,20 +4374,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684276196
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853728
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -4842,20 +4842,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853241
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -5455,20 +5455,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275858
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853331
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -6570,20 +6570,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684276196
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853728
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -7038,20 +7038,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853241
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -7651,20 +7651,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684275858
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853331
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -8766,20 +8766,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276264,
-                    "TimeStart": 1684276196
+                    "TimeEnd": 1684853804,
+                    "TimeStart": 1684853728
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/INJECTION_CAPACITANCE/2023-05-16_222259/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/INJECTION_CAPACITANCE/2023-05-23_144710/20UPGXM1234567.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853231, 'TimeEnd': 1684853276}}}}",*

 * * '1': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853231, 'TimeEnd': 1684853276}}}}",*

 * * '2': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853232, 'TimeEnd': 1684853276}}}}",*

 * * '3': "{0:  […]*

```diff
@@ -120,20 +120,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275844,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853276,
+                    "TimeStart": 1684853231
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -258,20 +258,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275844,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853276,
+                    "TimeStart": 1684853231
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -396,20 +396,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275844,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853276,
+                    "TimeStart": 1684853232
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -534,20 +534,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275844,
-                    "TimeStart": 1684275781
+                    "TimeEnd": 1684853276,
+                    "TimeStart": 1684853232
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/LP_MODE/2023-05-16_222257/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/LP_MODE/2023-05-23_144908/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909855769230769%*

 * *Differences: {'0': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853349, 'TimeEnd': 1684853370}}}}",*

 * * '1': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853349, 'TimeEnd': 1684853370}}}}",*

 * * '2': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853349, 'TimeEnd': 1684853370}}}}",*

 * * '3': "{0: {'results': {'property': {'LP_MODE_MEASURE […]*

```diff
@@ -164,20 +164,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275799,
-                    "TimeStart": 1684275777
+                    "TimeEnd": 1684853370,
+                    "TimeStart": 1684853349
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -346,20 +346,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275799,
-                    "TimeStart": 1684275778
+                    "TimeEnd": 1684853370,
+                    "TimeStart": 1684853349
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -528,20 +528,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275799,
-                    "TimeStart": 1684275778
+                    "TimeEnd": 1684853370,
+                    "TimeStart": 1684853349
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -710,20 +710,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275799,
-                    "TimeStart": 1684275778
+                    "TimeEnd": 1684853370,
+                    "TimeStart": 1684853349
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/OVERVOLTAGE_PROTECTION/2023-05-16_222254/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/OVERVOLTAGE_PROTECTION/2023-05-23_144903/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909855769230769%*

 * *Differences: {'0': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853343, 'TimeEnd': 1684853357}}}}",*

 * * '1': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853343, 'TimeEnd': 1684853357}}}}",*

 * * '2': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.0.0'}, "*

 * *      "'Metadata': {'TimeStart': 1684853343, 'TimeEnd': 1684853357}}}}",*

 * * '3': "{ […]*

```diff
@@ -136,20 +136,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275791,
-                    "TimeStart": 1684275775
+                    "TimeEnd": 1684853357,
+                    "TimeStart": 1684853343
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -290,20 +290,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275791,
-                    "TimeStart": 1684275775
+                    "TimeEnd": 1684853357,
+                    "TimeStart": 1684853343
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -444,20 +444,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275791,
-                    "TimeStart": 1684275775
+                    "TimeEnd": 1684853357,
+                    "TimeStart": 1684853343
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -598,20 +598,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275791,
-                    "TimeStart": 1684275775
+                    "TimeEnd": 1684853357,
+                    "TimeStart": 1684853344
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/SLDO/2023-05-16_222255/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/SLDO/2023-05-23_144651/20UPGXM1234567.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909855769230769%*

 * *Differences: {'0': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853212, 'TimeEnd': 1684853728}}}}",*

 * * '1': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853212, 'TimeEnd': 1684853728}}}}",*

 * * '2': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853212, 'TimeEnd': 1684853728}}}}",*

 * * '3': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION […]*

```diff
@@ -466,20 +466,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276226,
-                    "TimeStart": 1684275776
+                    "TimeEnd": 1684853728,
+                    "TimeStart": 1684853212
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "SLDO_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -950,20 +950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276226,
-                    "TimeStart": 1684275776
+                    "TimeEnd": 1684853728,
+                    "TimeStart": 1684853212
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "SLDO_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1434,20 +1434,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276226,
-                    "TimeStart": 1684275776
+                    "TimeEnd": 1684853728,
+                    "TimeStart": 1684853212
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "SLDO_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1918,20 +1918,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684276226,
-                    "TimeStart": 1684275776
+                    "TimeEnd": 1684853728,
+                    "TimeStart": 1684853212
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "SLDO_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "SLDO"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/Measurements/VCAL_CALIBRATION/2023-05-16_222245/20UPGXM1234567.json` & `module_qc_tools-2.0.0/Measurements/VCAL_CALIBRATION/2023-05-23_144703/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908854166666666%*

 * *Differences: {'0': "{0: {'results': {'property': {'VCAL_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': "*

 * *      "{'TimeStart': 1684853229, 'TimeEnd': 1684853248}}}, 1: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': {'TimeStart': 1684853248, "*

 * *      "'TimeEnd': 1684853266}}}, 2: {'results': {'property': "*

 * *      "{'VCAL_CALIBRATION_MEASUREMENT_VERSION': '2.0.0'}, 'Metadata': {'TimeStart': 1684853266, "*

 * *      "'TimeEnd': 1684853285}}}, 3: {'results': {'property': "*

 * * […]*

```diff
@@ -202,20 +202,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275780,
-                    "TimeStart": 1684275769
+                    "TimeEnd": 1684853248,
+                    "TimeStart": 1684853229
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -420,20 +420,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275791,
-                    "TimeStart": 1684275780
+                    "TimeEnd": 1684853266,
+                    "TimeStart": 1684853248
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -638,20 +638,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275802,
-                    "TimeStart": 1684275791
+                    "TimeEnd": 1684853285,
+                    "TimeStart": 1684853266
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -856,20 +856,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275813,
-                    "TimeStart": 1684275802
+                    "TimeEnd": 1684853303,
+                    "TimeStart": 1684853285
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1076,20 +1076,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275824,
-                    "TimeStart": 1684275813
+                    "TimeEnd": 1684853322,
+                    "TimeStart": 1684853303
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1294,20 +1294,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275834,
-                    "TimeStart": 1684275824
+                    "TimeEnd": 1684853340,
+                    "TimeStart": 1684853322
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1512,20 +1512,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275845,
-                    "TimeStart": 1684275834
+                    "TimeEnd": 1684853359,
+                    "TimeStart": 1684853340
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -1730,20 +1730,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275855,
-                    "TimeStart": 1684275845
+                    "TimeEnd": 1684853377,
+                    "TimeStart": 1684853359
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -1950,20 +1950,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275866,
-                    "TimeStart": 1684275855
+                    "TimeEnd": 1684853395,
+                    "TimeStart": 1684853377
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2168,20 +2168,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275877,
-                    "TimeStart": 1684275866
+                    "TimeEnd": 1684853414,
+                    "TimeStart": 1684853395
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2386,20 +2386,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275887,
-                    "TimeStart": 1684275877
+                    "TimeEnd": 1684853432,
+                    "TimeStart": 1684853414
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -2604,20 +2604,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275898,
-                    "TimeStart": 1684275887
+                    "TimeEnd": 1684853451,
+                    "TimeStart": 1684853432
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ],
@@ -2824,20 +2824,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275909,
-                    "TimeStart": 1684275898
+                    "TimeEnd": 1684853470,
+                    "TimeStart": 1684853451
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3042,20 +3042,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275919,
-                    "TimeStart": 1684275909
+                    "TimeEnd": 1684853489,
+                    "TimeStart": 1684853470
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_MED_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3260,20 +3260,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275931,
-                    "TimeStart": 1684275919
+                    "TimeEnd": 1684853508,
+                    "TimeStart": 1684853489
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH",
             "testType": "VCAL_CALIBRATION"
         },
         {
@@ -3478,20 +3478,20 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1684275942,
-                    "TimeStart": 1684275931
+                    "TimeEnd": 1684853526,
+                    "TimeStart": 1684853508
                 },
                 "comment": "",
                 "property": {
-                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "1.3.2rc1"
+                    "VCAL_CALIBRATION_MEASUREMENT_VERSION": "2.0.0"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "VCAL_HIGH_SMALL_RANGE",
             "testType": "VCAL_CALIBRATION"
         }
     ]
```

### Comparing `module_qc_tools-1.3.2rc1/emulator/README.md` & `module_qc_tools-2.0.0/emulator/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
-    log.info("[run_AnalogReadBack] Start V scan!")
+    log.info("[run_AnalogReadBack] Start T measurement!")
     log.info(
         f"[run_AnalogReadBack] TimeStart: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
     if yr.running_emulator():
         ps.on(
             analog_readback_config["v_max"],
@@ -264,15 +264,15 @@
         ps (Class power_supply): An instance of Class power_supply for power on and power off.
         yr (Class yarr): An instance of Class yarr for chip conifugration and change register.
         meter (Class meter): An instance of Class meter. Used to control the multimeter to measure voltages.
 
     Returns:
         None: The measurements are recorded in `data`.
     """
-    log.info("[run_AnalogReadBack] Start V scan!")
+    log.info("[run_AnalogReadBack] Start VDD vs Trim measurement!")
     log.info(
         f"[run_AnalogReadBack] TimeStart: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
     if yr.running_emulator():
         ps.on(
             analog_readback_config["v_max"],
@@ -280,55 +280,64 @@
         )  # Only for emulator do the emulation of power on/off.
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # Reset other chips
     reset = analog_readback_config["share_vmux"]
 
     # Trim to Vmux mapping
-    trim_maps = {
+    vmux_to_trim = {
         34: "SldoTrimA",
         38: "SldoTrimD",
     }
 
     i_mea = [{} for _ in range(yr._number_of_chips)]
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
 
         # Measure VDDA/VDDD vs SldoTrimA/SldoTrimD
-        for v_mux in trim_maps:
+        for v_mux in vmux_to_trim:
             yr.set_mux(chip_position=chip, v_mux=v_mux, reset_other_chips=reset)
-            for trim in analog_readback_config[trim_maps[v_mux]]:
-                yr.set_trim(
-                    chip_position=chip,
-                    v_mux=v_mux,
-                    trim=trim,
-                    reset_other_chips=reset,
+
+            # Read initial Trim in chip config
+            config_trim, status = yr.read_register(
+                name=vmux_to_trim[v_mux], chip_position=chip
+            )
+
+            for trim in analog_readback_config[vmux_to_trim[v_mux]]:
+                # Set Trim
+                yr.write_register(
+                    name=vmux_to_trim[v_mux], value=trim, chip_position=chip
                 )
+
                 mea, status = meter.measure_dcv(
                     channel=analog_readback_config["v_mux_channels"][chip]
                 )
                 # Reset i_mea[chip]
                 i_mea[chip] = {}
 
                 # Record vmux and trim.
                 i_mea[chip][f"Vmux{v_mux}"] = [mea]
-                i_mea[chip][trim_maps[v_mux]] = [trim]
+                i_mea[chip][vmux_to_trim[v_mux]] = [trim]
 
                 # Read ROSC vs trim
                 if v_mux == 38:
-                    chip_name = data[chip]._meta_data["Name"]
-                    mea, status = yr.read_ringosc(name=chip_name, chip_position=chip)
+                    mea, status = yr.read_ringosc(chip_position=chip)
                     rosc_mea = [float(num) for num in mea.split()]
                     for i in range(len(rosc_mea)):
                         i_mea[chip][f"ROSC{i}"] = [rosc_mea[i]]
 
                 # Update output dataframe
                 data[chip].add_data(i_mea[chip])
 
+            # Reset Trim to value in config
+            yr.write_register(
+                name=vmux_to_trim[v_mux], value=config_trim, chip_position=chip
+            )
+
         # Mwasure ground 16 times.
         max_n_measure = len(data[chip]["Vmux34"])
         n_measure = 0
         while n_measure < max_n_measure:
             i_mea[chip] = {}
             yr.set_mux(chip_position=chip, v_mux=30, reset_other_chips=reset)
             mea, status = meter.measure_dcv(
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/LP_MODE.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,14 +251,52 @@
         elif args.name == "InjVcalRange":
             module_state[f"Chip{chip+1}"]["InjVcalRange"] = int(args.value)
         module_state[f"Chip{chip+1}"] = update_Vmux(module_state[f"Chip{chip+1}"])
 
     update_module_state(module_state)
 
 
+def read_register():
+    """
+    This function emulates the effect of running YARR read-register
+    Currently only emulates register SldoTrimA and SldoTrimD. One needs to add a new if statement for a new register name.
+    """
+    parser = argparse.ArgumentParser()
+    parser.add_argument("name", type=str, help="Name")
+    parser.add_argument(
+        "-r",
+        "--controller",
+        default="configs/controller/specCfg-rd53b-16x1.json",
+        help="Controller",
+    )
+    parser.add_argument(
+        "-c",
+        "--connectivity",
+        default=_MODULE_CONNECTIVITY_FILE,
+        help="Connectivity",
+    )
+    parser.add_argument("-i", "--chipPosition", type=int, help="chip position")
+    args = parser.parse_args()
+
+    with Path(args.connectivity).open() as path:
+        spec_connectivity = json.load(path)
+
+    nChips = len(spec_connectivity["chips"])
+
+    for chip in range(nChips):
+        if args.chipPosition is not None and chip is not args.chipPosition:
+            continue
+        if args.name == "SldoTimA" or args.name == "SldoTrimD":
+            sys.stdout.write("8")
+            sys.exit(0)
+        else:
+            sys.stdout.write("0")
+            sys.exit(0)
+
+
 def control_PS():
     """
     This function emulates the effect of powering the module
     """
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-a", "--action", choices=["on", "off", "getV", "getI"], help="Action to PS"
@@ -428,15 +466,14 @@
 
 
 def read_ringosc():
     """
     This function emulates the effect of ROSC reading
     """
     parser = argparse.ArgumentParser()
-    parser.add_argument("name", type=str, help="Name")
     parser.add_argument(
         "-r",
         "--controller",
         default=data / "emulator/configs/controller/specCfg-rd53b-16x1.json",
         help="Controller",
     )
     parser.add_argument(
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/main.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-2.0.0/src/module_qc_tools/cli/upload_localdb.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/emulator_merged_vmux.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'yarr'": "{'read_register_exe': 'emulator-read-register'}"}*

```diff
@@ -337,14 +337,15 @@
         }
     },
     "yarr": {
         "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
         "controller": "configs/controller/emuCfg_rd53a.json",
         "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "emulator-read-adc",
+        "read_register_exe": "emulator-read-register",
         "read_ringosc_exe": "emulator-read-ringosc",
         "run_dir": "emulator",
         "scanConsole_exe": "emulator-scanConsole",
         "switchLPM_exe": "emulator-switch-lpm",
         "write_register_exe": "emulator-write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_merged_vmux.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888888888888889%*

 * *Differences: {"'yarr'": "{'read_register_exe': './bin/read-register'}"}*

```diff
@@ -343,14 +343,15 @@
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
         "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "./bin/read-adc",
+        "read_register_exe": "./bin/read-register",
         "read_ringosc_exe": "./bin/rd53bReadRingosc",
         "run_dir": "../Yarr",
         "scanConsole_exe": "./bin/scanConsole",
         "switchLPM_exe": "./bin/switchLPM",
         "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/configs/example_separate_vmux.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888888888888889%*

 * *Differences: {"'yarr'": "{'read_register_exe': './bin/read-register'}"}*

```diff
@@ -346,14 +346,15 @@
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
         "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "./bin/read-adc",
+        "read_register_exe": "./bin/read-register",
         "read_ringosc_exe": "./bin/rd53bReadRingosc",
         "run_dir": "../Yarr",
         "scanConsole_exe": "./bin/scanConsole",
         "switchLPM_exe": "./bin/switchLPM",
         "write_register_exe": "./bin/write-register"
     }
 }
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/LP_MODE.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/LP_MODE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/data/schema/config.json` & `module_qc_tools-2.0.0/src/module_qc_tools/data/schema/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997361111111112%*

 * *Differences: {"'properties'": "{'yarr': {'properties': {'read_register_exe': OrderedDict([('description', 'Path "*

 * *                 "(relative to run_dir or absolute) to the read_register executable')])}, "*

 * *                 "'required': {insert: [(4, 'read_register_exe')]}}}"}*

```diff
@@ -106,14 +106,17 @@
                 },
                 "lpm_digitalscan": {
                     "description": "Path (relative to run_dir or absolute) to the low-power mode digital scan in YARR"
                 },
                 "read_adc_exe": {
                     "description": "Path (relative to run_dir or absolute) to the read_adc executable"
                 },
+                "read_register_exe": {
+                    "description": "Path (relative to run_dir or absolute) to the read_register executable"
+                },
                 "read_ringosc_exe": {
                     "description": "Path (relative to run_dir or absolute) to the read_wringosc executbable"
                 },
                 "run_dir": {
                     "description": "Path (absolute or relative) to YARR directory"
                 },
                 "scanConsole_exe": {
@@ -130,14 +133,15 @@
                 }
             },
             "required": [
                 "run_dir",
                 "controller",
                 "scanConsole_exe",
                 "write_register_exe",
+                "read_register_exe",
                 "read_adc_exe",
                 "switchLPM_exe",
                 "lpm_digitalscan",
                 "read_ringosc_exe"
             ],
             "type": "object"
         }
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,26 +73,26 @@
         os.chdir(self._wd)
 
         log.debug(result.stdout.decode())
 
         # A while loop to retry communications in case of timeout error.
         # The maximum number of tries is determined by the function argument max_nTry.
         nTry = 0
-        while result.returncode != 0 and nTry < max_nTry:
+        while result.returncode != success_code and nTry < max_nTry:
             nTry += 1
             for extra_error_message in extra_error_messages:
                 log.info(f"[{self._name}] {extra_error_message}")
             log.info(f"Try again. Send command and read attempt {nTry} time(s).")
             os.chdir(self._wd)
             os.chdir(self.run_dir)
             result = subprocess.run(cmd, shell=True, stdout=subprocess.PIPE)
             os.chdir(self._wd)
             log.debug(result.stdout.decode())
 
         if result.returncode != success_code:
-            msg = f"[{self._name}] fail to {purpose}!!"
+            msg = f"[{self._name}] fail to {purpose}!! Exit with returncode {result.returncode}."
             raise RuntimeError(msg)
         value = type(result.stdout.decode())
         for _extra_error_message in extra_error_messages:
             log.info(f"[{self._name}] {purpose}: {value}{unit}")
 
         return value, result.returncode
```

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/misc.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/multimeter.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/ntc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/power_supply.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/src/module_qc_tools/utils/yarr.py` & `module_qc_tools-2.0.0/src/module_qc_tools/utils/yarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,18 +122,18 @@
         if chip_position in self._disabled_chip_positions:
             return 0
         cmd = f'{self.read_adc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""} {"-I " if readCurrent else ""} {"-R " if rawCounts else ""} {vmux}'
         return self.send_command_and_read(
             cmd, type=str, purpose="read adc", success_code=self.success_code
         )
 
-    def read_ringosc(self, name, chip_position=None):
+    def read_ringosc(self, chip_position=None):
         if chip_position in self._disabled_chip_positions:
             return 0
-        cmd = f'{self.read_ringosc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""} {name}'
+        cmd = f'{self.read_ringosc_exe} -r {self.controller} -c {self.connectivity} {"-i "+str(chip_position) if chip_position is not None else ""}'
         return self.send_command_and_read(cmd, type=str, purpose="read ringsoc")
 
     def set_mux(self, chip_position, v_mux=-1, i_mux=-1, reset_other_chips=True):
         for chip in range(self._number_of_chips):
             if chip == chip_position:
                 # self.write_register(name="MonitorEnable", value=1, chip_position=str(chip))
 
@@ -269,31 +269,26 @@
                     msg = "Incorrect VMUX value for measuring temperature!"
                     raise RuntimeError(msg)
             elif reset_other_chips:
                 self.reset_tempsens(chip_position=chip)
 
         return 0
 
-    def set_trim(self, chip_position, v_mux=-1, trim=0, reset_other_chips=True):
-        for chip in range(self._number_of_chips):
-            if chip == chip_position:
-                if v_mux == 34:
-                    self.write_register(
-                        name="SldoTrimA", value=trim, chip_position=chip
-                    )
-                elif v_mux == 38:
-                    self.write_register(
-                        name="SldoTrimD", value=trim, chip_position=chip
-                    )
-                else:
-                    msg = "Incorrect VMUX value for setting trim!"
-                    raise RuntimeError(msg)
-            elif reset_other_chips:
-                self.write_register(name="SldoTrimA", value=0, chip_position=chip)
-                self.write_register(name="SldoTrimD", value=0, chip_position=chip)
+    def set_trim(self, chip_position, v_mux=-1, trim=0):
+        if v_mux == 34:
+            self.write_register(
+                name="SldoTrimA", value=trim, chip_position=chip_position
+            )
+        elif v_mux == 38:
+            self.write_register(
+                name="SldoTrimD", value=trim, chip_position=chip_position
+            )
+        else:
+            msg = "Incorrect VMUX value for setting trim!"
+            raise RuntimeError(msg)
 
         return 0
 
     def switchLPM(self, position):
         cmd = f"{self.switchLPM_exe} {position}"
         return self.send_command(cmd, purpose="switch LP mode on/off")
```

### Comparing `module_qc_tools-1.3.2rc1/.gitignore` & `module_qc_tools-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/LICENSE` & `module_qc_tools-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-1.3.2rc1/README.md` & `module_qc_tools-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-tools v1.3.2rc1
+# module-qc-tools v2.0.0
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -66,15 +66,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.2rc1
+python -m pip install -U pip module-qc-tools==2.0.0
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -165,14 +165,16 @@
 - `run_dir`: path (relative or absolute) to the directory where `YARR` commands
   should be run
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
 - `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
 - `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
+- `read_register_exe`: path (relative to `run_dir` or absolute) to the
+  `read_register` executable
 - `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
 - `switchLPM_exe`: path (relative to `run_dir` or absolute) to the `switchLPM`
   executable
 - `lpm_digitalscan`: path (relative to `run_dir` or absolute) to the low-power
   mode digital scan in YARR
 - `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
@@ -334,14 +336,16 @@
   sensors
 - `MonSensSldoDigSelBias`: Bias 0 and 1 for MOS sensor near digital SLDO
 - `MonSensSldoAnaSelBias`: Bias 0 and 1 for MOS sensor near analog SLDO
 - `MonSensAcbSelBias`: Bias 0 and 1 for MOS sensor near center
 - `MonSensSldoDigDem`: Dem 0-15 for MOS sensor near digital SLDO
 - `MonSensSldoAnaDem`: Dem 0-15 for MOS sensor near analog SLDO
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
+- `SldoTrimA`: Sldo analog Trim 0-15
+- `SldoTrimD`: Sldo digital Trim 0-15
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-o OUTPUT_DIR]
```

### Comparing `module_qc_tools-1.3.2rc1/pyproject.toml` & `module_qc_tools-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues"
 "Source" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools"
 
 [project.scripts]
 module-qc-tools = "module_qc_tools.cli.main:main"
 emulator-scanConsole = "module_qc_tools.cli.hardware_emulator:scanConsole"
 emulator-write-register = "module_qc_tools.cli.hardware_emulator:write_register"
+emulator-read-register = "module_qc_tools.cli.hardware_emulator:read_register"
 emulator-read-adc = "module_qc_tools.cli.hardware_emulator:read_adc"
 emulator-read-ringosc = "module_qc_tools.cli.hardware_emulator:read_ringosc"
 emulator-switch-lpm = "module_qc_tools.cli.hardware_emulator:switchLPM"
 emulator-control-ps = "module_qc_tools.cli.hardware_emulator:control_PS"
 emulator-measureV = "module_qc_tools.cli.hardware_emulator:measureV"
 emulator-measureT = "module_qc_tools.cli.hardware_emulator:measureT"
 measurement-ADC-CALIBRATION = "module_qc_tools.cli.ADC_CALIBRATION:main"
```

### Comparing `module_qc_tools-1.3.2rc1/PKG-INFO` & `module_qc_tools-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_qc_tools
-Version: 1.3.2rc1
+Version: 2.0.0
 Summary: Module qc tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -36,15 +36,15 @@
 Requires-Dist: module-qc-data-tools>=1.0.5
 Requires-Dist: numpy
 Requires-Dist: pre-commit
 Requires-Dist: requests
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
-# module-qc-tools v1.3.2rc1
+# module-qc-tools v2.0.0
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -108,15 +108,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 python -m venv venv
 source venv/bin/activate
 python -m pip install -U pip
-python -m pip install -U pip module-qc-tools==1.3.2rc1
+python -m pip install -U pip module-qc-tools==2.0.0
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
 
@@ -207,14 +207,16 @@
 - `run_dir`: path (relative or absolute) to the directory where `YARR` commands
   should be run
 - `controller`: path (relative to `run_dir` or absolute) to the controller file
 - `scanConsole_exe`: path (relative to `run_dir` or absolute) to the
   `scanConsole` executable
 - `write_register_exe`: path (relative to `run_dir` or absolute) to the
   `write_register` executable
+- `read_register_exe`: path (relative to `run_dir` or absolute) to the
+  `read_register` executable
 - `read_adc_exe`: path (relative to `run_dir` or absolute) to the `read_adc`
   executable
 - `switchLPM_exe`: path (relative to `run_dir` or absolute) to the `switchLPM`
   executable
 - `lpm_digitalscan`: path (relative to `run_dir` or absolute) to the low-power
   mode digital scan in YARR
 - `read_ringosc_exe`: path (relative to `run_dir` or absolute) to the
@@ -376,14 +378,16 @@
   sensors
 - `MonSensSldoDigSelBias`: Bias 0 and 1 for MOS sensor near digital SLDO
 - `MonSensSldoAnaSelBias`: Bias 0 and 1 for MOS sensor near analog SLDO
 - `MonSensAcbSelBias`: Bias 0 and 1 for MOS sensor near center
 - `MonSensSldoDigDem`: Dem 0-15 for MOS sensor near digital SLDO
 - `MonSensSldoAnaDem`: Dem 0-15 for MOS sensor near analog SLDO
 - `MonSensAcbDem`: Dem 0-15 for MOS sensor near center
+- `SldoTrimA`: Sldo analog Trim 0-15
+- `SldoTrimD`: Sldo digital Trim 0-15
 
 </details>
 
 <details> <summary> Help message </summary>
 
 ```
 usage: measurement-ANALOG-READBACK [-h] [-c CONFIG] [-o OUTPUT_DIR]
```

