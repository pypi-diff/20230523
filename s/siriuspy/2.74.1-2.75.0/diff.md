# Comparing `tmp/siriuspy-2.74.1.tar.gz` & `tmp/siriuspy-2.75.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.74.1.tar", last modified: Mon May 15 15:30:00 2023, max compression
+gzip compressed data, was "siriuspy-2.75.0.tar", last modified: Tue May 23 19:09:19 2023, max compression
```

## Comparing `siriuspy-2.74.1.tar` & `siriuspy-2.75.0.tar`

### file list

```diff
@@ -1,389 +1,389 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.055994 siriuspy-2.74.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-05-15 15:29:51.000000 siriuspy-2.74.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-15 15:29:51.000000 siriuspy-2.74.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-15 15:30:00.055994 siriuspy-2.74.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-15 15:29:51.000000 siriuspy-2.74.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-15 15:29:51.000000 siriuspy-2.74.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 15:30:00.055994 siriuspy-2.74.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-05-15 15:29:51.000000 siriuspy-2.74.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.023994 siriuspy-2.74.1/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.023994 siriuspy-2.74.1/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.023994 siriuspy-2.74.1/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.027994 siriuspy-2.74.1/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.027994 siriuspy-2.74.1/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   122432 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.027994 siriuspy-2.74.1/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.027994 siriuspy-2.74.1/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.027994 siriuspy-2.74.1/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)     8382 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     9493 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    17596 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    28397 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.031994 siriuspy-2.74.1/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/diagsys/rfdiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.035994 siriuspy-2.74.1/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8294 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.039994 siriuspy-2.74.1/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    33182 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.043994 siriuspy-2.74.1/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-15 15:29:51.000000 siriuspy-2.74.1/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.023994 siriuspy-2.74.1/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9945 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-15 15:29:59.000000 siriuspy-2.74.1/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.047994 siriuspy-2.74.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.051994 siriuspy-2.74.1/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.055994 siriuspy-2.74.1/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.055994 siriuspy-2.74.1/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:30:00.055994 siriuspy-2.74.1/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-15 15:29:51.000000 siriuspy-2.74.1/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-05-23 19:09:08.000000 siriuspy-2.75.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-23 19:09:08.000000 siriuspy-2.75.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-23 19:09:19.874388 siriuspy-2.75.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-23 19:09:08.000000 siriuspy-2.75.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-23 19:09:08.000000 siriuspy-2.75.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 19:09:19.874388 siriuspy-2.75.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-05-23 19:09:08.000000 siriuspy-2.75.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.838384 siriuspy-2.75.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.838384 siriuspy-2.75.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14364 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9625 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17596 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29550 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7455 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13821 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/test_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34134 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9945 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.74.1/LICENSE` & `siriuspy-2.75.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/PKG-INFO` & `siriuspy-2.75.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.74.1
+Version: 2.75.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.74.1/README.md` & `siriuspy-2.75.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/setup.py` & `siriuspy-2.75.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/commands.py` & `siriuspy-2.75.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/constants.py` & `siriuspy-2.75.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/entities.py` & `siriuspy-2.75.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/exceptions.py` & `siriuspy-2.75.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/serial.py` & `siriuspy-2.75.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/bsmp/types.py` & `siriuspy-2.75.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/callbacks.py` & `siriuspy-2.75.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientarch/client.py` & `siriuspy-2.75.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientarch/devices.py` & `siriuspy-2.75.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientarch/exceptions.py` & `siriuspy-2.75.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientarch/pvarch.py` & `siriuspy-2.75.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientarch/time.py` & `siriuspy-2.75.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/_templates.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,14 +354,23 @@
     ['BO-Fam:TI-BPM:NrPulses-SP', 0, 0.0],
     ['BO-Fam:TI-BPM:Polarity-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:Src-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:State-Sel', 0, 0.0],
     ['BO-Fam:TI-BPM:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['BO-Fam:TI-BPM:LowLvlLock-Sel', 0, 0.0],
 
+    ['BO-Glob:TI-LLRF-Gen:DelayRaw-SP', 0, 0],
+    ['BO-Glob:TI-LLRF-Gen:WidthRaw-SP', 0, 0.0],
+    ['BO-Glob:TI-LLRF-Gen:NrPulses-SP', 0, 0.0],
+    ['BO-Glob:TI-LLRF-Gen:Polarity-Sel', 0, 0.0],
+    ['BO-Glob:TI-LLRF-Gen:Src-Sel', 0, 0.0],
+    ['BO-Glob:TI-LLRF-Gen:State-Sel', 0, 0.0],
+    ['BO-Glob:TI-LLRF-Gen:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['BO-Glob:TI-LLRF-Gen:LowLvlLock-Sel', 0, 0.0],
+
     ['BO-Glob:TI-LLRF-PsMtn:DelayRaw-SP', 0, 0],
     ['BO-Glob:TI-LLRF-PsMtn:WidthRaw-SP', 0, 0.0],
     ['BO-Glob:TI-LLRF-PsMtn:NrPulses-SP', 0, 0.0],
     ['BO-Glob:TI-LLRF-PsMtn:Polarity-Sel', 0, 0.0],
     ['BO-Glob:TI-LLRF-PsMtn:Src-Sel', 0, 0.0],
     ['BO-Glob:TI-LLRF-PsMtn:State-Sel', 0, 0.0],
     ['BO-Glob:TI-LLRF-PsMtn:DeltaDelayRaw-SP', 30*[0, ], 0],
@@ -709,14 +718,23 @@
     ['SI-Glob:TI-BbBProcV-Trig2:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-BbBProcV-Trig2:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-BbBProcV-Trig2:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-BbBProcV-Trig2:State-Sel', 0, 0.0],
     ['SI-Glob:TI-BbBProcV-Trig2:DeltaDelayRaw-SP', 30*[0, ], 0],
     ['SI-Glob:TI-BbBProcV-Trig2:LowLvlLock-Sel', 0, 0.0],
 
+    ['SI-Glob:TI-LLRF-Gen:DelayRaw-SP', 0, 0],
+    ['SI-Glob:TI-LLRF-Gen:WidthRaw-SP', 0, 0.0],
+    ['SI-Glob:TI-LLRF-Gen:NrPulses-SP', 0, 0.0],
+    ['SI-Glob:TI-LLRF-Gen:Polarity-Sel', 0, 0.0],
+    ['SI-Glob:TI-LLRF-Gen:Src-Sel', 0, 0.0],
+    ['SI-Glob:TI-LLRF-Gen:State-Sel', 0, 0.0],
+    ['SI-Glob:TI-LLRF-Gen:DeltaDelayRaw-SP', 30*[0, ], 0],
+    ['SI-Glob:TI-LLRF-Gen:LowLvlLock-Sel', 0, 0.0],
+
     ['SI-Glob:TI-LLRF-PsMtn:DelayRaw-SP', 0, 0],
     ['SI-Glob:TI-LLRF-PsMtn:WidthRaw-SP', 0, 0.0],
     ['SI-Glob:TI-LLRF-PsMtn:NrPulses-SP', 0, 0.0],
     ['SI-Glob:TI-LLRF-PsMtn:Polarity-Sel', 0, 0.0],
     ['SI-Glob:TI-LLRF-PsMtn:Src-Sel', 0, 0.0],
     ['SI-Glob:TI-LLRF-PsMtn:State-Sel', 0, 0.0],
     ['SI-Glob:TI-LLRF-PsMtn:DeltaDelayRaw-SP', 30*[0, ], 0],
```

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/clientweb/implementation.py` & `siriuspy-2.75.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/csdev.py` & `siriuspy-2.75.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/currinfo/csdev.py` & `siriuspy-2.75.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.75.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/currinfo/main.py` & `siriuspy-2.75.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/__init__.py` & `siriuspy-2.75.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.75.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/conn.py` & `siriuspy-2.75.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.75.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.75.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/main.py` & `siriuspy-2.75.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/cycle/util.py` & `siriuspy-2.75.0/siriuspy/cycle/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/__init__.py` & `siriuspy-2.75.0/siriuspy/devices/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 from .lillrf import LILLRF, DevLILLRF
 from .machshift import MachShift
 from .modltr import LIModltr
 from .orbit_interlock import BPMOrbitIntlk, BaseOrbitIntlk, OrbitInterlock
 from .posang import PosAng
 from .psconv import PSProperty, StrengthConv
 from .pssofb import PSCorrSOFB, PSApplySOFB
-from .pwrsupply import PowerSupply, PowerSupplyPU, PowerSupplyFC
+from .pwrsupply import PowerSupply, PowerSupplyPU, PowerSupplyFC, \
+    PowerSupplyFBP
 from .rf import RFGen, ASLLRF, BORFCavMonitor, SIRFCavMonitor, RFCav, \
     RFKillBeam
 from .screen import Screen
 from .sofb import SOFB
 from .syncd import DevicesSync
 from .timing import EVG, Event, Trigger, HLTiming
 from .tune import TuneFrac, TuneProc, Tune, TuneCorr
-from .dvf import DVF
+from .dvf import DVF, DVFImgProc
 from .lienergy import LIEnergy
 
 
 del device, bpm, dcct, egun, ict, lillrf, modltr
 del pwrsupply, posang, psconv, pssofb, rf, injsys, injctrl
 del screen, tune, sofb, timing, syncd, energy
 del ids, currinfo, bbb, machshift, dvf, lienergy
```

### Comparing `siriuspy-2.74.1/siriuspy/devices/bbb.py` & `siriuspy-2.75.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/bpm.py` & `siriuspy-2.75.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/currinfo.py` & `siriuspy-2.75.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/dcct.py` & `siriuspy-2.75.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/device.py` & `siriuspy-2.75.0/siriuspy/devices/device.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/egun.py` & `siriuspy-2.75.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/energy.py` & `siriuspy-2.75.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/fofb.py` & `siriuspy-2.75.0/siriuspy/devices/fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/ict.py` & `siriuspy-2.75.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/idff.py` & `siriuspy-2.75.0/siriuspy/devices/idff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Insertion Devices Feedforward Devices."""
 
 from ..namesys import SiriusPVName as _SiriusPVName
 from ..search import IDSearch as _IDSearch
 from ..idff.config import IDFFConfig as _IDFFConfig
 
 from .device import Device as _Device, Devices as _Devices
-from .pwrsupply import PowerSupply as _PowerSupply
+from .pwrsupply import PowerSupplyFBP as _PowerSupplyFBP
 from .ids import WIG as _WIG, APU as _APU, EPU as _EPU
 
 
 class IDFF(_Devices):
     """Insertion Device Feedforward Device."""
 
     class DEVICES:
@@ -224,29 +224,31 @@
     def get_polarization_state(
             self, pparameter_value=None, kparameter_value=None):
         """."""
         if pparameter_value is None:
             pparameter_value = self.pparameter_mon
         if kparameter_value is None:
             kparameter_value = self.kparameter_mon
+        if None in (pparameter_value, kparameter_value):
+            return None, pparameter_value, kparameter_value
         polarization = self.idffconfig.get_polarization_state(
             pparameter=pparameter_value, kparameter=kparameter_value)
         return polarization, pparameter_value, kparameter_value
 
     def _create_devices(self, devname):
         param_auto_mon = False
         devpp = _Device(
             devname=devname,
             properties=(self._pparametername, ), auto_mon=param_auto_mon)
         devkp = _Device(
             devname=devname,
             properties=(self._kparametername, ), auto_mon=param_auto_mon)
-        devsch = [_PowerSupply(devname=dev) for dev in self.chnames]
-        devscv = [_PowerSupply(devname=dev) for dev in self.cvnames]
-        devsqs = [_PowerSupply(devname=dev) for dev in self.qsnames]
+        devsch = [_PowerSupplyFBP(devname=dev) for dev in self.chnames]
+        devscv = [_PowerSupplyFBP(devname=dev) for dev in self.cvnames]
+        devsqs = [_PowerSupplyFBP(devname=dev) for dev in self.qsnames]
 
         return devpp, devkp, devsch, devscv, devsqs
 
 
 class WIGIDFF(IDFF):
     """Wiggler Feedforward."""
```

### Comparing `siriuspy-2.74.1/siriuspy/devices/ids.py` & `siriuspy-2.75.0/siriuspy/devices/ids.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/injctrl.py` & `siriuspy-2.75.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/injsys.py` & `siriuspy-2.75.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/lienergy.py` & `siriuspy-2.75.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/lillrf.py` & `siriuspy-2.75.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/machshift.py` & `siriuspy-2.75.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/modltr.py` & `siriuspy-2.75.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.75.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/posang.py` & `siriuspy-2.75.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/psconv.py` & `siriuspy-2.75.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/pssofb.py` & `siriuspy-2.75.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/pstesters.py` & `siriuspy-2.75.0/siriuspy/devices/pstesters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/pwrsupply.py` & `siriuspy-2.75.0/siriuspy/devices/pwrsupply.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         'Wfm-SP', 'Wfm-RB', 'WfmRef-Mon', 'Wfm-Mon',
         'CycleFreq-SP', 'CycleFreq-RB',
         'CycleAmpl-SP', 'CycleAmpl-RB',
         'CycleOffset-SP', 'CycleOffset-RB',
         'CycleAuxParam-SP', 'CycleAuxParam-RB',
         'CycleEnbl-Mon',
     )
+    _properties_fbp = _properties_magps + (
+        'SOFBMode-Sel', 'SOFBMode-Sts'
+        )
     _properties_fc = (
         'AlarmsAmp-Mon', 'OpMode-Sel', 'OpMode-Sts',
         'CurrLoopKp-RB', 'CurrLoopKp-SP', 'CurrLoopTi-RB', 'CurrLoopTi-SP',
         'CurrLoopMode-Sts', 'CurrLoopMode-Sel',
         'CurrGain-RB', 'CurrGain-SP', 'CurrOffset-RB', 'CurrOffset-SP',
         'Current-RB', 'Current-SP', 'Current-Mon', 'CurrentRef-Mon',
         'TestLimA-RB', 'TestLimA-SP', 'TestLimB-RB', 'TestLimB-SP',
@@ -77,15 +80,15 @@
         # check if device exists
         if devname not in _PSSearch.get_psnames():
             raise NotImplementedError(devname)
 
         # power supply type and magnetic function
         (self._pstype, self._psmodel, self._magfunc,
          self._strength_propty, self._strength_units,
-         self._is_linac, self._is_pulsed, self._is_fc,
+         self._is_linac, self._is_pulsed, self._is_fc, self._is_fbp,
          self._is_magps) = _PSDev.get_device_type(devname)
 
         # set attributes
         (self._strength_sp_propty,
          self._strength_rb_propty,
          self._strength_mon_propty,
          properties) = self._set_attributes_properties(devname)
@@ -235,18 +238,19 @@
         psmodel = _PSSearch.conv_psname_2_psmodel(devname)
         magfunc = _PSSearch.conv_psname_2_magfunc(devname)
         strength_propty = _util.get_strength_label(magfunc)
         strength_units = _util.get_strength_units(magfunc, pstype)
         is_linac = devname.sec.endswith('LI')
         is_pulsed = devname.dis == 'PU'
         is_fc = devname.dev == 'FCH' or devname.dev == 'FCV'
-        is_magps = not is_linac and not is_pulsed and not is_fc
+        is_fbp = psmodel == 'FBP'
+        is_magps = not is_linac and not is_pulsed and not is_fc and not is_fbp
         return (pstype, psmodel, magfunc,
                 strength_propty, strength_units,
-                is_linac, is_pulsed, is_fc, is_magps)
+                is_linac, is_pulsed, is_fc, is_fbp, is_magps)
 
     # --- private methods ---
 
     def _set_attributes_properties(self, devname):
 
         properties = _PSDev._properties_common
         if self._is_linac:
@@ -257,14 +261,16 @@
                 properties += _PSDev._properties_pulsed_kckr
             else:
                 properties += _PSDev._properties_pulsed_sept
             if 'NLKckr' in devname:
                 properties += _PSDev._properties_pulsed_nlkckr
         elif self._is_fc:
             properties += _PSDev._properties_fc
+        elif self._is_fbp:
+            properties += _PSDev._properties_fbp
         else:
             properties += _PSDev._properties_magps
 
         # strength properties
         strength_sp_propty = self._strength_propty + '-SP'
         strength_rb_propty = self._strength_propty + '-RB'
         strength_mon_propty = self._strength_propty + '-Mon'
@@ -964,7 +970,34 @@
     def fofbacc_satmin(self, value):
         self['FOFBAccSatMin-SP'] = value
 
     def cmd_fofbacc_clear(self):
         """Command to clear FOFB accumulator."""
         self['FOFBAccClear-Cmd'] = 1
         return True
+
+
+class PowerSupplyFBP(PowerSupply):
+    """FBP Power Supply Device."""
+
+    SOFBMODE_SEL = _Const.DsblEnbl
+    SOFBMODE_STS = _Const.DsblEnbl
+
+    @property
+    def sofbmode(self):
+        """SOFB mode status."""
+        return self['SOFBMode-Sts']
+
+    def cmd_sofbmode_enable(self, timeout=_PSDev._default_timeout):
+        """Command to enable SOFBMode. Send command and wait."""
+        return self._cmd_sofbmode(
+            timeout, self.SOFBMODE_SEL.Enbl, self.SOFBMODE_STS.Enbl)
+
+    def cmd_sofbmode_disable(self, timeout=_PSDev._default_timeout):
+        """Command to disable SOFBMode. Send command and wait."""
+        return self._cmd_sofbmode(
+            timeout, self.SOFBMODE_SEL.Dsbl, self.SOFBMODE_STS.Dsbl)
+
+    def _cmd_sofbmode(self, timeout, state_sel, state_sts):
+        self['SOFBMode-Sel'] = state_sel
+        return self._wait(
+            'SOFBMode-Sts', state_sts, timeout=timeout)
```

### Comparing `siriuspy-2.74.1/siriuspy/devices/rf.py` & `siriuspy-2.75.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/screen.py` & `siriuspy-2.75.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/sofb.py` & `siriuspy-2.75.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/syncd.py` & `siriuspy-2.75.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/timing.py` & `siriuspy-2.75.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/devices/tune.py` & `siriuspy-2.75.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.75.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.75.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.75.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.75.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.75.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/app.py` & `siriuspy-2.75.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.75.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.75.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.75.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.75.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.75.0/siriuspy/diagsys/psdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.75.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.75.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.75.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.75.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/pvs.py` & `siriuspy-2.75.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/envars.py` & `siriuspy-2.75.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/epics/multiproc.py` & `siriuspy-2.75.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/epics/properties.py` & `siriuspy-2.75.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/epics/pv_fake.py` & `siriuspy-2.75.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.75.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/fofb/csdev.py` & `siriuspy-2.75.0/siriuspy/fofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/fofb/main.py` & `siriuspy-2.75.0/siriuspy/fofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/idff/config.py` & `siriuspy-2.75.0/siriuspy/idff/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             raise ValueError('No IDFF configuration defined.')
         for pol, val in poldefs.items():
             if pol == 'none':
                 continue
             if abs(pparameter - val) < PPARAM_TOL:
                 return pol
         if abs(kparameter - poldefs['none']) < KPARAM_TOL:
-                return 'none'
+            return 'none'
         return 'not_defined'
 
     def check_valid_value(self, value):
         """."""
         if not super().check_valid_value(value):
             return False
         for pol, table in value['polarizations'].items():
```

### Comparing `siriuspy-2.74.1/siriuspy/idff/csdev.py` & `siriuspy-2.75.0/siriuspy/idff/csdev.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,26 +8,32 @@
 
 # --- Enumeration Types ---
 
 class ETypes(_csdev.ETypes):
     """Local enumerate types."""
 
     OPEN_CLOSED = ('Open', 'Closed')
+    STS_LBLS_CORR = (
+        'Connected', 'PwrStateOn', 'OpModeConfigured',
+        'SOFBModeConfigured')
 
 
 _et = ETypes
 
 
 # --- Const class ---
 
 class IDFFConst(_csdev.Const):
     """ID Feedforward Const class."""
 
     LoopState = _csdev.Const.register('LoopState', _et.OPEN_CLOSED)
-    DEFAULT_LOOP_FREQ = 5  # Hz
+    StsLblsCorr = _csdev.Const.register(
+        'StsLblsCorr', _et.STS_LBLS_CORR)
+
+    DEFAULT_LOOP_FREQ = 5  # [Hz]
 
     def __init__(self, idname):
         """Init."""
         self.idname = _PVName(idname)
         self.idffname = 'SI-' + self.idname.sub + ':AP-IDFF'
         ioc_fol = _os.path.join(
             '/home', 'sirius', 'iocs-log', 'si-ap-idff', 'data')
@@ -64,10 +70,21 @@
                 'value': self.DsblEnbl.Enbl,
                 'unit': 'If QS are included in loop'},
 
             'Polarization-Mon': {'type': 'string', 'value': 'none'},
 
             'ConfigName-SP': {'type': 'string', 'value': ''},
             'ConfigName-RB': {'type': 'string', 'value': ''},
