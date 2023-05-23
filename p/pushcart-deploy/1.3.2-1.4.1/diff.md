# Comparing `tmp/pushcart_deploy-1.3.2.tar.gz` & `tmp/pushcart_deploy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart_deploy-1.3.2.tar", max compression
+gzip compressed data, was "pushcart_deploy-1.4.1.tar", max compression
```

## Comparing `pushcart_deploy-1.3.2.tar` & `pushcart_deploy-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/LICENSE
--rw-r--r--   0        0        0       80 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/README.md
--rw-r--r--   0        0        0     1137 2023-05-05 15:45:56.364001 pushcart_deploy-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-05 15:45:56.364001 pushcart_deploy-1.3.2/src/pushcart_deploy/__init__.py
--rw-r--r--   0        0        0    12855 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/configuration.py
--rw-r--r--   0        0        0       79 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/__init__.py
--rw-r--r--   0        0        0     8550 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/job_settings.py
--rw-r--r--   0        0        0     4625 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py
--rw-r--r--   0        0        0     4494 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/repos_wrapper.py
--rw-r--r--   0        0        0     3232 2023-05-05 15:44:48.478549 pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py
--rw-r--r--   0        0        0     5265 2023-05-05 15:44:48.482549 pushcart_deploy-1.3.2/src/pushcart_deploy/setup.py
--rw-r--r--   0        0        0     1104 2023-05-05 15:44:48.482549 pushcart_deploy-1.3.2/src/pushcart_deploy/validation.py
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 pushcart_deploy-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-03 13:39:43.347561 pushcart_deploy-1.4.1/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-05 08:20:56.886928 pushcart_deploy-1.4.1/README.md
+-rw-r--r--   0        0        0     2428 2023-05-23 15:30:50.081098 pushcart_deploy-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/__init__.py
+-rw-r--r--   0        0        0    16059 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/configuration.py
+-rw-r--r--   0        0        0      200 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/__init__.py
+-rw-r--r--   0        0        0     7509 2023-05-23 15:16:36.981069 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/job_settings.py
+-rw-r--r--   0        0        0     4559 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py
+-rw-r--r--   0        0        0     4913 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/repos_wrapper.py
+-rw-r--r--   0        0        0     3461 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py
+-rw-r--r--   0        0        0     7784 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/metadata.py
+-rw-r--r--   0        0        0     2087 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/setup.py
+-rw-r--r--   0        0        0     4163 2023-05-23 15:16:36.984402 pushcart_deploy-1.4.1/src/pushcart_deploy/validation.py
+-rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 pushcart_deploy-1.4.1/PKG-INFO
```

### Comparing `pushcart_deploy-1.3.2/LICENSE` & `pushcart_deploy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/job_settings.py` & `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/job_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,48 @@
+"""Load Databricks job settings for a data pipeline from file or from defaults.
+
+Job settings may come in JSON, TOML or YAML formats when loaded from file
+
+Example:
+-------
+    job_settings = JobSettings(api_client)
+    settings_from_file = job_settings.load_job_settings(settings_path="/path/to/pipeline.json")
+    default_settings = job_settings.load_job_settings(default_settings="checkpoint")
+
+Notes:
+-----
+Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
+environment.
+
+"""
+
+import asyncio
 import logging
 import operator
 from functools import lru_cache
 from pathlib import Path
-from typing import Optional
 
 from databricks_cli.clusters.api import ClusterApi
 from databricks_cli.sdk.api_client import ApiClient
 from pydantic import constr, dataclasses, validate_arguments, validator
 
 from pushcart_deploy.configuration import get_config_from_file
 from pushcart_deploy.validation import (
     PydanticArbitraryTypesConfig,
     validate_databricks_api_client,
 )
 
 
 @lru_cache(maxsize=1)
-@validate_arguments(config=dict(arbitrary_types_allowed=True))
+@validate_arguments(config={"arbitrary_types_allowed": True})
 def _get_smallest_cluster_node_type(client: ApiClient = None) -> str:
