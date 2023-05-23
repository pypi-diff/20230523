# Comparing `tmp/edgerun-galileo-experiments-0.0.2.dev8.tar.gz` & `tmp/edgerun-galileo-experiments-0.0.2.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgerun-galileo-experiments-0.0.2.dev8.tar", last modified: Sun Jul 17 17:28:58 2022, max compression
+gzip compressed data, was "edgerun-galileo-experiments-0.0.2.dev9.tar", last modified: Wed Jul 27 14:48:32 2022, max compression
```

## Comparing `edgerun-galileo-experiments-0.0.2.dev8.tar` & `edgerun-galileo-experiments-0.0.2.dev9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.532011 edgerun-galileo-experiments-0.0.2.dev8/
--rw-r--r--   0 philipp   (1000) philipp   (1000)     1065 2022-03-24 12:03:14.000000 edgerun-galileo-experiments-0.0.2.dev8/LICENSE
--rw-r--r--   0 philipp   (1000) philipp   (1000)     8849 2022-07-17 17:28:58.532011 edgerun-galileo-experiments-0.0.2.dev8/PKG-INFO
--rw-r--r--   0 philipp   (1000) philipp   (1000)     8388 2022-03-30 11:23:25.000000 edgerun-galileo-experiments-0.0.2.dev8/README.md
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.530011 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/
--rw-r--r--   0 philipp   (1000) philipp   (1000)     8849 2022-07-17 17:28:58.000000 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/PKG-INFO
--rw-r--r--   0 philipp   (1000) philipp   (1000)      907 2022-07-17 17:28:58.000000 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 philipp   (1000) philipp   (1000)        1 2022-07-17 17:28:58.000000 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 philipp   (1000) philipp   (1000)      186 2022-07-17 17:28:58.000000 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/requires.txt
--rw-r--r--   0 philipp   (1000) philipp   (1000)       19 2022-07-17 17:28:58.000000 edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/top_level.txt
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.530011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-24 12:31:31.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/__init__.py
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.531011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-24 16:45:21.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/__init__.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     4949 2022-07-17 15:53:51.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/model.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)      607 2022-07-06 15:36:18.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/profiling.py
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.531011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2021-09-07 13:13:38.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/__init__.py
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.531011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/profiling/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-28 12:42:44.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/profiling/__init__.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     8104 2022-07-17 16:03:51.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/profiling/run.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     3035 2022-07-17 10:01:58.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/run.py
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.531011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/scenario/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-07-06 15:36:18.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/scenario/__init__.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     7001 2022-07-17 15:13:04.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/scenario/run.py
-drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-17 17:28:58.532011 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/
--rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-22 08:22:41.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/__init__.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)      803 2022-07-15 20:11:22.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/arrivalprofile.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)      456 2022-03-22 08:22:41.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/constants.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     4106 2022-07-17 15:39:54.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/helpers.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)     7713 2022-07-17 17:28:03.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/k8s.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)      188 2022-03-28 12:47:42.000000 edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/rds.py
--rw-r--r--   0 philipp   (1000) philipp   (1000)       38 2022-07-17 17:28:58.532011 edgerun-galileo-experiments-0.0.2.dev8/setup.cfg
--rw-r--r--   0 philipp   (1000) philipp   (1000)     1013 2022-07-17 16:07:44.000000 edgerun-galileo-experiments-0.0.2.dev8/setup.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.532620 edgerun-galileo-experiments-0.0.2.dev9/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     1065 2022-03-24 12:03:14.000000 edgerun-galileo-experiments-0.0.2.dev9/LICENSE
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     8849 2022-07-27 14:48:32.532620 edgerun-galileo-experiments-0.0.2.dev9/PKG-INFO
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     8388 2022-03-30 11:23:25.000000 edgerun-galileo-experiments-0.0.2.dev9/README.md
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.530620 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     8849 2022-07-27 14:48:32.000000 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      907 2022-07-27 14:48:32.000000 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        1 2022-07-27 14:48:32.000000 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      186 2022-07-27 14:48:32.000000 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/requires.txt
+-rw-r--r--   0 philipp   (1000) philipp   (1000)       19 2022-07-27 14:48:32.000000 edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/top_level.txt
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.530620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-24 12:31:31.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/__init__.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.530620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-24 16:45:21.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/__init__.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     4949 2022-07-27 12:53:58.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/model.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      607 2022-07-06 15:36:18.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/profiling.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.530620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2021-09-07 13:13:38.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/__init__.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.531620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/profiling/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-28 12:42:44.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/profiling/__init__.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     8271 2022-07-27 14:46:31.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/profiling/run.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     3035 2022-07-17 10:01:58.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/run.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.531620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/scenario/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-07-06 15:36:18.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/scenario/__init__.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     7194 2022-07-27 14:48:01.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/scenario/run.py
+drwxr-xr-x   0 philipp   (1000) philipp   (1000)        0 2022-07-27 14:48:32.531620 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/
+-rw-r--r--   0 philipp   (1000) philipp   (1000)        0 2022-03-22 08:22:41.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/__init__.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      803 2022-07-15 20:11:22.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/arrivalprofile.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      456 2022-03-22 08:22:41.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/constants.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     4106 2022-07-27 12:53:58.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/helpers.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     8278 2022-07-27 14:46:31.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/k8s.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)      188 2022-03-28 12:47:42.000000 edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/rds.py
+-rw-r--r--   0 philipp   (1000) philipp   (1000)       38 2022-07-27 14:48:32.532620 edgerun-galileo-experiments-0.0.2.dev9/setup.cfg
+-rw-r--r--   0 philipp   (1000) philipp   (1000)     1013 2022-07-27 14:45:19.000000 edgerun-galileo-experiments-0.0.2.dev9/setup.py
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/LICENSE` & `edgerun-galileo-experiments-0.0.2.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/PKG-INFO` & `edgerun-galileo-experiments-0.0.2.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgerun-galileo-experiments
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: Galileo Experiments
 Home-page: https://github.com/edgerun/galileo-experiments
 Author: Philipp Raith, Thomas Rausch
 Author-email: p.raith@dsg.tuwien.ac.at, t.rausch@dsg.tuwien.ac.at
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/README.md` & `edgerun-galileo-experiments-0.0.2.dev9/README.md`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/PKG-INFO` & `edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgerun-galileo-experiments
-Version: 0.0.2.dev8
+Version: 0.0.2.dev9
 Summary: Galileo Experiments
 Home-page: https://github.com/edgerun/galileo-experiments
 Author: Philipp Raith, Thomas Rausch
 Author-email: p.raith@dsg.tuwien.ac.at, t.rausch@dsg.tuwien.ac.at
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/edgerun_galileo_experiments.egg-info/SOURCES.txt` & `edgerun-galileo-experiments-0.0.2.dev9/edgerun_galileo_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/model.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/model.py`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/api/profiling.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/api/profiling.py`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/profiling/run.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/profiling/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,21 @@
 
     try:
         labels = {
             function_label: config.app_name,
             zone_label: config.zone
         }
 
-        pod_names = spawn_pods(image, pod_prefix, host, labels, no_pods, config.app_workload_config.pod_factory)
+        lb_pods = get_load_balancer_pods()
+        env_vars = {
+            'API_GATEWAY': lb_pods[config.zone].ip
+        }
+
+        pod_names = spawn_pods(image, pod_prefix, host, labels, no_pods, config.app_workload_config.pod_factory,
+                               env_vars)
         pods = get_pods(pod_names)
 
         logger.info("Set weights for Pod(s)")
         pods_per_fn_and_cluster = {
             (name, config.zone): pods
         }
         lb_pods = get_load_balancer_pods()
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/run.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/run.py`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/experiment/scenario/run.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/experiment/scenario/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,34 @@
 from galileoexperiments.utils.constants import function_label, zone_label
 from galileoexperiments.utils.helpers import EtcdClient, update_weights
 from galileoexperiments.utils.k8s import spawn_pods, get_pods, remove_pods, get_load_balancer_pods
 
 logger = logging.getLogger(__name__)
 
 