+            'SOFBMode-Sel': {
+                'type': 'enum', 'enums': _et.DSBL_ENBL,
+                'value': self.DsblEnbl.Dsbl, 'unit': 'sofbmode'},
+            'SOFBMode-Sts': {
+                'type': 'enum', 'enums': _et.DSBL_ENBL,
+                'value': self.DsblEnbl.Dsbl, 'unit': 'sofbmode'},
+            'CorrConfig-Cmd': {'type': 'int', 'value': 0},
+            'CorrStatus-Mon': {'type': 'int', 'value': 0b1111},
+            'CorrStatusLabels-Cte': {
+                'type': 'string', 'count': len(self.StsLblsCorr._fields),
+                'value': self.StsLblsCorr._fields}
         }
         dbase = _csdev.add_pvslist_cte(dbase)
         return dbase
```

### Comparing `siriuspy-2.74.1/siriuspy/idff/main.py` & `siriuspy-2.75.0/siriuspy/stabinfo/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,99 @@
-"""ID feedforward App."""
+"""Beam stability info App."""
 
 import os as _os
 import logging as _log
 import time as _time
+from functools import partial as _part
 import epics as _epics
 
+import numpy as _np
+
+from ..epics import PV as _PV
 from ..callbacks import Callback as _Callback
-from ..devices import IDFF as _IDFF
+from ..envars import VACA_PREFIX as _vaca_prefix
+from ..namesys import SiriusPVName as _PVName
+from ..devices import Device as _Device
 
