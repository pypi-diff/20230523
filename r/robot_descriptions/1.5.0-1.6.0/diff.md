# Comparing `tmp/robot_descriptions-1.5.0.tar.gz` & `tmp/robot_descriptions-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_descriptions-1.5.0.tar", last modified: Thu Apr 13 09:26:43 2023, max compression
+gzip compressed data, was "robot_descriptions-1.6.0.tar", last modified: Tue May 23 16:46:56 2023, max compression
```

## Comparing `robot_descriptions-1.5.0.tar` & `robot_descriptions-1.6.0.tar`

### file list

```diff
@@ -1,115 +1,118 @@
--rw-r--r--   0        0        0     2290 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0       42 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/.gitignore
--rw-r--r--   0        0        0     5071 2023-04-13 09:25:54.436823 robot_descriptions-1.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     2039 2023-04-13 09:16:00.609377 robot_descriptions-1.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/LICENSE
--rw-r--r--   0        0        0    15234 2023-04-13 09:11:45.925423 robot_descriptions-1.5.0/README.md
--rw-r--r--   0        0        0     2905 2023-03-16 09:00:10.280693 robot_descriptions-1.5.0/examples/display_urdf_frames.py
--rw-r--r--   0        0        0     1295 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_idyntree.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_mujoco.py
--rw-r--r--   0        0        0     1276 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_pinocchio.py
--rw-r--r--   0        0        0     1370 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_pybullet.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_robomeshcat.py
--rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/load_in_yourdfpy.py
--rw-r--r--   0        0        0     1642 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_meshcat.py
--rw-r--r--   0        0        0     1716 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_mujoco.py
--rw-r--r--   0        0        0     1505 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_pybullet.py
--rw-r--r--   0        0        0     1665 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_robomeshcat.py
--rw-r--r--   0        0        0     1579 2023-01-06 14:01:23.817479 robot_descriptions-1.5.0/examples/show_in_yourdfpy.py
--rw-r--r--   0        0        0     1863 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-04-13 09:26:03.117116 robot_descriptions-1.5.0/robot_descriptions/__init__.py
--rw-r--r--   0        0        0     4385 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_cache.py
--rw-r--r--   0        0        0     5604 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_command_line.py
--rw-r--r--   0        0        0     5090 2023-04-13 09:12:36.338206 robot_descriptions-1.5.0/robot_descriptions/_descriptions.py
--rw-r--r--   0        0        0      674 2023-02-13 11:16:52.063235 robot_descriptions-1.5.0/robot_descriptions/_empty_description.py
--rw-r--r--   0        0        0     1114 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/_package_dirs.py
--rw-r--r--   0        0        0     9642 2023-04-13 09:09:48.451600 robot_descriptions-1.5.0/robot_descriptions/_repositories.py
--rw-r--r--   0        0        0     1024 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/a1_description.py
--rw-r--r--   0        0        0     1078 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/a1_mj_description.py
--rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/aliengo_description.py
--rw-r--r--   0        0        0     1325 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/allegro_hand_description.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_b_description.py
--rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_b_mj_description.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_c_description.py
--rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/anymal_c_mj_description.py
--rw-r--r--   0        0        0     1171 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/atlas_drc_description.py
--rw-r--r--   0        0        0     1381 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/atlas_v4_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/b1_description.py
--rw-r--r--   0        0        0     1016 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/barrett_hand_description.py
--rw-r--r--   0        0        0     1028 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/baxter_description.py
--rw-r--r--   0        0        0     1039 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/bolt_description.py
--rw-r--r--   0        0        0     1012 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cassie_description.py
--rw-r--r--   0        0        0     1023 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cassie_mj_description.py
--rw-r--r--   0        0        0     1048 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/cf2_description.py
--rw-r--r--   0        0        0     1304 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/double_pendulum_description.py
--rw-r--r--   0        0        0     1011 2023-02-22 15:58:12.265767 robot_descriptions-1.5.0/robot_descriptions/draco3_description.py
--rw-r--r--   0        0        0      997 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/edo_description.py
--rw-r--r--   0        0        0     1042 2023-02-28 10:22:37.917012 robot_descriptions-1.5.0/robot_descriptions/ergocub_description.py
--rw-r--r--   0        0        0     1034 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/eve_r3_description.py
--rw-r--r--   0        0        0     1060 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/fetch_description.py
--rw-r--r--   0        0        0     1065 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/finger_edu_description.py
--rw-r--r--   0        0        0     1043 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/gen2_description.py
--rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/gen3_mj_description.py
--rw-r--r--   0        0        0     1007 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ginger_description.py
--rw-r--r--   0        0        0     1027 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/go1_description.py
--rw-r--r--   0        0        0     1082 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/go1_mj_description.py
--rw-r--r--   0        0        0     1047 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/hyq_description.py
--rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/icub_description.py
--rw-r--r--   0        0        0     1427 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/iiwa_description.py
--rw-r--r--   0        0        0     1013 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jaxon_description.py
--rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jvrc_description.py
--rw-r--r--   0        0        0     1014 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/jvrc_mj_description.py
--rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/laikago_description.py
--rw-r--r--   0        0        0      683 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/__init__.py
--rw-r--r--   0        0        0     2587 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/idyntree.py
--rw-r--r--   0        0        0     1514 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/mujoco.py
--rw-r--r--   0        0        0     2173 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/pinocchio.py
--rw-r--r--   0        0        0     2157 2023-04-03 09:25:58.942767 robot_descriptions-1.5.0/robot_descriptions/loaders/pybullet.py
--rw-r--r--   0        0        0     1612 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/loaders/robomeshcat.py
--rw-r--r--   0        0        0     1732 2023-02-22 15:58:12.265767 robot_descriptions-1.5.0/robot_descriptions/loaders/yourdfpy.py
--rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/mini_cheetah_description.py
--rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/minitaur_description.py
--rw-r--r--   0        0        0     1036 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/nextage_description.py
--rw-r--r--   0        0        0     1040 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/panda_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/panda_mj_description.py
--rw-r--r--   0        0        0     1011 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/pepper_description.py
--rw-r--r--   0        0        0     1032 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/poppy_ergo_jr_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/poppy_torso_description.py
--rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/pr2_description.py
--rw-r--r--   0        0        0     2748 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/r2_description.py
--rw-r--r--   0        0        0     1003 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/reachy_description.py
--rw-r--r--   0        0        0     1005 2023-03-16 16:25:43.136050 robot_descriptions-1.5.0/robot_descriptions/rhea_description.py
--rw-r--r--   0        0        0     1052 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_mj_description.py
--rw-r--r--   0        0        0     1053 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/romeo_description.py
--rw-r--r--   0        0        0     1190 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/shadow_hand_mj_description.py
--rw-r--r--   0        0        0      999 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/sigmaban_description.py
--rw-r--r--   0        0        0     1139 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/simple_humanoid_description.py
--rw-r--r--   0        0        0     1041 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/solo_description.py
--rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/spryped_description.py
--rw-r--r--   0        0        0     1008 2023-04-13 09:12:21.205971 robot_descriptions-1.5.0/robot_descriptions/stretch_description.py
--rw-r--r--   0        0        0     1286 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/talos_description.py
--rw-r--r--   0        0        0     1238 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/tiago_description.py
--rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/upkie_description.py
--rw-r--r--   0        0        0     1175 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur10_description.py
--rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur3_description.py
--rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur5_description.py
--rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/ur5e_mj_description.py
--rw-r--r--   0        0        0     1350 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/valkyrie_description.py
--rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/yumi_description.py
--rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/robot_descriptions/z1_description.py
--rw-r--r--   0        0        0     1002 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0       59 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/__init__.py
--rwxr-xr-x   0        0        0     1531 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_idyntree.py
--rw-r--r--   0        0        0     1479 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_mujoco.py
--rw-r--r--   0        0        0     1536 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_pinocchio.py
--rw-r--r--   0        0        0     1976 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_pybullet.py
--rw-r--r--   0        0        0     1547 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_robomeshcat.py
--rw-r--r--   0        0        0     1488 2023-01-06 14:01:23.821479 robot_descriptions-1.5.0/tests/loaders/test_yourdfpy.py
--rw-r--r--   0        0        0     2802 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_clone_to_cache.py
--rw-r--r--   0        0        0     3585 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_clone_to_directory.py
--rw-r--r--   0        0        0     2373 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_descriptions.py
--rw-r--r--   0        0        0     2583 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_loaders.py
--rw-r--r--   0        0        0      987 2023-02-08 17:58:19.351928 robot_descriptions-1.5.0/tests/test_progress_bar.py
--rw-r--r--   0        0        0     2225 2023-02-13 11:16:52.067235 robot_descriptions-1.5.0/tox.ini
--rw-r--r--   0        0        0    16702 1970-01-01 00:00:00.000000 robot_descriptions-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2290 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       42 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/.gitignore
+-rw-r--r--   0        0        0     5237 2023-05-23 16:14:37.942132 robot_descriptions-1.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2039 2023-05-23 15:38:35.116178 robot_descriptions-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/LICENSE
+-rw-r--r--   0        0        0    15520 2023-05-23 16:13:37.895816 robot_descriptions-1.6.0/README.md
+-rw-r--r--   0        0        0     2905 2023-03-16 09:00:10.280693 robot_descriptions-1.6.0/examples/display_urdf_frames.py
+-rw-r--r--   0        0        0     1295 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_idyntree.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_mujoco.py
+-rw-r--r--   0        0        0     1276 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_pinocchio.py
+-rw-r--r--   0        0        0     1370 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_pybullet.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_robomeshcat.py
+-rw-r--r--   0        0        0     1280 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/load_in_yourdfpy.py
+-rw-r--r--   0        0        0     1642 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/show_in_meshcat.py
+-rw-r--r--   0        0        0     1716 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/show_in_mujoco.py
+-rw-r--r--   0        0        0     1505 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/show_in_pybullet.py
+-rw-r--r--   0        0        0     1665 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/show_in_robomeshcat.py
+-rw-r--r--   0        0        0     1579 2023-01-06 14:01:23.817479 robot_descriptions-1.6.0/examples/show_in_yourdfpy.py
+-rw-r--r--   0        0        0     1863 2023-02-13 11:16:52.063235 robot_descriptions-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-23 16:14:49.541832 robot_descriptions-1.6.0/robot_descriptions/__init__.py
+-rw-r--r--   0        0        0     4385 2023-02-13 11:16:52.063235 robot_descriptions-1.6.0/robot_descriptions/_cache.py
+-rw-r--r--   0        0        0     5604 2023-02-13 11:16:52.063235 robot_descriptions-1.6.0/robot_descriptions/_command_line.py
+-rw-r--r--   0        0        0     5257 2023-05-23 16:13:37.895816 robot_descriptions-1.6.0/robot_descriptions/_descriptions.py
+-rw-r--r--   0        0        0      674 2023-02-13 11:16:52.063235 robot_descriptions-1.6.0/robot_descriptions/_empty_description.py
+-rw-r--r--   0        0        0     1114 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/_package_dirs.py
+-rw-r--r--   0        0        0    10131 2023-05-23 16:13:37.895816 robot_descriptions-1.6.0/robot_descriptions/_repositories.py
+-rw-r--r--   0        0        0     1024 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/a1_description.py
+-rw-r--r--   0        0        0     1078 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/a1_mj_description.py
+-rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/aliengo_description.py
+-rw-r--r--   0        0        0     1325 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/allegro_hand_description.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/anymal_b_description.py
+-rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/anymal_b_mj_description.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/anymal_c_description.py
+-rw-r--r--   0        0        0     1031 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/anymal_c_mj_description.py
+-rw-r--r--   0        0        0     1171 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/atlas_drc_description.py
+-rw-r--r--   0        0        0     1381 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/atlas_v4_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/b1_description.py
+-rw-r--r--   0        0        0     1016 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/barrett_hand_description.py
+-rw-r--r--   0        0        0     1028 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/baxter_description.py
+-rw-r--r--   0        0        0     1039 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/bolt_description.py
+-rw-r--r--   0        0        0     1012 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/cassie_description.py
+-rw-r--r--   0        0        0     1023 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/cassie_mj_description.py
+-rw-r--r--   0        0        0     1048 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/cf2_description.py
+-rw-r--r--   0        0        0     1304 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/double_pendulum_description.py
+-rw-r--r--   0        0        0     1011 2023-02-22 15:58:12.265767 robot_descriptions-1.6.0/robot_descriptions/draco3_description.py
+-rw-r--r--   0        0        0      997 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/edo_description.py
+-rw-r--r--   0        0        0     1042 2023-02-28 10:22:37.917012 robot_descriptions-1.6.0/robot_descriptions/ergocub_description.py
+-rw-r--r--   0        0        0     1034 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/eve_r3_description.py
+-rw-r--r--   0        0        0     1026 2023-05-23 16:13:37.895816 robot_descriptions-1.6.0/robot_descriptions/fanuc_m710ic_description.py
+-rw-r--r--   0        0        0     1060 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/fetch_description.py
+-rw-r--r--   0        0        0     1065 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/finger_edu_description.py
+-rw-r--r--   0        0        0     1055 2023-05-23 15:38:35.116178 robot_descriptions-1.6.0/robot_descriptions/gen2_description.py
+-rw-r--r--   0        0        0     1074 2023-05-23 15:38:35.116178 robot_descriptions-1.6.0/robot_descriptions/gen3_description.py
+-rw-r--r--   0        0        0     1032 2023-05-23 15:38:35.116178 robot_descriptions-1.6.0/robot_descriptions/gen3_mj_description.py
+-rw-r--r--   0        0        0     1007 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/ginger_description.py
+-rw-r--r--   0        0        0     1027 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/go1_description.py
+-rw-r--r--   0        0        0     1082 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/go1_mj_description.py
+-rw-r--r--   0        0        0     1047 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/hyq_description.py
+-rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/icub_description.py
+-rw-r--r--   0        0        0     1427 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/iiwa_description.py
+-rw-r--r--   0        0        0     1013 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/jaxon_description.py
+-rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/jvrc_description.py
+-rw-r--r--   0        0        0     1014 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/jvrc_mj_description.py
+-rw-r--r--   0        0        0     1093 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/laikago_description.py
+-rw-r--r--   0        0        0      683 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/loaders/__init__.py
+-rw-r--r--   0        0        0     2587 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/loaders/idyntree.py
+-rw-r--r--   0        0        0     1514 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/loaders/mujoco.py
+-rw-r--r--   0        0        0     2173 2023-04-13 12:49:25.532815 robot_descriptions-1.6.0/robot_descriptions/loaders/pinocchio.py
+-rw-r--r--   0        0        0     2157 2023-04-03 09:25:58.942767 robot_descriptions-1.6.0/robot_descriptions/loaders/pybullet.py
+-rw-r--r--   0        0        0     1612 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/loaders/robomeshcat.py
+-rw-r--r--   0        0        0     1732 2023-02-22 15:58:12.265767 robot_descriptions-1.6.0/robot_descriptions/loaders/yourdfpy.py
+-rw-r--r--   0        0        0     1022 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/mini_cheetah_description.py
+-rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/minitaur_description.py
+-rw-r--r--   0        0        0     1036 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/nextage_description.py
+-rw-r--r--   0        0        0     1040 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/panda_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/panda_mj_description.py
+-rw-r--r--   0        0        0     1011 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/pepper_description.py
+-rw-r--r--   0        0        0     1032 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/poppy_ergo_jr_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/poppy_torso_description.py
+-rw-r--r--   0        0        0     1017 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/pr2_description.py
+-rw-r--r--   0        0        0     2748 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/r2_description.py
+-rw-r--r--   0        0        0     1003 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/reachy_description.py
+-rw-r--r--   0        0        0     1005 2023-03-16 16:25:43.136050 robot_descriptions-1.6.0/robot_descriptions/rhea_description.py
+-rw-r--r--   0        0        0     1052 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/robotiq_2f85_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/robotiq_2f85_mj_description.py
+-rw-r--r--   0        0        0     1053 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/romeo_description.py
+-rw-r--r--   0        0        0     1190 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/shadow_hand_mj_description.py
+-rw-r--r--   0        0        0      999 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/sigmaban_description.py
+-rw-r--r--   0        0        0     1139 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/simple_humanoid_description.py
+-rw-r--r--   0        0        0     1041 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/solo_description.py
+-rw-r--r--   0        0        0     1035 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/spryped_description.py
+-rw-r--r--   0        0        0     1008 2023-04-13 09:12:21.205971 robot_descriptions-1.6.0/robot_descriptions/stretch_description.py
+-rw-r--r--   0        0        0     1286 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/talos_description.py
+-rw-r--r--   0        0        0     1238 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/tiago_description.py
+-rw-r--r--   0        0        0     1078 2023-05-23 15:38:35.116178 robot_descriptions-1.6.0/robot_descriptions/trifinger_edu_description.py
+-rw-r--r--   0        0        0     1008 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/upkie_description.py
+-rw-r--r--   0        0        0     1175 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/ur10_description.py
+-rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/ur3_description.py
+-rw-r--r--   0        0        0     1251 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/ur5_description.py
+-rw-r--r--   0        0        0     1026 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/ur5e_mj_description.py
+-rw-r--r--   0        0        0     1350 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/valkyrie_description.py
+-rw-r--r--   0        0        0     1020 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/yumi_description.py
+-rw-r--r--   0        0        0     1025 2023-02-13 11:16:52.067235 robot_descriptions-1.6.0/robot_descriptions/z1_description.py
+-rw-r--r--   0        0        0     1002 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/__init__.py
+-rw-r--r--   0        0        0       59 2023-01-06 14:01:23.821479 robot_descriptions-1.6.0/tests/loaders/__init__.py
+-rw-r--r--   0        0        0     1531 2023-04-13 13:43:23.617024 robot_descriptions-1.6.0/tests/loaders/test_idyntree.py
+-rw-r--r--   0        0        0     1479 2023-01-06 14:01:23.821479 robot_descriptions-1.6.0/tests/loaders/test_mujoco.py
+-rw-r--r--   0        0        0     1537 2023-04-13 13:43:23.617024 robot_descriptions-1.6.0/tests/loaders/test_pinocchio.py
+-rw-r--r--   0        0        0     1976 2023-01-06 14:01:23.821479 robot_descriptions-1.6.0/tests/loaders/test_pybullet.py
+-rw-r--r--   0        0        0     1547 2023-01-06 14:01:23.821479 robot_descriptions-1.6.0/tests/loaders/test_robomeshcat.py
+-rw-r--r--   0        0        0     1488 2023-01-06 14:01:23.821479 robot_descriptions-1.6.0/tests/loaders/test_yourdfpy.py
+-rw-r--r--   0        0        0     2802 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/test_clone_to_cache.py
+-rw-r--r--   0        0        0     3585 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/test_clone_to_directory.py
+-rw-r--r--   0        0        0     2373 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/test_descriptions.py
+-rw-r--r--   0        0        0     2583 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/test_loaders.py
+-rw-r--r--   0        0        0      987 2023-02-08 17:58:19.351928 robot_descriptions-1.6.0/tests/test_progress_bar.py
+-rw-r--r--   0        0        0     2223 2023-04-13 13:43:23.617024 robot_descriptions-1.6.0/tox.ini
+-rw-r--r--   0        0        0    16988 1970-01-01 00:00:00.000000 robot_descriptions-1.6.0/PKG-INFO
```

### Comparing `robot_descriptions-1.5.0/.github/workflows/test.yml` & `robot_descriptions-1.6.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/CHANGELOG.md` & `robot_descriptions-1.6.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [1.6.0] - 2023/5/23
+
+### Added
+
+- Description: FANUC M-710iC
+- Description: Gen3
+- Description: TriFingerEdu
+
+### Changed
+
+- Update Stretch description to v1.0.0
+
 ## [1.5.0] - 2023/4/13
 
 ### Added
 
 - Description: Rhea
 - Description: Stretch
 - Frame selector in URDF frame display example