-    """
-    Retrieve the smallest Photon-capable cluster node type from a Databricks cluster
-    using the Databricks CLI and SDK APIs. The function caches the result to improve
-    performance.
-
-    Inputs:
-    - client: an instance of the ApiClient class from the Databricks CLI SDK.
-    """
+    """Retrieve the smallest Photon-capable cluster node type from a Databricks cluster."""
     cluster_api = ClusterApi(client)
 
     log = logging.getLogger(__name__)
-    log.setLevel(logging.INFO)
 
     node_types = [
         t
         for t in cluster_api.list_node_types()["node_types"]
         if t["is_deprecated"] is False
         and t["is_hidden"] is False
         and t["photon_driver_capable"] is True
@@ -41,83 +50,60 @@
     ]
 
     if not node_types:
         log.error("No Photon-capable node type could be selected")
         return None
 
     node = sorted(
-        node_types, key=operator.itemgetter("num_cores", "memory_mb", "num_gpus")
+        node_types,
+        key=operator.itemgetter("num_cores", "memory_mb", "num_gpus"),
     )[0]["node_type_id"]
     log.info(f"Using node type ID: {node}")
 
     return node
 
 
 @lru_cache(maxsize=1)
-@validate_arguments(config=dict(arbitrary_types_allowed=True))
+@validate_arguments(config={"arbitrary_types_allowed": True})
 def _get_newest_spark_version(client: ApiClient = None) -> str:
-    """
-    Retrieve the newest version of Apache Spark that is not labeled as "ML" and is an
-    LTS version. The function uses the Databricks CLI and API to retrieve and filter
-    the available Spark versions. The function caches the result to improve performance
-
-    Inputs:
-    - client: an instance of the ApiClient class from the Databricks CLI SDK.
-
-    Additional aspects:
-    - The function assumes that there is at least one Spark version that meets the
-      specified criteria, otherwise it will raise an exception.
-    """
+    """Retrieve the newest version of Apache Spark that is not labeled as "ML" and is an LTS version."""
     cluster_api = ClusterApi(client)
 
     log = logging.getLogger(__name__)
-    log.setLevel(logging.INFO)
 
     spark_versions = [
         v
         for v in cluster_api.spark_versions()["versions"]
         if "ML" not in v["name"] and "LTS" in v["name"]
     ]
 
     if not spark_versions:
-        log.error(f"No spark versions.")
+        log.error("No spark versions.")
         return None
 
     version = sorted(
         spark_versions,
         key=lambda x: float(x["name"].split(" LTS ")[0]),
         reverse=True,
     )[0]["key"]
     log.info(f"Using Spark version: {version}")
 
     return version
 
 
 @lru_cache(maxsize=50)
-@validate_arguments(config=dict(arbitrary_types_allowed=True))
+@validate_arguments(config={"arbitrary_types_allowed": True})
 def _get_existing_cluster_id(
-    client: ApiClient = None, cluster_name: constr(min_length=1, strict=True) = None
+    client: ApiClient = None,
+    cluster_name: constr(min_length=1, strict=True) = None,
 ) -> str:
-    """
-    Retrieve the ID of an existing Databricks cluster by its name using the Databricks
-    API. The function caches the result to improve performance
-
-    Inputs:
-    - client: an instance of the ApiClient class from the Databricks CLI SDK
-    - `cluster_name`: the name of the cluster to retrieve the ID for
-
-    Additional aspects:
-    - The `constr` class from the `pydantic` library is used to enforce input
-    validation for the `cluster_name` input, requiring a string with a minimum length
-    of 1 and no leading or trailing whitespace.
-    """
+    """Retrieve the ID of an existing Databricks cluster by its name."""
     cluster_api = ClusterApi(client)
 
     log = logging.getLogger(__name__)
