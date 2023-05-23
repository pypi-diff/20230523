# Comparing `tmp/apstools-1.6.9.tar.gz` & `tmp/apstools-1.6.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apstools-1.6.9.tar", last modified: Wed Nov 30 17:25:10 2022, max compression
+gzip compressed data, was "apstools-1.6.9rc1.tar", last modified: Wed Nov 30 16:31:45 2022, max compression
```

## Comparing `apstools-1.6.9.tar` & `apstools-1.6.9rc1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.070318 apstools-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (122)    36894 2022-11-30 17:25:00.000000 apstools-1.6.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1978 2022-11-30 17:25:00.000000 apstools-1.6.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      225 2022-11-30 17:25:00.000000 apstools-1.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3301 2022-11-30 17:25:10.070318 apstools-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1587 2022-11-30 17:25:00.000000 apstools-1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.030317 apstools-1.6.9/apstools/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-30 17:25:09.000000 apstools-1.6.9/apstools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.030317 apstools-1.6.9/apstools/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      945 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10004 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/callback_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/doc_collector.py
--rw-r--r--   0 runner    (1001) docker     (122)    25884 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/nexus_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)    24313 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/spec_file_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.030317 apstools-1.6.9/apstools/callbacks/tests/
--rwxr-xr-x   0 runner    (1001) docker     (122)    66108 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/tests/440_specwriter_problem_run.zip
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2724 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/tests/test_440_specwriter.py
--rw-r--r--   0 runner    (1001) docker     (122)    14052 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/callbacks/tests/test_filewriter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.042317 apstools-1.6.9/apstools/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     6141 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2210 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/aps_bss_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     4192 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/aps_cycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3520 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/aps_cycle_info.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4520 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/aps_machine.py
--rw-r--r--   0 runner    (1001) docker     (122)     3103 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/aps_undulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    24419 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/area_detector_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     3938 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/axis_tuner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1973 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/description_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2128 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/dict_device_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     1331 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/epics_scan_id_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/eurotherm_2216e.py
--rw-r--r--   0 runner    (1001) docker     (122)    19868 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/flyer_motor_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5138 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/kohzu_monochromator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8718 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/lakeshore_controllers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5284 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/linkam_controllers.py
--rw-r--r--   0 runner    (1001) docker     (122)      731 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     6985 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/motor_mixins.py
--rw-r--r--   0 runner    (1001) docker     (122)     8018 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/positioner_soft_done.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/preamp_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      877 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/pss_shutter.db
--rw-r--r--   0 runner    (1001) docker     (122)     4787 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/pss_shutter.ui
--rw-r--r--   0 runner    (1001) docker     (122)     6292 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/ptc10_controller.py
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/scaler_support.py
--rw-r--r--   0 runner    (1001) docker     (122)    23559 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/shutters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3678 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/srs570_preamplifier.py
--rw-r--r--   0 runner    (1001) docker     (122)     2583 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/struck3820.py
--rw-r--r--   0 runner    (1001) docker     (122)     5231 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/synth_pseudo_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.046317 apstools-1.6.9/apstools/devices/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     9545 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_SingleTrigger_V34.py
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_aps_cycle.py
--rw-r--r--   0 runner    (1001) docker     (122)     9571 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_area_detector_support.py
--rw-r--r--   0 runner    (1001) docker     (122)      941 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_dict_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1055 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_epics_scan_id_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_eurotherm_2216e.py
--rw-r--r--   0 runner    (1001) docker     (122)     5187 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_flyer_motor_scaler.py
--rw-r--r--   0 runner    (1001) docker     (122)     7202 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_issue651.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_kohzu_monochromator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_lakeshores.py
--rw-r--r--   0 runner    (1001) docker     (122)    12913 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_positioner_soft_done.py
--rw-r--r--   0 runner    (1001) docker     (122)     1208 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tests/test_xia_slit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/tracking_signal.py
--rw-r--r--   0 runner    (1001) docker     (122)     4771 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/xia_pf4.py
--rw-r--r--   0 runner    (1001) docker     (122)     4430 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/devices/xia_slit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.046317 apstools-1.6.9/apstools/migration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6153 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/config
--rw-r--r--   0 runner    (1001) docker     (122)     6861 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/config-CNTPAR
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/config-MOTPAR
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/config_fourc
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/config_spec
--rwxr-xr-x   0 runner    (1001) docker     (122)    17852 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/spec2ophyd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.046317 apstools-1.6.9/apstools/migration/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4893 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/migration/tests/test_spec2ophyd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.050317 apstools-1.6.9/apstools/plans/
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18763 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/alignment.py
--rw-r--r--   0 runner    (1001) docker     (122)    11112 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/command_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2511 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/doc_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1632 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/input_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/nscan_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/run_blocking_function_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     7126 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/sscan_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     1889 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/stage_sigs_support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.054317 apstools-1.6.9/apstools/plans/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/actions.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8021 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/actions.xlsx
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/demo3.xlsx
--rw-r--r--   0 runner    (1001) docker     (122)     5985 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_alignment.py
--rw-r--r--   0 runner    (1001) docker     (122)     4941 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_commandlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_input_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_issue606.py
--rw-r--r--   0 runner    (1001) docker     (122)     6256 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_plans.py
--rw-r--r--   0 runner    (1001) docker     (122)     2100 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_run_blocking_function_plan.py
--rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/plans/tests/test_stage_sigs_support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.058317 apstools-1.6.9/apstools/synApps/
--rw-r--r--   0 runner    (1001) docker     (122)     2514 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4886 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2321 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/asyn.py
--rw-r--r--   0 runner    (1001) docker     (122)      925 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/busy.py
--rw-r--r--   0 runner    (1001) docker     (122)    11252 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/calcout.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/db_2slit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/epid.py
--rw-r--r--   0 runner    (1001) docker     (122)     4260 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/iocstats.py
--rw-r--r--   0 runner    (1001) docker     (122)     6331 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/luascript.py
--rw-r--r--   0 runner    (1001) docker     (122)     2746 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/save_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     7430 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/scalcout.py
--rw-r--r--   0 runner    (1001) docker     (122)    11111 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/sscan.py
--rw-r--r--   0 runner    (1001) docker     (122)     6404 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/sseq.py
--rw-r--r--   0 runner    (1001) docker     (122)     6801 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/sub.py
--rw-r--r--   0 runner    (1001) docker     (122)    11214 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/swait.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.058317 apstools-1.6.9/apstools/synApps/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_2slit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_calcout.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_iocstats.py
--rw-r--r--   0 runner    (1001) docker     (122)     5371 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_luascript.py
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_scalcout.py
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_sseq.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/tests/test_swait.py
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/synApps/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.062317 apstools-1.6.9/apstools/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/tests/test_package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.066317 apstools-1.6.9/apstools/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    12716 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     5307 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/device_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     2270 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/image_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/list_plans.py
--rw-r--r--   0 runner    (1001) docker     (122)    19046 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/list_runs.py
--rw-r--r--   0 runner    (1001) docker     (122)     4804 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)    16754 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/override_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     5148 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/profile_support.py
--rw-r--r--   0 runner    (1001) docker     (122)     7021 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/pvregistry.py
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/query.py
--rw-r--r--   0 runner    (1001) docker     (122)      648 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/slit_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10367 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/spreadsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.070318 apstools-1.6.9/apstools/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_connect_pvlist.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_exceltable.py
--rw-r--r--   0 runner    (1001) docker     (122)     2690 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_findpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     3894 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_image_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)     4815 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_listdevice.py
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_listplans.py
--rw-r--r--   0 runner    (1001) docker     (122)     9617 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_listruns_class.py
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_override_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)    16529 2022-11-30 17:25:00.000000 apstools-1.6.9/apstools/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.070318 apstools-1.6.9/apstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5160 2022-11-30 17:25:10.000000 apstools-1.6.9/apstools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      720 2022-11-30 17:25:00.000000 apstools-1.6.9/environment.yml
--rw-r--r--   0 runner    (1001) docker     (122)      566 2022-11-30 17:25:00.000000 apstools-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-30 17:25:00.000000 apstools-1.6.9/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-30 17:25:00.000000 apstools-1.6.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-30 17:25:00.000000 apstools-1.6.9/requirements-sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2022-11-30 17:25:00.000000 apstools-1.6.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 17:25:10.070318 apstools-1.6.9/resources/
--rwxr-xr-x   0 runner    (1001) docker     (122)   120744 2022-11-30 17:25:00.000000 apstools-1.6.9/resources/apstools_test.zip
--rwxr-xr-x   0 runner    (1001) docker     (122)      377 2022-11-30 17:25:00.000000 apstools-1.6.9/resources/unpack.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)   276508 2022-11-30 17:25:00.000000 apstools-1.6.9/resources/usaxs_test.zip
--rw-r--r--   0 runner    (1001) docker     (122)     2688 2022-11-30 17:25:10.070318 apstools-1.6.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)      810 2022-11-30 17:25:00.000000 apstools-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.826258 apstools-1.6.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)    36849 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3304 2022-11-30 16:31:45.826258 apstools-1.6.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1587 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.806258 apstools-1.6.9rc1/apstools/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2022-11-30 16:31:45.000000 apstools-1.6.9rc1/apstools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.806258 apstools-1.6.9rc1/apstools/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10004 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/callback_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/doc_collector.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25884 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/nexus_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24313 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/spec_file_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.806258 apstools-1.6.9rc1/apstools/callbacks/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    66108 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/tests/440_specwriter_problem_run.zip
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2724 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/tests/test_440_specwriter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14052 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/callbacks/tests/test_filewriter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.810258 apstools-1.6.9rc1/apstools/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     6141 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2210 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/aps_bss_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4192 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/aps_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3520 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/aps_cycle_info.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4520 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/aps_machine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3103 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/aps_undulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24419 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/area_detector_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3938 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/axis_tuner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1973 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/description_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2128 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/dict_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/epics_scan_id_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/eurotherm_2216e.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19868 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/flyer_motor_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5138 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/kohzu_monochromator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8718 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/lakeshore_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5284 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/linkam_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6985 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/motor_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8018 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/positioner_soft_done.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/preamp_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/pss_shutter.db
+-rw-r--r--   0 runner    (1001) docker     (122)     4787 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/pss_shutter.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6292 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/ptc10_controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/scaler_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23559 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/shutters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3678 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/srs570_preamplifier.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2583 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/struck3820.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5231 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/synth_pseudo_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.814258 apstools-1.6.9rc1/apstools/devices/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9545 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_SingleTrigger_V34.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_aps_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9571 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_area_detector_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_dict_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1055 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_epics_scan_id_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_eurotherm_2216e.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5187 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_flyer_motor_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7202 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_issue651.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_kohzu_monochromator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_lakeshores.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12913 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_positioner_soft_done.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1208 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tests/test_xia_slit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/tracking_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4771 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/xia_pf4.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4430 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/devices/xia_slit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.814258 apstools-1.6.9rc1/apstools/migration/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6153 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/config
+-rw-r--r--   0 runner    (1001) docker     (122)     6861 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/config-CNTPAR
+-rw-r--r--   0 runner    (1001) docker     (122)    11852 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/config-MOTPAR
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/config_fourc
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/config_spec
+-rwxr-xr-x   0 runner    (1001) docker     (122)    17852 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/spec2ophyd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.814258 apstools-1.6.9rc1/apstools/migration/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4893 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/migration/tests/test_spec2ophyd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.814258 apstools-1.6.9rc1/apstools/plans/
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18763 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11112 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/command_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2511 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/doc_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1632 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/input_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/nscan_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/run_blocking_function_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7126 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/sscan_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1889 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/stage_sigs_support.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.818258 apstools-1.6.9rc1/apstools/plans/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/actions.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8021 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/actions.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/demo3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (122)     5985 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4941 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_commandlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_input_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2539 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_issue606.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6256 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2100 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_run_blocking_function_plan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/plans/tests/test_stage_sigs_support.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.818258 apstools-1.6.9rc1/apstools/synApps/
+-rw-r--r--   0 runner    (1001) docker     (122)     2514 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4886 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2321 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/busy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11252 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/calcout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/db_2slit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/epid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4260 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/iocstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6331 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/luascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2746 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/save_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/scalcout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11111 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/sscan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6404 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/sseq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6801 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/sub.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11214 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/swait.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.818258 apstools-1.6.9rc1/apstools/synApps/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_2slit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_calcout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_iocstats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5371 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_luascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_scalcout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_sseq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2259 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/tests/test_swait.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/synApps/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.818258 apstools-1.6.9rc1/apstools/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2308 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.822258 apstools-1.6.9rc1/apstools/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12716 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5307 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/image_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/list_plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19046 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/list_runs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4804 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16754 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/override_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5148 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/profile_support.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7021 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/pvregistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1563 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)      648 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/slit_core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10367 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/spreadsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.822258 apstools-1.6.9rc1/apstools/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_connect_pvlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_exceltable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2690 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_findpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3894 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_image_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4815 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_listdevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_listplans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9617 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_listruns_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2535 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_override_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16529 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/apstools/utils/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.826258 apstools-1.6.9rc1/apstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5160 2022-11-30 16:31:45.000000 apstools-1.6.9rc1/apstools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/requirements-sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 16:31:45.822258 apstools-1.6.9rc1/resources/
+-rwxr-xr-x   0 runner    (1001) docker     (122)   120744 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/resources/apstools_test.zip
+-rwxr-xr-x   0 runner    (1001) docker     (122)      377 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/resources/unpack.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)   276508 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/resources/usaxs_test.zip
+-rw-r--r--   0 runner    (1001) docker     (122)     2688 2022-11-30 16:31:45.826258 apstools-1.6.9rc1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)      810 2022-11-30 16:31:36.000000 apstools-1.6.9rc1/setup.py
```

### Comparing `apstools-1.6.9/CHANGES.rst` & `apstools-1.6.9rc1/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,29 +14,23 @@
 Change History
 ##############
 
 The project `milestones <https://github.com/BCDA-APS/apstools/milestones>`_
 describe the future plans.
 
 ..