```

### Comparing `robot_descriptions-1.5.0/CONTRIBUTING.md` & `robot_descriptions-1.6.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 2. **Repository:** If needed, add the repository containing the new description to ``_repositories.py``.
     - Use a specific git commit ID. This way the robot description will still work in the interval between a change in the file structure of the target repository and the corresponding update in `robot_descriptions`.
 3. **Submodule:** add a Python file for the robot descriptions to ``robot_descriptions/``.
     - The file name for the new submodule is ``<robot_name>_description.py`` in snake-case.
     - For example, the file name for the Kinova (maker) Gen2 (robot name) is ``gen2_description.py``.
     - Use the ``mj_description`` suffix for an MJCF description.
 4. **Listing:** Add the description metadata to the ``DESCRIPTIONS`` dictionary in ``_descriptions.py``.
-5. **Testing:** Check that all unit tests are successful by ``tox``.
-6. **README:** Document the description's submodule name in the Descriptions section of the [README](README.md).
-7. **Changelog:** Write down the new model at the top of the [changelog](CHANGELOG.md).
+5. **README:** Document the description's submodule name in the Descriptions section of the [README](README.md).
+6. **CHANGELOG:** Write down the new model at the top of the [changelog](CHANGELOG.md).
+7. **Testing:** Check that all unit tests are successful by ``tox``.
```

### Comparing `robot_descriptions-1.5.0/LICENSE` & `robot_descriptions-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/README.md` & `robot_descriptions-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -123,25 +123,27 @@
 The DOF column denotes the number of actuated degrees of freedom.
 
 ### Arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `edo_description`             | e.DO                  | Comau                    | 6   | URDF       |