-from .csdev import IDFFConst as _Const, ETypes as _ETypes
+from .csdev import StabInfoConst as _Const
 
 
 class App(_Callback):
     """Main application for handling machine shift."""
 
-    def __init__(self, idname):
+    SCAN_FREQUENCY = 2  # [Hz]
+
+    def __init__(self):
         """Class constructor."""
         super().__init__()
-        self._const = _Const(idname)
-        self._pvs_prefix = self._const.idffname
+        self._const = _Const()
         self._pvs_database = self._const.get_propty_database()
 
-        self._loop_state = _Const.DsblEnbl.Dsbl
-        self._loop_freq = _Const.DEFAULT_LOOP_FREQ
-        self._control_qs = _Const.DsblEnbl.Dsbl
-        self._polarization = 'none'
-        self._config_name = ''
+        self._bbbh_oscamp = 0
+        self._bbbv_oscamp = 0
+        self._bbbl_oscamp = 0
+        self._bbbh_oscamp_thres = self._const.BBBH_OSCAMP_THRES
+        self._bbbv_oscamp_thres = self._const.BBBV_OSCAMP_THRES
+        self._bbbl_oscamp_thres = self._const.BBBL_OSCAMP_THRES
+        self._bbbh_status = self._const.StabUnstab.Stable
+        self._bbbv_status = self._const.StabUnstab.Stable
+        self._bbbl_status = self._const.StabUnstab.Stable
+        self._bbbh_calibfactor = self._const.DEF_BBBH_CALIBFACTOR
+        self._bbbv_calibfactor = self._const.DEF_BBBV_CALIBFACTOR
+        self._bbbl_calibfactor = self._const.DEF_BBBL_CALIBFACTOR
         self.read_autosave_file()
 