-    log.setLevel(logging.INFO)
 
     clusters = cluster_api.list_clusters().get("clusters", [])
     clusters_filtered = [c for c in clusters if c["cluster_name"] == cluster_name]
 
     if not clusters_filtered:
         log.error(f"Cluster not found: {cluster_name}")
         return None
@@ -126,101 +112,92 @@
     log.info(f"Cluster ID: {cluster_id}")
 
     return cluster_id
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class JobSettings:
-    """
-    Manages job settings for Databricks jobs. It provides methods for loading job
-    settings from a JSON file or string, as well as for retrieving default job settings
-    for checkpoint, pipeline, and release jobs.
-
-    Fields:
-    - client: instance of ApiClient used for interacting with the Databricks API
-    - log: logger instance used for logging messages during job settings loading and
-      validation
+    """Manages job settings for Databricks jobs.
+
+    Provides methods for loading job settings from a JSON file or string, as well as
+    for retrieving default job settings for checkpoint, pipeline, and release jobs.
     """
 
     client: ApiClient
 
     @validator("client")
     @classmethod
-    def check_api_client(cls, value):
-        """
-        Validator method that ensures the provided ApiClient is valid
-        """
+    def check_api_client(cls, value: ApiClient) -> ApiClient:
+        """Validate the provided ApiClient."""
         return validate_databricks_api_client(value)
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
+        """Initialize logger."""
         self.log = logging.getLogger(__name__)
-        self.log.setLevel(logging.INFO)
 
-    @validate_arguments(config=dict(arbitrary_types_allowed=True))
+    @validate_arguments(config={"arbitrary_types_allowed": True})
     def load_job_settings(
         self,
-        settings_path: Optional[Path] = None,
-        default_settings: Optional[
-            constr(min_length=1, strict=True, regex=r"^(checkpoint|pipeline|release)$")
-        ] = None,
+        settings_path: Path | None = None,
+        default_settings: constr(
+            min_length=1,
+            strict=True,
+            regex="^(checkpoint|pipeline)$",
+        )
+        | None = None,
     ) -> dict:
-        """
-        Load job settings from a file, or retrieve default job settings if none are
-        provided
-        """
+        """Load job settings from a file, or retrieve default job settings if none are provided."""
         job_settings = None
 
         if settings_path:
-            job_settings = get_config_from_file(settings_path)
+            job_settings = asyncio.run(get_config_from_file(settings_path))
 
         if not job_settings:
             self.log.info("Creating job using default settings")
 
             if settings_path and not default_settings:
+                msg = "Failed to load provided job settings, and default settings were not specified."
                 raise RuntimeError(
-                    "Failed to load provided job settings, and default settings were not specified."
+                    msg,
                 )
 
             job_settings = self._get_default_job_settings(default_settings)
 
         return job_settings
 
     def _get_default_job_settings(
         self,
         settings_name: constr(
-            min_length=1, strict=True, regex=r"^(checkpoint|pipeline|release)$"
+            min_length=1,
+            strict=True,
+            regex=r"^(checkpoint|pipeline)$",
         ),
     ) -> dict:
-        """
-        Helper method for retrieving default job settings for checkpoint, pipeline,
-        and release jobs
-        """
+        """Retrieve default job settings for checkpoint and pipeline jobs."""
         settings_map = {
             "checkpoint": _get_default_checkpoint_job_settings,
             "pipeline": _get_default_pipeline_job_settings,
-            "release": _get_default_release_job_settings,
         }
 
         settings_getter = settings_map.get(settings_name)
 
         if not settings_getter:
-            raise ValueError("Could not find default settings for {settings_name}")
+            msg = "Could not find default settings for {settings_name}"
+            raise ValueError(msg)
 
         return settings_getter(self.client)
 
 
-def _get_default_checkpoint_job_settings(client: ApiClient = None) -> dict:
+def _get_default_pipeline_job_settings(
+    client: ApiClient = None,  # noqa: ARG001
+) -> dict:
     return {}
 
 
-def _get_default_pipeline_job_settings(client: ApiClient = None) -> dict:
-    return {}
-
-
-def _get_default_release_job_settings(client: ApiClient = None) -> dict:
+def _get_default_checkpoint_job_settings(client: ApiClient = None) -> dict:
     return {
         "name": "release",
         "timeout_seconds": 0,
         "max_concurrent_runs": 1,
         "tasks": [
             {
                 "task_key": "release",
@@ -232,15 +209,15 @@
                 "job_cluster_key": "release",
                 "libraries": [{"pypi": {"package": "pushcart"}}],
                 "max_retries": 1,
                 "min_retry_interval_millis": 15000,
                 "retry_on_timeout": False,
                 "timeout_seconds": 0,
                 "email_notifications": {},
-            }
+            },
         ],
         "job_clusters": [
             {
                 "job_cluster_key": "release",
                 "new_cluster": {
                     "spark_version": _get_newest_spark_version(client),
                     "spark_conf": {
@@ -250,11 +227,11 @@
                     "node_type_id": _get_smallest_cluster_node_type(client),
                     "driver_node_type_id": _get_smallest_cluster_node_type(client),
                     "custom_tags": {"ResourceClass": "SingleNode"},
                     "enable_elastic_disk": True,
                     "runtime_engine": "PHOTON",
                     "num_workers": 0,
                 },
-            }
+            },
         ],
         "format": "MULTI_TASK",
     }
```

### Comparing `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/jobs_wrapper.py` & `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+"""Manage Pushcart data pipeline jobs.
+
+Wrapper class around the Databricks Jobs API, creating, retrieving, updating and
+deleting jobs.
+
+Example:
+-------
+    jobs_wrapper = JobsWrapper(api_client)
+    checkpoint_job = jobs_wrapper.get_or_create_checkpoint_job("/path/to/settings.json")
+    jobs_wrapper.run(checkpoint_job)
+    jobs_wrapper.delete(checkpoint_job)
+
+Notes:
+-----
+Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
+environment.
+
+"""
+
 import logging
 from pathlib import Path
 from time import sleep
-from typing import Optional, Tuple
 
 from databricks_cli.jobs.api import JobsApi
 from databricks_cli.runs.api import RunsApi
 from databricks_cli.sdk.api_client import ApiClient
 from pydantic import dataclasses, validate_arguments, validator
 
 from pushcart_deploy.databricks_api.job_settings import JobSettings
@@ -13,129 +31,108 @@
     PydanticArbitraryTypesConfig,
     validate_databricks_api_client,
 )
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class JobsWrapper:
-    """
-    Manages Databricks jobs. It provides methods for creating, retrieving, and deleting
-    jobs, as well as for running jobs and retrieving their status. It also uses the
-    JobSettings class to load job settings from a JSON file or string, or to retrieve
-    default job settings for checkpoint, pipeline, and release jobs.
-
-    Fields:
-    - client: instance of ApiClient used for interacting with the Databricks API
-    - log: logger instance used for logging messages during job management
-    - jobs_api: instance of JobsApi used for interacting with the Databricks Jobs API
-    - runs_api: instance of RunsApi used for interacting with the Databricks Runs API
+    """Manages Databricks jobs.
+
+    Provides methods for creating, retrieving, and deleting jobs, as well as for
+    running jobs and retrieving their status. Uses the JobSettings class to load
+    job settings from a JSON file or string, or to retrieve default job settings
+    for checkpoint, pipeline, and release jobs.
     """
 
     client: ApiClient
 
     @validator("client")
     @classmethod