-   1.6.11
-   ******
-
-   release expected by 2023-02-01
-
-..
    1.6.10
    ******
 
-   release expected by 2023-01-06
+   release expected by 2023-01-05
 
 1.6.9
 ******
 
-released 2022-11-30
+   release expected by 2022-12-18
 
 New Features
 ------------
 
 * Add ``ScalerMotorFlyer()`` device.
 * Add functions to support reporting of logging messages.
 * Add :meth:`restorable_stage_sigs` decorator.
```

### Comparing `apstools-1.6.9/LICENSE.txt` & `apstools-1.6.9rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/PKG-INFO` & `apstools-1.6.9rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apstools
-Version: 1.6.9
+Version: 1.6.9rc1
 Summary: Various Python tools for use with the Bluesky Framework at the APS.
 Home-page: https://bcda-aps.github.io/apstools
 Author: Pete R. Jemian
 Author-email: jemian@anl.gov
 License: Free To Use But Restricted (see LICENSE.txt file)
 Keywords: ["SPEC","diffraction","data acquisition","NeXus","HDF5","MatPlotLib"]
 Classifier: Development Status :: 6 - Mature
```

### Comparing `apstools-1.6.9/README.md` & `apstools-1.6.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/__init__.py` & `apstools-1.6.9rc1/apstools/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/__init__.py` & `apstools-1.6.9rc1/apstools/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/callback_base.py` & `apstools-1.6.9rc1/apstools/callbacks/callback_base.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/doc_collector.py` & `apstools-1.6.9rc1/apstools/callbacks/doc_collector.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/nexus_writer.py` & `apstools-1.6.9rc1/apstools/callbacks/nexus_writer.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/spec_file_writer.py` & `apstools-1.6.9rc1/apstools/callbacks/spec_file_writer.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/tests/440_specwriter_problem_run.zip` & `apstools-1.6.9rc1/apstools/callbacks/tests/440_specwriter_problem_run.zip`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/tests/test_440_specwriter.py` & `apstools-1.6.9rc1/apstools/callbacks/tests/test_440_specwriter.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/callbacks/tests/test_filewriter.py` & `apstools-1.6.9rc1/apstools/callbacks/tests/test_filewriter.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/__init__.py` & `apstools-1.6.9rc1/apstools/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/aps_bss_user.py` & `apstools-1.6.9rc1/apstools/devices/aps_bss_user.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/aps_cycle.py` & `apstools-1.6.9rc1/apstools/devices/aps_cycle.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/aps_cycle_info.yml` & `apstools-1.6.9rc1/apstools/devices/aps_cycle_info.yml`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/aps_machine.py` & `apstools-1.6.9rc1/apstools/devices/aps_machine.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/aps_undulator.py` & `apstools-1.6.9rc1/apstools/devices/aps_undulator.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/area_detector_support.py` & `apstools-1.6.9rc1/apstools/devices/area_detector_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/axis_tuner.py` & `apstools-1.6.9rc1/apstools/devices/axis_tuner.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/description_mixin.py` & `apstools-1.6.9rc1/apstools/devices/description_mixin.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/dict_device_support.py` & `apstools-1.6.9rc1/apstools/devices/dict_device_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/epics_scan_id_signal.py` & `apstools-1.6.9rc1/apstools/devices/epics_scan_id_signal.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/eurotherm_2216e.py` & `apstools-1.6.9rc1/apstools/devices/eurotherm_2216e.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/flyer_motor_scaler.py` & `apstools-1.6.9rc1/apstools/devices/flyer_motor_scaler.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/kohzu_monochromator.py` & `apstools-1.6.9rc1/apstools/devices/kohzu_monochromator.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/lakeshore_controllers.py` & `apstools-1.6.9rc1/apstools/devices/lakeshore_controllers.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/linkam_controllers.py` & `apstools-1.6.9rc1/apstools/devices/linkam_controllers.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/mixin_base.py` & `apstools-1.6.9rc1/apstools/devices/mixin_base.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/motor_mixins.py` & `apstools-1.6.9rc1/apstools/devices/motor_mixins.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/positioner_soft_done.py` & `apstools-1.6.9rc1/apstools/devices/positioner_soft_done.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/preamp_base.py` & `apstools-1.6.9rc1/apstools/devices/preamp_base.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/pss_shutter.db` & `apstools-1.6.9rc1/apstools/devices/pss_shutter.db`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/pss_shutter.ui` & `apstools-1.6.9rc1/apstools/devices/pss_shutter.ui`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/ptc10_controller.py` & `apstools-1.6.9rc1/apstools/devices/ptc10_controller.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/scaler_support.py` & `apstools-1.6.9rc1/apstools/devices/scaler_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/shutters.py` & `apstools-1.6.9rc1/apstools/devices/shutters.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/srs570_preamplifier.py` & `apstools-1.6.9rc1/apstools/devices/srs570_preamplifier.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/struck3820.py` & `apstools-1.6.9rc1/apstools/devices/struck3820.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/synth_pseudo_voigt.py` & `apstools-1.6.9rc1/apstools/devices/synth_pseudo_voigt.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/conftest.py` & `apstools-1.6.9rc1/apstools/devices/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_SingleTrigger_V34.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_SingleTrigger_V34.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_aps_cycle.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_aps_cycle.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_area_detector_support.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_area_detector_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_dict_device.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_dict_device.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_epics_scan_id_signal.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_epics_scan_id_signal.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_eurotherm_2216e.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_eurotherm_2216e.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_flyer_motor_scaler.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_flyer_motor_scaler.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_issue651.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_issue651.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_kohzu_monochromator.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_kohzu_monochromator.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_lakeshores.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_lakeshores.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_positioner_soft_done.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_positioner_soft_done.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tests/test_xia_slit.py` & `apstools-1.6.9rc1/apstools/devices/tests/test_xia_slit.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/tracking_signal.py` & `apstools-1.6.9rc1/apstools/devices/tracking_signal.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/xia_pf4.py` & `apstools-1.6.9rc1/apstools/devices/xia_pf4.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/devices/xia_slit.py` & `apstools-1.6.9rc1/apstools/devices/xia_slit.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/config` & `apstools-1.6.9rc1/apstools/migration/config`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/config-CNTPAR` & `apstools-1.6.9rc1/apstools/migration/config-CNTPAR`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/config-MOTPAR` & `apstools-1.6.9rc1/apstools/migration/config-MOTPAR`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/config_fourc` & `apstools-1.6.9rc1/apstools/migration/config_fourc`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/config_spec` & `apstools-1.6.9rc1/apstools/migration/config_spec`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/spec2ophyd.py` & `apstools-1.6.9rc1/apstools/migration/spec2ophyd.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/migration/tests/test_spec2ophyd.py` & `apstools-1.6.9rc1/apstools/migration/tests/test_spec2ophyd.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/__init__.py` & `apstools-1.6.9rc1/apstools/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/alignment.py` & `apstools-1.6.9rc1/apstools/plans/alignment.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/command_list.py` & `apstools-1.6.9rc1/apstools/plans/command_list.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/doc_run.py` & `apstools-1.6.9rc1/apstools/plans/doc_run.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/input_plan.py` & `apstools-1.6.9rc1/apstools/plans/input_plan.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/nscan_support.py` & `apstools-1.6.9rc1/apstools/plans/nscan_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/run_blocking_function_plan.py` & `apstools-1.6.9rc1/apstools/plans/run_blocking_function_plan.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/sscan_support.py` & `apstools-1.6.9rc1/apstools/plans/sscan_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/stage_sigs_support.py` & `apstools-1.6.9rc1/apstools/plans/stage_sigs_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/actions.xlsx` & `apstools-1.6.9rc1/apstools/plans/tests/actions.xlsx`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/demo3.xlsx` & `apstools-1.6.9rc1/apstools/plans/tests/demo3.xlsx`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_alignment.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_commandlist.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_commandlist.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_input_plan.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_input_plan.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_issue606.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_issue606.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_plans.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_plans.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_run_blocking_function_plan.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_run_blocking_function_plan.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/plans/tests/test_stage_sigs_support.py` & `apstools-1.6.9rc1/apstools/plans/tests/test_stage_sigs_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/__init__.py` & `apstools-1.6.9rc1/apstools/synApps/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/_common.py` & `apstools-1.6.9rc1/apstools/synApps/_common.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/asyn.py` & `apstools-1.6.9rc1/apstools/synApps/asyn.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/busy.py` & `apstools-1.6.9rc1/apstools/synApps/busy.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/calcout.py` & `apstools-1.6.9rc1/apstools/synApps/calcout.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/db_2slit.py` & `apstools-1.6.9rc1/apstools/synApps/db_2slit.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/epid.py` & `apstools-1.6.9rc1/apstools/synApps/epid.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/iocstats.py` & `apstools-1.6.9rc1/apstools/synApps/iocstats.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/luascript.py` & `apstools-1.6.9rc1/apstools/synApps/luascript.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/save_data.py` & `apstools-1.6.9rc1/apstools/synApps/save_data.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/scalcout.py` & `apstools-1.6.9rc1/apstools/synApps/scalcout.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/sscan.py` & `apstools-1.6.9rc1/apstools/synApps/sscan.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/sseq.py` & `apstools-1.6.9rc1/apstools/synApps/sseq.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/sub.py` & `apstools-1.6.9rc1/apstools/synApps/sub.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/swait.py` & `apstools-1.6.9rc1/apstools/synApps/swait.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_2slit.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_2slit.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_calcout.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_calcout.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_iocstats.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_iocstats.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_luascript.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_luascript.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_scalcout.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_scalcout.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_sseq.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_sseq.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_sub.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_sub.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/tests/test_swait.py` & `apstools-1.6.9rc1/apstools/synApps/tests/test_swait.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/synApps/transform.py` & `apstools-1.6.9rc1/apstools/synApps/transform.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/tests/__init__.py` & `apstools-1.6.9rc1/apstools/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/__init__.py` & `apstools-1.6.9rc1/apstools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/_core.py` & `apstools-1.6.9rc1/apstools/utils/_core.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/catalog.py` & `apstools-1.6.9rc1/apstools/utils/catalog.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/device_info.py` & `apstools-1.6.9rc1/apstools/utils/device_info.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/email.py` & `apstools-1.6.9rc1/apstools/utils/email.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/image_analysis.py` & `apstools-1.6.9rc1/apstools/utils/image_analysis.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/list_plans.py` & `apstools-1.6.9rc1/apstools/utils/list_plans.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/list_runs.py` & `apstools-1.6.9rc1/apstools/utils/list_runs.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/log_utils.py` & `apstools-1.6.9rc1/apstools/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/memory.py` & `apstools-1.6.9rc1/apstools/utils/memory.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/misc.py` & `apstools-1.6.9rc1/apstools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/override_parameters.py` & `apstools-1.6.9rc1/apstools/utils/override_parameters.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/plot.py` & `apstools-1.6.9rc1/apstools/utils/plot.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/profile_support.py` & `apstools-1.6.9rc1/apstools/utils/profile_support.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/pvregistry.py` & `apstools-1.6.9rc1/apstools/utils/pvregistry.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/query.py` & `apstools-1.6.9rc1/apstools/utils/query.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/slit_core.py` & `apstools-1.6.9rc1/apstools/utils/slit_core.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/spreadsheet.py` & `apstools-1.6.9rc1/apstools/utils/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_exceltable.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_exceltable.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_findpv.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_findpv.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_image_analysis.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_image_analysis.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_listdevice.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_listdevice.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_listplans.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_listplans.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_listruns_class.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_listruns_class.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_log_utils.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_log_utils.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_override_parameters.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_override_parameters.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools/utils/tests/test_utils.py` & `apstools-1.6.9rc1/apstools/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/apstools.egg-info/SOURCES.txt` & `apstools-1.6.9rc1/apstools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/environment.yml` & `apstools-1.6.9rc1/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   - aps-anl-tag
   - conda-forge
   - defaults
   # nsls2forge channel for newer mongoquery 1.3.6 (issue #673)
   - nsls2forge
 
 dependencies:
-  - python >=3.8, <=3.11
+  - python >=3.8, <3.11
   - area-detector-handlers
   - bluesky >=1.6.7
   - databroker =1.2.5
   - databroker-pack
   - h5py
   - intake
   - matplotlib-base
```

### Comparing `apstools-1.6.9/pyproject.toml` & `apstools-1.6.9rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/pytest.ini` & `apstools-1.6.9rc1/pytest.ini`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/resources/apstools_test.zip` & `apstools-1.6.9rc1/resources/apstools_test.zip`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/resources/usaxs_test.zip` & `apstools-1.6.9rc1/resources/usaxs_test.zip`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/setup.cfg` & `apstools-1.6.9rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `apstools-1.6.9/setup.py` & `apstools-1.6.9rc1/setup.py`

 * *Files identical despite different names*