-        self._idff = _IDFF(idname)
-
-        self._load_config(self._config_name)
+        # connections
+        # use pyepics recommendations for threading
+        _epics.ca.use_initial_context()
+
+        self._dev_bbb = dict()
+        bbbprops = ['SRAM_PEAK1', ]
+        for plane in ['H', 'V', 'L']:
+            devname = 'SI-Glob:DI-BbBProc-'+plane
+            self._dev_bbb[plane] = _Device(devname, properties=bbbprops)
+
+        sicurrent_pvname = _PVName(
+            'SI-Glob:AP-CurrInfo:Current-Mon').substitute(
+                prefix=_vaca_prefix)
+        self.si_current_pv = _PV(sicurrent_pvname, connection_timeout=0.05)
 
         # pvs to write methods
         self.map_pv2write = {
-            'LoopState-Sel': self.set_loop_state,
-            'LoopFreq-SP': self.set_loop_freq,
-            'ControlQS-Sel': self.set_control_qs,
-            'ConfigName-SP': self.set_config_name,
+            'BbBHCalibFactor-SP': _part(self.set_bbbcalibfactor, 'h'),
+            'BbBVCalibFactor-SP': _part(self.set_bbbcalibfactor, 'v'),
+            'BbBLCalibFactor-SP': _part(self.set_bbbcalibfactor, 'l'),
         }
 
         self.quit = False