-    def check_api_client(cls, value):
-        """
-        Validator method for the provided ApiClient
-        """
+    def check_api_client(cls, value: ApiClient) -> ApiClient:
+        """Validate the provided ApiClient."""
         return validate_databricks_api_client(value)
 
-    def __post_init_post_parse__(self):
-        """
-        Initializes the logger instance and creates instances of JobsApi and RunsApi
-        """
+    def __post_init_post_parse__(self) -> None:
+        """Initialize the logger instance and creates instances of JobsApi and RunsApi."""
         self.log = logging.getLogger(__name__)
-        self.log.setLevel(logging.INFO)
 
         self.jobs_api = JobsApi(self.client)
         self.runs_api = RunsApi(self.client)
 
     @validate_arguments
-    def get_or_create_release_job(self, settings_json: Optional[Path] = None) -> str:
-        """
-        Retrieves or creates a release job using the provided job settings
-        """
+    def get_or_create_checkpoint_job(self, settings_json: Path | None = None) -> str:
+        """Retrieve or create a checkpoint job using the provided job settings."""
         job_settings = JobSettings(self.client).load_job_settings(
-            settings_json, "release"
+            settings_json,
+            "checkpoint",
         )
 
         return self.get_or_create_job(job_settings)
 
     def _get_job(self, job_name: str) -> list:
