# Comparing `tmp/novel_swarms-0.1.2a0.tar.gz` & `tmp/novel_swarms-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novel_swarms-0.1.2a0.tar", last modified: Mon May 22 16:06:08 2023, max compression
+gzip compressed data, was "novel_swarms-0.1.3a0.tar", last modified: Mon May 22 21:45:37 2023, max compression
```

## Comparing `novel_swarms-0.1.2a0.tar` & `novel_swarms-0.1.3a0.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/
--rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.2a0/.gitignore
--rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.2a0/LICENSE
--rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.2a0/MANIFEST.in
--rw-rw-r--   0 connor    (1001) connor    (1001)     6782 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     6242 2023-04-19 21:16:59.000000 novel_swarms-0.1.2a0/README.md
--rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.2a0/git.sh
--rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-05-22 16:06:00.000000 novel_swarms-0.1.2a0/pyproject.toml
--rw-rw-r--   0 connor    (1001) connor    (1001)     1061 2023-04-27 20:54:12.000000 novel_swarms-0.1.2a0/requirements.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/setup.cfg
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/agent/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1199 2023-05-17 17:50:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/Agent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1472 2023-05-19 17:51:10.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/AgentFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7341 2023-04-24 18:59:47.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/DiffDriveAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     6651 2023-04-27 23:29:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/DroneAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1208 2023-04-27 17:48:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/HumanAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4726 2023-05-12 20:50:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/LevyAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7272 2023-05-19 16:23:44.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/MazeAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      885 2023-05-17 18:40:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/ModeSwitchingAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/StaticAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     8166 2023-04-04 02:15:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/UnicycleAgent.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.2a0/src/novel_swarms/agent/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/behavior/
--rw-rw-r--   0 connor    (1001) connor    (1001)      993 2023-05-18 23:13:24.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AbstractBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AgentsAtGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1249 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AngularMomentum.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      583 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/AverageSpeed.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2604 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/BehaviorFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1340 2023-05-12 16:44:43.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/Centroid.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1621 2023-05-03 16:44:51.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/DistanceToGoal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/GroupRotationBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/PersistentHomology.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1746 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/RadialVariance.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1387 2023-04-24 22:53:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/ScatterBehavior.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      700 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorOffset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-05-19 16:08:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorRotation.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1514 2023-04-24 23:01:45.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorSignal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      616 2023-05-18 23:41:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/TotalCollisions.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/behavior/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/cache/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.2a0/src/novel_swarms/cache/ExternalSimulationArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/cache/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/config/
--rw-rw-r--   0 connor    (1001) connor    (1001)    13756 2023-05-19 17:55:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/AgentConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/EvolutionaryConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1513 2023-05-19 16:59:04.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/HeterogenSwarmConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)       56 2023-05-17 17:50:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/ModeConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/OutputTensorConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/ResultsConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4114 2023-05-19 17:03:21.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/WorldConfig.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1961 2023-05-19 18:43:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/config/defaults.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/gui/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      479 2023-05-12 21:01:36.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/abstractGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3431 2023-04-27 22:51:31.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/agentGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/connectivityGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4143 2023-05-15 22:49:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/controllerGUI.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.2a0/src/novel_swarms/gui/evolutionGUI.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/novelty/
--rw-rw-r--   0 connor    (1001) connor    (1001)    10186 2023-03-14 00:06:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/BehaviorDiscovery.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-03-14 00:05:33.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/GeneRule.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/NoveltyArchive.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3834 2023-03-13 23:07:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/novelty/evolve.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/optim/
--rw-rw-r--   0 connor    (1001) connor    (1001)     7106 2023-05-16 16:48:55.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/CMAES.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      113 2023-05-03 18:10:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/OptimVar.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-27 15:37:22.000000 novel_swarms-0.1.2a0/src/novel_swarms/optim/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/results/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6708 2023-03-13 23:21:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/Cluster.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/ClusterPoint.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/Trends.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4590 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/behavior_metrics.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      424 2023-03-13 23:23:49.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/results.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/domain_codomain.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/sensors/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/AbstractSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)    13602 2023-05-19 17:20:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryFOVSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4032 2023-05-19 17:21:38.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryLOSSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/GenomeDependentSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1973 2023-04-27 21:53:05.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/RegionalSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      710 2023-05-19 18:17:23.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1818 2023-05-19 18:16:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      319 2023-04-28 19:58:35.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/StaticSensor.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.2a0/src/novel_swarms/sensors/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AABB.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/CircularCollider.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/collider/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1832 2023-05-17 18:31:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/ControllerConverter.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1179 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/GenomeDataSet.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/ConvexHull.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1287 2023-05-05 19:12:46.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Point.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Polygon.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/labeler.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1707 2023-05-03 20:18:52.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/processing/multicoreprocessing.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/
--rw-rw-r--   0 connor    (1001) connor    (1001)     1809 2023-04-21 17:51:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/Signal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-21 17:17:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/signal/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.2a0/src/novel_swarms/util/timer.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms/world/
--rw-rw-r--   0 connor    (1001) connor    (1001)    16018 2023-05-18 23:51:03.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/RectangularWorld.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     3115 2023-05-18 22:57:09.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/World.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/WorldFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1315 2023-05-19 18:23:26.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/WorldIO.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/
--rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/Maze.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/generation/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/
--rw-rw-r--   0 connor    (1001) connor    (1001)     2165 2023-05-18 23:15:12.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/Goal.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      418 2023-05-19 15:51:16.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/GoalFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1128 2023-05-19 15:45:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/GrowthRegion.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/goals/__init__.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.744903 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/
--rw-rw-r--   0 connor    (1001) connor    (1001)      313 2023-05-19 15:48:02.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/ObjectFactory.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     1507 2023-05-19 15:45:54.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/Wall.py
--rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-05-19 15:46:02.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/WorldObject.py
--rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/objects/__init__.py
--rw-rw-r--   0 connor    (1001) connor    (1001)     4977 2023-05-18 23:51:23.000000 novel_swarms-0.1.2a0/src/novel_swarms/world/simulate.py
-drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 16:06:08.740903 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/
--rw-rw-r--   0 connor    (1001) connor    (1001)     6782 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/PKG-INFO
--rw-rw-r--   0 connor    (1001) connor    (1001)     4699 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/SOURCES.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/dependency_links.txt
--rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-05-22 16:06:08.000000 novel_swarms-0.1.2a0/src/novel_swarms.egg-info/top_level.txt
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      486 2023-04-18 02:45:46.000000 novel_swarms-0.1.3a0/.gitignore
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1107 2023-04-19 20:59:13.000000 novel_swarms-0.1.3a0/LICENSE
+-rw-rw-r--   0 connor    (1001) connor    (1001)       42 2022-09-19 15:01:24.000000 novel_swarms-0.1.3a0/MANIFEST.in
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6256 2023-05-22 21:45:25.000000 novel_swarms-0.1.3a0/README.md
+-rw-rw-r--   0 connor    (1001) connor    (1001)       72 2023-04-17 22:17:05.000000 novel_swarms-0.1.3a0/git.sh
+-rw-rw-r--   0 connor    (1001) connor    (1001)      617 2023-05-22 21:42:20.000000 novel_swarms-0.1.3a0/pyproject.toml
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1061 2023-04-27 20:54:12.000000 novel_swarms-0.1.3a0/requirements.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       38 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/setup.cfg
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.3a0/src/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-15 20:43:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/agent/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1199 2023-05-17 17:50:16.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/Agent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1472 2023-05-19 17:51:10.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/AgentFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7341 2023-04-24 18:59:47.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/DiffDriveAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6651 2023-04-27 23:29:00.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/DroneAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1208 2023-04-27 17:48:12.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/HumanAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4726 2023-05-12 20:50:55.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/LevyAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7272 2023-05-19 16:23:44.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/MazeAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      885 2023-05-17 18:40:54.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/ModeSwitchingAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2595 2023-03-04 01:21:09.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/StaticAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     8166 2023-04-04 02:15:06.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/UnicycleAgent.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:30.000000 novel_swarms-0.1.3a0/src/novel_swarms/agent/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/behavior/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      993 2023-05-18 23:13:24.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/AbstractBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2085 2023-04-04 14:55:04.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/AgentsAtGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1249 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/AlgebraicConnectivity.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1196 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/AngularMomentum.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      583 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/AverageSpeed.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2604 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/BehaviorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1340 2023-05-12 16:44:43.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/Centroid.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3349 2023-04-18 15:30:56.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1621 2023-05-03 16:44:51.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/DistanceToGoal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1176 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/GroupRotationBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1849 2023-04-18 19:46:18.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/PersistentHomology.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1746 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/RadialVariance.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1387 2023-04-24 22:53:06.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/ScatterBehavior.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      700 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorOffset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-05-19 16:08:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorRotation.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1514 2023-04-24 23:01:45.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorSignal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      616 2023-05-18 23:41:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/TotalCollisions.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:40.000000 novel_swarms-0.1.3a0/src/novel_swarms/behavior/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/cache/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1681 2023-01-17 23:54:56.000000 novel_swarms-0.1.3a0/src/novel_swarms/cache/ExternalSimulationArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 22:42:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/cache/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/config/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13756 2023-05-19 17:55:12.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/AgentConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1800 2023-03-13 23:06:38.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/EvolutionaryConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2470 2023-05-22 17:57:25.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/HeterogenSwarmConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)       56 2023-05-17 17:50:16.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/ModeConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      637 2023-01-20 15:33:41.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/OutputTensorConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      520 2022-09-15 20:43:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/ResultsConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4155 2023-05-22 18:50:28.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/WorldConfig.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:49.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1961 2023-05-19 18:43:55.000000 novel_swarms-0.1.3a0/src/novel_swarms/config/defaults.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/gui/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:31:58.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      479 2023-05-12 21:01:36.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/abstractGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3431 2023-04-27 22:51:31.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/agentGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2401 2022-12-07 17:37:58.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/connectivityGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4143 2023-05-15 22:49:40.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/controllerGUI.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2670 2022-09-16 18:13:19.000000 novel_swarms-0.1.3a0/src/novel_swarms/gui/evolutionGUI.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/novelty/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    10678 2023-05-22 17:43:57.000000 novel_swarms-0.1.3a0/src/novel_swarms/novelty/BehaviorDiscovery.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7812 2023-05-22 17:42:55.000000 novel_swarms-0.1.3a0/src/novel_swarms/novelty/GeneRule.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3931 2022-10-26 23:42:12.000000 novel_swarms-0.1.3a0/src/novel_swarms/novelty/NoveltyArchive.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:05.000000 novel_swarms-0.1.3a0/src/novel_swarms/novelty/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3884 2023-05-22 17:31:33.000000 novel_swarms-0.1.3a0/src/novel_swarms/novelty/evolve.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms/optim/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     7106 2023-05-16 16:48:55.000000 novel_swarms-0.1.3a0/src/novel_swarms/optim/CMAES.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      113 2023-05-03 18:10:54.000000 novel_swarms-0.1.3a0/src/novel_swarms/optim/OptimVar.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-27 15:37:22.000000 novel_swarms-0.1.3a0/src/novel_swarms/optim/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/results/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6926 2023-05-22 18:21:21.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/Cluster.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      612 2022-10-10 15:58:53.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/ClusterPoint.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2728 2023-03-13 21:38:40.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/Trends.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:12.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4590 2023-04-19 21:01:00.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/behavior_metrics.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      474 2023-05-22 18:28:05.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/results.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/results/scripts/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/scripts/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4869 2022-09-16 18:58:24.000000 novel_swarms-0.1.3a0/src/novel_swarms/results/scripts/domain_codomain.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/sensors/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1021 2023-01-23 17:59:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/AbstractSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)    13602 2023-05-19 17:20:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/BinaryFOVSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4032 2023-05-19 17:21:38.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/BinaryLOSSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1779 2023-03-14 00:02:26.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/GenomeDependentSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1973 2023-04-27 21:53:05.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/RegionalSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      710 2023-05-19 18:17:23.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/SensorFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1818 2023-05-19 18:16:53.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/SensorSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      319 2023-04-28 19:58:35.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/StaticSensor.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:21.000000 novel_swarms-0.1.3a0/src/novel_swarms/sensors/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:29.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/collider/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1072 2023-03-04 01:09:15.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/collider/AABB.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2396 2023-03-13 18:33:33.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/collider/AngleSensitiveCC.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1024 2023-04-18 16:06:10.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/collider/CircularCollider.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/collider/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/conversion/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1832 2023-05-17 18:31:53.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/conversion/ControllerConverter.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-19 21:00:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/conversion/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1179 2023-04-19 21:01:00.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/DiffDriveDataset.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1553 2022-09-15 20:43:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/GenomeDataSet.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5151 2023-04-17 22:41:54.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/ConvexHull.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1287 2023-05-05 19:12:46.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/Point.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1184 2023-04-17 21:58:13.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/Polygon.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3058 2023-04-19 21:01:00.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/labeler.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/processing/
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:39.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/processing/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1707 2023-05-03 20:18:52.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/processing/multicoreprocessing.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/util/signal/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1809 2023-04-21 17:51:53.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/signal/Signal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-04-21 17:17:09.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/signal/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      549 2023-03-30 19:03:58.000000 novel_swarms-0.1.3a0/src/novel_swarms/util/timer.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/world/
+-rw-rw-r--   0 connor    (1001) connor    (1001)    16018 2023-05-18 23:51:03.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/RectangularWorld.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     3115 2023-05-18 22:57:09.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/World.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      273 2022-09-19 15:08:06.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/WorldFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1325 2023-05-22 19:16:38.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/WorldIO.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2022-09-16 17:32:45.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/world/generation/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     5347 2023-01-17 20:19:42.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/generation/Maze.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 17:04:53.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/generation/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/world/goals/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     2165 2023-05-18 23:15:12.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/goals/Goal.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      418 2023-05-19 15:51:16.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/goals/GoalFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1128 2023-05-19 15:45:54.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/goals/GrowthRegion.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 20:36:43.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/goals/__init__.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.500108 novel_swarms-0.1.3a0/src/novel_swarms/world/objects/
+-rw-rw-r--   0 connor    (1001) connor    (1001)      313 2023-05-19 15:48:02.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/objects/ObjectFactory.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     1507 2023-05-19 15:45:54.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/objects/Wall.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)      320 2023-05-19 15:46:02.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/objects/WorldObject.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)        0 2023-01-17 16:14:14.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/objects/__init__.py
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4977 2023-05-18 23:51:23.000000 novel_swarms-0.1.3a0/src/novel_swarms/world/simulate.py
+drwxrwxr-x   0 connor    (1001) connor    (1001)        0 2023-05-22 21:45:37.496108 novel_swarms-0.1.3a0/src/novel_swarms.egg-info/
+-rw-rw-r--   0 connor    (1001) connor    (1001)     6796 2023-05-22 21:45:37.000000 novel_swarms-0.1.3a0/src/novel_swarms.egg-info/PKG-INFO
+-rw-rw-r--   0 connor    (1001) connor    (1001)     4699 2023-05-22 21:45:37.000000 novel_swarms-0.1.3a0/src/novel_swarms.egg-info/SOURCES.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)        1 2023-05-22 21:45:37.000000 novel_swarms-0.1.3a0/src/novel_swarms.egg-info/dependency_links.txt
+-rw-rw-r--   0 connor    (1001) connor    (1001)       22 2023-05-22 21:45:37.000000 novel_swarms-0.1.3a0/src/novel_swarms.egg-info/top_level.txt
```

### Comparing `novel_swarms-0.1.2a0/LICENSE` & `novel_swarms-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/PKG-INFO` & `novel_swarms-0.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: novel_swarms
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Connor Mattson, Daniel S. Brown
+Contributors: Connor Mattson, Jeremy Clark, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.2a0/README.md` & `novel_swarms-0.1.3a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Connor Mattson, Daniel S. Brown
+Contributors: Connor Mattson, Jeremy Clark, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.2a0/pyproject.toml` & `novel_swarms-0.1.3a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "novel_swarms"
-version = "0.1.2-alpha"
+version = "0.1.3-alpha"
 authors = [
   { name="Connor Mattson", email="c.mattson@utah.edu" },
 ]
 description = "A Swarm Simulation Package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `novel_swarms-0.1.2a0/requirements.txt` & `novel_swarms-0.1.3a0/requirements.txt`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/Agent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/Agent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/AgentFactory.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/DiffDriveAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/DiffDriveAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/DroneAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/DroneAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/HumanAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/HumanAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/LevyAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/LevyAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/MazeAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/MazeAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/ModeSwitchingAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/ModeSwitchingAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/StaticAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/StaticAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/agent/UnicycleAgent.py` & `novel_swarms-0.1.3a0/src/novel_swarms/agent/UnicycleAgent.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AbstractBehavior.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/AbstractBehavior.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AgentsAtGoal.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/AgentsAtGoal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AlgebraicConnectivity.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/AlgebraicConnectivity.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AngularMomentum.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/AngularMomentum.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/AverageSpeed.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/AverageSpeed.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/BehaviorFactory.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/BehaviorFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/Centroid.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/Centroid.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/ConvexHull.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/DistanceToGoal.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/DistanceToGoal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/GroupRotationBehavior.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/GroupRotationBehavior.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/PersistentHomology.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/PersistentHomology.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/RadialVariance.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/RadialVariance.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/ScatterBehavior.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/ScatterBehavior.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorOffset.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorOffset.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorRotation.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorRotation.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/SensorSignal.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/SensorSignal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/behavior/TotalCollisions.py` & `novel_swarms-0.1.3a0/src/novel_swarms/behavior/TotalCollisions.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/cache/ExternalSimulationArchive.py` & `novel_swarms-0.1.3a0/src/novel_swarms/cache/ExternalSimulationArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/AgentConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/AgentConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/EvolutionaryConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/EvolutionaryConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/HeterogenSwarmConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/HeterogenSwarmConfig.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,20 @@
     def __init__(self):
         self.subpopulation_information = {}
         self.world = None
 
     def add_sub_populuation(self, config, count):
         self.subpopulation_information[config] = count
 