-def spawn_pods_for_config(workload_config: ScenarioWorkloadConfiguration) -> List[Pod]:
+def spawn_pods_for_config(workload_config: ScenarioWorkloadConfiguration, lb_pods: Dict[str, str]) -> List[Pod]:
     pod_names = []
     for host, values in workload_config.services.items():
         for image, no_pods in values.items():
             name = workload_config.app_names[image]
 
+            zone = workload_config.zone_mapping[host]
             labels = {
                 function_label: name,
-                zone_label: workload_config.zone_mapping[host]
+                zone_label: zone
             }
+
+            env_vars = {
+                'API_GATEWAY': lb_pods[zone]
+            }
+
             profiling_app = workload_config.profiling_apps[image]
             pod_name_prefix = f'{name}-deployment'
-            names = spawn_pods(image, pod_name_prefix, host, labels, no_pods, profiling_app.pod_factory)
+            names = spawn_pods(image, pod_name_prefix, host, labels, no_pods, profiling_app.pod_factory,
+                               env_vars=env_vars)
             pod_names.extend(names)
     return get_pods(pod_names)
 
 
 def _map_pods_to_dict(pods: List[Pod]) -> Dict[Tuple[str, str], List[Pod]]:
     pods_map = {}
     for pod in pods:
@@ -125,15 +132,15 @@
     lb_ips = {}
     for zone, pod in lb_pods.items():
         lb_ips[zone] = pod.ip
 
     workload_config.lb_ips = lb_ips
     try:
         client_groups, requests = prepare_client_groups_for_services(workload_config)