-| `gen2_description`            | Gen2                  | Kinova                   | 6   | URDF       |
-| `gen3_mj_description`         | Gen3                  | Kinova                   | 7   | MJCF       |
+| `fanuc_m710ic_description`    | M-710iC               | Fanuc                    | 6   | URDF       |
+| `gen2_description`            | Gen2 (Jaco)           | Kinova                   | 6   | URDF       |
+| `gen3_description`            | Gen3 (Jaco)           | Kinova                   | 6   | URDF       |
+| `gen3_mj_description`         | Gen3 (Jaco)           | Kinova                   | 7   | MJCF       |
 | `iiwa_description`            | iiwa                  | KUKA                     | 7   | URDF       |
 | `panda_description`           | Panda                 | Franka Emika             | 8   | URDF       |
 | `panda_mj_description`        | Panda                 | Franka Emika             | 8   | MJCF       |
 | `poppy_ergo_jr_description`   | Poppy Ergo Jr         | Poppy Project            | 6   | URDF       |
 | `ur10_description`            | UR10                  | Universal Robots         | 6   | URDF       |
 | `ur3_description`             | UR3                   | Universal Robots         | 6   | URDF       |
 | `ur5_description`             | UR5                   | Universal Robots         | 6   | URDF       |
 | `ur5e_mj_description`         | UR5e                  | Universal Robots         | 6   | MJCF       |