-        """
-        Retrieves a job by name
-        """
+        """Retrieve a job by name."""
         jobs = self.jobs_api.list_jobs().get("jobs", [])
         jobs_filtered = [j for j in jobs if j["settings"]["name"] == job_name]
 
         return jobs_filtered[0]["job_id"] if jobs_filtered else None
 
     def _create_job(self, job_settings: dict) -> str:
-        """
-        Creates a new job using the provided job settings
-        """
+        """Create a new job using the provided job settings."""
         job = self.jobs_api.create_job(job_settings)
         self.log.info(f"Created job {job_settings['name']} with ID: {job['job_id']}")
 
         return job["job_id"]
 
     @validate_arguments
     def get_or_create_job(self, job_settings: dict) -> str:
-        """
-        Retrieves or creates a job using the provided job settings
-        """
+        """Retrieve or create a job using the provided job settings."""
         job_name = job_settings.get("name")
 
         if not job_name:
-            raise ValueError("Please provide a job name in the job settings")
+            msg = "Please provide a job name in the job settings"
+            raise ValueError(msg)
 
         job_id = self._get_job(job_name)
 
         if not job_id:
             self.log.warning(f"Job not found: {job_name}. Creating a new one.")
             return self._create_job(job_settings)
 
         self.jobs_api.reset_job({"job_id": job_id, "new_settings": job_settings})
 
         self.log.info(f"Job ID: {job_id}")
 
         return job_id
 
     @validate_arguments
-    def run_job(self, job_id: str) -> Tuple[str, str]:
-        """
-        Runs a job and retrieves its status
-        """
+    def run_job(self, job_id: str) -> tuple[str, str]:
+        """Run a job and retrieve its status."""
         run_id = self.jobs_api.run_now(
             job_id=job_id,
             jar_params=None,
             notebook_params=None,
             python_params=None,
             spark_submit_params=None,
         )["run_id"]
 
-        SLEEP_TIME = 2
         job_status = "PENDING"
         job = {}
 
         while job_status in ["PENDING", "RUNNING"]:
-            sleep(SLEEP_TIME)
+            sleep(2)
             job = self.runs_api.get_run(run_id)
             job_status = job["state"]["life_cycle_state"]
 
-            logging.info(f"Job is {job_status}: {job['run_page_url']}")
+            self.log.info(f"Job is {job_status}: {job['run_page_url']}")
 
         return (
             job["state"].get("result_state", job["state"]["life_cycle_state"]),
             job["run_page_url"],
         )
 
     @validate_arguments
     def delete_job(self, job_id: str) -> None:
-        """
-        Deletes a job by ID
-        """
+        """Delete a job by ID."""
         job_name = self.jobs_api.get_job(job_id=job_id)["settings"]["name"]
         self.jobs_api.delete_job(job_id=job_id)
 
