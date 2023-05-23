# Comparing `tmp/frequenz-api-common-0.1.0.tar.gz` & `tmp/frequenz-api-common-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-common-0.1.0.tar", last modified: Wed May 17 08:47:35 2023, max compression
+gzip compressed data, was "frequenz-api-common-0.2.0.tar", last modified: Tue May 23 11:39:02 2023, max compression
```

## Comparing `frequenz-api-common-0.1.0.tar` & `frequenz-api-common-0.2.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.999148 frequenz-api-common-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-17 08:47:34.999148 frequenz-api-common-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.991148 frequenz-api-common-0.1.0/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.991148 frequenz-api-common-0.1.0/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.991148 frequenz-api-common-0.1.0/py/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/py/frequenz/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.991148 frequenz-api-common-0.1.0/py/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/py/frequenz/api/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/py/frequenz/api/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.991148 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-17 08:47:34.000000 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-05-17 08:47:34.000000 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 08:47:34.000000 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-05-17 08:47:34.000000 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-17 08:47:34.000000 frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2042 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 08:47:34.999148 frequenz-api-common-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.987148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 08:47:34.995148 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-17 08:47:20.000000 frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.241513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.241513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/timeofday.proto
```

### Comparing `frequenz-api-common-0.1.0/CONTRIBUTING.md` & `frequenz-api-common-0.2.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Contributing to Frequenz Microgrid API
-======================================
+Contributing to Frequenz Common API
+===================================
 
 
 Build
 =====
 
 You can use `build` to simply build the source and binary distribution:
 
@@ -60,19 +60,19 @@
    git tag -s -F RELEASE_NOTES.md v0.0.1
    ```
 
 4. Push the new tag.
 
 5. A GitHub action will test the tag and if all goes well it will create
    a [GitHub
-   Release](https://github.com/frequenz-floss/frequenz-api-microgrid/releases),
+   Release](https://github.com/frequenz-floss/frequenz-api-common/releases),
    create a new
-   [announcement](https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/announcements)
+   [announcement](https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/announcements)
    about the release, and upload a new package to
-   [PyPI](https://pypi.org/project/frequenz-api-microgrid/) automatically.
+   [PyPI](https://pypi.org/project/frequenz-api-common/) automatically.
 
 6. Once this is done, reset the `RELEASE_NOTES.md` with the template:
 
    ```sh
    cp .github/RELEASE_NOTES.template.md RELEASE_NOTES.md
    ```
```

### Comparing `frequenz-api-common-0.1.0/LICENSE` & `frequenz-api-common-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/PKG-INFO` & `frequenz-api-common-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.1.0/proto/frequenz/api/common/components.proto` & `frequenz-api-common-0.2.0/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/proto/frequenz/api/common/metrics.proto` & `frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/PKG-INFO` & `frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.1.0
+Version: 0.2.0
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.1.0/py/frequenz_api_common.egg-info/SOURCES.txt` & `frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/pyproject.toml` & `frequenz-api-common-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [build-system]
 requires = [
-  "setuptools >= 67.3.2, < 68",
-  "setuptools_scm[toml] >= 7.1.0, < 8",
+  "setuptools == 67.7.2",
+  "setuptools_scm[toml] == 7.1.0",
   "frequenz-repo-config[api] == 0.1.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-api-common"
 description = "Frequenz common gRPC API and bindings"
@@ -31,25 +31,25 @@
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
 dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
 dev-mypy = [
-  "mypy == 1.1.1",
+  "mypy == 1.3.0",
   # For checking the noxfile and tests
   "frequenz-api-common[dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2022.11.21", "frequenz-repo-config[api] == 0.1.0"]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[api] == 0.1.0"]
 dev-pylint = [
-  "pylint == 2.17.1",
+  "pylint == 2.17.4",
   # For checking the noxfile and tests
   "frequenz-api-common[dev-noxfile,dev-pytest]",
 ]
-dev-pytest = ["pytest == 7.2.2"]
+dev-pytest = ["pytest == 7.3.1"]
 dev = [
   "frequenz-api-common[dev-docstrings,dev-formatting,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Changelog = "https://github.com/frequenz-floss/frequenz-api-common/releases"
 Repository = "https://github.com/frequenz-floss/frequenz-api-common"
```

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.1.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