-| `z1_description`              | Z1                    | UNITREE Robotics         | 6  | URDF       |
+| `z1_description`              | Z1                    | UNITREE Robotics         | 6   | URDF       |
 
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
 | `cassie_description`          | Cassie                | Agility Robotics         | 16  | URDF       |
@@ -168,14 +170,15 @@
 ### Educational
 
 | Name                          | Robot                 | DOF | Format     |
 |-------------------------------|-----------------------|-----|------------|
 | `double_pendulum_description` | Double Pendulum       | 2   | URDF       |
 | `finger_edu_description`      | FingerEdu             | 3   | URDF       |
 | `simple_humanoid_description` | Simple Humanoid       | 29  | URDF       |
+| `trifinger_edu_description`   | TriFingerEdu          | 9   | URDF       |
 
 ### End effectors
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `allegro_hand_description`    | Allegro Hand          | Wonik Robotics           | 16  | URDF       |
 | `barrett_hand_description`    | BarrettHand           | Barrett Technology       | 8   | URDF       |
```

### Comparing `robot_descriptions-1.5.0/examples/display_urdf_frames.py` & `robot_descriptions-1.6.0/examples/display_urdf_frames.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_idyntree.py` & `robot_descriptions-1.6.0/examples/load_in_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_mujoco.py` & `robot_descriptions-1.6.0/examples/load_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_pinocchio.py` & `robot_descriptions-1.6.0/examples/load_in_pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_pybullet.py` & `robot_descriptions-1.6.0/examples/load_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_robomeshcat.py` & `robot_descriptions-1.6.0/examples/load_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/load_in_yourdfpy.py` & `robot_descriptions-1.6.0/examples/load_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/show_in_meshcat.py` & `robot_descriptions-1.6.0/examples/show_in_meshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/show_in_mujoco.py` & `robot_descriptions-1.6.0/examples/show_in_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/show_in_pybullet.py` & `robot_descriptions-1.6.0/examples/show_in_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/show_in_robomeshcat.py` & `robot_descriptions-1.6.0/examples/show_in_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/examples/show_in_yourdfpy.py` & `robot_descriptions-1.6.0/examples/show_in_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/pyproject.toml` & `robot_descriptions-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/__init__.py` & `robot_descriptions-1.6.0/robot_descriptions/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Import open source robot description as Python modules."""
 
-__version__ = "1.5.0"
+__version__ = "1.6.0"
```

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_cache.py` & `robot_descriptions-1.6.0/robot_descriptions/_cache.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_command_line.py` & `robot_descriptions-1.6.0/robot_descriptions/_command_line.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_descriptions.py` & `robot_descriptions-1.6.0/robot_descriptions/_descriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,19 @@
     "cassie_mj_description": Description(Format.MJCF),
     "cf2_description": Description(Format.URDF),
     "double_pendulum_description": Description(Format.URDF),
     "draco3_description": Description(Format.URDF),
     "edo_description": Description(Format.URDF),
     "ergocub_description": Description(Format.URDF),
     "eve_r3_description": Description(Format.URDF),
+    "fanuc_m710ic_description": Description(Format.URDF),
     "fetch_description": Description(Format.URDF),
     "finger_edu_description": Description(Format.URDF),
     "gen2_description": Description(Format.URDF),
+    "gen3_description": Description(Format.URDF),
     "gen3_mj_description": Description(Format.MJCF),
     "ginger_description": Description(Format.URDF),
     "go1_description": Description(Format.URDF),
     "go1_mj_description": Description(Format.MJCF),
     "hyq_description": Description(Format.URDF),
     "icub_description": Description(Format.URDF),
     "iiwa_description": Description(Format.URDF),
@@ -113,14 +115,15 @@
     "shadow_hand_mj_description": Description(Format.MJCF),
     "simple_humanoid_description": Description(Format.URDF),
     "solo_description": Description(Format.URDF),
     "spryped_description": Description(Format.URDF),
     "stretch_description": Description(Format.URDF),
     "talos_description": Description(Format.URDF),
     "tiago_description": Description(Format.URDF),
+    "trifinger_edu_description": Description(Format.URDF),
     "upkie_description": Description(Format.URDF),
     "ur10_description": Description(Format.URDF),
     "ur3_description": Description(Format.URDF),
     "ur5_description": Description(Format.URDF),
     "ur5e_mj_description": Description(Format.MJCF),
     "valkyrie_description": Description(Format.URDF),
     "yumi_description": Description(Format.URDF),
```

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_empty_description.py` & `robot_descriptions-1.6.0/robot_descriptions/_empty_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_package_dirs.py` & `robot_descriptions-1.6.0/robot_descriptions/_package_dirs.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/_repositories.py` & `robot_descriptions-1.6.0/robot_descriptions/_repositories.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,19 @@
         cache_path="cassie_description",
     ),
     "cassie_mj_description": Repository(
         url="https://github.com/rohanpsingh/cassie_mj_description.git",
         commit="fcc3775453e4da6797cd4eacd3d8321d9906755a",
         cache_path="cassie_mj_description",
     ),
+    "differentiable-robot-model": Repository(
+        url="https://github.com/facebookresearch/differentiable-robot-model",
+        commit="d7bd1b3b8ef1d6dabe9b68474a622185c510e112",
+        cache_path="differentiable-robot-model",
+    ),
     "draco3_description": Repository(
         url="https://github.com/shbang91/draco3_description.git",
         commit="5afd19733d7b3e9f1135ba93e0aad90ed1a24cc7",
         cache_path="draco3_description",
     ),
     "drake": Repository(
         url="https://github.com/RobotLocomotion/drake.git",
@@ -93,14 +98,20 @@
         cache_path="ergocub-software",
     ),
     "example-robot-data": Repository(
         url="https://github.com/Gepetto/example-robot-data.git",
         commit="9ba565ca1491efa92ebac38cdd499e5b1c256bf1",  # v4.0.3
         cache_path="example-robot-data",
     ),
+    "fanuc_m710ic_description": Repository(
+        url="https://github.com/"
+        "robot-descriptions/fanuc_m710ic_description.git",
+        commit="d12af44559cd7e46f7afd513237f159f82f8402e",
+        cache_path="fanuc_m710ic_description",
+    ),
     "GingerURDF": Repository(
         url="https://github.com/Rayckey/GingerURDF.git",
         commit="6a1307cd0ee2b77c82f8839cdce3a2e2eed2bd8f",
         cache_path="gingerurdf",  # match package name
     ),
     "gym-pybullet-drones": Repository(
         url="https://github.com/utiasDSL/gym-pybullet-drones.git",
@@ -220,15 +231,15 @@
     "spryped": Repository(
         url="https://github.com/bbokser/spryped.git",
         commit="f360a6b78667a4d97c86cad465ef8f4c9512462b",
         cache_path="spryped",
     ),
     "stretch_description": Repository(
         url="https://github.com/robot-descriptions/stretch_description.git",
-        commit="d9a614f8572d5a73f78a7f358107233c40a78b13",
+        commit="4b838429fe4c5d9f2937efe698444bd68968f376",
         cache_path="stretch_description",
     ),
     "talos-data": Repository(
         url="https://github.com/stack-of-tasks/talos-data.git",
         commit="v2.0.0",
         cache_path="talos_data",  # match package name
     ),
```

### Comparing `robot_descriptions-1.5.0/robot_descriptions/a1_description.py` & `robot_descriptions-1.6.0/robot_descriptions/a1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/a1_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/a1_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/aliengo_description.py` & `robot_descriptions-1.6.0/robot_descriptions/aliengo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/allegro_hand_description.py` & `robot_descriptions-1.6.0/robot_descriptions/allegro_hand_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/anymal_b_description.py` & `robot_descriptions-1.6.0/robot_descriptions/anymal_b_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/anymal_b_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/anymal_b_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/anymal_c_description.py` & `robot_descriptions-1.6.0/robot_descriptions/anymal_c_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/anymal_c_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/anymal_c_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/atlas_drc_description.py` & `robot_descriptions-1.6.0/robot_descriptions/atlas_drc_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/atlas_v4_description.py` & `robot_descriptions-1.6.0/robot_descriptions/atlas_v4_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/b1_description.py` & `robot_descriptions-1.6.0/robot_descriptions/b1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/barrett_hand_description.py` & `robot_descriptions-1.6.0/robot_descriptions/barrett_hand_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/baxter_description.py` & `robot_descriptions-1.6.0/robot_descriptions/baxter_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/bolt_description.py` & `robot_descriptions-1.6.0/robot_descriptions/bolt_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/cassie_description.py` & `robot_descriptions-1.6.0/robot_descriptions/cassie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/cassie_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/cassie_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/cf2_description.py` & `robot_descriptions-1.6.0/robot_descriptions/cf2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/double_pendulum_description.py` & `robot_descriptions-1.6.0/robot_descriptions/double_pendulum_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/draco3_description.py` & `robot_descriptions-1.6.0/robot_descriptions/draco3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/edo_description.py` & `robot_descriptions-1.6.0/robot_descriptions/edo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ergocub_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ergocub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/eve_r3_description.py` & `robot_descriptions-1.6.0/robot_descriptions/eve_r3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/fetch_description.py` & `robot_descriptions-1.6.0/robot_descriptions/fetch_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/finger_edu_description.py` & `robot_descriptions-1.6.0/robot_descriptions/finger_edu_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/gen2_description.py` & `robot_descriptions-1.6.0/robot_descriptions/gen2_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Gen2 description."""
+"""Kinova Jaco Gen2 description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
```

### Comparing `robot_descriptions-1.5.0/robot_descriptions/gen3_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/fanuc_m710ic_description.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Gen3 description."""
+"""Fanuc M-710iC description."""
 
 from os import getenv as _getenv
 from os import path as _path
 
 from ._cache import clone_to_cache as _clone_to_cache
 
 REPOSITORY_PATH: str = _clone_to_cache(
-    "kinova_mj_description",
+    "fanuc_m710ic_description",
     commit=_getenv("ROBOT_DESCRIPTION_COMMIT", None),
 )
 
 PACKAGE_PATH: str = _path.join(REPOSITORY_PATH)
 