-        logging.info(f"Deleted job {job_name} ({job_id})")
+        self.log.info(f"Deleted job {job_name} ({job_id})")
```

### Comparing `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/repos_wrapper.py` & `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/repos_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,78 @@
+"""Create or sync a Git repository containing Pushcart configuration files.
+
+Wrapper class around the Databricks Repos API.
+
+Example:
+-------
+    repos_wrapper = ReposWrapper(api_client)
+    repos_wrapper.get_or_create_repo("pushcart", "https://github.com/GeorgelPreput/pushcart-config")
+    repos_wrapper.update("pushcart", "main")
+
+Notes:
+-----
+Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
+environment.
+
+"""
+
 import logging
-import os
 import re
 from pathlib import Path
-from typing import Optional
 
 from databricks_cli.repos.api import ReposApi
 from databricks_cli.sdk.api_client import ApiClient
 from pydantic import HttpUrl, constr, dataclasses, validate_arguments, validator
+from requests.exceptions import HTTPError
 
 from pushcart_deploy.validation import (
     PydanticArbitraryTypesConfig,
     validate_databricks_api_client,
 )
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class ReposWrapper:
-    """
-    The ReposWrapper class provides a wrapper around the Databricks Repos API. It
-    allows users to get or create a repository, update the repository with a new
+    """Wrapper around the Databricks Repos API.
+
+    Allows users to get or create a repository, update the repository with a new
     branch, and detect the Git provider from a given URL.
 