+    def get_configs(self):
+        return self.subpopulation_information.keys()
+
+    def get_counts(self):
+        return self.subpopulation_information.values()
+
     def build_agent_population(self):
         population = []
         for key in self.subpopulation_information:
             for n in range(self.subpopulation_information[key]):
                 agent = AgentFactory.create(key)
                 population.append(agent)
         return population
@@ -44,7 +50,36 @@
 
         i = 0
         for config in configs:
             ret.add_sub_populuation(config, counts[i])
             i += 1
 
         return ret
+
+    def clone(self):
+        return HeterogeneousSwarmConfig.from_dict(self.as_dict())
+
+    def from_n_species_controller(self, c):
+        import math
+        configs = list(self.get_configs())
+        cA, cB, ratio = c[0:4], c[4:8], c[8]
+
+        # Correctly Subdivide Population
+        print(c)
+        n_agents = sum(list(self.get_counts()))
+        if math.isnan(ratio):
+            ratio = 0.5
+        v = n_agents * ratio
+        n_A, n_B = math.ceil(v), n_agents - math.floor(v)
+
+        # Assign Genome Controllers
+        print(configs)
+        configs[0].controller = cA
+        configs[1].controller = cB
+
+        # Re-attach Config
+        self.subpopulation_information = {}
+        self.add_sub_populuation(configs[0], n_A)
+        self.add_sub_populuation(configs[1], n_B)
+
+
+
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/OutputTensorConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/OutputTensorConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/ResultsConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/ResultsConfig.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/WorldConfig.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/WorldConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             "show_walls": self.show_walls,
             "collide_walls": self.collide_walls,
             "stop_at": self.stop_at,
             "objects": [o.as_config_dict() for o in self.objects],
             "goals": [g.as_config_dict() for g in self.goals],
             "background_color": self.background_color,
             "metadata": self.metadata,