-        pods = spawn_pods_for_config(workload_config)
+        pods = spawn_pods_for_config(workload_config, lb_ips)
 
         pods_per_fn_and_cluster = _map_pods_to_dict(pods)
 
         etcd_service_keys = set_loadbalancer_weights(pods_per_fn_and_cluster, lb_pods)
         rtbl_services = set_rtbl(list(workload_config.app_names.values()), workload_config.lb_ips, rtbl)
 
         set_params(workload_config)
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/arrivalprofile.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/arrivalprofile.py`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/helpers.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/galileoexperiments/utils/k8s.py` & `edgerun-galileo-experiments-0.0.2.dev9/galileoexperiments/utils/k8s.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import logging
 import time
-from dataclasses import dataclass
 from typing import List, Dict, Callable
 
 import kubernetes
+from galileoexperiments.api.model import Pod
+from galileoexperiments.utils.constants import zone_label
 from kubernetes import client, config
 from kubernetes.client import V1Deployment, V1ObjectMeta, V1DeploymentSpec, V1LabelSelector, V1PodTemplateSpec, \
     V1PodSpec, V1Toleration, V1Container, V1EnvFromSource, V1ConfigMapEnvSource
-from kubernetes.client import V1ResourceRequirements, V1EnvVar, V1EnvVarSource, V1ObjectFieldSelector
-
-from galileoexperiments.api.model import Pod
-from galileoexperiments.utils.constants import zone_label
+from kubernetes.client import V1EnvVar
 
 logger = logging.getLogger(__name__)
 
 
 def start_telemd_kubernetes_adapter(master_node: str) -> V1Deployment:
     # Configs can be set in Configuration class directly or using helper utility
     config.load_kube_config()
@@ -69,15 +67,15 @@
     # Configs can be set in Configuration class directly or using helper utility
     config.load_kube_config()
 
     v1 = client.AppsV1Api()
     v1.delete_namespaced_deployment(name='telemd-kubernetes-adapter', namespace='default')
 
 
-def get_pods(pod_names: List[str], v1: client.CoreV1Api=None) -> List[Pod]:
+def get_pods(pod_names: List[str], v1: client.CoreV1Api = None) -> List[Pod]:
     if v1 is None:
         config.load_kube_config()
         v1 = client.CoreV1Api()
     pod_list = v1.list_namespaced_pod("default")
     pods = []
     for pod in pod_list.items:
         if pod.metadata.name in pod_names:
@@ -90,42 +88,60 @@
             pod_id = pod.metadata.uid
             name = pod.metadata.name
             pods.append(Pod(pod_id, ip, labels, name))
 
     return pods
 
 
-def spawn_pods(image: str, name: str, node: str, labels: Dict[str, str], n: int, pod_factory: Callable[[str, str, Dict], client.V1Container]) -> List[str]:
+def spawn_pods(image: str, name: str, node: str, labels: Dict[str, str], n: int,
+               pod_factory: Callable[[str, str, Dict], client.V1Container], env_vars: Dict[str,str]= None) -> List[str]:
     """
     Function spawns n pods on the given node. The pod factory creates the containers to allow
     different kinds of containers.
     :param image: the container imag
     :param name: the pod name prefix
     :param node: the node
     :param labels: labels to attach
     :param n: the number of pods to spawn on the given node
     :param pod_factory: factory function to create V1Containers
+    :param env_vars: a dict containing env variables that will be available in each Pod
     :return: a list containing the names of pods created
     """
     # Configs can be set in Configuration class directly or using helper utility
     config.load_kube_config()
     resource_requests = {}
     v1 = client.CoreV1Api()
     pods = []
     for idx in range(n):
         selector = {'kubernetes.io/hostname': node}
         pod_name = f'{name}-{node}-{idx}'
+        container = pod_factory(pod_name, image, resource_requests)
+
+        if env_vars is not None:
+            for k, v in env_vars.items():
+                container.env.append(V1EnvVar(k, v))
+
         pod = client.V1Pod(
             api_version="v1",
             kind="Pod",
             metadata=client.V1ObjectMeta(name=pod_name, labels=labels),
             spec=client.V1PodSpec(
                 node_selector=selector,
                 containers=[
-                    pod_factory(pod_name, image, resource_requests)
+                    container
+                ],
+                volumes=[
+                    {
+                        'name': 'podinfo',
+                        'downwardAPI': {
+                            'items': [
+                                {'path': 'labels', 'fieldRef': {'fieldPath': 'metadata.labels'}}
+                            ]
+                        }
+                    }
                 ]
             ),
         )
         logger.info(f"Create pod '{pod_name}'")
         v1.create_namespaced_pod('default', pod, async_req=False)
         pods.append(pod_name)
     return pods
@@ -136,14 +152,15 @@
     v1 = client.CoreV1Api()
     for name in names:
         try:
             v1.delete_namespaced_pod(name, 'default', async_req=False)
         except kubernetes.client.exceptions.ApiException:
             logger.debug(f'Pod {name} was not available to teardown anymore')
 
+
 def fetch_pods(label: str, value: str):
     config.load_kube_config()
     v1 = client.CoreV1Api()
     pods_list = v1.list_namespaced_pod('default')
     pods = []
     for pod in pods_list.items:
         fn_value = pod.metadata.labels.get(label)
@@ -163,8 +180,8 @@
         # not used
         pod_id = ''
         labels = {
             'type': 'api-gateway',
             zone_label: zone
         }
         lb[zone] = Pod(pod_id, ip, labels, pod_name)
-    return lb
+    return lb
```

### Comparing `edgerun-galileo-experiments-0.0.2.dev8/setup.py` & `edgerun-galileo-experiments-0.0.2.dev9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     tests_require = [line for line in fh.read().split(os.linesep) if line]
 
 with open("requirements.txt", "r") as fh:
     install_requires = [line for line in fh.read().split(os.linesep) if line]
 
 setuptools.setup(
     name="edgerun-galileo-experiments",
-    version="0.0.2.dev8",
+    version="0.0.2.dev9",
     author="Philipp Raith, Thomas Rausch",
     author_email="p.raith@dsg.tuwien.ac.at, t.rausch@dsg.tuwien.ac.at",
     description="Galileo Experiments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/edgerun/galileo-experiments",
     packages=setuptools.find_packages(),
```