-    Fields:
-    - client: an ApiClient object used to interact with the Databricks Repos API
-    - log: a logger object used for logging messages
-    - repos_api: a ReposApi object used to interact with the Databricks Repos API
-    - repo_id: the ID of the repository (initialized to None)
+    Returns
+    -------
+    ReposWrapper
+        Wrapper object to sync a Pushcart configurations repo to the environment.
+
+    Raises
+    ------
+    ValueError
+        Git provider must be provided explicitly, unless it can be derived from the repo URL.
+    ValueError
+        Can only update a repo that has been initialized.
     """
 
     client: ApiClient
 
     @validator("client")
     @classmethod
-    def check_api_client(cls, value):
-        """
-        Validates that the ApiClient object is properly initialized
-        """
+    def check_api_client(cls, value: ApiClient) -> ApiClient:
+        """Validate that the ApiClient object is properly initialized."""
         return validate_databricks_api_client(value)
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
+        """Initialize logger."""
         self.log = logging.getLogger(__name__)
-        self.log.setLevel(logging.INFO)
 
         self.repos_api = ReposApi(self.client)
         self.repo_id = None
 
     @staticmethod
     @validate_arguments
     def _detect_git_provider(repo_url: str) -> str:
-        """
-        Detects the Git provider from a given URL
-        """
-
+        """Detect the Git provider from a given URL."""
         providers = {
             "gitHub": r"(?:https?://|git@)github\.com[:/]",
             "bitbucketCloud": r"(?:https?://|git@)bitbucket\.org[:/]",
             "gitLab": r"(?:https?://|git@)gitlab\.com[:/]",
             "azureDevOpsServices": r"(?:https?://|git@ssh?\.?)([\w-]+@)?\.?dev\.azure\.com[:/]",
             "gitHubEnterprise": r"(?:https?://|git@)([\w-]+)\.github(?:usercontent)?\.com[:/]",
             "bitbucketServer": r"(?:https?://|git@)([\w-]+)\.bitbucket(?:usercontent)?\.com[:/]",
@@ -63,66 +80,61 @@
             "awsCodeCommit": r"(?:https?://|git@)git-codecommit\.[^/]+\.amazonaws\.com[:/]",
         }
 
         for provider, regex in providers.items():
             if re.match(regex, repo_url):
                 return provider
 
-        raise ValueError(
-            "Could not detect Git provider from URL. Please specify git_provider explicitly."
-        )
+        msg = "Could not detect Git provider from URL. Please specify git_provider explicitly."
+        raise ValueError(msg)
 
     @validate_arguments
     def get_or_create_repo(
         self,
         repo_user: constr(min_length=1, strict=True, regex=r"^[^'\"]*$"),
         git_url: HttpUrl,
-        git_provider: Optional[
-            constr(
-                min_length=1,
-                strict=True,
-                regex=r"^(gitHub|bitbucketCloud|gitLab|azureDevOpsServices|gitHubEnterprise|bitbucketServer|gitLabEnterpriseEdition|awsCodeCommit)$",
-            )
-        ] = None,
+        git_provider: constr(
+            min_length=1,
+            strict=True,
+            regex="^(gitHub|bitbucketCloud|gitLab|azureDevOpsServices|gitHubEnterprise|bitbucketServer|gitLabEnterpriseEdition|awsCodeCommit)$",
+        )
+        | None = None,
     ) -> str:
-        """
-        Gets or creates a repository with a given user, Git URL and Git provider (if
-        not detected from URL)
-        """
-
+        """Get or create a repository with a given user, Git URL and Git provider (if not detected from URL)."""
         if not git_provider:
             self.log.warning(
-                "No Git provider specified. Attempting to guess based on URL."
+                "No Git provider specified. Attempting to guess based on URL.",
             )
             git_provider = self._detect_git_provider(git_url)
 
         git_repo = git_url.split("/")[-1].replace(".git", "")
 
-        repo_path = Path(os.path.join("/", "Repos", repo_user, git_repo)).as_posix()
+        repo_path = (Path("/Repos") / repo_user / git_repo).as_posix()
         try:
             self.repo_id = self.repos_api.get_repo_id(path=repo_path)
-        except Exception:
+        except (HTTPError, ValueError, RuntimeError):
             self.log.warning("Failed to get repo ID")
 
         if not self.repo_id:
             self.log.warning(f"Repo not found, cloning from URL: {git_url}")
 
             repo = self.repos_api.create(git_url, git_provider, repo_path)
             self.repo_id = repo["id"]
 
         self.log.info(f"Repository ID: {self.repo_id}")
 
         return self.repo_id
 
     @validate_arguments
-    def update(self, git_branch: constr(min_length=1, strict=True, regex=r"^[^'\"]*$")):
-        """
-        Updates the Databricks repository with a new branch
-        """
-
+    def update(
+        self,
+        git_branch: constr(min_length=1, strict=True, regex=r"^[^'\"]*$"),
+    ) -> None:
+        """Update the Databricks repository with a new branch."""
         if not self.repo_id:
+            msg = "Repo not initialized. Please first run get_or_create_repo()"
             raise ValueError(
-                "Repo not initialized. Please first run get_or_create_repo()"
+                msg,
             )
 
         # TODO: Support Git tags as well
         self.repos_api.update(self.repo_id, branch=git_branch, tag=None)
```

### Comparing `pushcart_deploy-1.3.2/src/pushcart_deploy/databricks_api/secrets_wrapper.py` & `pushcart_deploy-1.4.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,71 @@
+"""Create secrets and secret scopes to be used by Pushcart.
+
+Wrapper class around the Databricks Secrets API used in setting Pushcart-specific
+secrets to be read by data pipelines.
+
+Example:
+-------
+    secrets_wrapper = SecretsWrapper(api_client)
+    secrets_wrapper.create_scope_if_not_exists("pushcart")
+    secrets_wrapper.push_secrets("pushcart", secrets_dict)
+
+Notes:
+-----
+Needs a Databricks CLI ApiClient to be configured and connected to a Databricks
+environment.
+
+"""
+
 import logging
-from typing import Dict
 
 from databricks_cli.sdk.api_client import ApiClient
 from databricks_cli.secrets.api import SecretApi
 from pydantic import Field, constr, dataclasses, validate_arguments, validator
 
 from pushcart_deploy.validation import (
     PydanticArbitraryTypesConfig,
     validate_databricks_api_client,
 )
 
 
 @dataclasses.dataclass(config=PydanticArbitraryTypesConfig)
 class SecretsWrapper:
-    """
-    Wrapper around the Databricks Secrets API to manage secrets in a Databricks
-    workspace. It allows creating a secret scope if it does not exist and pushing
-    secrets to the scope.
-    Fields:
-    - client: an instance of the Databricks API client used to interact with the Secrets API.
-    - log: a logger instance used to log messages.
-    - secrets_api: an instance of the SecretApi class used to interact with the Secrets API.
+    """Wrapper around the Databricks Secrets API.
+
+    Manage secrets in a Databricks workspace. It allows creating a secret scope if it
+    does not exist and pushing secrets to the scope.
     """
 
     client: ApiClient
 
     @validator("client")
     @classmethod