-            "agent_init": self.agent_init
+            "agent_init": self.agent_init if hasattr(self, "agent_init") else None
         }
 
     @staticmethod
     def from_dict(d):
         from src.novel_swarms.world.objects.ObjectFactory import ObjectFactory
         from src.novel_swarms.world.goals.GoalFactory import GoalFactory
         from src.novel_swarms.behavior.BehaviorFactory import BehaviorFactory
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/config/defaults.py` & `novel_swarms-0.1.3a0/src/novel_swarms/config/defaults.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/gui/agentGUI.py` & `novel_swarms-0.1.3a0/src/novel_swarms/gui/agentGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/gui/connectivityGUI.py` & `novel_swarms-0.1.3a0/src/novel_swarms/gui/connectivityGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/gui/controllerGUI.py` & `novel_swarms-0.1.3a0/src/novel_swarms/gui/controllerGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/gui/evolutionGUI.py` & `novel_swarms-0.1.3a0/src/novel_swarms/gui/evolutionGUI.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/novelty/BehaviorDiscovery.py` & `novel_swarms-0.1.3a0/src/novel_swarms/novelty/BehaviorDiscovery.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 import random
 import numpy as np
 from .NoveltyArchive import NoveltyArchive
+from ..config.HeterogenSwarmConfig import HeterogeneousSwarmConfig
 from ..results.Trends import Trends
 from ..world.WorldFactory import WorldFactory
 from ..cache.ExternalSimulationArchive import ExternalSimulationArchive
 from ..util.timer import Timer
 
 
 class BehaviorDiscovery:
@@ -60,23 +61,31 @@
     def initializePopulation(self):
         self.population = np.array([
             self.gene_builder.fetch_random_genome() for j in range(self.population_size)
         ])
         self.scores = np.array([0.0 for i in range(self.population_size)])
         self.behavior = np.array([[-1.0 for j in range(len(self.behavior_config))] for i in range(self.population_size)])
 
-    def runSinglePopulation(self, screen=None, i=0, save=True, genome=None, seed=None, output_config=None):
+    def runSinglePopulation(self, screen=None, i=0, save=True, genome=None, seed=None, output_config=None, heterogeneous=False):
         """
         Evaluates the Novelty of a Single Genome located at the ith index
         """
+        print(f"Ratio Rule: {self.gene_builder.rules[-1].domain}")
         if genome is None:
             genome = self.population[i]
 
         self.status = "Simulation"
-        self.world_config.agentConfig.controller = genome
+        if not heterogeneous:
+            self.world_config.agentConfig.controller = genome
+        else:
+            # Currently Assumes Two Species Only
+            self.world_config.agentConfig.from_n_species_controller(genome)
+            self.world_config.agentConfig = self.world_config.agentConfig.clone()
+            self.world_config.agentConfig.attach_world_config(self.world_config)
+
         for key in self.genome_dependent_world:
             print("Setting Key!", key, " with Value: ", genome[self.genome_dependent_world[key]])
             setattr(self.world_config, key, genome[self.genome_dependent_world[key]])
 
         behavior = None
         output = None
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/novelty/GeneRule.py` & `novel_swarms-0.1.3a0/src/novel_swarms/novelty/GeneRule.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/novelty/NoveltyArchive.py` & `novel_swarms-0.1.3a0/src/novel_swarms/novelty/NoveltyArchive.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/novelty/evolve.py` & `novel_swarms-0.1.3a0/src/novel_swarms/novelty/evolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..gui.evolutionGUI import EvolutionGUI
 from .BehaviorDiscovery import BehaviorDiscovery
 
 FRAMERATE = 200
 GUI_WIDTH = 200
 
 
