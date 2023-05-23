# Comparing `tmp/iam_actions-1.2.20230522.tar.gz` & `tmp/iam_actions-1.2.20230523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230522.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230523.tar", max compression
```

## Comparing `iam_actions-1.2.20230522.tar` & `iam_actions-1.2.20230523.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/README.md
--rw-r--r--   0        0        0      228 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/__init__.py
--rw-r--r--   0        0        0  4259559 2023-05-22 02:34:07.261606 iam_actions-1.2.20230522/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-22 02:32:36.580226 iam_actions-1.2.20230522/iam_actions/generate/services.py
--rw-r--r--   0        0        0   547482 2023-05-22 02:34:07.261606 iam_actions-1.2.20230522/iam_actions/policies.json
--rw-r--r--   0        0        0   194246 2023-05-22 02:34:07.261606 iam_actions-1.2.20230522/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   531071 2023-05-22 02:34:07.261606 iam_actions-1.2.20230522/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-22 02:34:08.029617 iam_actions-1.2.20230522/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230522/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230522/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/README.md
+-rw-r--r--   0        0        0      228 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4262607 2023-05-23 02:29:46.060009 iam_actions-1.2.20230523/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-23 02:28:07.695140 iam_actions-1.2.20230523/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   547895 2023-05-23 02:29:46.060009 iam_actions-1.2.20230523/iam_actions/policies.json
+-rw-r--r--   0        0        0   194246 2023-05-23 02:29:46.060009 iam_actions-1.2.20230523/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   531470 2023-05-23 02:29:46.060009 iam_actions-1.2.20230523/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-23 02:29:46.828016 iam_actions-1.2.20230523/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230523/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230523/PKG-INFO
```

### Comparing `iam_actions-1.2.20230522/LICENSE` & `iam_actions-1.2.20230523/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/README.md` & `iam_actions-1.2.20230523/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/actions.json` & `iam_actions-1.2.20230523/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999684887149367%*

 * *Differences: {"'datasync'": "{'GenerateRecommendations': OrderedDict([('access_level', 'Undocumented'), "*

 * *               "('action', 'GenerateRecommendations'), ('condition_keys', []), ('description', "*

 * *               "'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *               "'DescribeStorageSystemResourceMetrics': OrderedDict([('access_level', "*

 * *               "'Undocumented'), ('action', 'DescribeStorageSystemResourceMetrics'), "*

 * *               "('condition_keys', []), ('description', 'Not Do […]*

```diff
@@ -33835,14 +33835,22 @@
             "orphan": false,
             "resources": [
                 "pipeline"
             ]
         }
     },
     "datasync": {
+        "AddStorageSystem": {
+            "access_level": "Undocumented",
+            "action": "AddStorageSystem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CancelTaskExecution": {
             "access_level": "Write",
             "action": "CancelTaskExecution",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to cancel execution of a sync task",
@@ -34022,14 +34030,22 @@
             "condition_keys": [],
             "description": "Grants permission to view metadata such as name, network interfaces, and the status (that is, whether the agent is running or not) about a sync agent",
             "orphan": false,
             "resources": [
                 "agent"
             ]
         },
+        "DescribeDiscoveryJob": {
+            "access_level": "Undocumented",
+            "action": "DescribeDiscoveryJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeLocationEfs": {
             "access_level": "Read",
             "action": "DescribeLocationEfs",
             "condition_keys": [],
             "description": "Grants permission to view metadata, such as the path information about an Amazon EFS sync location",
             "orphan": false,
             "resources": [
@@ -34122,14 +34138,38 @@
             "condition_keys": [],
             "description": "Grants permission to view metadata, such as the path information, about an SMB sync location",
             "orphan": false,
             "resources": [
                 "location"
             ]
         },
+        "DescribeStorageSystem": {
+            "access_level": "Undocumented",
+            "action": "DescribeStorageSystem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeStorageSystemResourceMetrics": {
+            "access_level": "Undocumented",
+            "action": "DescribeStorageSystemResourceMetrics",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DescribeStorageSystemResources": {
+            "access_level": "Undocumented",
+            "action": "DescribeStorageSystemResources",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeTask": {
             "access_level": "Read",
             "action": "DescribeTask",
             "condition_keys": [],
             "description": "Grants permission to view metadata about a sync task",
             "orphan": false,
             "resources": [
@@ -34144,30 +34184,54 @@
             ],
             "description": "Grants permission to view metadata about a sync task that is being executed",
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         },
+        "GenerateRecommendations": {
+            "access_level": "Undocumented",
+            "action": "GenerateRecommendations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAgents": {
             "access_level": "List",
             "action": "ListAgents",
             "condition_keys": [],
             "description": "Grants permission to list agents owned by an AWS account in a region specified in the request",
             "orphan": false,
             "resources": []
         },
+        "ListDiscoveryJobs": {
+            "access_level": "Undocumented",
+            "action": "ListDiscoveryJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListLocations": {
             "access_level": "List",
             "action": "ListLocations",
             "condition_keys": [],
             "description": "Grants permission to list source and destination sync locations",
             "orphan": false,
             "resources": []
         },
+        "ListStorageSystems": {
+            "access_level": "Undocumented",
+            "action": "ListStorageSystems",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags that have been added to the specified resource",
             "orphan": false,
             "resources": [
@@ -34193,28 +34257,52 @@
             "access_level": "List",
             "action": "ListTasks",
             "condition_keys": [],
             "description": "Grants permission to list of all the sync tasks",
             "orphan": false,
             "resources": []
         },
+        "RemoveStorageSystem": {
+            "access_level": "Undocumented",
+            "action": "RemoveStorageSystem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartDiscoveryJob": {
+            "access_level": "Undocumented",
+            "action": "StartDiscoveryJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartTaskExecution": {
             "access_level": "Write",
             "action": "StartTaskExecution",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to start a specific invocation of a sync task",
             "orphan": false,
             "resources": [
                 "task"
             ]
         },
+        "StopDiscoveryJob": {
+            "access_level": "Undocumented",
+            "action": "StopDiscoveryJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -34288,14 +34376,22 @@
             "condition_keys": [],
             "description": "Grants permission to update a SMB sync location",
             "orphan": false,
             "resources": [
                 "location"
             ]
         },
+        "UpdateStorageSystem": {
+            "access_level": "Undocumented",
+            "action": "UpdateStorageSystem",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateTask": {
             "access_level": "Write",
             "action": "UpdateTask",
             "condition_keys": [],
             "description": "Grants permission to update metadata associated with a sync task",
             "orphan": false,
             "resources": [
@@ -67633,14 +67729,22 @@
             "access_level": "Permissions management",
             "action": "TerminateNotebook",
             "condition_keys": [],
             "description": "Grants permission to terminate Glue Studio Notebooks",
             "orphan": false,
             "resources": []
         },
+        "TestConnection": {
+            "access_level": "Undocumented",
+            "action": "TestConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -132393,14 +132497,22 @@
             ],
             "description": "Grants permission to move a dedicated IP address to an existing dedicated IP pool",
             "orphan": false,
             "resources": [
                 "dedicated-ip-pool"
             ]
         },
+        "PutDedicatedIpPoolScalingAttributes": {
+            "access_level": "Undocumented",
+            "action": "PutDedicatedIpPoolScalingAttributes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PutDedicatedIpWarmupAttributes": {
             "access_level": "Write",
             "action": "PutDedicatedIpWarmupAttributes",
             "condition_keys": [
                 "ses:ApiVersion"
             ],
             "description": "Grants permission to enable dedicated IP warm up attributes",
@@ -137388,25 +137500,27 @@
         "UpdateMaintenanceWindowTarget": {
             "access_level": "Write",
             "action": "UpdateMaintenanceWindowTarget",
             "condition_keys": [],
             "description": "Grants permission to update a specified maintenance window target",
             "orphan": false,
             "resources": [
-                "maintenancewindow"
+                "maintenancewindow",
+                "windowtarget"
             ]
         },
         "UpdateMaintenanceWindowTask": {
             "access_level": "Write",
             "action": "UpdateMaintenanceWindowTask",
             "condition_keys": [],
             "description": "Grants permission to update a specified maintenance window task",
             "orphan": false,
             "resources": [
-                "maintenancewindow"
+                "maintenancewindow",
+                "windowtask"
             ]
         },
         "UpdateManagedInstanceRole": {
             "access_level": "Write",
             "action": "UpdateManagedInstanceRole",
             "condition_keys": [
                 "ssm:resourceTag/tag-key"
```

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230523/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230523/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/generate.py` & `iam_actions-1.2.20230523/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230523/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230523/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/generate/services.py` & `iam_actions-1.2.20230523/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/policies.json` & `iam_actions-1.2.20230523/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99999744548644%*

 * *Differences: {"'serviceMap'": "{'AWS Glue': {'Actions': {insert: [(186, 'TestConnection')]}}, 'Amazon Simple "*

 * *                 "Email Service v2': {'Actions': {insert: [(66, "*

 * *                 "'PutDedicatedIpPoolScalingAttributes')]}}, 'AWS DataSync': {'Actions': {insert: "*

 * *                 "[(0, 'AddStorageSystem'), (18, 'DescribeDiscoveryJob'), (29, "*

 * *                 "'DescribeStorageSystem'), (30, 'DescribeStorageSystemResourceMetrics'), (31, "*

 * *                 "'DescribeStorageSystemResources'), (34, 'GenerateRec […]*

```diff
@@ -2546,14 +2546,15 @@
                 "datapipeline:workerGroup"
             ]
         },
         "AWS DataSync": {
             "ARNFormat": "arn:aws:datasync:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:datasync:.+",
             "Actions": [
+                "AddStorageSystem",
                 "CancelTaskExecution",
                 "CreateAgent",
                 "CreateLocationEfs",
                 "CreateLocationFsxLustre",
                 "CreateLocationFsxOntap",
                 "CreateLocationFsxOpenZfs",
                 "CreateLocationFsxWindows",
@@ -2563,39 +2564,50 @@
                 "CreateLocationS3",
                 "CreateLocationSmb",
                 "CreateTask",
                 "DeleteAgent",
                 "DeleteLocation",
                 "DeleteTask",
                 "DescribeAgent",
+                "DescribeDiscoveryJob",
                 "DescribeLocationEfs",
                 "DescribeLocationFsxLustre",
                 "DescribeLocationFsxOntap",
                 "DescribeLocationFsxOpenZfs",
                 "DescribeLocationFsxWindows",
                 "DescribeLocationHdfs",
                 "DescribeLocationNfs",
                 "DescribeLocationObjectStorage",
                 "DescribeLocationS3",
                 "DescribeLocationSmb",
+                "DescribeStorageSystem",
+                "DescribeStorageSystemResourceMetrics",
+                "DescribeStorageSystemResources",
                 "DescribeTask",
                 "DescribeTaskExecution",
+                "GenerateRecommendations",
                 "ListAgents",
+                "ListDiscoveryJobs",
                 "ListLocations",
+                "ListStorageSystems",
                 "ListTagsForResource",
                 "ListTaskExecutions",
                 "ListTasks",
+                "RemoveStorageSystem",
+                "StartDiscoveryJob",
                 "StartTaskExecution",
+                "StopDiscoveryJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateAgent",
                 "UpdateLocationHdfs",
                 "UpdateLocationNfs",
                 "UpdateLocationObjectStorage",
                 "UpdateLocationSmb",
+                "UpdateStorageSystem",
                 "UpdateTask",
                 "UpdateTaskExecution"
             ],
             "HasResource": true,
             "StringPrefix": "datasync",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
@@ -4071,14 +4083,15 @@
                 "StopCrawler",
                 "StopCrawlerSchedule",
                 "StopSession",
                 "StopTrigger",
                 "StopWorkflowRun",
                 "TagResource",
                 "TerminateNotebook",
+                "TestConnection",
                 "UntagResource",
                 "UpdateBlueprint",
                 "UpdateClassifier",
                 "UpdateColumnStatisticsForPartition",
                 "UpdateColumnStatisticsForTable",
                 "UpdateConnection",
                 "UpdateCrawler",
@@ -18721,14 +18734,15 @@
                 "PutConfigurationSetDeliveryOptions",
                 "PutConfigurationSetReputationOptions",
                 "PutConfigurationSetSendingOptions",
                 "PutConfigurationSetSuppressionOptions",
                 "PutConfigurationSetTrackingOptions",
                 "PutConfigurationSetVdmOptions",
                 "PutDedicatedIpInPool",
+                "PutDedicatedIpPoolScalingAttributes",
                 "PutDedicatedIpWarmupAttributes",
                 "PutDeliverabilityDashboardOption",
                 "PutEmailIdentityConfigurationSetAttributes",
                 "PutEmailIdentityDkimAttributes",
                 "PutEmailIdentityDkimSigningAttributes",
                 "PutEmailIdentityFeedbackAttributes",
                 "PutEmailIdentityMailFromAttributes",
```

### Comparing `iam_actions-1.2.20230522/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230523/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230522/iam_actions/services.json` & `iam_actions-1.2.20230523/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999737732712137%*

 * *Differences: {"'datasync'": "{'Actions': {insert: [(0, 'AddStorageSystem'), (18, 'DescribeDiscoveryJob'), (29, "*

 * *               "'DescribeStorageSystem'), (30, 'DescribeStorageSystemResourceMetrics'), (31, "*

 * *               "'DescribeStorageSystemResources'), (34, 'GenerateRecommendations'), (36, "*

 * *               "'ListDiscoveryJobs'), (38, 'ListStorageSystems'), (42, 'RemoveStorageSystem'), "*

 * *               "(43, 'StartDiscoveryJob'), (45, 'StopDiscoveryJob'), (53, "*

 * *               "'UpdateStorageSystem')]}}",*

 * * "'glue'" […]*

```diff
@@ -5070,14 +5070,15 @@
         "ARNFormats": [
             "arn:aws:datasync:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:datasync:.+"
         ],
         "Actions": [
+            "AddStorageSystem",
             "CancelTaskExecution",
             "CreateAgent",
             "CreateLocationEfs",
             "CreateLocationFsxLustre",
             "CreateLocationFsxOntap",
             "CreateLocationFsxOpenZfs",
             "CreateLocationFsxWindows",
@@ -5087,39 +5088,50 @@
             "CreateLocationS3",
             "CreateLocationSmb",
             "CreateTask",
             "DeleteAgent",
             "DeleteLocation",
             "DeleteTask",
             "DescribeAgent",
+            "DescribeDiscoveryJob",
             "DescribeLocationEfs",
             "DescribeLocationFsxLustre",
             "DescribeLocationFsxOntap",
             "DescribeLocationFsxOpenZfs",
             "DescribeLocationFsxWindows",
             "DescribeLocationHdfs",
             "DescribeLocationNfs",
             "DescribeLocationObjectStorage",
             "DescribeLocationS3",
             "DescribeLocationSmb",
+            "DescribeStorageSystem",
+            "DescribeStorageSystemResourceMetrics",
+            "DescribeStorageSystemResources",
             "DescribeTask",
             "DescribeTaskExecution",
+            "GenerateRecommendations",
             "ListAgents",
+            "ListDiscoveryJobs",
             "ListLocations",
+            "ListStorageSystems",
             "ListTagsForResource",
             "ListTaskExecutions",
             "ListTasks",
+            "RemoveStorageSystem",
+            "StartDiscoveryJob",
             "StartTaskExecution",
+            "StopDiscoveryJob",
             "TagResource",
             "UntagResource",
             "UpdateAgent",
             "UpdateLocationHdfs",
             "UpdateLocationNfs",
             "UpdateLocationObjectStorage",
             "UpdateLocationSmb",
+            "UpdateStorageSystem",
             "UpdateTask",
             "UpdateTaskExecution"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
@@ -9218,14 +9230,15 @@
             "StopCrawler",
             "StopCrawlerSchedule",
             "StopSession",
             "StopTrigger",
             "StopWorkflowRun",
             "TagResource",
             "TerminateNotebook",
+            "TestConnection",
             "UntagResource",
             "UpdateBlueprint",
             "UpdateClassifier",
             "UpdateColumnStatisticsForPartition",
             "UpdateColumnStatisticsForTable",
             "UpdateConnection",
             "UpdateCrawler",
@@ -18358,14 +18371,15 @@
             "PutConfigurationSetDeliveryOptions",
             "PutConfigurationSetReputationOptions",
             "PutConfigurationSetSendingOptions",
             "PutConfigurationSetSuppressionOptions",
             "PutConfigurationSetTrackingOptions",
             "PutConfigurationSetVdmOptions",
             "PutDedicatedIpInPool",
+            "PutDedicatedIpPoolScalingAttributes",
             "PutDedicatedIpWarmupAttributes",
             "PutDeliverabilityDashboardOption",
             "PutEmailIdentityConfigurationSetAttributes",
             "PutEmailIdentityDkimAttributes",
             "PutEmailIdentityDkimSigningAttributes",
             "PutEmailIdentityFeedbackAttributes",
             "PutEmailIdentityMailFromAttributes",
```

### Comparing `iam_actions-1.2.20230522/pyproject.toml` & `iam_actions-1.2.20230523/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230522"
+version = "1.2.20230523"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230522/setup.py` & `iam_actions-1.2.20230523/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230522',
+    'version': '1.2.20230523',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230522/PKG-INFO` & `iam_actions-1.2.20230523/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230522
+Version: 1.2.20230523
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