-        self._thread_ff = _epics.ca.CAThread(
-            target=self._do_ff, daemon=True)
-        self._thread_ff.start()
+        self.scanning = False
+        self._thread_update = _epics.ca.CAThread(
+            target=self._update_pvs, daemon=True)
+        self._thread_update.start()
 
     def init_database(self):
         """Set initial PV values."""
-        pvn2vals = {
-            'LoopState-Sel': self._loop_state,
-            'LoopState-Sts': self._loop_state,
-            'LoopFreq-SP': self._loop_freq,
-            'LoopFreq-RB': self._loop_freq,
-            'ControlQS-Sel': self._control_qs,
-            'ControlQS-Sts': self._control_qs,
-            'ConfigName-SP': self._config_name,
-            'ConfigName-RB': self._config_name,
-            'Polarization-Mon': self._polarization,
-        }
-        for pvn, val in pvn2vals.items():
-            self.run_callbacks(pvn, val)
+        self.run_callbacks('BbBHCalibFactor-SP', self._bbbh_calibfactor)
+        self.run_callbacks('BbBHCalibFactor-RB', self._bbbh_calibfactor)
+        self.run_callbacks('BbBHOscAmp-Mon', self._bbbh_oscamp)
+        self.run_callbacks('BbBHOscAmpThres-Cte', self._bbbh_oscamp_thres)
+        self.run_callbacks('BbBHStatus-Mon', self._bbbh_status)
+        self.run_callbacks('BbBVCalibFactor-SP', self._bbbv_calibfactor)
+        self.run_callbacks('BbBVCalibFactor-RB', self._bbbv_calibfactor)
+        self.run_callbacks('BbBVOscAmp-Mon', self._bbbv_oscamp)
+        self.run_callbacks('BbBVOscAmpThres-Cte', self._bbbv_oscamp_thres)
+        self.run_callbacks('BbBVStatus-Mon', self._bbbv_status)
+        self.run_callbacks('BbBLCalibFactor-SP', self._bbbl_calibfactor)
+        self.run_callbacks('BbBLCalibFactor-RB', self._bbbl_calibfactor)
+        self.run_callbacks('BbBLOscAmp-Mon', self._bbbl_oscamp)
+        self.run_callbacks('BbBLOscAmpThres-Cte', self._bbbl_oscamp_thres)
+        self.run_callbacks('BbBLStatus-Mon', self._bbbl_status)
         self._update_log('Started.')
 
     @property
-    def pvs_prefix(self):
-        """Return pvs_prefix."""
-        return self._pvs_prefix
-
-    @property
     def pvs_database(self):
         """Return pvs_database."""
         return self._pvs_database
 
     def process(self, interval):
         """Sleep."""
         _time.sleep(interval)
@@ -88,63 +110,19 @@
             status = self.map_pv2write[reason](value)
             _log.info('%s Write for: %s --> %s',
                       str(status).upper(), reason, str(value))
             return status
         _log.warning('PV %s does not have a set function.', reason)
         return False
 