-def main(config: GeneticEvolutionConfig, output_config=None):
+def main(config: GeneticEvolutionConfig, output_config=None, heterogeneous=False):
 
     # initialize the pygame module
     pygame.init()
     pygame.display.set_caption("Evolutionary Novelty Search")
 
     # screen must be global so that other modules can access + draw to the window
     width = config.world_config.w
@@ -74,15 +74,15 @@
 
             if not running:
                 break
 
             screen.fill((0, 0, 0))
 
             evolution.curr_genome = i
-            evolution.runSinglePopulation(screen=screen, i=i, seed=i, output_config=output_config)
+            evolution.runSinglePopulation(screen=screen, i=i, seed=i, output_config=output_config, heterogeneous=heterogeneous)
 
             if config.show_gui:
                 gui.draw(screen=screen)
 
             pygame.display.flip()
 
             # Limit the FPS of the simulation to FRAMERATE
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/optim/CMAES.py` & `novel_swarms-0.1.3a0/src/novel_swarms/optim/CMAES.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/results/Cluster.py` & `novel_swarms-0.1.3a0/src/novel_swarms/results/Cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,30 @@
         (211, 84, 0),  # DARKER ORANGE
         (64, 224, 208),  # CYAN
         (125, 206, 160),  # MINT
         (34, 153, 84),  # GREEN
         (133, 146, 158),  # GREY
     ]
 
