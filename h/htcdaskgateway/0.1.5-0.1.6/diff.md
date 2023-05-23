# Comparing `tmp/htcdaskgateway-0.1.5.tar.gz` & `tmp/htcdaskgateway-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htcdaskgateway-0.1.5.tar", last modified: Mon Feb  6 21:50:05 2023, max compression
+gzip compressed data, was "htcdaskgateway-0.1.6.tar", last modified: Tue May 23 21:41:26 2023, max compression
```

## Comparing `htcdaskgateway-0.1.5.tar` & `htcdaskgateway-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-02-06 21:50:05.599323 htcdaskgateway-0.1.5/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-02-06 21:50:05.599323 htcdaskgateway-0.1.5/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.5/README.md
--rw-r--r--   0 macosta  (53128)     5063       38 2023-02-06 21:50:05.600323 htcdaskgateway-0.1.5/setup.cfg
--rw-r--r--   0 macosta  (53128)     5063      786 2023-02-06 21:49:42.000000 htcdaskgateway-0.1.5/setup.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-02-06 21:50:05.584323 htcdaskgateway-0.1.5/src/
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-02-06 21:50:05.589323 htcdaskgateway-0.1.5/src/htcdaskgateway/
--rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.5/src/htcdaskgateway/__init__.py
--rw-r--r--   0 macosta  (53128)     5063     8703 2023-02-06 21:49:25.000000 htcdaskgateway-0.1.5/src/htcdaskgateway/cluster.py
--rw-r--r--   0 macosta  (53128)     5063     3319 2022-12-02 20:09:14.000000 htcdaskgateway-0.1.5/src/htcdaskgateway/gateway.py
-drwxr-xr-x   0 macosta  (53128)     5063        0 2023-02-06 21:50:05.594323 htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/
--rw-r--r--   0 macosta  (53128)     5063     2673 2023-02-06 21:50:05.000000 htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/PKG-INFO
--rw-r--r--   0 macosta  (53128)     5063      277 2023-02-06 21:50:05.000000 htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/SOURCES.txt
--rw-r--r--   0 macosta  (53128)     5063        1 2023-02-06 21:50:05.000000 htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/dependency_links.txt
--rw-r--r--   0 macosta  (53128)     5063       15 2023-02-06 21:50:05.000000 htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/top_level.txt
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.181128 htcdaskgateway-0.1.6/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:41:26.179128 htcdaskgateway-0.1.6/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063     2173 2022-11-02 21:00:56.000000 htcdaskgateway-0.1.6/README.md
+-rw-r--r--   0 macosta  (53128)     5063       38 2023-05-23 21:41:26.181128 htcdaskgateway-0.1.6/setup.cfg
+-rw-r--r--   0 macosta  (53128)     5063      786 2023-05-23 21:36:27.000000 htcdaskgateway-0.1.6/setup.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.170128 htcdaskgateway-0.1.6/src/
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.174128 htcdaskgateway-0.1.6/src/htcdaskgateway/
+-rw-r--r--   0 macosta  (53128)     5063      153 2022-11-02 20:44:23.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/__init__.py
+-rw-r--r--   0 macosta  (53128)     5063     8750 2023-05-23 21:38:35.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/cluster.py
+-rw-r--r--   0 macosta  (53128)     5063     3286 2023-05-23 21:39:58.000000 htcdaskgateway-0.1.6/src/htcdaskgateway/gateway.py
+drwxr-xr-x   0 macosta  (53128)     5063        0 2023-05-23 21:41:26.178128 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/
+-rw-r--r--   0 macosta  (53128)     5063     2673 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/PKG-INFO
+-rw-r--r--   0 macosta  (53128)     5063      277 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/SOURCES.txt
+-rw-r--r--   0 macosta  (53128)     5063        1 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/dependency_links.txt
+-rw-r--r--   0 macosta  (53128)     5063       15 2023-05-23 21:41:25.000000 htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/top_level.txt
```

### Comparing `htcdaskgateway-0.1.5/PKG-INFO` & `htcdaskgateway-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.5
+Version: 0.1.6
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `htcdaskgateway-0.1.5/README.md` & `htcdaskgateway-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `htcdaskgateway-0.1.5/setup.py` & `htcdaskgateway-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="htcdaskgateway",
-    version="0.1.5",
+    version="0.1.6",
     author="Maria P. Acosta F./Fermilab EAF project",
     author_email="macosta@fnal.gov",
     description="Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache',
     url="https://github.com/mapsacosta/htcdaskgateway",