-MJCF_PATH: str = _path.join(PACKAGE_PATH, "xml", "gen3_7dof_mujoco.xml")
+URDF_PATH: str = _path.join(PACKAGE_PATH, "urdf", "m710ic70.urdf")
```

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ginger_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ginger_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/go1_description.py` & `robot_descriptions-1.6.0/robot_descriptions/go1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/go1_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/go1_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/hyq_description.py` & `robot_descriptions-1.6.0/robot_descriptions/hyq_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/icub_description.py` & `robot_descriptions-1.6.0/robot_descriptions/icub_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/iiwa_description.py` & `robot_descriptions-1.6.0/robot_descriptions/iiwa_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/jaxon_description.py` & `robot_descriptions-1.6.0/robot_descriptions/jaxon_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/jvrc_description.py` & `robot_descriptions-1.6.0/robot_descriptions/jvrc_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/jvrc_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/jvrc_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/laikago_description.py` & `robot_descriptions-1.6.0/robot_descriptions/laikago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/__init__.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/idyntree.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/mujoco.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/pinocchio.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/pinocchio.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/pybullet.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/robomeshcat.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/loaders/yourdfpy.py` & `robot_descriptions-1.6.0/robot_descriptions/loaders/yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/mini_cheetah_description.py` & `robot_descriptions-1.6.0/robot_descriptions/mini_cheetah_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/minitaur_description.py` & `robot_descriptions-1.6.0/robot_descriptions/minitaur_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/nextage_description.py` & `robot_descriptions-1.6.0/robot_descriptions/nextage_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/panda_description.py` & `robot_descriptions-1.6.0/robot_descriptions/panda_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/panda_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/panda_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/pepper_description.py` & `robot_descriptions-1.6.0/robot_descriptions/pepper_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/poppy_ergo_jr_description.py` & `robot_descriptions-1.6.0/robot_descriptions/poppy_ergo_jr_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/poppy_torso_description.py` & `robot_descriptions-1.6.0/robot_descriptions/poppy_torso_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/pr2_description.py` & `robot_descriptions-1.6.0/robot_descriptions/pr2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/r2_description.py` & `robot_descriptions-1.6.0/robot_descriptions/r2_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/reachy_description.py` & `robot_descriptions-1.6.0/robot_descriptions/reachy_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/rhea_description.py` & `robot_descriptions-1.6.0/robot_descriptions/rhea_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_description.py` & `robot_descriptions-1.6.0/robot_descriptions/robotiq_2f85_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/robotiq_2f85_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/robotiq_2f85_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/romeo_description.py` & `robot_descriptions-1.6.0/robot_descriptions/romeo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/shadow_hand_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/shadow_hand_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/sigmaban_description.py` & `robot_descriptions-1.6.0/robot_descriptions/sigmaban_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/simple_humanoid_description.py` & `robot_descriptions-1.6.0/robot_descriptions/simple_humanoid_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/solo_description.py` & `robot_descriptions-1.6.0/robot_descriptions/solo_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/spryped_description.py` & `robot_descriptions-1.6.0/robot_descriptions/spryped_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/stretch_description.py` & `robot_descriptions-1.6.0/robot_descriptions/stretch_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/talos_description.py` & `robot_descriptions-1.6.0/robot_descriptions/talos_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/tiago_description.py` & `robot_descriptions-1.6.0/robot_descriptions/tiago_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/upkie_description.py` & `robot_descriptions-1.6.0/robot_descriptions/upkie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ur10_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ur10_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ur3_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ur3_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ur5_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ur5_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/ur5e_mj_description.py` & `robot_descriptions-1.6.0/robot_descriptions/ur5e_mj_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/valkyrie_description.py` & `robot_descriptions-1.6.0/robot_descriptions/valkyrie_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/yumi_description.py` & `robot_descriptions-1.6.0/robot_descriptions/yumi_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/robot_descriptions/z1_description.py` & `robot_descriptions-1.6.0/robot_descriptions/z1_description.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/__init__.py` & `robot_descriptions-1.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_idyntree.py` & `robot_descriptions-1.6.0/tests/loaders/test_idyntree.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_mujoco.py` & `robot_descriptions-1.6.0/tests/loaders/test_mujoco.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_pinocchio.py` & `robot_descriptions-1.6.0/tests/loaders/test_pinocchio.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
 from robot_descriptions._descriptions import DESCRIPTIONS
-
 from robot_descriptions.loaders.pinocchio import load_robot_description
 
+
 class TestPinocchio(unittest.TestCase):
 
     """
     Check that all descriptions are loaded properly in Pinocchio.
     """
 
     @staticmethod
@@ -40,14 +40,15 @@
         """
 
         def test(self):
             load_robot_description(description)
 
         return test
 
+
 # Add a test function for each URDF description
 for name, description in DESCRIPTIONS.items():
     if description.has_urdf:
         setattr(
             TestPinocchio,
             f"test_{name}",
             TestPinocchio.get_test_for_description(name),
```

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_pybullet.py` & `robot_descriptions-1.6.0/tests/loaders/test_pybullet.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_robomeshcat.py` & `robot_descriptions-1.6.0/tests/loaders/test_robomeshcat.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/loaders/test_yourdfpy.py` & `robot_descriptions-1.6.0/tests/loaders/test_yourdfpy.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/test_clone_to_cache.py` & `robot_descriptions-1.6.0/tests/test_clone_to_cache.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/test_clone_to_directory.py` & `robot_descriptions-1.6.0/tests/test_clone_to_directory.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/test_descriptions.py` & `robot_descriptions-1.6.0/tests/test_descriptions.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/test_loaders.py` & `robot_descriptions-1.6.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tests/test_progress_bar.py` & `robot_descriptions-1.6.0/tests/test_progress_bar.py`

 * *Files identical despite different names*

### Comparing `robot_descriptions-1.5.0/tox.ini` & `robot_descriptions-1.6.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -40,54 +40,54 @@
 commands =
     black --check --diff robot_descriptions
     ruff robot_descriptions
     pylint robot_descriptions --exit-zero --rcfile={toxinidir}/tox.ini
     mypy robot_descriptions --ignore-missing-imports
 
 [testenv:loader-idyntree]