-    def check_api_client(cls, value):
-        """
-        Validates that the ApiClient object is properly initialized
-        """
+    def check_api_client(cls, value: ApiClient) -> ApiClient:
+        """Validate that the ApiClient object is properly initialized."""
         return validate_databricks_api_client(value)
 
-    def __post_init_post_parse__(self):
+    def __post_init_post_parse__(self) -> None:
+        """Initialize logger."""
         self.log = logging.getLogger(__name__)
-        self.log.setLevel(logging.INFO)
 
         self.secrets_api = SecretApi(self.client)
 
     @validate_arguments
     def create_scope_if_not_exists(
         self,
         secret_scope_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
             regex=r"^[A-Za-z0-9\-_.]{1,128}$",
-        ) = "pushcart",
+        ) = "pushcart",  # noqa: S107
     ) -> None:
-        """
-        Creates a secret scope if it does not exist in the workspace.
-        """
+        """Create a secret scope if it does not exist in the workspace."""
         scopes = self.secrets_api.list_scopes()["scopes"]
         if secret_scope_name not in [scope["name"] for scope in scopes]:
             self.secrets_api.create_scope(
                 initial_manage_principal="users",
                 scope=secret_scope_name,
                 scope_backend_type="DATABRICKS",
                 backend_azure_keyvault=None,
@@ -68,31 +77,31 @@
         self,
         secret_scope_name: constr(
             strip_whitespace=True,
             to_lower=True,
             strict=True,
             min_length=1,
             regex=r"^[A-Za-z0-9\-_.]{1,128}$",
-        ) = "pushcart",
-        secrets_dict: Dict[
+        ) = "pushcart",  # noqa: S107
+        secrets_dict: dict[
             constr(
                 strip_whitespace=True,
                 to_lower=True,
                 strict=True,
                 min_length=1,
                 regex=r"^[A-Za-z0-9\-_.]{1,128}$",
             ),
             str,
-        ] = Field(default_factory=dict),
+        ] = Field(  # noqa: B008
+            default_factory=dict,
+        ),
     ) -> None:
-        """
-        Pushes secrets to a secret scope in the workspace.
-        """
+        """Pushes secrets to a secret scope in the workspace."""
         if not secrets_dict:
             self.log.warning("No secrets to push to secret scope")
-            return None
+            return
 
         self.create_scope_if_not_exists(secret_scope_name)
 
         for key, value in secrets_dict.items():
             self.secrets_api.put_secret(secret_scope_name, key, value, bytes_value=None)
             self.log.info(f"Put secret '{key}' in '{secret_scope_name}' secret scope.")
```

### Comparing `pushcart_deploy-1.3.2/PKG-INFO` & `pushcart_deploy-1.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: pushcart-deploy
-Version: 1.3.2
+Version: 1.4.1
 Summary: Deployment helper for pipeline configurations using Pushcart
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
+Requires-Dist: databricks-connect (>=13.0.0,<14.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: urllib3 (>=1,<2)
 Description-Content-Type: text/markdown
 
 # pushcart-deploy
```