-    def __init__(self, config: ResultsConfig, world_metadata=None):
+    def __init__(self, config: ResultsConfig, world_metadata=None, heterogeneous=False):
 
         archive = config.archive
         if archive is None or not issubclass(type(archive), NoveltyArchive):
             raise Exception("Object of type NoveltyArchive must be provided to the Cluster Class")
         self.archive = archive
         self.reduced = np.array([])
         self.point_population = []
         self.center_population = []
         self.cluster_indices = []
         self.cluster_medoids = []
         self.medoid_genomes = []
         self.world_config = config.world
         self.world_metadata = world_metadata
         self.results_config = config
+        self.heterogeneous = heterogeneous
 
         self.initTSNE()
         self.clustering()
         self.pointMapping()
 
     def initTSNE(self):
         """
@@ -125,15 +126,19 @@
             dist = np.linalg.norm(click_point - poi)
             if dist < self.MEDOID_RADIUS:
                 controller = self.archive.genotypes[i]
                 from ..world.simulate import main
                 print(f"Display Controller: {controller}")
 
                 metadata = self.sync_metadata_with_controller(controller)
-                self.world_config.agentConfig.controller = controller
+                if self.heterogeneous:
+                    self.world_config.agentConfig.from_n_species_controller(controller)
+                else:
+                    self.world_config.agentConfig.controller = controller
+
                 self.world_config.set_attributes(metadata)
 
                 main(world_config=self.world_config)
                 return
 
     def runDisplayLoop(self, screen):
         running = True
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/results/ClusterPoint.py` & `novel_swarms-0.1.3a0/src/novel_swarms/results/ClusterPoint.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/results/Trends.py` & `novel_swarms-0.1.3a0/src/novel_swarms/results/Trends.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/results/behavior_metrics.py` & `novel_swarms-0.1.3a0/src/novel_swarms/results/behavior_metrics.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/results/scripts/domain_codomain.py` & `novel_swarms-0.1.3a0/src/novel_swarms/results/scripts/domain_codomain.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/AbstractSensor.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/AbstractSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryFOVSensor.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/BinaryFOVSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/BinaryLOSSensor.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/BinaryLOSSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/GenomeDependentSensor.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/GenomeDependentSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/RegionalSensor.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/RegionalSensor.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorFactory.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/SensorFactory.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/sensors/SensorSet.py` & `novel_swarms-0.1.3a0/src/novel_swarms/sensors/SensorSet.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AABB.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/collider/AABB.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/AngleSensitiveCC.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/collider/AngleSensitiveCC.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/collider/CircularCollider.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/collider/CircularCollider.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/conversion/ControllerConverter.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/conversion/ControllerConverter.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/DiffDriveDataset.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/DiffDriveDataset.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/datasets/GenomeDataSet.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/datasets/GenomeDataSet.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/ConvexHull.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/ConvexHull.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Point.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/geometry/Polygon.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/labeler.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/labeler.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/processing/multicoreprocessing.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/processing/multicoreprocessing.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/signal/Signal.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/signal/Signal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/util/timer.py` & `novel_swarms-0.1.3a0/src/novel_swarms/util/timer.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/RectangularWorld.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/RectangularWorld.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/World.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/World.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/WorldIO.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/WorldIO.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,9 +37,9 @@
 
 
 
 """
 Given a File, JSON_WORLD, simulate the entire experiment with a single function call
 """
 if __name__ == "__main__":
-    JSON_WORLD = "../../../demo/results/experiments/heterogeneous_behaviors/2_Species_Engulfing.json"
+    JSON_WORLD = "../../../demo/results/experiments/heterogeneous_behaviors/embedded-cycles-heterogeneous.json"
     WorldIO.sim_from_json(JSON_WORLD)
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/generation/Maze.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/generation/Maze.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/goals/Goal.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/goals/Goal.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/goals/GrowthRegion.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/goals/GrowthRegion.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/objects/Wall.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/objects/Wall.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms/world/simulate.py` & `novel_swarms-0.1.3a0/src/novel_swarms/world/simulate.py`

 * *Files identical despite different names*

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms.egg-info/PKG-INFO` & `novel_swarms-0.1.3a0/src/novel_swarms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: novel-swarms
-Version: 0.1.2a0
+Version: 0.1.3a0
 Summary: A Swarm Simulation Package
 Author-email: Connor Mattson <c.mattson@utah.edu>
 Project-URL: Homepage, https://github.com/Connor-Mattson/RobotSwarmSimulator
 Project-URL: Bug Tracker, https://github.com/Connor-Mattson/RobotSwarmSimulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Novel Behavior Discovery in Computation Free Swarms
-Contributors: Connor Mattson, Daniel S. Brown
+Contributors: Connor Mattson, Jeremy Clark, Daniel S. Brown
 
 ## Required Software
 - Python & Pip
 - External Python Packages as defined in [requirements.txt](requirements.txt) 
 
 ## Setup
 Install Python Packages
```

### Comparing `novel_swarms-0.1.2a0/src/novel_swarms.egg-info/SOURCES.txt` & `novel_swarms-0.1.3a0/src/novel_swarms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