-    def set_loop_state(self, value):
-        """Set loop state."""
-        if not 0 <= value < len(_ETypes.OPEN_CLOSED):
-            return False
-        self._loop_state = value
-        act = ('En' if value else 'Dis')
-        self._update_log(f'Feedforward loop {act}abled.')
-        self.run_callbacks('LoopState-Sts', value)
-        return True
-
-    def set_loop_freq(self, value):
-        """Set loop frequency."""
-        if not 1e-3 <= value < 60:
-            return False
-        self._loop_freq = value
-        self._update_log(f'Loop frequency updated to {value:.2f}Hz.')
-        self.run_callbacks('LoopFreq-RB', value)
-        return True
-
-    def set_control_qs(self, value):
-        """Set whether to include QS or not in feedforward."""
-        if not 0 <= value < len(_ETypes.DSBL_ENBL):
-            return False
-        self._control_qs = value
-        act = ('En' if value else 'Dis')
-        self._update_log(f'{act}abled QS control.')
-        self.run_callbacks('ControlQS-Sts', value)
-        return True
-
-    def set_config_name(self, value):
-        """Set configuration name."""
-        if self._loop_state == self._const.LoopState.Closed:
-            self._update_log('ERR:Open loop before changing configuration.')
-            return False
-
-        if not self._load_config(value):
-            return False
-
-        self._config_name = value
-        self.run_callbacks('ConfigName-RB', value)
-        return True
-
-    def _load_config(self, config_name):
-        try:
-            self._idff.load_config(config_name)
-            self._update_log(f'Updated configuration: {config_name}.')
-        except ValueError as err:
-            self._update_log('ERR:'+str(err))
-            return False
+    def set_bbbcalibfactor(self, plane, value):
+        """Set BbB calibration factor."""
+        setattr(self, '_bbb'+plane+'_calibfactor', value)
+        self.run_callbacks('BbB'+plane.upper()+'CalibFactor-RB', value)
+        self.update_autosave_file()
         return True
 
     #  ----- log auxiliary methods -----
 
     def _update_log(self, msg):
         if 'ERR' in msg:
             _log.error(msg[4:])
@@ -154,99 +132,77 @@
             _log.warning(msg[5:])
         else:
             _log.info(msg)
         self.run_callbacks('Log-Mon', msg)
 
     # ----- auto save methods -----
 
+    @property
+    def auto_save_data(self):
+        """Data to be saved in autosave file."""
+        data = [
+            self._bbbh_calibfactor,
+            self._bbbv_calibfactor,
+            self._bbbl_calibfactor,
+            ]
+        return _np.array(data)
+
     def read_autosave_file(self):
         """Read autosave file."""
         filename = self._const.autosave_fname
-        config_name = None
+        data = None
         if _os.path.isfile(filename):
-            with open(filename, 'r') as fil:
-                config_name = fil.read().strip('\n')
-        if config_name is not None:
-            self._config_name = config_name
+            data = _np.loadtxt(filename)
+        if data is not None:
+            bbbh, bbbv, bbbl = data
+            self._bbbh_calibfactor = bbbh
+            self._bbbv_calibfactor = bbbv
+            self._bbbl_calibfactor = bbbl
         else:
             _log.info(
-                'No backup file was found, default value '
-                'was used for si_idff configuration name.')
-            self._config_name = self._get_default_configname()
+                'No backup file was found, default values '
+                'were used for calibration factors.')
             self.update_autosave_file()
             _log.info('First autosave file was created.')
 
     def update_autosave_file(self):
         """Update autosave file."""
         path = _os.path.split(self._const.autosave_fname)[0]
         _os.makedirs(path, exist_ok=True)
-        with open(self._const.autosave_fname, 'w+') as fil:
-            fil.write(self._config_name)
-
-    def _get_default_configname(self):
-        if self._const.idname.dev == 'EPU50':
-            return 'epu50_ref'
-        return ''
+        _np.savetxt(
+            self._const.autosave_fname, self.auto_save_data)
 
     # ----- update pvs methods -----
 
-    def _do_sleep(self, time0, tplanned):
-        ttook = _time.time() - time0
-        tsleep = tplanned - ttook
-        if tsleep > 0:
-            _time.sleep(tsleep)
-        else:
-            _log.warning(
-                'Feedforward step took more than planned... '
-                '{0:.3f}/{1:.3f} s'.format(ttook, tplanned))
-
-    def _do_update_polarization(self):
-        new_pol, *_ = self._idff.get_polarization_state()
-        if new_pol != self._polarization:
-            self._polarization = new_pol
-            self.run_callbacks('Polarization-Mon', new_pol)
-
-    def _do_update_correctors(self):
-        corrs = None
-        if self._control_qs == self._const.DsblEnbl.Dsbl:
-            corrs = self._idff.chdevs + self._idff.cvdevs
-        try:
-            # ret = self._idff.calculate_setpoints()
-            # setpoints, polarization, *parameters = ret
-            # pparameter_value, kparameter_value = parameters
-            # print('pparameter: ', pparameter_value)
-            # print('kparameter: ', kparameter_value)
-            # print('polarization: ', polarization)
-            # print('setpoints: ', setpoints)
-            # print()
-            self._idff.implement_setpoints(corrdevs=corrs)
-        except ValueError as err:
-            self._update_log('ERR:'+str(err))
-
-    def _do_ff(self):
-        # updating loop
+    def _update_pvs(self):
+        tplanned = 1.0/App.SCAN_FREQUENCY
         while not self.quit:
-            # updating interval
-            tplanned = 1.0/self._loop_freq
-
-            # initial time
-            _t0 = _time.time()
-
-            # check IDFF device connection
-            if not self._idff.connected:
-                self._update_log('ERR: IDFF device is disconnected.')
-                self._do_sleep(_t0, tplanned)
+            if not self.scanning:
+                _time.sleep(tplanned)
                 continue
 
-            # update polarization state
-            self._do_update_polarization()
-
-            # return if loop is not closed
-            if not self._loop_state:
-                self._do_sleep(_t0, tplanned)
-                continue
-
-            # correctors setpoint implementation
-            self._do_update_correctors()
+            _t0 = _time.time()
 
