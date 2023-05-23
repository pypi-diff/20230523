# Comparing `tmp/aws-cloudformation-visualizer-0.0.2.tar.gz` & `tmp/aws-cloudformation-visualizer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cloudformation-visualizer-0.0.2.tar", last modified: Wed Jan 25 01:25:36 2023, max compression
+gzip compressed data, was "aws-cloudformation-visualizer-0.0.3.tar", last modified: Tue May 23 07:03:58 2023, max compression
```

## Comparing `aws-cloudformation-visualizer-0.0.2.tar` & `aws-cloudformation-visualizer-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:25:36.980320 aws-cloudformation-visualizer-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-25 01:25:36.980320 aws-cloudformation-visualizer-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:25:36.976319 aws-cloudformation-visualizer-0.0.2/aws_cloudformation_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-25 01:25:36.000000 aws-cloudformation-visualizer-0.0.2/aws_cloudformation_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-01-25 01:25:36.000000 aws-cloudformation-visualizer-0.0.2/aws_cloudformation_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 01:25:36.000000 aws-cloudformation-visualizer-0.0.2/aws_cloudformation_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-25 01:25:36.000000 aws-cloudformation-visualizer-0.0.2/aws_cloudformation_visualizer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:25:36.980320 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/cfn_visualizer/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-25 01:25:36.980320 aws-cloudformation-visualizer-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-25 01:25:16.000000 aws-cloudformation-visualizer-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:03:58.530543 aws-cloudformation-visualizer-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-23 07:03:58.530543 aws-cloudformation-visualizer-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:03:58.530543 aws-cloudformation-visualizer-0.0.3/aws_cloudformation_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-23 07:03:58.000000 aws-cloudformation-visualizer-0.0.3/aws_cloudformation_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-23 07:03:58.000000 aws-cloudformation-visualizer-0.0.3/aws_cloudformation_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:03:58.000000 aws-cloudformation-visualizer-0.0.3/aws_cloudformation_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-23 07:03:58.000000 aws-cloudformation-visualizer-0.0.3/aws_cloudformation_visualizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:03:58.530543 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/cfn_visualizer/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 07:03:58.530543 aws-cloudformation-visualizer-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 07:03:30.000000 aws-cloudformation-visualizer-0.0.3/setup.py
```

### Comparing `aws-cloudformation-visualizer-0.0.2/cfn_visualizer/utils.py` & `aws-cloudformation-visualizer-0.0.3/cfn_visualizer/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def get_timestamp(timestamp: datetime):
     return timestamp.astimezone(tz.tzlocal()).strftime('%I:%M:%S %p')
 
 
 def print_event(event: dict):
-    event_info = ' {:>11} | {} | {:<40} | {:<35} | {}'.format(
+    event_info = ' {:>11} | {} | {:<41} | {:<36} | {}'.format(
         # 10:20:58 AM | CREATE_IN_PROGRESS          | AWS::CloudFormation::Stack                     | User Initiated
         get_timestamp(event.get('Timestamp')),
         get_status(event.get('ResourceStatus')),
         event.get('ResourceType'),
         event.get('LogicalResourceId'),
         event.get('ResourceStatusReason', '')
     )
```

### Comparing `aws-cloudformation-visualizer-0.0.2/cfn_visualizer/visualizer.py` & `aws-cloudformation-visualizer-0.0.3/cfn_visualizer/visualizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,17 @@
             event_count = _initial_visualize(client, stack_name)
 
             while True:
                 stack_response = client.describe_stacks(StackName=stack_name)
                 stack_status = stack_response['Stacks'][0]['StackStatus']
                 stack_name = stack_response['Stacks'][0]['StackId']
 
-                if 'FAILED' in stack_status or 'ROLLBACK' in stack_status:  # creation, deletion, update failed
+                if 'FAILED' in stack_status or 'ROLLBACK_COMPLETE' == stack_status:  # creation, deletion, update failed
+                    events = client.describe_stack_events(StackName=stack_name)['StackEvents']
+                    print_event(events[0])
                     raise StackFailedError(stack_name)
 
                 elif 'COMPLETE' in stack_status:
                     events = client.describe_stack_events(StackName=stack_name)['StackEvents']
 
                     if len(events) >= event_count:
                         remainder_count = len(events) - event_count
```