+changedir = {toxinidir}/tests/loaders
 deps =
     idyntree >= 8.0.0
-    pytest
 commands =
-    pytest --import-mode=importlib tests/loaders/test_idyntree.py
+    python -m unittest test_idyntree.py
 
 [testenv:loader-mujoco]
+changedir = {toxinidir}/tests/loaders
 deps =
     mujoco >=2.2.1
-    pytest
 commands =
-    mujoco: pytest --import-mode=importlib tests/loaders/test_mujoco.py
+    python -m unittest test_mujoco.py
 
 [testenv:loader-pinocchio]
+changedir = {toxinidir}/tests/loaders
 deps =
     pin >=2.6.14
-    pytest
 commands =
-    pytest --import-mode=importlib tests/loaders/test_pinocchio.py
+    python -m unittest test_pinocchio.py
 
 [testenv:loader-pybullet]
+changedir = {toxinidir}/tests/loaders
 deps =
     numpy >=1.23.4
     pybullet >=3.2.5
-    pytest
 commands =
-    pytest --import-mode=importlib tests/loaders/test_pybullet.py
+    python -m unittest test_pybullet.py
 
 [testenv:loader-robomeshcat]
+changedir = {toxinidir}/tests/loaders
 deps =
     pycollada >=0.6
-    pytest
     robomeshcat >= 1.0.4
 commands =