-            # sleep unused time or signal overtime to stdout
-            self._do_sleep(_t0, tplanned)
+            pvcurr = self.si_current_pv
+            if pvcurr.connected and pvcurr.value is not None:
+                curr = pvcurr.value
+                for pln in ['H', 'V', 'L']:
+                    dev = self._dev_bbb[pln]
+                    harmn = self._const.SI_HARMNUM
+                    calib = getattr(self, '_bbb'+pln.lower()+'_calibfactor')
+                    thres = getattr(self, '_bbb'+pln.lower()+'_oscamp_thres')
+                    cthres = self._const.CURR_THRES
+                    oscamp_db = dev['SRAM_PEAK1']
+                    if oscamp_db is not None:
+                        oscamp_phy = 10**(oscamp_db/20) * harmn / curr / calib
+                        self.run_callbacks('BbB'+pln+'OscAmp-Mon', oscamp_phy)
+                        status = curr > cthres and oscamp_phy > thres
+                        self.run_callbacks('BbB'+pln+'Status-Mon', int(status))
+
+            ttook = _time.time() - _t0
+            tsleep = tplanned - ttook
+            if tsleep > 0:
+                _time.sleep(tsleep)
+            else:
+                _log.warning(
+                    'Update loop took more than planned... '
+                    '{0:.3f}/{1:.3f} s'.format(ttook, tplanned))
```

### Comparing `siriuspy-2.74.1/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.75.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/injctrl/csdev.py` & `siriuspy-2.75.0/siriuspy/injctrl/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/injctrl/main.py` & `siriuspy-2.75.0/siriuspy/injctrl/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/csdev.py` & `siriuspy-2.75.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/macreport.py` & `siriuspy-2.75.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/macschedule.py` & `siriuspy-2.75.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/main.py` & `siriuspy-2.75.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/test_macreport.py` & `siriuspy-2.75.0/siriuspy/machshift/test_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/machshift/utils.py` & `siriuspy-2.75.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/magnet/data.py` & `siriuspy-2.75.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/magnet/excdata.py` & `siriuspy-2.75.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/magnet/factory.py` & `siriuspy-2.75.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/magnet/normalizer.py` & `siriuspy-2.75.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/magnet/util.py` & `siriuspy-2.75.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/csdev.py` & `siriuspy-2.75.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.75.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/liemit/main.py` & `siriuspy-2.75.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.75.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/lienergy/main.py` & `siriuspy-2.75.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/meas/util.py` & `siriuspy-2.75.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/namesys/implementation.py` & `siriuspy-2.75.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/optics/lattice_survey.py` & `siriuspy-2.75.0/siriuspy/optics/lattice_survey.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/base.py` & `siriuspy-2.75.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/chrom.py` & `siriuspy-2.75.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/csdev.py` & `siriuspy-2.75.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.75.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/tune.py` & `siriuspy-2.75.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/opticscorr/utils.py` & `siriuspy-2.75.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.75.0/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.75.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/posang/csdev.py` & `siriuspy-2.75.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/posang/main.py` & `siriuspy-2.75.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/posang/utils.py` & `siriuspy-2.75.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/data.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/factory.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/pssofb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import numpy as _np
 from epics import get_pv as _get_pv
 from socket import timeout as _socket_timeout
 
 from ..thread import AsyncWorker as _AsyncWorker
 from ..search import PSSearch as _PSSearch
+from ..search import IDSearch as _IDSearch
 from ..bsmp import SerialError as _SerialError
 from ..bsmp import constants as _const_bsmp
 from ..devices import StrengthConv as _StrengthConv
 from ..epics import CAProcessSpawn as _Process
 
 from .bsmp.constants import ConstFBP as _const_fbp
 from .bsmp.constants import UDC_MAX_NR_DEV as _UDC_MAX_NR_DEV
@@ -40,32 +41,56 @@
     """."""
 
     _sofb = dict()
     _sofb_factory = None
 
     @staticmethod
     def get_psnames_ch(acc):
-        """Return horizontal corrector psnames of a given sector."""
+        """Return horizontal corrector psnames of a given sector/ID."""
+        if 'ID-' in acc:
+            return _IDSearch.conv_idname_2_idff_chnames(acc)
         if PSNamesSOFB._sofb_factory is None:
             from ..sofb.csdev import SOFBFactory
             PSNamesSOFB._sofb_factory = SOFBFactory
         if acc not in PSNamesSOFB._sofb:
             PSNamesSOFB._sofb[acc] = PSNamesSOFB._sofb_factory.create(acc)
         return PSNamesSOFB._sofb[acc].ch_names
 
     @staticmethod
     def get_psnames_cv(acc):
-        """Return vertical corrector psnames of a given sector."""
+        """Return vertical corrector psnames of a given sector/ID."""
+        if 'ID-' in acc:
+            return _IDSearch.conv_idname_2_idff_cvnames(acc)
         if PSNamesSOFB._sofb_factory is None:
             from ..sofb.csdev import SOFBFactory
             PSNamesSOFB._sofb_factory = SOFBFactory
         if acc not in PSNamesSOFB._sofb:
             PSNamesSOFB._sofb[acc] = PSNamesSOFB._sofb_factory.create(acc)
         return PSNamesSOFB._sofb[acc].cv_names
 
+    @staticmethod
+    def get_psnames_qs(acc):
+        """Return skew corrector psnames of a ID."""
+        if 'ID-' in acc:
+            return _IDSearch.conv_idname_2_idff_qsnames(acc)
+        return []
+
+    @staticmethod
+    def get_bbbnames(acc):
+        """Return bbbnames."""
+        corrnames = \
+            PSNamesSOFB.get_psnames_ch(acc) + \
+            PSNamesSOFB.get_psnames_cv(acc) + \
+            PSNamesSOFB.get_psnames_qs(acc)
+        bbbnames = set()
+        for corrname in corrnames:
+            bbbname = _PSSearch.conv_psname_2_bbbname(corrname)
+            bbbnames.add(bbbname)
+        return list(bbbnames)
+
 
 class UnitConverter:
     """."""
 
     DIPOLE_PROPTY = 'Ref-Mon'
 
     def __init__(self, psnames, dipoleoff=False):
@@ -145,35 +170,36 @@
     PS_PWRSTATE = _PSCStatus.PWRSTATE
     PS_OPMODE = _PSCStatus.OPMODE
     SOCKET_TIMEOUT_ERR = 255
     SERIAL_ERR = 254
 
     def __init__(
             self, ethbridgeclnt_class, bbbnames=None, mproc=None,
-            sofb_update_iocs=False, dipoleoff=False):
+            sofb_update_iocs=False, dipoleoff=False, acc=None):
         """."""
         # check arguments
         if mproc is not None and \
                 (not isinstance(mproc, dict) or
                  set(mproc.keys()) != {'rbref', 'ref', 'fret'}):
             raise ValueError('Invalid mproc dictionary!')
 
         self._dipoleoff = dipoleoff