```

### Comparing `htcdaskgateway-0.1.5/src/htcdaskgateway/cluster.py` & `htcdaskgateway-0.1.6/src/htcdaskgateway/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,24 +107,24 @@
 Queue """+str(n)+""
     
         with open(f"{tmproot}/htcdask_submitfile.jdl", 'w+') as f:
             f.writelines(jdl)
         
         # Prepare singularity command
         singularity_cmd = """#!/bin/bash
-export SINGULARITYENV_DASK_GATEWAY_WORKER_NAME=$2
-export SINGULARITYENV_DASK_GATEWAY_API_URL="https://dask-gateway-api.fnal.gov/api"
-export SINGULARITYENV_DASK_GATEWAY_CLUSTER_NAME=$1
-export SINGULARITYENV_DASK_GATEWAY_API_TOKEN=/etc/dask-credentials/api-token
-export SINGULARITYENV_DASK_DISTRIBUTED__LOGGING__DISTRIBUTED="debug"
+export APPTAINERENV_DASK_GATEWAY_WORKER_NAME=$2
+export APPTAINERENV_DASK_GATEWAY_API_URL="https://dask-gateway-api.fnal.gov/api"
+export APPTAINERENV_DASK_GATEWAY_CLUSTER_NAME=$1
+export APPTAINERENV_DASK_GATEWAY_API_TOKEN=/etc/dask-credentials/api-token
+export APPTAINERENV_DASK_DISTRIBUTED__LOGGING__DISTRIBUTED="debug"
 
 worker_space_dir=${PWD}/dask-worker-space/$2
 mkdir $worker_space_dir
 
-singularity exec -B ${worker_space_dir}:/srv/dask-worker-space -B dask-credentials:/etc/dask-credentials """+image_name+""" \
+/cvmfs/oasis.opensciencegrid.org/mis/apptainer/current/bin/apptainer exec -B ${worker_space_dir}:/srv/dask-worker-space -B dask-credentials:/etc/dask-credentials """+image_name+""" \
 dask-worker --name $2 --tls-ca-file /etc/dask-credentials/dask.crt --tls-cert /etc/dask-credentials/dask.crt --tls-key /etc/dask-credentials/dask.pem --worker-port 10000:10070 --no-nanny --no-dashboard --local-directory /srv --scheduler-sni daskgateway-"""+cluster_name+""" --nthreads 1 tls://"""+self.scheduler_proxy_ip+""":80"""
     
         with open(f"{tmproot}/start.sh", 'w+') as f:
             f.writelines(singularity_cmd)
         os.chmod(f"{tmproot}/start.sh", 0o775)
         
         logger.info(" Sandbox: "+tmproot)
```

### Comparing `htcdaskgateway-0.1.5/src/htcdaskgateway/gateway.py` & `htcdaskgateway-0.1.6/src/htcdaskgateway/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger("htcdaskgateway.HTCGateway")
 
 
 class HTCGateway(Gateway):
     
     def __init__(self, **kwargs):
-        address = kwargs.pop('address', 'http://172.30.92.196')
+        #address = kwargs.pop('address', 'http://172.30.92.196')
         super().__init__(address, auth="jupyterhub", **kwargs)
     
     def new_cluster(self, cluster_options=None, shutdown_on_close=True, **kwargs):
         """Submit a new cluster to the gateway, and wait for it to be started.
         Same as calling ``submit`` and ``connect`` in one go.
         Parameters
         ----------
@@ -47,15 +47,14 @@
             ``cluster_options`` for more information.
         Returns
         -------
         cluster : GatewayCluster
         """
         logger.info(" Creating HTCGatewayCluster ")
         return HTCGatewayCluster(
-            address=self.address,
             proxy_address=self.proxy_address,
             public_address=self._public_address,
             auth=self.auth,
             asynchronous=self.asynchronous,
             loop=self.loop,
             cluster_options=cluster_options,
             shutdown_on_close=shutdown_on_close,
```

### Comparing `htcdaskgateway-0.1.5/src/htcdaskgateway.egg-info/PKG-INFO` & `htcdaskgateway-0.1.6/src/htcdaskgateway.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htcdaskgateway
-Version: 0.1.5
+Version: 0.1.6
 Summary: Launches a Dask Gateway cluster in K8s and joins HTCondor workers to it
 Home-page: https://github.com/mapsacosta/htcdaskgateway
 Author: Maria P. Acosta F./Fermilab EAF project
 Author-email: macosta@fnal.gov
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