-    pytest --import-mode=importlib tests/loaders/test_robomeshcat.py
+    python -m unittest test_robomeshcat.py
 
 [testenv:loader-yourdfpy]
+changedir = {toxinidir}/tests/loaders
 deps =
     numpy >=1.23.4
-    pytest
     trimesh ~=3.16.0
     yourdfpy >=0.0.53
 commands =
-    pytest --import-mode=importlib tests/loaders/test_yourdfpy.py
+    python -m unittest test_yourdfpy.py
 
 [pylint]
 generated-members=mujoco.MjModel, pin.JointModelFreeFlyer, pin.JointModelPX, pin.JointModelPY, pin.JointModelPZ, pin.JointModelPlanar, pin.JointModelRX, pin.JointModelRY, pin.JointModelRZ, pin.JointModelSpherical, pin.JointModelSphericalZYX, pin.JointModelTranslation, pin.Model, pybullet.loadURDF, pybullet.setAdditionalSearchPath
```

### Comparing `robot_descriptions-1.5.0/PKG-INFO` & `robot_descriptions-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot_descriptions
-Version: 1.5.0
+Version: 1.6.0
 Summary: Import open source robot description as Python modules.
 Keywords: robot,description,urdf,mjcf
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -154,25 +154,27 @@
 The DOF column denotes the number of actuated degrees of freedom.
 
 ### Arms
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `edo_description`             | e.DO                  | Comau                    | 6   | URDF       |
-| `gen2_description`            | Gen2                  | Kinova                   | 6   | URDF       |
-| `gen3_mj_description`         | Gen3                  | Kinova                   | 7   | MJCF       |
+| `fanuc_m710ic_description`    | M-710iC               | Fanuc                    | 6   | URDF       |
+| `gen2_description`            | Gen2 (Jaco)           | Kinova                   | 6   | URDF       |
+| `gen3_description`            | Gen3 (Jaco)           | Kinova                   | 6   | URDF       |
+| `gen3_mj_description`         | Gen3 (Jaco)           | Kinova                   | 7   | MJCF       |
 | `iiwa_description`            | iiwa                  | KUKA                     | 7   | URDF       |
 | `panda_description`           | Panda                 | Franka Emika             | 8   | URDF       |
 | `panda_mj_description`        | Panda                 | Franka Emika             | 8   | MJCF       |
 | `poppy_ergo_jr_description`   | Poppy Ergo Jr         | Poppy Project            | 6   | URDF       |
 | `ur10_description`            | UR10                  | Universal Robots         | 6   | URDF       |
 | `ur3_description`             | UR3                   | Universal Robots         | 6   | URDF       |
 | `ur5_description`             | UR5                   | Universal Robots         | 6   | URDF       |
 | `ur5e_mj_description`         | UR5e                  | Universal Robots         | 6   | MJCF       |
-| `z1_description`              | Z1                    | UNITREE Robotics         | 6  | URDF       |
+| `z1_description`              | Z1                    | UNITREE Robotics         | 6   | URDF       |
 
 ### Bipeds
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `bolt_description`            | Bolt                  | ODRI                     | 6   | URDF       |
 | `cassie_description`          | Cassie                | Agility Robotics         | 16  | URDF       |
@@ -199,14 +201,15 @@
 ### Educational
 
 | Name                          | Robot                 | DOF | Format     |
 |-------------------------------|-----------------------|-----|------------|
 | `double_pendulum_description` | Double Pendulum       | 2   | URDF       |
 | `finger_edu_description`      | FingerEdu             | 3   | URDF       |
 | `simple_humanoid_description` | Simple Humanoid       | 29  | URDF       |
+| `trifinger_edu_description`   | TriFingerEdu          | 9   | URDF       |
 
 ### End effectors
 
 | Name                          | Robot                 | Maker                    | DOF | Format     |
 |-------------------------------|-----------------------|--------------------------|-----|------------|
 | `allegro_hand_description`    | Allegro Hand          | Wonik Robotics           | 16  | URDF       |
 | `barrett_hand_description`    | BarrettHand           | Barrett Technology       | 8   | URDF       |
```