-        self._acc = 'SI'
+        self._acc = acc or 'SI'
         self._pru = None
         self._udc = None
         self.bbbnames = bbbnames or _dcopy(PSSOFB.BBBNAMES)
         self.bbb2devs = dict()
 
         # flag that controls sending sofbupdate signal to IOCs
         self._sofb_update_iocs = sofb_update_iocs
 
         self._sofb_psnames = \
             PSNamesSOFB.get_psnames_ch(self._acc) + \
-            PSNamesSOFB.get_psnames_cv(self._acc)
+            PSNamesSOFB.get_psnames_cv(self._acc) + \
+            PSNamesSOFB.get_psnames_qs(self._acc)
 
         # snapshot of sofb current values
         ncorrs = len(self._sofb_psnames)
         arr = _np.zeros(ncorrs, dtype=float)
         self._sofb_current_rb = arr.copy()
         self._sofb_current_mon = arr.copy()
 
@@ -201,18 +227,20 @@
         self._pscstatus = [_PSCStatus() for _ in self._sofb_psnames]
 
         # strength to current converters
         if mproc is None:
             self.converter = UnitConverter(
                 self._sofb_psnames, dipoleoff=dipoleoff)
 
+    @property
     def pru(self):
         """Return Beagle-name to PRU-object dictionary."""
         return self._pru
 
+    @property
     def udc(self):
         """Return Beagle-name to UDC-object dictionary."""
         return self._udc
 
     # --- threads manipulation methods ---
 
     def threads_shutdown(self):
```

### Comparing `siriuspy-2.74.1/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.75.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/conn.py` & `siriuspy-2.75.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/magnet.py` & `siriuspy-2.75.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/ramp.py` & `siriuspy-2.75.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.75.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.75.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/testwfm.py` & `siriuspy-2.75.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/util.py` & `siriuspy-2.75.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/ramp/waveform.py` & `siriuspy-2.75.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/bpms_search.py` & `siriuspy-2.75.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/hl_time_search.py` & `siriuspy-2.75.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/id_search.py` & `siriuspy-2.75.0/siriuspy/search/id_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/ioc_search.py` & `siriuspy-2.75.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/ll_time_search.py` & `siriuspy-2.75.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/ma_search.py` & `siriuspy-2.75.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/search/ps_search.py` & `siriuspy-2.75.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/simul/simfactory.py` & `siriuspy-2.75.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/simul/simps.py` & `siriuspy-2.75.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/simul/simpv.py` & `siriuspy-2.75.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/simul/simulation.py` & `siriuspy-2.75.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/simul/simulator.py` & `siriuspy-2.75.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/base_class.py` & `siriuspy-2.75.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/bpms.py` & `siriuspy-2.75.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/correctors.py` & `siriuspy-2.75.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/csdev.py` & `siriuspy-2.75.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/main.py` & `siriuspy-2.75.0/siriuspy/sofb/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/matrix.py` & `siriuspy-2.75.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/orbit.py` & `siriuspy-2.75.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/sofb/utils.py` & `siriuspy-2.75.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/stabinfo/csdev.py` & `siriuspy-2.75.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/thread.py` & `siriuspy-2.75.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/timesys/csdev.py` & `siriuspy-2.75.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/timesys/hl_classes.py` & `siriuspy-2.75.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/timesys/ll_classes.py` & `siriuspy-2.75.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/timesys/plot_network.py` & `siriuspy-2.75.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/timesys/static_table.py` & `siriuspy-2.75.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy/util.py` & `siriuspy-2.75.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.75.0/siriuspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.74.1
+Version: 2.75.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.74.1/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.75.0/siriuspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/bsmp/test_bsmp.py` & `siriuspy-2.75.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/bsmp/test_commands.py` & `siriuspy-2.75.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/bsmp/test_entities.py` & `siriuspy-2.75.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/bsmp/test_serial.py` & `siriuspy-2.75.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/bsmp/test_types.py` & `siriuspy-2.75.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.75.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/clientweb/test_implementation.py` & `siriuspy-2.75.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.75.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/currinfo/test_csdev.py` & `siriuspy-2.75.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/currinfo/test_main.py` & `siriuspy-2.75.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/magnet/test_factory.py` & `siriuspy-2.75.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/magnet/tests_normalizer.py` & `siriuspy-2.75.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/mock_servweb.py` & `siriuspy-2.75.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/namesys/test_implementation.py` & `siriuspy-2.75.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/opticscorr/test_chrom.py` & `siriuspy-2.75.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/opticscorr/test_csdev.py` & `siriuspy-2.75.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.75.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/opticscorr/test_tune.py` & `siriuspy-2.75.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/opticscorr/test_utils.py` & `siriuspy-2.75.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/posang/test_csdev.py` & `siriuspy-2.75.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/posang/test_main.py` & `siriuspy-2.75.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/db.py` & `siriuspy-2.75.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.75.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.75.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/test_csdev.py` & `siriuspy-2.75.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/test_data.py` & `siriuspy-2.75.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/test_siggen.py` & `siriuspy-2.75.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/pwrsupply/variables.py` & `siriuspy-2.75.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/ramp/test_magnet.py` & `siriuspy-2.75.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/ramp/test_waveform.py` & `siriuspy-2.75.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/search/test_hl_time_search.py` & `siriuspy-2.75.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/search/test_init.py` & `siriuspy-2.75.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/search/test_ll_time_search.py` & `siriuspy-2.75.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/search/test_ma_search.py` & `siriuspy-2.75.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/search/test_ps_search.py` & `siriuspy-2.75.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/test_callbacks.py` & `siriuspy-2.75.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/test_csdev.py` & `siriuspy-2.75.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/test_envars.py` & `siriuspy-2.75.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/test_util.py` & `siriuspy-2.75.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/timesys/test_csdev.py` & `siriuspy-2.75.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.74.1/tests/timesys/test_plot_network.py` & `siriuspy-2.75.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

