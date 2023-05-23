# Comparing `tmp/phiterm-1.6.7.tar.gz` & `tmp/phiterm-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.7.tar", last modified: Fri May 19 12:43:09 2023, max compression
+gzip compressed data, was "phiterm-1.6.8.tar", last modified: Tue May 23 01:10:36 2023, max compression
```

## Comparing `phiterm-1.6.7.tar` & `phiterm-1.6.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.172700 phiterm-1.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-19 12:42:44.000000 phiterm-1.6.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 12:43:09.172700 phiterm-1.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 12:42:44.000000 phiterm-1.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.148700 phiterm-1.6.7/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.156700 phiterm-1.6.7/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.160700 phiterm-1.6.7/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.160700 phiterm-1.6.7/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.160700 phiterm-1.6.7/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.160700 phiterm-1.6.7/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.148700 phiterm-1.6.7/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.164700 phiterm-1.6.7/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.164700 phiterm-1.6.7/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.164700 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.164700 phiterm-1.6.7/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.164700 phiterm-1.6.7/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.168700 phiterm-1.6.7/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.168700 phiterm-1.6.7/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.168700 phiterm-1.6.7/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-19 12:42:44.000000 phiterm-1.6.7/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.152700 phiterm-1.6.7/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 12:43:09.000000 phiterm-1.6.7/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-19 12:42:44.000000 phiterm-1.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:43:09.172700 phiterm-1.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-19 12:42:44.000000 phiterm-1.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:43:09.168700 phiterm-1.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-19 12:42:44.000000 phiterm-1.6.7/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.849757 phiterm-1.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-23 01:10:17.000000 phiterm-1.6.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:10:36.845756 phiterm-1.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 01:10:17.000000 phiterm-1.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.817756 phiterm-1.6.8/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-23 01:10:17.000000 phiterm-1.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:10:36.849757 phiterm-1.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:10:17.000000 phiterm-1.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:10:17.000000 phiterm-1.6.8/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.7/LICENSE.md` & `phiterm-1.6.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/api/client.py` & `phiterm-1.6.8/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/api/routes.py` & `phiterm-1.6.8/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/api/user.py` & `phiterm-1.6.8/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/api/workspace.py` & `phiterm-1.6.8/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/aws/aws_operator.py` & `phiterm-1.6.8/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/cli_app.py` & `phiterm-1.6.8/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/cli_operator.py` & `phiterm-1.6.8/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.8/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.8/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.8/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.8/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.8/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.8/phiterm/cli/ws/ws_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         return
 
     current_path: Path = Path(".").resolve()
     if active_ws_data.ws_root_path != current_path and not auto_confirm:
         ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
         if ws_at_current_path is not None:
             print_info(
-                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({active_ws_data.ws_name})"
             )
             update_active_workspace = typer.confirm(
                 f"Update active workspace to {ws_at_current_path.ws_name}", default=True
             )
             if update_active_workspace:
                 phi_conf.active_ws_name = ws_at_current_path.ws_name
                 active_ws_data = ws_at_current_path
@@ -390,15 +390,15 @@
         return
 
     current_path: Path = Path(".").resolve()
     if active_ws_data.ws_root_path != current_path and not auto_confirm:
         ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
         if ws_at_current_path is not None:
             print_info(
-                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({active_ws_data.ws_name})"
             )
             update_active_workspace = typer.confirm(
                 f"Update active workspace to {ws_at_current_path.ws_name}", default=True
             )
             if update_active_workspace:
                 phi_conf.active_ws_name = ws_at_current_path.ws_name
                 active_ws_data = ws_at_current_path
@@ -582,15 +582,15 @@
         return
 
     current_path: Path = Path(".").resolve()
     if active_ws_data.ws_root_path != current_path and not auto_confirm:
         ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
         if ws_at_current_path is not None:
             print_info(
-                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({active_ws_data.ws_name})"
             )
             update_active_workspace = typer.confirm(
                 f"Update active workspace to {ws_at_current_path.ws_name}", default=True
             )
             if update_active_workspace:
                 phi_conf.active_ws_name = ws_at_current_path.ws_name
                 active_ws_data = ws_at_current_path
@@ -862,15 +862,15 @@
         return
 
     current_path: Path = Path(".").resolve()
     if active_ws_data.ws_root_path != current_path and not auto_confirm:
         ws_at_current_path = phi_conf.get_ws_data_by_path(current_path)
         if ws_at_current_path is not None:
             print_info(
-                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({ws_at_current_path.ws_name})"
+                f"Workspace at the current directory ({ws_at_current_path.ws_name}) is not the Active Workspace ({active_ws_data.ws_name})"
             )
             update_active_workspace = typer.confirm(
                 f"Update active workspace to {ws_at_current_path.ws_name}", default=True
             )
             if update_active_workspace:
                 phi_conf.active_ws_name = ws_at_current_path.ws_name
                 active_ws_data = ws_at_current_path
```

### Comparing `phiterm-1.6.7/phiterm/conf/auth.py` & `phiterm-1.6.8/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/conf/constants.py` & `phiterm-1.6.8/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/conf/phi_conf.py` & `phiterm-1.6.8/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/databox/databox_operator.py` & `phiterm-1.6.8/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/docker/docker_operator.py` & `phiterm-1.6.8/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/enums/user.py` & `phiterm-1.6.8/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.8/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.8/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.8/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.8/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.8/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/local/local_operator.py` & `phiterm-1.6.8/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/release/release_schemas.py` & `phiterm-1.6.8/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/release/ws_releases.py` & `phiterm-1.6.8/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/schemas/user.py` & `phiterm-1.6.8/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/schemas/user_schemas.py` & `phiterm-1.6.8/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/schemas/workspace.py` & `phiterm-1.6.8/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.8/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.8/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.8/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.8/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.8/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.8/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.8/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.8/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/cli_console.py` & `phiterm-1.6.8/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/common.py` & `phiterm-1.6.8/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/dttm.py` & `phiterm-1.6.8/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/enums.py` & `phiterm-1.6.8/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/filesystem.py` & `phiterm-1.6.8/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/git.py` & `phiterm-1.6.8/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/load_env.py` & `phiterm-1.6.8/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/log.py` & `phiterm-1.6.8/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/pyproject.py` & `phiterm-1.6.8/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/utils/ws_filter.py` & `phiterm-1.6.8/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workflow/wf_operator.py` & `phiterm-1.6.8/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workflow/wf_utils.py` & `phiterm-1.6.8/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.8/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/ws_enums.py` & `phiterm-1.6.8/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/ws_loader.py` & `phiterm-1.6.8/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/ws_operator.py` & `phiterm-1.6.8/phiterm/workspace/ws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.8/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm/workspace/ws_utils.py` & `phiterm-1.6.8/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.8/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.7/pyproject.toml` & `phiterm-1.6.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.7"
+version = "1.6.8"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

